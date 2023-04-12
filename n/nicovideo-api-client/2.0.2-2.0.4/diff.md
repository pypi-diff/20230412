# Comparing `tmp/nicovideo_api_client-2.0.2.tar.gz` & `tmp/nicovideo_api_client-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nicovideo_api_client-2.0.2.tar", max compression
+gzip compressed data, was "nicovideo_api_client-2.0.4.tar", max compression
```

## Comparing `nicovideo_api_client-2.0.2.tar` & `nicovideo_api_client-2.0.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1593 2023-01-17 03:09:32.411564 nicovideo_api_client-2.0.2/README.md
--rw-r--r--   0        0        0        0 2023-01-17 03:09:32.412973 nicovideo_api_client-2.0.2/nicovideo_api_client/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 03:09:32.413065 nicovideo_api_client-2.0.2/nicovideo_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 03:09:32.413162 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/__init__.py
--rw-r--r--   0        0        0      843 2023-01-17 03:09:32.413247 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/field.py
--rw-r--r--   0        0        0     1892 2023-01-17 03:09:32.413334 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/filter.py
--rw-r--r--   0        0        0     5731 2023-01-17 03:09:32.413446 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/json_filter.py
--rw-r--r--   0        0        0      734 2023-01-17 03:09:32.413528 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/limit.py
--rw-r--r--   0        0        0     4143 2023-01-17 03:09:32.413626 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/request.py
--rw-r--r--   0        0        0     4006 2023-01-17 03:09:32.413725 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/result.py
--rw-r--r--   0        0        0     5749 2023-01-17 03:09:32.413846 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/simple_filter.py
--rw-r--r--   0        0        0     3951 2023-01-17 03:09:32.413956 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/snapshot_search_api_v2.py
--rw-r--r--   0        0        0      882 2023-01-17 03:09:32.414082 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/sort.py
--rw-r--r--   0        0        0     5716 2023-01-17 03:09:32.414189 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/targets.py
--rw-r--r--   0        0        0     1342 2023-01-17 03:09:32.414289 nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/user_agent.py
--rw-r--r--   0        0        0     2833 2023-01-17 03:09:32.414381 nicovideo_api_client-2.0.2/nicovideo_api_client/constants.py
--rw-r--r--   0        0        0     1380 2023-03-13 03:40:28.857131 nicovideo_api_client-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2472 1970-01-01 00:00:00.000000 nicovideo_api_client-2.0.2/setup.py
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 nicovideo_api_client-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1593 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/__init__.py
+-rw-r--r--   0        0        0      843 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/field.py
+-rw-r--r--   0        0        0     1892 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/filter.py
+-rw-r--r--   0        0        0     5731 2023-04-12 09:46:31.509125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/json_filter.py
+-rw-r--r--   0        0        0      734 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/limit.py
+-rw-r--r--   0        0        0     4143 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/request.py
+-rw-r--r--   0        0        0     4006 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/result.py
+-rw-r--r--   0        0        0     5749 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/simple_filter.py
+-rw-r--r--   0        0        0     3951 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/snapshot_search_api_v2.py
+-rw-r--r--   0        0        0      882 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/sort.py
+-rw-r--r--   0        0        0     5716 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/targets.py
+-rw-r--r--   0        0        0     1342 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/user_agent.py
+-rw-r--r--   0        0        0     2833 2023-04-12 09:46:31.513125 nicovideo_api_client-2.0.4/nicovideo_api_client/constants.py
+-rw-r--r--   0        0        0     1446 2023-04-12 09:46:50.494626 nicovideo_api_client-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 nicovideo_api_client-2.0.4/PKG-INFO
```

### Comparing `nicovideo_api_client-2.0.2/README.md` & `nicovideo_api_client-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/field.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/field.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/filter.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/filter.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/json_filter.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/json_filter.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/limit.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/limit.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/request.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/request.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/result.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/result.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/simple_filter.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/simple_filter.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/snapshot_search_api_v2.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/snapshot_search_api_v2.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/sort.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/sort.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/targets.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/targets.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/api/v2/user_agent.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/api/v2/user_agent.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/nicovideo_api_client/constants.py` & `nicovideo_api_client-2.0.4/nicovideo_api_client/constants.py`

 * *Files identical despite different names*

### Comparing `nicovideo_api_client-2.0.2/pyproject.toml` & `nicovideo_api_client-2.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nicovideo_api_client"
-version = "2.0.2"
+version = "2.0.4"
 description = "ニコニコ動画 スナップショット検索APIv2の Python クライアント"
 authors = ["Javakky <iemura.java@gmail.com>"]
 homepage = "https://github.com/Javakky/NicoApiClient"
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python",
@@ -46,7 +46,11 @@
 [tool.black]
 line-length = 120
 
 [tool.isort]
 include_trailing_comma = true
 line_length = 120
 multi_line_output = 3
+
+[tool.poetry-dynamic-versioning]
+enable = false
+style = "pep440"
```

### Comparing `nicovideo_api_client-2.0.2/setup.py` & `nicovideo_api_client-2.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,65 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nicovideo-api-client
+Version: 2.0.4
+Summary: ニコニコ動画 スナップショット検索APIv2の Python クライアント
+Home-page: https://github.com/Javakky/NicoApiClient
+Author: Javakky
+Author-email: iemura.java@gmail.com
+Requires-Python: >=3.10.2,<4.0.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.6,<2.0.0)
+Description-Content-Type: text/markdown
+
+# NicoApiClient
+
+## 概要
+[ニコニコ動画 『スナップショット検索API v2』](https://site.nicovideo.jp/search-api-docs/snapshot) などの API について、仕様をなるべく意識せずに利用できるクライアントを提供する。
+
+## install
+
+PyPIリポジトリ: https://pypi.org/project/nicovideo-api-client/
+
+```shell
+pip install nicovideo-api-client
+```
+
+### installed
+
+[![Downloads](https://pepy.tech/badge/nicovideo-api-client)](https://pepy.tech/project/nicovideo-api-client) [![Downloads](https://pepy.tech/badge/nicovideo-api-client/month)](https://pepy.tech/project/nicovideo-api-client) [![Downloads](https://pepy.tech/badge/nicovideo-api-client/week)](https://pepy.tech/project/nicovideo-api-client)
+
+## Code Climate
+
+[![Maintainability](https://api.codeclimate.com/v1/badges/9d090928fdb99bf5fa06/maintainability)](https://codeclimate.com/github/Javakky/NicoApiClient/maintainability)
+
+### documentation
+
+[NicoApiClient コードドキュメント](https://javakky.github.io/NicoApiClientDocs/)
+
+## example
+
+```python
+from nicovideo_api_client.api.v2.snapshot_search_api_v2 import SnapshotSearchAPIV2
+from nicovideo_api_client.constants import FieldType
+
+json = SnapshotSearchAPIV2() \
+    .tags_exact() \
+    .single_query("VOCALOID") \
+    .field({FieldType.TITLE, FieldType.CONTENT_ID}) \
+    .sort(FieldType.VIEW_COUNTER) \
+    .no_filter() \
+    .limit(100) \
+    .user_agent("NicoApiClient", "0.5.0") \
+    .request() \
+    .json()
+```
 
-packages = \
-['nicovideo_api_client',
- 'nicovideo_api_client.api',
- 'nicovideo_api_client.api.v2']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.26.0,<3.0.0', 'urllib3>=1.26.6,<2.0.0']
-
-setup_kwargs = {
-    'name': 'nicovideo-api-client',
-    'version': '2.0.2',
-    'description': 'ニコニコ動画 スナップショット検索APIv2の Python クライアント',
-    'long_description': '# NicoApiClient\n\n## 概要\n[ニコニコ動画 『スナップショット検索API v2』](https://site.nicovideo.jp/search-api-docs/snapshot) などの API について、仕様をなるべく意識せずに利用できるクライアントを提供する。\n\n## install\n\nPyPIリポジトリ: https://pypi.org/project/nicovideo-api-client/\n\n```shell\npip install nicovideo-api-client\n```\n\n### installed\n\n[![Downloads](https://pepy.tech/badge/nicovideo-api-client)](https://pepy.tech/project/nicovideo-api-client) [![Downloads](https://pepy.tech/badge/nicovideo-api-client/month)](https://pepy.tech/project/nicovideo-api-client) [![Downloads](https://pepy.tech/badge/nicovideo-api-client/week)](https://pepy.tech/project/nicovideo-api-client)\n\n## Code Climate\n\n[![Maintainability](https://api.codeclimate.com/v1/badges/9d090928fdb99bf5fa06/maintainability)](https://codeclimate.com/github/Javakky/NicoApiClient/maintainability)\n\n### documentation\n\n[NicoApiClient コードドキュメント](https://javakky.github.io/NicoApiClientDocs/)\n\n## example\n\n```python\nfrom nicovideo_api_client.api.v2.snapshot_search_api_v2 import SnapshotSearchAPIV2\nfrom nicovideo_api_client.constants import FieldType\n\njson = SnapshotSearchAPIV2() \\\n    .tags_exact() \\\n    .single_query("VOCALOID") \\\n    .field({FieldType.TITLE, FieldType.CONTENT_ID}) \\\n    .sort(FieldType.VIEW_COUNTER) \\\n    .no_filter() \\\n    .limit(100) \\\n    .user_agent("NicoApiClient", "0.5.0") \\\n    .request() \\\n    .json()\n```\n\n## 利用規約\n\nhttps://site.nicovideo.jp/search-api-docs/snapshot#api%E5%88%A9%E7%94%A8%E8%A6%8F%E7%B4%84\n',
-    'author': 'Javakky',
-    'author_email': 'iemura.java@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Javakky/NicoApiClient',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10.2,<4.0.0',
-}
+## 利用規約
 
+https://site.nicovideo.jp/search-api-docs/snapshot#api%E5%88%A9%E7%94%A8%E8%A6%8F%E7%B4%84
 
-setup(**setup_kwargs)
```

