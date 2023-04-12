# Comparing `tmp/pyriksdagen-0.4.0.tar.gz` & `tmp/pyriksdagen-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksdagen-0.4.0.tar", max compression
+gzip compressed data, was "pyriksdagen-0.8.0.tar", max compression
```

## Comparing `pyriksdagen-0.4.0.tar` & `pyriksdagen-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1249 2022-11-01 12:04:45.361073 pyriksdagen-0.4.0/LICENSE
--rw-r--r--   0        0        0     3525 2022-11-01 12:04:45.361143 pyriksdagen-0.4.0/README.md
--rw-r--r--   0        0        0      718 2023-03-01 10:37:29.215036 pyriksdagen-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1107 2022-11-01 12:05:01.901342 pyriksdagen-0.4.0/pyriksdagen/LICENSE
--rw-r--r--   0        0        0       84 2022-11-01 12:05:01.901407 pyriksdagen-0.4.0/pyriksdagen/__init__.py
--rw-r--r--   0        0        0      225 2022-11-01 12:05:01.901564 pyriksdagen-0.4.0/pyriksdagen/data/queries/alias.rq
--rw-r--r--   0        0        0      494 2023-02-07 15:52:31.495339 pyriksdagen-0.4.0/pyriksdagen/data/queries/government.rq
--rw-r--r--   0        0        0      729 2023-02-07 15:52:31.495749 pyriksdagen-0.4.0/pyriksdagen/data/queries/member_of_parliament.rq
--rw-r--r--   0        0        0      148 2022-11-01 12:05:01.901748 pyriksdagen-0.4.0/pyriksdagen/data/queries/member_of_parliament.txt
--rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.901837 pyriksdagen-0.4.0/pyriksdagen/data/queries/minister.rq
--rw-r--r--   0        0        0      235 2022-11-01 12:05:01.901892 pyriksdagen-0.4.0/pyriksdagen/data/queries/minister.txt
--rw-r--r--   0        0        0      262 2022-11-01 12:05:01.901962 pyriksdagen-0.4.0/pyriksdagen/data/queries/name_location_specifier.rq
--rw-r--r--   0        0        0      484 2023-02-07 15:52:31.496167 pyriksdagen-0.4.0/pyriksdagen/data/queries/party_affiliation.rq
--rw-r--r--   0        0        0      549 2023-02-07 15:52:31.496580 pyriksdagen-0.4.0/pyriksdagen/data/queries/person.rq
--rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902171 pyriksdagen-0.4.0/pyriksdagen/data/queries/speaker.rq
--rw-r--r--   0        0        0      253 2022-11-01 12:05:01.902229 pyriksdagen-0.4.0/pyriksdagen/data/queries/speaker.txt
--rw-r--r--   0        0        0      208 2022-11-01 12:05:01.902286 pyriksdagen-0.4.0/pyriksdagen/data/queries/twitter.rq
--rw-r--r--   0        0        0      225 2022-11-01 12:05:01.902412 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/alias.rq
--rw-r--r--   0        0        0      482 2022-11-01 12:05:01.902473 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/government.rq
--rw-r--r--   0        0        0      722 2022-11-01 12:05:01.902539 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
--rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.902591 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/minister.rq
--rw-r--r--   0        0        0     1013 2022-11-01 12:05:01.902681 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
--rw-r--r--   0        0        0     1230 2022-11-01 12:05:01.902743 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/party_affiliation.rq
--rw-r--r--   0        0        0     1412 2022-11-01 12:05:01.902796 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/person.rq
--rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902856 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/speaker.rq
--rw-r--r--   0        0        0      959 2022-11-01 12:05:01.902940 pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/twitter.rq
--rw-r--r--   0        0        0     2195 2022-11-01 12:05:01.903003 pyriksdagen-0.4.0/pyriksdagen/dataset.py
--rw-r--r--   0        0        0     6193 2023-02-07 15:52:31.497165 pyriksdagen-0.4.0/pyriksdagen/db.py
--rw-r--r--   0        0        0     9747 2023-03-01 10:25:07.959327 pyriksdagen-0.4.0/pyriksdagen/download.py
--rw-r--r--   0        0        0     6813 2023-03-01 10:25:07.959687 pyriksdagen-0.4.0/pyriksdagen/export.py
--rw-r--r--   0        0        0     4532 2022-11-01 12:05:01.903384 pyriksdagen-0.4.0/pyriksdagen/match_mp.py
--rw-r--r--   0        0        0     6915 2023-02-07 15:52:31.497997 pyriksdagen-0.4.0/pyriksdagen/metadata.py
--rw-r--r--   0        0        0    11120 2022-11-01 12:05:01.903558 pyriksdagen-0.4.0/pyriksdagen/mp.py
--rw-r--r--   0        0        0    16044 2023-02-28 12:07:33.769520 pyriksdagen-0.4.0/pyriksdagen/refine.py
--rwxr-xr-x   0        0        0      237 2023-03-01 10:25:07.959885 pyriksdagen-0.4.0/pyriksdagen/requirements.txt
--rw-r--r--   0        0        0     7039 2023-02-28 12:07:33.771508 pyriksdagen-0.4.0/pyriksdagen/segmentation.py
--rw-r--r--   0        0        0     5497 2023-02-28 12:07:33.772871 pyriksdagen-0.4.0/pyriksdagen/utils.py
--rw-r--r--   0        0        0     5265 2023-02-07 15:52:31.499089 pyriksdagen-0.4.0/pyriksdagen/wikidata.py
--rw-r--r--   0        0        0     4527 2023-03-01 10:37:54.354519 pyriksdagen-0.4.0/setup.py
--rw-r--r--   0        0        0     4563 2023-03-01 10:37:54.354789 pyriksdagen-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1249 2022-11-01 12:04:45.361073 pyriksdagen-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3519 2023-04-12 10:51:21.978195 pyriksdagen-0.8.0/README.md
+-rw-r--r--   0        0        0      745 2023-04-12 11:07:15.247115 pyriksdagen-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1107 2022-11-01 12:05:01.901342 pyriksdagen-0.8.0/pyriksdagen/LICENSE
+-rw-r--r--   0        0        0       84 2022-11-01 12:05:01.901407 pyriksdagen-0.8.0/pyriksdagen/__init__.py
+-rw-r--r--   0        0        0      225 2022-11-01 12:05:01.901564 pyriksdagen-0.8.0/pyriksdagen/data/queries/alias.rq
+-rw-r--r--   0        0        0      494 2023-02-07 15:52:31.495339 pyriksdagen-0.8.0/pyriksdagen/data/queries/government.rq
+-rw-r--r--   0        0        0      729 2023-02-07 15:52:31.495749 pyriksdagen-0.8.0/pyriksdagen/data/queries/member_of_parliament.rq
+-rw-r--r--   0        0        0      148 2022-11-01 12:05:01.901748 pyriksdagen-0.8.0/pyriksdagen/data/queries/member_of_parliament.txt
+-rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.901837 pyriksdagen-0.8.0/pyriksdagen/data/queries/minister.rq
+-rw-r--r--   0        0        0      235 2022-11-01 12:05:01.901892 pyriksdagen-0.8.0/pyriksdagen/data/queries/minister.txt
+-rw-r--r--   0        0        0      262 2022-11-01 12:05:01.901962 pyriksdagen-0.8.0/pyriksdagen/data/queries/name_location_specifier.rq
+-rw-r--r--   0        0        0      484 2023-02-07 15:52:31.496167 pyriksdagen-0.8.0/pyriksdagen/data/queries/party_affiliation.rq
+-rw-r--r--   0        0        0      549 2023-02-07 15:52:31.496580 pyriksdagen-0.8.0/pyriksdagen/data/queries/person.rq
+-rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902171 pyriksdagen-0.8.0/pyriksdagen/data/queries/speaker.rq
+-rw-r--r--   0        0        0      253 2022-11-01 12:05:01.902229 pyriksdagen-0.8.0/pyriksdagen/data/queries/speaker.txt
+-rw-r--r--   0        0        0      208 2022-11-01 12:05:01.902286 pyriksdagen-0.8.0/pyriksdagen/data/queries/twitter.rq
+-rw-r--r--   0        0        0      225 2022-11-01 12:05:01.902412 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/alias.rq
+-rw-r--r--   0        0        0      482 2022-11-01 12:05:01.902473 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/government.rq
+-rw-r--r--   0        0        0      722 2022-11-01 12:05:01.902539 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/member_of_parliament.rq
+-rw-r--r--   0        0        0     1380 2022-11-01 12:05:01.902591 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/minister.rq
+-rw-r--r--   0        0        0     1013 2022-11-01 12:05:01.902681 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/name_location_specifier.rq
+-rw-r--r--   0        0        0     1230 2022-11-01 12:05:01.902743 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/party_affiliation.rq
+-rw-r--r--   0        0        0     1412 2022-11-01 12:05:01.902796 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/person.rq
+-rw-r--r--   0        0        0      616 2022-11-01 12:05:01.902856 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/speaker.rq
+-rw-r--r--   0        0        0      959 2022-11-01 12:05:01.902940 pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/twitter.rq
+-rw-r--r--   0        0        0     2195 2022-11-01 12:05:01.903003 pyriksdagen-0.8.0/pyriksdagen/dataset.py
+-rw-r--r--   0        0        0     6193 2023-02-07 15:52:31.497165 pyriksdagen-0.8.0/pyriksdagen/db.py
+-rw-r--r--   0        0        0     9747 2023-03-01 12:15:10.843910 pyriksdagen-0.8.0/pyriksdagen/download.py
+-rw-r--r--   0        0        0     6813 2023-03-01 12:15:10.844248 pyriksdagen-0.8.0/pyriksdagen/export.py
+-rw-r--r--   0        0        0     4532 2022-11-01 12:05:01.903384 pyriksdagen-0.8.0/pyriksdagen/match_mp.py
+-rw-r--r--   0        0        0     6915 2023-02-07 15:52:31.497997 pyriksdagen-0.8.0/pyriksdagen/metadata.py
+-rw-r--r--   0        0        0    11120 2022-11-01 12:05:01.903558 pyriksdagen-0.8.0/pyriksdagen/mp.py
+-rw-r--r--   0        0        0    16044 2023-04-05 08:32:54.043579 pyriksdagen-0.8.0/pyriksdagen/refine.py
+-rwxr-xr-x   0        0        0      237 2023-03-01 12:15:10.846196 pyriksdagen-0.8.0/pyriksdagen/requirements.txt
+-rw-r--r--   0        0        0     7039 2023-04-05 08:32:54.044723 pyriksdagen-0.8.0/pyriksdagen/segmentation.py
+-rw-r--r--   0        0        0     5497 2023-03-01 12:15:10.850360 pyriksdagen-0.8.0/pyriksdagen/utils.py
+-rw-r--r--   0        0        0     5265 2023-03-01 12:14:56.389831 pyriksdagen-0.8.0/pyriksdagen/wikidata.py
+-rw-r--r--   0        0        0     4545 2023-04-12 11:07:27.882668 pyriksdagen-0.8.0/setup.py
+-rw-r--r--   0        0        0     4592 2023-04-12 11:07:27.882917 pyriksdagen-0.8.0/PKG-INFO
```

### Comparing `pyriksdagen-0.4.0/LICENSE` & `pyriksdagen-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/README.md` & `pyriksdagen-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)
 [![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)
 [![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)
 
-# Swedish parliamentary proceedings - Riksdagens protokoll 1920-2021
+# Swedish parliamentary proceedings - Riksdagens protokoll 1867-2023
 
-_Westac Project, 2020-2021_
+_Westac Project, 2020-2023_
 
 The full data set consists of multiple parts:
 
-- Riksdagens protokoll between from 1920 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
+- Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
 - Comprehensive list of MPs and cabinet members during this period
 - [Documentation](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/) of the corpus and the curation process
 - [A Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing) that demonstrates how the dataset can be used with Python
 
 ## Basic use
 
-A full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/download/v0.4.3/corpus-0.4.3.zip). It has the following structure
+A full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/latest/download/corpus.zip). It has the following structure
 
 - Annual protocol files in the ```corpus/protocols/``` folder
 - Structured metadata on MPs, speakers, ministers, and governments in the ```corpus/metadata/``` folder
 
 The workflow to use the data is demonstrated in [this Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing).
 
 ## Design choices of the project
```

### Comparing `pyriksdagen-0.4.0/pyproject.toml` & `pyriksdagen-0.8.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksdagen"
-version = "0.4.0"
+version = "0.8.0"
 description = "Access the Riksdagen corpus"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/riksdagen-corpus"
 readme = "README.md"
 license = "MIT"
 packages = [
     { include = "pyriksdagen", from = "" }
@@ -22,14 +22,15 @@
 dateparser = "*"
 beautifulsoup4 = "*"
 requests = "*"
 numpy = "*"
 SPARQLWrapper = "*"
 tqdm = "*"
 matplotlib = "*"
+importlib_resources = "*"
 
 [tool.poetry.dev-dependencies]
 devtools = "^0.5.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.masonry.api"
```

### Comparing `pyriksdagen-0.4.0/pyriksdagen/LICENSE` & `pyriksdagen-0.8.0/pyriksdagen/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries/member_of_parliament.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries/minister.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries/person.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries/speaker.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/member_of_parliament.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/member_of_parliament.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/minister.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/minister.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/name_location_specifier.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/name_location_specifier.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/party_affiliation.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/party_affiliation.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/person.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/person.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/speaker.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/speaker.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/data/queries_backup/twitter.rq` & `pyriksdagen-0.8.0/pyriksdagen/data/queries_backup/twitter.rq`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/dataset.py` & `pyriksdagen-0.8.0/pyriksdagen/dataset.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/db.py` & `pyriksdagen-0.8.0/pyriksdagen/db.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/download.py` & `pyriksdagen-0.8.0/pyriksdagen/download.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/export.py` & `pyriksdagen-0.8.0/pyriksdagen/export.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/match_mp.py` & `pyriksdagen-0.8.0/pyriksdagen/match_mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/metadata.py` & `pyriksdagen-0.8.0/pyriksdagen/metadata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/mp.py` & `pyriksdagen-0.8.0/pyriksdagen/mp.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/refine.py` & `pyriksdagen-0.8.0/pyriksdagen/refine.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/segmentation.py` & `pyriksdagen-0.8.0/pyriksdagen/segmentation.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/utils.py` & `pyriksdagen-0.8.0/pyriksdagen/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/pyriksdagen/wikidata.py` & `pyriksdagen-0.8.0/pyriksdagen/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyriksdagen-0.4.0/setup.py` & `pyriksdagen-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,31 @@
 {'': ['*'], 'pyriksdagen': ['data/queries/*', 'data/queries_backup/*']}
 
 install_requires = \
 ['SPARQLWrapper',
  'base58',
  'beautifulsoup4',
  'dateparser',
+ 'importlib_resources',
  'kblab-client',
  'lxml',
  'matplotlib',
  'numpy',
  'pandas',
  'progressbar2',
  'pyparlaclarin',
  'requests',
  'tqdm',
  'unidecode']
 
 setup_kwargs = {
     'name': 'pyriksdagen',
-    'version': '0.4.0',
+    'version': '0.8.0',
     'description': 'Access the Riksdagen corpus',
-    'long_description': '[![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)\n[![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)\n[![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)\n\n# Swedish parliamentary proceedings - Riksdagens protokoll 1920-2021\n\n_Westac Project, 2020-2021_\n\nThe full data set consists of multiple parts:\n\n- Riksdagens protokoll between from 1920 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format\n- Comprehensive list of MPs and cabinet members during this period\n- [Documentation](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/) of the corpus and the curation process\n- [A Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing) that demonstrates how the dataset can be used with Python\n\n## Basic use\n\nA full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/download/v0.4.3/corpus-0.4.3.zip). It has the following structure\n\n- Annual protocol files in the ```corpus/protocols/``` folder\n- Structured metadata on MPs, speakers, ministers, and governments in the ```corpus/metadata/``` folder\n\nThe workflow to use the data is demonstrated in [this Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing).\n\n## Design choices of the project\n\nThe Riksdagen corpus is released as an iterative process, where the corpus is curated and expanded. Semantic versioning is used for the whole corpus, following the established major-minor-patch practices as they apply to data. For each major and minor release, a statistical sample is drawn, annotated and quantitatively evaluated. Errors are fixed as they are detected in order of priority. Moreover, the edit history is kept as a traceable git repository.\n\n![Estimate of mapping accuracy](https://raw.githubusercontent.com/welfare-state-analytics/riksdagen-corpus/main/input/accuracy/version_plot.png)\n\nWhile the contents of the corpus will change due to curation and expansion, we aim to keep the deliverable API, the corpus/ folder, as stable as possible. This means we avoid relocating files or folders, changing formats, changing columns in metadata files, or any other changes that might break downstream scripts. Conversely, files outside the corpus/ folder are internal to the project. End users may find utility in them but we make no effort to keep them consistent.\n\nThe data in the corpus is delivered as TEI XML files to follow established practices. The metadata is delivered as CSV files, following a normal form database structure while allowing for a legible git history. A more detailed description of the data and metadata structure and formats can be found in the README files in the corpus/ folder.\n\n## Participate in the curation process\n\nIf you find any errors, it is possible to submit corrections to them. This is documented in the [project wiki](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/Submit-corrections).\n',
+    'long_description': '[![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)\n[![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)\n[![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)\n\n# Swedish parliamentary proceedings - Riksdagens protokoll 1867-2023\n\n_Westac Project, 2020-2023_\n\nThe full data set consists of multiple parts:\n\n- Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format\n- Comprehensive list of MPs and cabinet members during this period\n- [Documentation](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/) of the corpus and the curation process\n- [A Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing) that demonstrates how the dataset can be used with Python\n\n## Basic use\n\nA full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/latest/download/corpus.zip). It has the following structure\n\n- Annual protocol files in the ```corpus/protocols/``` folder\n- Structured metadata on MPs, speakers, ministers, and governments in the ```corpus/metadata/``` folder\n\nThe workflow to use the data is demonstrated in [this Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing).\n\n## Design choices of the project\n\nThe Riksdagen corpus is released as an iterative process, where the corpus is curated and expanded. Semantic versioning is used for the whole corpus, following the established major-minor-patch practices as they apply to data. For each major and minor release, a statistical sample is drawn, annotated and quantitatively evaluated. Errors are fixed as they are detected in order of priority. Moreover, the edit history is kept as a traceable git repository.\n\n![Estimate of mapping accuracy](https://raw.githubusercontent.com/welfare-state-analytics/riksdagen-corpus/main/input/accuracy/version_plot.png)\n\nWhile the contents of the corpus will change due to curation and expansion, we aim to keep the deliverable API, the corpus/ folder, as stable as possible. This means we avoid relocating files or folders, changing formats, changing columns in metadata files, or any other changes that might break downstream scripts. Conversely, files outside the corpus/ folder are internal to the project. End users may find utility in them but we make no effort to keep them consistent.\n\nThe data in the corpus is delivered as TEI XML files to follow established practices. The metadata is delivered as CSV files, following a normal form database structure while allowing for a legible git history. A more detailed description of the data and metadata structure and formats can be found in the README files in the corpus/ folder.\n\n## Participate in the curation process\n\nIf you find any errors, it is possible to submit corrections to them. This is documented in the [project wiki](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/Submit-corrections).\n',
     'author': 'ninpnin',
     'author_email': 'vainoyrjanainen@icloud.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/welfare-state-analytics/riksdagen-corpus',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pyriksdagen-0.4.0/PKG-INFO` & `pyriksdagen-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksdagen
-Version: 0.4.0
+Version: 0.8.0
 Summary: Access the Riksdagen corpus
 Home-page: https://github.com/welfare-state-analytics/riksdagen-corpus
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: SPARQLWrapper
 Requires-Dist: base58
 Requires-Dist: beautifulsoup4
 Requires-Dist: dateparser
+Requires-Dist: importlib_resources
 Requires-Dist: kblab-client
 Requires-Dist: lxml
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: progressbar2
 Requires-Dist: pyparlaclarin
@@ -30,28 +31,28 @@
 Project-URL: Repository, https://github.com/welfare-state-analytics/riksdagen-corpus
 Description-Content-Type: text/markdown
 
 [![Check unchanged](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/check_unchanged.yml)
 [![Unit tests](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/push.yml)
 [![Validate Parla-Clarin XML](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml/badge.svg)](https://github.com/welfare-state-analytics/riksdagen-corpus/actions/workflows/validate.yml)
 
-# Swedish parliamentary proceedings - Riksdagens protokoll 1920-2021
+# Swedish parliamentary proceedings - Riksdagens protokoll 1867-2023
 
-_Westac Project, 2020-2021_
+_Westac Project, 2020-2023_
 
 The full data set consists of multiple parts:
 
-- Riksdagens protokoll between from 1920 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
+- Riksdagens protokoll between from 1867 until today in the [Parla-clarin](https://github.com/clarin-eric/parla-clarin) format
 - Comprehensive list of MPs and cabinet members during this period
 - [Documentation](https://github.com/welfare-state-analytics/riksdagen-corpus/wiki/) of the corpus and the curation process
 - [A Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing) that demonstrates how the dataset can be used with Python
 
 ## Basic use
 
-A full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/download/v0.4.3/corpus-0.4.3.zip). It has the following structure
+A full dataset is available under [this download link](https://github.com/welfare-state-analytics/riksdagen-corpus/releases/latest/download/corpus.zip). It has the following structure
 
 - Annual protocol files in the ```corpus/protocols/``` folder
 - Structured metadata on MPs, speakers, ministers, and governments in the ```corpus/metadata/``` folder
 
 The workflow to use the data is demonstrated in [this Google Colab notebook](https://colab.research.google.com/drive/1C3e2gwi9z83ikXbYXNPfB6RF7spTgzxA?usp=sharing).
 
 ## Design choices of the project
```

