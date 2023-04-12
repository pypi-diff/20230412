# Comparing `tmp/dhlab-2.9.4.tar.gz` & `tmp/dhlab-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhlab-2.9.4.tar", last modified: Tue Oct  4 06:34:01 2022, max compression
+gzip compressed data, was "dhlab-2.9.5.tar", last modified: Wed Oct 26 14:23:59 2022, max compression
```

## Comparing `dhlab-2.9.4.tar` & `dhlab-2.9.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.787728 dhlab-2.9.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.787728 dhlab-2.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-10-04 06:33:41.000000 dhlab-2.9.4/.github/workflows/bump-version.yml
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-04 06:33:41.000000 dhlab-2.9.4/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-10-04 06:33:41.000000 dhlab-2.9.4/.github/workflows/deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-04 06:33:41.000000 dhlab-2.9.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-10-04 06:33:41.000000 dhlab-2.9.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-04 06:33:41.000000 dhlab-2.9.4/.github/workflows/upload-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-10-04 06:33:41.000000 dhlab-2.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    19548 2022-10-04 06:33:41.000000 dhlab-2.9.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-04 06:33:41.000000 dhlab-2.9.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4782 2022-10-04 06:33:41.000000 dhlab-2.9.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-10-04 06:34:01.795728 dhlab-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-10-04 06:33:41.000000 dhlab-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/api/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28463 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/api/dhlab_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/api/nb_ngram_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4492 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/api/nb_search_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/css_style_sheets/
--rw-r--r--   0 runner    (1001) docker     (121)    72064 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/css_style_sheets/grade3.css
--rw-r--r--   0 runner    (1001) docker     (121)    72138 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/css_style_sheets/monokai.css
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/css_style_sheets/nb_notebook.css
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/css_style_sheets/nb_notebook_2.css
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/css_style_sheets/nb_notebook_blue.css
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/graph_networkx_louvain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/images/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/images/nbpictures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15394 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/graph_networkx_louvain.py
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/module_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/nb_external_files.py
--rw-r--r--   0 runner    (1001) docker     (121)    14179 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/nbpictures.py
--rw-r--r--   0 runner    (1001) docker     (121)    71589 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/nbtext.py
--rw-r--r--   0 runner    (1001) docker     (121)     8822 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/legacy/token_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/metadata/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/module_update.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/nbpictures.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/nbtext.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/nbtokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/ngram/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/ngram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/ngram/nb_ngram.py
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/ngram/ngram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab/text/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/chunking.py
--rw-r--r--   0 runner    (1001) docker     (121)     5538 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/conc_coll.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/corpus.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/dispersion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/geo_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/nb_search_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     9632 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/nbtokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/text/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/token_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/dhlab/trigram_lang_model/
--rw-r--r--   0 runner    (1001) docker     (121)   126476 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/trigram_lang_model/nno_trilangmodel.json
--rw-r--r--   0 runner    (1001) docker     (121)   126751 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/trigram_lang_model/nob_trilangmodel.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/dhlab/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     3832 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/dhlab/wordbank/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/wordbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-04 06:33:41.000000 dhlab-2.9.4/dhlab/wordbank/wordbank.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.791728 dhlab-2.9.4/dhlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 06:34:01.000000 dhlab-2.9.4/dhlab.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/DOCS_CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/_images/NB-symbol-farge.png
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/_images/dhlab_logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/_images/nb_symbol_farge_z5B_icon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    10923 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/docs_getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/docs_notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/notebooks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/package_summary.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/usage_api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/usage_images.rst
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/usage_metadata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/usage_ngrams.rst
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/usage_text.rst
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-10-04 06:33:41.000000 dhlab-2.9.4/docs/usage_utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-04 06:33:41.000000 dhlab-2.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-04 06:33:41.000000 dhlab-2.9.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-04 06:34:01.795728 dhlab-2.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 06:34:01.795728 dhlab-2.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-04 06:33:41.000000 dhlab-2.9.4/tests/test_nbtext.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.494017 dhlab-2.9.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/bump-version.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      879 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      867 2022-10-26 14:23:47.000000 dhlab-2.9.5/.github/workflows/upload-package.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-10-26 14:23:47.000000 dhlab-2.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    19548 2022-10-26 14:23:47.000000 dhlab-2.9.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-26 14:23:47.000000 dhlab-2.9.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-10-26 14:23:47.000000 dhlab-2.9.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-10-26 14:23:59.506018 dhlab-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-10-26 14:23:47.000000 dhlab-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28463 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/dhlab_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/nb_ngram_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4492 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/api/nb_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/css_style_sheets/
+-rw-r--r--   0 runner    (1001) docker     (121)    72064 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/grade3.css
+-rw-r--r--   0 runner    (1001) docker     (121)    72138 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/monokai.css
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_2.css
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_blue.css
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/graph_networkx_louvain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/images/
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/images/nbpictures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15394 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/graph_networkx_louvain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/module_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/nb_external_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14179 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/nbpictures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71589 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/nbtext.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8822 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/legacy/token_map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/module_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/nbpictures.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/nbtext.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/nbtokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/ngram/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/ngram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2903 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/ngram/nb_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/ngram/ngram.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/text/
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/chunking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5538 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/conc_coll.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/geo_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/nb_search_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9717 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/nbtokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/text/parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/token_map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/trigram_lang_model/
+-rw-r--r--   0 runner    (1001) docker     (121)   126476 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/trigram_lang_model/nno_trilangmodel.json
+-rw-r--r--   0 runner    (1001) docker     (121)   126751 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/trigram_lang_model/nob_trilangmodel.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2301 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3832 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.502017 dhlab-2.9.5/dhlab/wordbank/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/wordbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-10-26 14:23:47.000000 dhlab-2.9.5/dhlab/wordbank/wordbank.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.498017 dhlab-2.9.5/dhlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 14:23:59.000000 dhlab-2.9.5/dhlab.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/DOCS_CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/_images/NB-symbol-farge.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/_images/dhlab_logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/_images/nb_symbol_farge_z5B_icon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    10923 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/docs_getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/docs_notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1583 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/notebooks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/package_summary.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_images.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_ngrams.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_text.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-10-26 14:23:47.000000 dhlab-2.9.5/docs/usage_utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-26 14:23:47.000000 dhlab-2.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-10-26 14:23:47.000000 dhlab-2.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-26 14:23:59.506018 dhlab-2.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 14:23:59.506018 dhlab-2.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-26 14:23:47.000000 dhlab-2.9.5/tests/test_nbtext.py
```

### Comparing `dhlab-2.9.4/.github/workflows/bump-version.yml` & `dhlab-2.9.5/.github/workflows/bump-version.yml`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.github/workflows/deployment.yml` & `dhlab-2.9.5/.github/workflows/deployment.yml`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.github/workflows/lint.yml` & `dhlab-2.9.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.github/workflows/test.yml` & `dhlab-2.9.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.github/workflows/upload-package.yml` & `dhlab-2.9.5/.github/workflows/upload-package.yml`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.gitignore` & `dhlab-2.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.pylintrc` & `dhlab-2.9.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/.readthedocs.yaml` & `dhlab-2.9.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/CHANGELOG.md` & `dhlab-2.9.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v2.9.5 (2022-10-26)
+
+### Fix
+
+- nbtokenizer now handles numbers combined with words, e.g. '1800-tallet'
+
 ## v2.9.4 (2022-10-04)
 
 ### Fix
 
 - relative and absolute
 
 ## v2.9.3 (2022-10-04)
```

### Comparing `dhlab-2.9.4/PKG-INFO` & `dhlab-2.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhlab
-Version: 2.9.4
+Version: 2.9.5
 Summary: Text and image analysis of NB's digital collection
 Home-page: https://github.com/NationalLibraryOfNorway/DHLAB
 Author: The Digital Humanities Lab at The National Library of Norway (NB)
 Author-email: dh-lab@nb.no
 License: MIT
 Project-URL: Documentation, https://dhlab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/NationalLibraryOfNorway/DHLAB/issues
@@ -69,14 +69,20 @@
 ## Contact
 If you have any questions, or run into any problems with the code, please log them in our [issue 
 tracker](https://github.com/NationalLibraryOfNorway/DHLAB/issues) in the DHLAB repo. 
 
 
 # Changelog
 
+## v2.9.5 (2022-10-26)
+
+### Fix
+
+- nbtokenizer now handles numbers combined with words, e.g. '1800-tallet'
+
 ## v2.9.4 (2022-10-04)
 
 ### Fix
 
 - relative and absolute
 
 ## v2.9.3 (2022-10-04)
```

### Comparing `dhlab-2.9.4/README.md` & `dhlab-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/__init__.py` & `dhlab-2.9.5/dhlab/__init__.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/api/dhlab_api.py` & `dhlab-2.9.5/dhlab/api/dhlab_api.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/api/nb_ngram_api.py` & `dhlab-2.9.5/dhlab/api/nb_ngram_api.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/api/nb_search_api.py` & `dhlab-2.9.5/dhlab/api/nb_search_api.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/css_style_sheets/grade3.css` & `dhlab-2.9.5/dhlab/css_style_sheets/grade3.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/css_style_sheets/monokai.css` & `dhlab-2.9.5/dhlab/css_style_sheets/monokai.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/css_style_sheets/nb_notebook.css` & `dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/css_style_sheets/nb_notebook_2.css` & `dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_2.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/css_style_sheets/nb_notebook_blue.css` & `dhlab-2.9.5/dhlab/css_style_sheets/nb_notebook_blue.css`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/images/nbpictures.py` & `dhlab-2.9.5/dhlab/images/nbpictures.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/legacy/graph_networkx_louvain.py` & `dhlab-2.9.5/dhlab/legacy/graph_networkx_louvain.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/legacy/module_update.py` & `dhlab-2.9.5/dhlab/legacy/module_update.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/legacy/nb_external_files.py` & `dhlab-2.9.5/dhlab/legacy/nb_external_files.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/legacy/nbpictures.py` & `dhlab-2.9.5/dhlab/legacy/nbpictures.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/legacy/nbtext.py` & `dhlab-2.9.5/dhlab/legacy/nbtext.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/legacy/token_map.py` & `dhlab-2.9.5/dhlab/legacy/token_map.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/ngram/nb_ngram.py` & `dhlab-2.9.5/dhlab/ngram/nb_ngram.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/ngram/ngram.py` & `dhlab-2.9.5/dhlab/ngram/ngram.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/chunking.py` & `dhlab-2.9.5/dhlab/text/chunking.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/conc_coll.py` & `dhlab-2.9.5/dhlab/text/conc_coll.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/corpus.py` & `dhlab-2.9.5/dhlab/text/corpus.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/dispersion.py` & `dhlab-2.9.5/dhlab/text/dispersion.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/geo_data.py` & `dhlab-2.9.5/dhlab/text/geo_data.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/nb_search_text.py` & `dhlab-2.9.5/dhlab/text/nb_search_text.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/text/nbtokenizer.py` & `dhlab-2.9.5/dhlab/text/nbtokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,17 +372,19 @@
 num3 = r'\.\d+'
 """Det var .2 prosent økning."""
 
 
 num4 = r'\.\.\.+'
 """Tre eller flere punktum blir ett token."""
 
+num5 = r'\d+(?:[-–]\w+)'
+"""Tallord kombinert med ord, f.eks. 1900-tallet"""
 
 # TODO: kombiner til det regulære uttrykket num eller num0 eller...
-num = '|'.join([num0, num1, num2, num3, num4, num])
+num = '|'.join([num0, num1, num2, num3, num4, num5, num])
 
 
 parnum0 = r'(?<=§ )\d+(?:[-–—]\d+)*|(?<=§)\d+(?:[-–—]\d+)*'
 """Paragraftegn kan komme i en eller to (eller flere?) utgaver.
 
 Tolk tall etter § som rene tall uten punktum,
 men også med bindestrek så i § 2-5  blir 2-5 et token.
```

### Comparing `dhlab-2.9.4/dhlab/text/parse.py` & `dhlab-2.9.5/dhlab/text/parse.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/trigram_lang_model/nno_trilangmodel.json` & `dhlab-2.9.5/dhlab/trigram_lang_model/nno_trilangmodel.json`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/trigram_lang_model/nob_trilangmodel.json` & `dhlab-2.9.5/dhlab/trigram_lang_model/nob_trilangmodel.json`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/utils/display.py` & `dhlab-2.9.5/dhlab/utils/display.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/utils/files.py` & `dhlab-2.9.5/dhlab/utils/files.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab/wordbank/wordbank.py` & `dhlab-2.9.5/dhlab/wordbank/wordbank.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/dhlab.egg-info/PKG-INFO` & `dhlab-2.9.5/dhlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhlab
-Version: 2.9.4
+Version: 2.9.5
 Summary: Text and image analysis of NB's digital collection
 Home-page: https://github.com/NationalLibraryOfNorway/DHLAB
 Author: The Digital Humanities Lab at The National Library of Norway (NB)
 Author-email: dh-lab@nb.no
 License: MIT
 Project-URL: Documentation, https://dhlab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/NationalLibraryOfNorway/DHLAB/issues
@@ -69,14 +69,20 @@
 ## Contact
 If you have any questions, or run into any problems with the code, please log them in our [issue 
 tracker](https://github.com/NationalLibraryOfNorway/DHLAB/issues) in the DHLAB repo. 
 
 
 # Changelog
 
+## v2.9.5 (2022-10-26)
+
+### Fix
+
+- nbtokenizer now handles numbers combined with words, e.g. '1800-tallet'
+
 ## v2.9.4 (2022-10-04)
 
 ### Fix
 
 - relative and absolute
 
 ## v2.9.3 (2022-10-04)
```

### Comparing `dhlab-2.9.4/dhlab.egg-info/SOURCES.txt` & `dhlab-2.9.5/dhlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/DOCS_CHANGELOG.md` & `dhlab-2.9.5/docs/DOCS_CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/LICENSE` & `dhlab-2.9.5/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/Makefile` & `dhlab-2.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/_images/NB-symbol-farge.png` & `dhlab-2.9.5/docs/_images/NB-symbol-farge.png`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/_images/dhlab_logo.png` & `dhlab-2.9.5/docs/_images/dhlab_logo.png`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/_images/nb_symbol_farge_z5B_icon.ico` & `dhlab-2.9.5/docs/_images/nb_symbol_farge_z5B_icon.ico`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/conf.py` & `dhlab-2.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/docs_notebooks.rst` & `dhlab-2.9.5/docs/docs_notebooks.rst`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/index.rst` & `dhlab-2.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/make.bat` & `dhlab-2.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/package_summary.rst` & `dhlab-2.9.5/docs/package_summary.rst`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/usage_api.rst` & `dhlab-2.9.5/docs/usage_api.rst`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/usage_ngrams.rst` & `dhlab-2.9.5/docs/usage_ngrams.rst`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/docs/usage_text.rst` & `dhlab-2.9.5/docs/usage_text.rst`

 * *Files identical despite different names*

### Comparing `dhlab-2.9.4/pyproject.toml` & `dhlab-2.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     pytest-cov >= 3.0.0
 commands =
     python -m pytest tests --doctest-modules --cov=dhlab --cov-report=html
 """
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.9.4"
+version = "2.9.5"
 tag_format = "v$major.$minor.$patch$prerelease"
 bump_message = "bump: version $current_version → $new_version [skip-ci]"
 update_changelog_on_bump = true
 annotated_tag = true
 changelog_file = "CHANGELOG.md"
 changelog_incremental = true
 style = [
```

### Comparing `dhlab-2.9.4/setup.cfg` & `dhlab-2.9.5/setup.cfg`

 * *Files identical despite different names*

