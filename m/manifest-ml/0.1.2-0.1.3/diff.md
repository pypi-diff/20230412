# Comparing `tmp/manifest-ml-0.1.2.tar.gz` & `tmp/manifest-ml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifest-ml-0.1.2.tar", last modified: Sat Apr  8 21:13:25 2023, max compression
+gzip compressed data, was "manifest-ml-0.1.3.tar", last modified: Wed Apr 12 20:14:11 2023, max compression
```

## Comparing `manifest-ml-0.1.2.tar` & `manifest-ml-0.1.3.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.651185 manifest-ml-0.1.2/
--rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/LICENSE
--rw-r--r--   0 laurelorr   (501) staff       (20)     6955 2023-04-08 21:13:25.651064 manifest-ml-0.1.2/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     6267 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/README.md
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.643382 manifest-ml-0.1.2/manifest/
--rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/__init__.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.643922 manifest-ml-0.1.2/manifest/api/
--rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/api/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8339 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/app.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.644859 manifest-ml-0.1.2/manifest/api/models/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/api/models/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3991 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/models/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    22438 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/models/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2839 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/models/model.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1612 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/api/response.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.646159 manifest-ml-0.1.2/manifest/caches/
--rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3420 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/caches/cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/noop.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/caches/postgres.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/redis.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3825 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/serializers.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/caches/sqlite.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.648139 manifest-ml-0.1.2/manifest/clients/
--rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/manifest/clients/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3298 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/ai21.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    11662 2023-04-08 20:45:20.000000 manifest-ml-0.1.2/manifest/clients/client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3458 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/cohere.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2780 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3738 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/dummy.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3424 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/clients/huggingface.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     3966 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/openai.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5109 2023-04-08 20:44:48.000000 manifest-ml-0.1.2/manifest/clients/openaichat.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5159 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/toma.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1943 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/clients/toma_diffuser.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    17517 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2730 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/manifest/request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     7351 2023-03-27 02:06:27.000000 manifest-ml-0.1.2/manifest/response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-04-08 19:58:13.000000 manifest-ml-0.1.2/manifest/version.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.648727 manifest-ml-0.1.2/manifest_ml.egg-info/
--rw-r--r--   0 laurelorr   (501) staff       (20)     6955 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/PKG-INFO
--rw-r--r--   0 laurelorr   (501) staff       (20)     1291 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/SOURCES.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/dependency_links.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)     1557 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/requires.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-04-08 21:13:25.000000 manifest-ml-0.1.2/manifest_ml.egg-info/top_level.txt
--rw-r--r--   0 laurelorr   (501) staff       (20)      759 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/pyproject.toml
--rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-04-08 21:13:25.651229 manifest-ml-0.1.2/setup.cfg
--rw-r--r--   0 laurelorr   (501) staff       (20)     5309 2023-04-08 20:03:25.000000 manifest-ml-0.1.2/setup.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.650443 manifest-ml-0.1.2/tests/
--rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/tests/test_array_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     6833 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_cache.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     2053 2023-04-08 20:44:48.000000 manifest-ml-0.1.2/tests/test_client.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     8101 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_huggingface_api.py
--rw-r--r--   0 laurelorr   (501) staff       (20)    25170 2023-04-08 20:44:57.000000 manifest-ml-0.1.2/tests/test_manifest.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_request.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     5756 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/tests/test_response.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      531 2023-03-12 04:05:54.000000 manifest-ml-0.1.2/tests/test_serializer.py
-drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-08 21:13:25.650864 manifest-ml-0.1.2/web_app/
--rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/web_app/__init__.py
--rw-r--r--   0 laurelorr   (501) staff       (20)     1733 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/web_app/main.py
--rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.2/web_app/schemas.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.040597 manifest-ml-0.1.3/
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11357 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/LICENSE
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8190 2023-04-12 20:14:11.040463 manifest-ml-0.1.3/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     7502 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/README.md
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.032367 manifest-ml-0.1.3/manifest/
+-rw-r--r--   0 laurelorr   (501) staff       (20)      183 2023-03-12 04:05:54.000000 manifest-ml-0.1.3/manifest/__init__.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.033006 manifest-ml-0.1.3/manifest/api/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       16 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/api/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8947 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/app.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.033971 manifest-ml-0.1.3/manifest/api/models/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/api/models/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4383 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    23121 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2798 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/model.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3880 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/models/sentence_transformer.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1801 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/api/response.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.035386 manifest-ml-0.1.3/manifest/caches/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       18 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3725 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     4463 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/caches/cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1131 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/noop.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3944 2023-03-12 04:05:54.000000 manifest-ml-0.1.3/manifest/caches/postgres.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1716 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/redis.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5773 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/caches/serializers.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1772 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/caches/sqlite.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.037502 manifest-ml-0.1.3/manifest/clients/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       19 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/manifest/clients/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3301 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/ai21.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    11825 2023-04-12 19:53:13.000000 manifest-ml-0.1.3/manifest/clients/client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3459 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/cohere.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2819 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3738 2023-03-27 02:06:27.000000 manifest-ml-0.1.3/manifest/clients/dummy.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3463 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/huggingface.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2334 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/huggingface_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     3997 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/openai.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5132 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/openai_chat.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     6558 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/openai_embedding.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5162 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/toma.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1938 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/clients/toma_diffuser.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    17784 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2811 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     7558 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/manifest/response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)       22 2023-04-12 20:13:56.000000 manifest-ml-0.1.3/manifest/version.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.038214 manifest-ml-0.1.3/manifest_ml.egg-info/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     8190 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/PKG-INFO
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1415 2023-04-12 20:14:11.000000 manifest-ml-0.1.3/manifest_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)        1 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1615 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/requires.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)       17 2023-04-12 20:14:10.000000 manifest-ml-0.1.3/manifest_ml.egg-info/top_level.txt
+-rw-r--r--   0 laurelorr   (501) staff       (20)      786 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/pyproject.toml
+-rw-r--r--   0 laurelorr   (501) staff       (20)       38 2023-04-12 20:14:11.040650 manifest-ml-0.1.3/setup.cfg
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5349 2023-04-12 20:13:43.000000 manifest-ml-0.1.3/setup.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.039721 manifest-ml-0.1.3/tests/
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2275 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/tests/test_array_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9111 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_cache.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     2053 2023-04-08 21:15:06.000000 manifest-ml-0.1.3/tests/test_client.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     9132 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_huggingface_api.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)    31611 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_manifest.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1949 2023-03-12 04:05:54.000000 manifest-ml-0.1.3/tests/test_request.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     5756 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/tests/test_response.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      997 2023-04-09 06:56:02.000000 manifest-ml-0.1.3/tests/test_serializer.py
+drwxr-xr-x   0 laurelorr   (501) staff       (20)        0 2023-04-12 20:14:11.040181 manifest-ml-0.1.3/web_app/
+-rw-r--r--   0 laurelorr   (501) staff       (20)       36 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/web_app/__init__.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)     1733 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/web_app/main.py
+-rw-r--r--   0 laurelorr   (501) staff       (20)      721 2023-02-14 19:01:23.000000 manifest-ml-0.1.3/web_app/schemas.py
```

### Comparing `manifest-ml-0.1.2/LICENSE` & `manifest-ml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/PKG-INFO` & `manifest-ml-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifest-ml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Manifest for Prompting Foundation Models.
 Home-page: https://github.com/HazyResearch/manifest
 Author: Laurel Orr
 Author-email: laurel.orr@numbersstation.ai
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -27,14 +27,15 @@
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
+- [Embedding Models](#embedding-models)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
 ```bash
@@ -67,14 +68,17 @@
 # Start a manifest session to OpenAI - default `engine=text-davinci-002`
 manifest = Manifest(
     client_name = "openai",
 )
 manifest.run("Why is the grass green?")
 ```
 
+## Examples
+We have example notebook and python scripts located at [examples](examples). These show how to use different models, model types (i.e. text, diffusers, or embedding models), and async running.
+
 # Manifest Components
 Manifest is meant to be a very light weight package to help with prompt design and iteration. Three key design decisions of Manifest are
 
 * All models are behind APIs
 * Supports caching of model inputs/outputs for iteration, reproducibility, and cost saving
 * Unified API of generate, score, and embed
 
@@ -132,14 +136,20 @@
 ```
 
 You can also run over multiple examples if supported by the client.
 ```python
 results = manifest.run(["Where are the cats?", "Where are the dogs?"])
 ```
 
+We support async queries as well via
+```python
+import asyncio
+results = asyncio.run(manifest.arun_batch(["Where are the cats?", "Where are the dogs?"]))
+```
+
 If something doesn't go right, you can also ask to get a raw manifest Response.
 ```python
 result_object = manifest.run(["Where are the cats?", "Where are the dogs?"], return_response=True)
 print(result_object.get_request())
 print(result_object.is_cached())
 print(result_object.get_json_response())
 ```
@@ -198,14 +208,31 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
+# Embedding Models
+Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
+
+To use OpenAI's embedding models, simply run
+```python
+manifest = Manifest(client_name="openaiembedding")
+embedding_as_np = manifest.run("Get me an embedding for a bunny")
+```
+
+As explained above, you can load local HuggingFace models that give you embeddings, too. If you want to use a standard generative model, load the model as above use use `client_name="huggingfaceembedding"`. If you want to use a standard embedding model, like those from SentenceTransformers, load your local model via
+```bash
+python3 -m manifest.api.app \
+    --model_type sentence_transformers \
+    --model_name_or_path all-mpnet-base-v2 \
+    --device 0
+```
+
 # Development
 Before submitting a PR, run
 ```bash
 export REDIS_PORT="6379"  # or whatever PORT local redis is running for those tests
 cd <REDIS_PATH>
 docker run -d -p 127.0.0.1:${REDIS_PORT}:6379 -v `pwd`:`pwd` -w `pwd` --name manifest_redis_test redis
 make test
```

### Comparing `manifest-ml-0.1.2/README.md` & `manifest-ml-0.1.3/manifest_ml.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,41 @@
+Metadata-Version: 2.1
+Name: manifest-ml
+Version: 0.1.3
+Summary: Manifest for Prompting Foundation Models.
+Home-page: https://github.com/HazyResearch/manifest
+Author: Laurel Orr
+Author-email: laurel.orr@numbersstation.ai
+License: Apache 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: api
+Provides-Extra: app
+Provides-Extra: diffusers
+Provides-Extra: gcp
+Provides-Extra: dev
+Provides-Extra: all
+License-File: LICENSE
+
+
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
+- [Embedding Models](#embedding-models)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
 ```bash
@@ -43,14 +68,17 @@
 # Start a manifest session to OpenAI - default `engine=text-davinci-002`
 manifest = Manifest(
     client_name = "openai",
 )
 manifest.run("Why is the grass green?")
 ```
 
+## Examples
+We have example notebook and python scripts located at [examples](examples). These show how to use different models, model types (i.e. text, diffusers, or embedding models), and async running.
+
 # Manifest Components
 Manifest is meant to be a very light weight package to help with prompt design and iteration. Three key design decisions of Manifest are
 
 * All models are behind APIs
 * Supports caching of model inputs/outputs for iteration, reproducibility, and cost saving
 * Unified API of generate, score, and embed
 
@@ -108,14 +136,20 @@
 ```
 
 You can also run over multiple examples if supported by the client.
 ```python
 results = manifest.run(["Where are the cats?", "Where are the dogs?"])
 ```
 
+We support async queries as well via
+```python
+import asyncio
+results = asyncio.run(manifest.arun_batch(["Where are the cats?", "Where are the dogs?"]))
+```
+
 If something doesn't go right, you can also ask to get a raw manifest Response.
 ```python
 result_object = manifest.run(["Where are the cats?", "Where are the dogs?"], return_response=True)
 print(result_object.get_request())
 print(result_object.is_cached())
 print(result_object.get_json_response())
 ```
@@ -174,14 +208,31 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
+# Embedding Models
+Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
+
+To use OpenAI's embedding models, simply run
+```python
+manifest = Manifest(client_name="openaiembedding")
+embedding_as_np = manifest.run("Get me an embedding for a bunny")
+```
+
+As explained above, you can load local HuggingFace models that give you embeddings, too. If you want to use a standard generative model, load the model as above use use `client_name="huggingfaceembedding"`. If you want to use a standard embedding model, like those from SentenceTransformers, load your local model via
+```bash
+python3 -m manifest.api.app \
+    --model_type sentence_transformers \
+    --model_name_or_path all-mpnet-base-v2 \
+    --device 0
+```
+
 # Development
 Before submitting a PR, run
 ```bash
 export REDIS_PORT="6379"  # or whatever PORT local redis is running for those tests
 cd <REDIS_PATH>
 docker run -d -p 127.0.0.1:${REDIS_PORT}:6379 -v `pwd`:`pwd` -w `pwd` --name manifest_redis_test redis
 make test
@@ -194,7 +245,9 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
+
+
```

### Comparing `manifest-ml-0.1.2/manifest/api/app.py` & `manifest-ml-0.1.3/manifest/api/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,28 @@
 
 from manifest.api.models.diffuser import DiffuserModel
 from manifest.api.models.huggingface import (
     MODEL_GENTYPE_REGISTRY,
     CrossModalEncoderModel,
     TextGenerationModel,
 )
+from manifest.api.models.sentence_transformer import SentenceTransformerModel
 from manifest.api.response import ModelResponse
 
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 logger = logging.getLogger(__name__)
 app = Flask(__name__)  # define app using Flask
 # Will be global
 model = None
 model_type = None
 PORT = int(os.environ.get("FLASK_PORT", 5000))
 MODEL_CONSTRUCTORS = {
     "huggingface": TextGenerationModel,
+    "sentence_transformers": SentenceTransformerModel,
     "huggingface_crossmodal": CrossModalEncoderModel,
     "diffuser": DiffuserModel,
 }
 
 
 def parse_args() -> argparse.Namespace:
     """Generate args."""
@@ -194,39 +196,59 @@
         return Response(
             json.dumps({"message": str(e)}),
             status=400,
         )
 
 
 @app.route("/embed", methods=["POST"])
-def embed() -> Dict:
+def embed() -> Response:
     """Get embed for generation."""
-    modality = request.json["modality"]
+    if "modality" in request.json:
+        modality = request.json["modality"]
+    else:
+        modality = "text"
     if modality == "text":
-        prompts = request.json["prompts"]
+        prompts = request.json["prompt"]
     elif modality == "image":
         import base64
 
         from PIL import Image
 
         prompts = [
             Image.open(io.BytesIO(base64.b64decode(data)))
-            for data in request.json["prompts"]
+            for data in request.json["prompt"]
         ]
     else:
         raise ValueError("modality must be text or image")
 
-    results = []
-    embeddings = model.embed(prompts)
-    for embedding in embeddings:
-        results.append(embedding.tolist())
-
-    # transform the result into the openai format
-    # return Response(results, response_type="text_completion").__dict__()
-    return {"result": results}
+    try:
+        results = []
+        embeddings = model.embed(prompts)
+        for embedding in embeddings:
+            results.append(
+                {
+                    "array": embedding,
+                    "logprob": None,
+                    "tokens": None,
+                    "token_logprobs": None,
+                }
+            )
+
+        return Response(
+            json.dumps(
+                ModelResponse(results, response_type="embedding_generation").__dict__()
+            ),
+            status=200,
+        )
+    except Exception as e:
+        logger.error(e)
+        return Response(
+            json.dumps({"message": str(e)}),
+            status=400,
+        )
 
 
 @app.route("/score_sequence", methods=["POST"])
 def score_sequence() -> Response:
     """Get logprob of prompt."""
     prompt = request.json["prompt"]
     del request.json["prompt"]
```

### Comparing `manifest-ml-0.1.2/manifest/api/models/diffuser.py` & `manifest-ml-0.1.3/manifest/api/models/diffuser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""Huggingface model."""
+"""Diffuser model."""
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import torch
 from diffusers import StableDiffusionPipeline
 
 from manifest.api.models.model import Model
 
 
 class DiffuserModel(Model):
@@ -90,14 +91,27 @@
         if isinstance(prompt, str):
             prompt = [prompt]
         result = self.pipeline(prompt, output_type="np.array", **kwargs)
         # Return None for logprobs and token logprobs
         return [(im, None, None, None) for im in result["images"]]
 
     @torch.no_grad()
+    def embed(self, prompt: Union[str, List[str]], **kwargs: Any) -> np.ndarray:
+        """
+        Embed the prompt from model.
+
+        Args:
+            prompt: promt to embed from.
+
+        Returns:
+            list of embeddings (list of length 1 for 1 embedding).
+        """
+        raise NotImplementedError("Embed not supported for diffusers")
+
+    @torch.no_grad()
     def score_sequence(
         self, prompt: Union[str, List[str]], **kwargs: Any
     ) -> List[Tuple[float, List[int], List[float]]]:
         """
         Score a sequence of choices.
 
         Args:
```

### Comparing `manifest-ml-0.1.2/manifest/api/models/huggingface.py` & `manifest-ml-0.1.3/manifest/api/models/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -531,23 +531,40 @@
             bitsandbytes=use_bitsandbytes,
             is_encdec=self.is_encdec,
         )
 
     @torch.no_grad()
     def embed(self, prompt: Union[str, List[str]], **kwargs: Any) -> np.ndarray:
         """
-        Compute embedding for prompts.
+        Embed the prompt from model.
 
         Args:
-            prompt: promt to generate from.
+            prompt: promt to embed from.
 
         Returns:
-            embedding
+            list of embeddings (list of length 1 for 1 embedding).
         """
-        pass
+        if isinstance(prompt, str):
+            prompt = [prompt]
+        encoded_prompt = self.pipeline.tokenizer(
+            prompt,
+            max_length=self.pipeline.max_length,
+            truncation=True,
+            padding=True,
+            return_tensors="pt",
+        )
+        encoded_prompt = encoded_prompt.to(self.pipeline.device)
+        # Get last hidden state
+        output = self.pipeline.model(  # type: ignore
+            **encoded_prompt,
+            output_hidden_states=True,
+            return_dict=True,
+        )
+        last_hidden_state = output["hidden_states"][-1][:, -1, :]
+        return last_hidden_state.cpu().numpy()
 
     @torch.no_grad()
     def generate(
         self, prompt: Union[str, List[str]], **kwargs: Any
     ) -> List[Tuple[Any, float, List[int], List[float]]]:
         """
         Generate the prompt from model.
```

### Comparing `manifest-ml-0.1.2/manifest/api/models/model.py` & `manifest-ml-0.1.3/manifest/api/models/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Model class."""
-from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 
 
-class Model(ABC):
+class Model:
     """Model class."""
 
-    @abstractmethod
     def __init__(
         self,
         model_name_or_path: str,
         model_type: str,
         cache_dir: str,
         device: int,
         use_accelerate: bool,
@@ -37,15 +35,14 @@
             use_bitsandbytes: use HF bits and bytes
             use_deepspeed: use deepspeed
             perc_max_gpu_mem_red: percent max memory reduction in accelerate
             use_fp16: use fp16 for model weights.
         """
         raise NotImplementedError()
 
-    @abstractmethod
     def get_init_params(self) -> Dict:
         """Return init params to determine what model is being used."""
         raise NotImplementedError()
 
     def generate(
         self, prompt: Union[str, List[str]], **kwargs: Any
     ) -> List[Tuple[Any, float, List[int], List[float]]]:
@@ -62,21 +59,21 @@
             Each item is the response, answer logprob, list of tokens,
             and list of logprobs for each token.
         """
         raise NotImplementedError()
 
     def embed(self, prompt: Union[str, List[str]], **kwargs: Any) -> np.ndarray:
         """
-        Compute embedding for prompts.
+        Embed the prompt from model.
 
         Args:
-            prompt: promt to generate from.
+            prompt: promt to embed from.
 
         Returns:
-            embedding
+            list of embeddings (list of length 1 for 1 embedding).
         """
         raise NotImplementedError()
 
     def score_sequence(
         self, prompt: Union[str, List[str]], **kwargs: Any
     ) -> List[Tuple[float, List[int], List[float]]]:
         """
```

### Comparing `manifest-ml-0.1.2/manifest/api/response.py` & `manifest-ml-0.1.3/manifest/api/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,32 @@
         """Initialize response."""
         self.results = results
         self.response_type = response_type
         if self.response_type not in {
             "text_completion",
             "prompt_logit_score",
             "image_generation",
+            "embedding_generation",
         }:
             raise ValueError(
                 f"Invalid response type: {self.response_type}. "
-                "Must be one of: text_completion, prompt_logit_score, image_generation."
+                "Must be one of: text_completion, prompt_logit_score, "
+                "image_generation, embedding_generation."
             )
         self.response_id = str(uuid.uuid4())
         self.created = int(time.time())
 
     def __dict__(self) -> Dict[str, Any]:  # type: ignore
         """Return dictionary representation of response."""
-        key = "text" if self.response_type != "image_generation" else "array"
+        key = (
+            "text"
+            if self.response_type
+            not in {"prompt_logit_score", "image_generation", "embedding_generation"}
+            else "array"
+        )
         return {
             "id": self.response_id,
             "object": self.response_type,
             "created": self.created,
             "model": "flask_model",
             "choices": [
                 {
```

### Comparing `manifest-ml-0.1.2/manifest/caches/array_cache.py` & `manifest-ml-0.1.3/manifest/caches/array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/manifest/caches/cache.py` & `manifest-ml-0.1.3/manifest/caches/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,71 @@
 """Cache for queries and responses."""
 from abc import ABC, abstractmethod
 from typing import Any, Dict, Union
 
-from manifest.caches.serializers import ArraySerializer, Serializer
+from manifest.caches.serializers import ArraySerializer, NumpyByteSerializer, Serializer
 from manifest.response import RESPONSE_CONSTRUCTORS, Response
 
-CACHE_CONSTRUCTOR = {
-    "diffuser": ArraySerializer,
-    "tomadiffuser": ArraySerializer,
+# Non-text return type caches
+ARRAY_CACHE_TYPES = {
+    "diffuser",
+    "tomadiffuser",
+    "openaiembedding",
+    "huggingfaceembedding",
 }
 
 
 class Cache(ABC):
     """A cache for request/response pairs."""
 
     def __init__(
         self,
         connection_str: str,
         client_name: str = "None",
         cache_args: Dict[str, Any] = {},
     ):
         """
-        Initialize client.
+        Initialize cache.
 
         Args:
             connection_str: connection string.
             client_name: name of client.
             cache_args: arguments for cache.
 
-        cache_args are passed to client as default parameters.
+        cache_args are any arguments needed to initialize the cache.
 
-        For clients like OpenAI that do not require a connection,
-        the connection_str can be None.
+        Further, cache_args can contain `array_serializer` as a string
+        for embedding or image return types (e.g. diffusers) with values
+        as `local_file` or `byte_string`. `local_file` will save the
+        array in a local file and cache a pointer to the file.
+        `byte_string` will convert the array to a byte string and cache
+        the entire byte string. `byte_string` is default.
 
         Args:
             connection_str: connection string for client.
             cache_args: cache arguments.
         """
         self.client_name = client_name
         self.connect(connection_str, cache_args)
-        self.serializer = CACHE_CONSTRUCTOR.get(client_name, Serializer)()
+        if self.client_name in ARRAY_CACHE_TYPES:
+            array_serializer = cache_args.pop("array_serializer", "byte_string")
+            if array_serializer not in ["local_file", "byte_string"]:
+                raise ValueError(
+                    "array_serializer must be local_file or byte_string,"
+                    f" not {array_serializer}"
+                )
+            self.serializer = (
+                ArraySerializer()
+                if array_serializer == "local_file"
+                else NumpyByteSerializer()
+            )
+        else:
+            # If user has array_serializer type, it will throw an error as
+            # it is not recognized for non-array return types.
+            self.serializer = Serializer()
 
     @abstractmethod
     def close(self) -> None:
         """Close the client."""
         raise NotImplementedError()
 
     @abstractmethod
@@ -103,15 +125,15 @@
         if cached_response:
             cached = True
             response = self.serializer.key_to_response(cached_response)
             return Response(
                 response,
                 cached,
                 request,
-                **RESPONSE_CONSTRUCTORS.get(self.client_name, {})
+                **RESPONSE_CONSTRUCTORS.get(self.client_name, {}),
             )
         return None
 
     def set(self, request: Dict, response: Dict) -> None:
         """Set the value for the key.
 
         Args:
```

### Comparing `manifest-ml-0.1.2/manifest/caches/noop.py` & `manifest-ml-0.1.3/manifest/caches/noop.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/manifest/caches/postgres.py` & `manifest-ml-0.1.3/manifest/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/manifest/caches/redis.py` & `manifest-ml-0.1.3/manifest/caches/redis.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/manifest/caches/serializers.py` & `manifest-ml-0.1.3/manifest/caches/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Serializer."""
 
+import io
 import json
 import os
 from pathlib import Path
 from typing import Dict
 
+import numpy as np
 import xxhash
 
 from manifest.caches.array_cache import ArrayCache
 
 
 class Serializer:
     """Serializer."""
@@ -58,14 +60,72 @@
 
         Returns:
             unnormalized response dict.
         """
         return json.loads(key)
 
 
+class NumpyByteSerializer(Serializer):
+    """Serializer by casting array to byte string."""
+
+    def response_to_key(self, response: Dict) -> str:
+        """
+        Normalize a response into a key.
+
+        Args:
+            response: response to normalize.
+
+        Returns:
+            normalized key.
+        """
+        # Assume response is a dict with keys "choices" -> List dicts
+        # with keys "array".
+        choices = response["choices"]
+        # We don't want to modify the response in place
+        # but we want to avoid calling deepcopy on an array
+        del response["choices"]
+        response_copy = response.copy()
+        response["choices"] = choices
+        response_copy["choices"] = []
+        for choice in choices:
+            if "array" not in choice:
+                raise ValueError(
+                    f"Choice with keys {choice.keys()} does not have array key."
+                )
+            arr = choice["array"]
+            # Avoid copying an array
+            del choice["array"]
+            new_choice = choice.copy()
+            choice["array"] = arr
+            with io.BytesIO() as f:
+                np.savez_compressed(f, data=arr)
+                hash_str = f.getvalue().hex()
+            new_choice["array"] = hash_str
+            response_copy["choices"].append(new_choice)
+        return json.dumps(response_copy, sort_keys=True)
+
+    def key_to_response(self, key: str) -> Dict:
+        """
+        Convert the normalized version to the response.
+
+        Args:
+            key: normalized key to convert.
+
+        Returns:
+            unnormalized response dict.
+        """
+        response = json.loads(key)
+        for choice in response["choices"]:
+            hash_str = choice["array"]
+            byte_str = bytes.fromhex(hash_str)
+            with io.BytesIO(byte_str) as f:
+                choice["array"] = np.load(f)["data"]
+        return response
+
+
 class ArraySerializer(Serializer):
     """Serializer for array."""
 
     def __init__(self) -> None:
         """
         Initialize array serializer.
```

### Comparing `manifest-ml-0.1.2/manifest/caches/sqlite.py` & `manifest-ml-0.1.3/manifest/caches/sqlite.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/manifest/clients/ai21.py` & `manifest-ml-0.1.3/manifest/clients/ai21.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "ai21", "engine": getattr(self, "engine")}
+        return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
     def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
```

### Comparing `manifest-ml-0.1.2/manifest/clients/client.py` & `manifest-ml-0.1.3/manifest/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 """Client class."""
 import asyncio
 import copy
 import logging
 import math
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import aiohttp
 import requests
 from tenacity import RetryCallState, retry, stop_after_attempt, wait_random_exponential
 
 from manifest.request import DEFAULT_REQUEST_KEYS, NOT_CACHE_KEYS, Request
 from manifest.response import RESPONSE_CONSTRUCTORS, Response
 
 logger = logging.getLogger(__name__)
 
 
 def retry_if_ratelimit(retry_base: RetryCallState) -> bool:
     """Return whether to retry if ratelimited."""
-    if isinstance(retry_base.outcome.exception(), requests.exceptions.HTTPError):
-        if retry_base.outcome.exception().response.status_code == 429:  # type: ignore
-            return True
+    try:
+        if isinstance(retry_base.outcome.exception(), requests.exceptions.HTTPError):
+            exception = cast(
+                requests.exceptions.HTTPError, retry_base.outcome.exception()
+            )
+            if exception.response.status_code == 429:  # type: ignore
+                return True
+    except Exception:
+        pass
     return False
 
 
 class Client(ABC):
     """Client class."""
 
     # Must be overridden by child class
```

### Comparing `manifest-ml-0.1.2/manifest/clients/cohere.py` & `manifest-ml-0.1.3/manifest/clients/cohere.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "cohere", "engine": getattr(self, "engine")}
+        return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
     def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
```

### Comparing `manifest-ml-0.1.2/manifest/clients/diffuser.py` & `manifest-ml-0.1.3/manifest/clients/diffuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,17 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        res = requests.post(self.host + "/params")
-        return res.json()
+        res = requests.post(self.host + "/params").json()
+        res["client_name"] = self.NAME
+        return res
 
     def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
```

### Comparing `manifest-ml-0.1.2/manifest/clients/dummy.py` & `manifest-ml-0.1.3/manifest/clients/dummy.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/manifest/clients/huggingface.py` & `manifest-ml-0.1.3/manifest/clients/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,17 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        res = requests.post(self.host + "/params")
-        return res.json()
+        res = requests.post(self.host + "/params").json()
+        res["client_name"] = self.NAME
+        return res
 
     def get_score_prompt_request(
         self,
         request: Request,
     ) -> Response:
         """
         Get the logit score of the prompt via a forward pass of the model.
```

### Comparing `manifest-ml-0.1.2/manifest/clients/openai.py` & `manifest-ml-0.1.3/manifest/clients/openai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """OpenAI client."""
 import logging
 import os
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Type
 
 import tiktoken
 
 from manifest.clients.client import Client
-from manifest.request import LMRequest
+from manifest.request import LMRequest, Request
 
 logger = logging.getLogger(__name__)
 
 OPENAI_ENGINES = {
     "text-davinci-003",
     "text-davinci-002",
     "text-davinci-001",
@@ -37,15 +37,15 @@
         "n": ("n", 1),
         "top_p": ("top_p", 1.0),
         "top_k": ("best_of", 1),
         "stop_sequences": ("stop", None),  # OpenAI doesn't like empty lists
         "presence_penalty": ("presence_penalty", 0.0),
         "frequency_penalty": ("frequency_penalty", 0.0),
     }
-    REQUEST_CLS = LMRequest
+    REQUEST_CLS: Type[Request] = LMRequest
     NAME = "openai"
 
     def connect(
         self,
         connection_str: Optional[str] = None,
         client_args: Dict[str, Any] = {},
     ) -> None:
@@ -99,15 +99,15 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "openai", "engine": getattr(self, "engine")}
+        return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
     def split_usage(self, request: Dict, choices: List[str]) -> List[Dict[str, int]]:
         """Split usage into list of usages for each prompt."""
         try:
             encoding = tiktoken.encoding_for_model(getattr(self, "engine"))
         except Exception:
             return []
```

### Comparing `manifest-ml-0.1.2/manifest/clients/openaichat.py` & `manifest-ml-0.1.3/manifest/clients/openai_chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "openaichat", "engine": getattr(self, "engine")}
+        return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
     def _format_request_for_chat(self, request_params: Dict[str, Any]) -> Dict:
         """Format request params for chat.
 
         Args:
             request_params: request params.
 
@@ -95,16 +95,16 @@
             prompt_list = [prompt]
         else:
             prompt_list = prompt
         messages = [{"role": "user", "content": prompt} for prompt in prompt_list]
         request_params["messages"] = messages
         return request_params
 
-    def _format_request_for_text(self, response_dict: Dict[str, Any]) -> Dict:
-        """Format response for text.
+    def _format_request_from_chat(self, response_dict: Dict[str, Any]) -> Dict:
+        """Format response for standard response from chat.
 
         Args:
             response_dict: response.
 
         Return:
             formatted response.
         """
@@ -127,15 +127,15 @@
         Returns:
             response as dict.
         """
         # Format for chat model
         request_params = self._format_request_for_chat(request_params)
         response_dict = super()._run_completion(request_params, retry_timeout)
         # Reformat for text model
-        response_dict = self._format_request_for_text(response_dict)
+        response_dict = self._format_request_from_chat(response_dict)
         return response_dict
 
     async def _arun_completion(
         self, request_params: Dict[str, Any], retry_timeout: int, batch_size: int
     ) -> Dict:
         """Async execute completion request.
 
@@ -149,9 +149,9 @@
         """
         # Format for chat model
         request_params = self._format_request_for_chat(request_params)
         response_dict = await super()._arun_completion(
             request_params, retry_timeout, batch_size
         )
         # Reformat for text model
-        response_dict = self._format_request_for_text(response_dict)
+        response_dict = self._format_request_from_chat(response_dict)
         return response_dict
```

### Comparing `manifest-ml-0.1.2/manifest/clients/toma.py` & `manifest-ml-0.1.3/manifest/clients/toma.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "toma", "engine": getattr(self, "engine")}
+        return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
     def get_model_heartbeats(self) -> Dict[str, Dict]:
         """
         Get TOMA models and their last ping time.
 
         Some TOMA models are not loaded and will not response.
```

### Comparing `manifest-ml-0.1.2/manifest/clients/toma_diffuser.py` & `manifest-ml-0.1.3/manifest/clients/toma_diffuser.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         By getting model params from the server, we can add to request
         and make sure cache keys are unique to model.
 
         Returns:
             model params.
         """
-        return {"model_name": "tomadiffuser", "engine": getattr(self, "engine")}
+        return {"model_name": self.NAME, "engine": getattr(self, "engine")}
 
     def format_response(self, response: Dict, request: Dict) -> Dict[str, Any]:
         """
         Format response to dict.
 
         Args:
             response: response
```

### Comparing `manifest-ml-0.1.2/manifest/manifest.py` & `manifest-ml-0.1.3/manifest/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 from manifest.caches.postgres import PostgresCache
 from manifest.caches.redis import RedisCache
 from manifest.caches.sqlite import SQLiteCache
 from manifest.clients.ai21 import AI21Client
 from manifest.clients.cohere import CohereClient
 from manifest.clients.dummy import DummyClient
 from manifest.clients.huggingface import HuggingFaceClient
+from manifest.clients.huggingface_embedding import HuggingFaceEmbeddingClient
 from manifest.clients.openai import OpenAIClient
-from manifest.clients.openaichat import OpenAIChatClient
+from manifest.clients.openai_chat import OpenAIChatClient
+from manifest.clients.openai_embedding import OpenAIEmbeddingClient
 from manifest.clients.toma import TOMAClient
 from manifest.request import Request
 from manifest.response import Response
 
 logging.getLogger("openai").setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
 
 CLIENT_CONSTRUCTORS = {
     OpenAIClient.NAME: OpenAIClient,
     OpenAIChatClient.NAME: OpenAIChatClient,
+    OpenAIEmbeddingClient.NAME: OpenAIEmbeddingClient,
     CohereClient.NAME: CohereClient,
     AI21Client.NAME: AI21Client,
     HuggingFaceClient.NAME: HuggingFaceClient,
+    HuggingFaceEmbeddingClient.NAME: HuggingFaceEmbeddingClient,
     DummyClient.NAME: DummyClient,
     TOMAClient.NAME: TOMAClient,
 }
 
 # Diffusion
 DIFFUSION_CLIENTS = ["diffuser", "tomadiffuser"]
 try:
```

### Comparing `manifest-ml-0.1.2/manifest/request.py` & `manifest-ml-0.1.3/manifest/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,20 @@
     # Penalize resence
     presence_penalty: float = 0
 
     # Penalize frequency
     frequency_penalty: float = 0
 
 
+class EmbeddingRequest(Request):
+    """Embedding Request object."""
+
+    pass
+
+
 class DiffusionRequest(Request):
     """Diffusion Model Request object."""
 
     # Request type
     request_type: str = "diffusion"
 
     # Number of steps
```

### Comparing `manifest-ml-0.1.2/manifest/response.py` & `manifest-ml-0.1.3/manifest/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,22 @@
         "logits_key": "token_logprobs",
         "item_key": "array",
     },
     "tomadiffuser": {
         "logits_key": "token_logprobs",
         "item_key": "array",
     },
+    "openaiembedding": {
+        "logits_key": "token_logprobs",
+        "item_key": "array",
+    },
+    "huggingfaceembedding": {
+        "logits_key": "token_logprobs",
+        "item_key": "array",
+    },
 }
 
 
 class NumpyArrayEncoder(json.JSONEncoder):
     """Numpy array encoder."""
 
     def default(self, obj: Any) -> str:
```

### Comparing `manifest-ml-0.1.2/manifest_ml.egg-info/PKG-INFO` & `manifest-ml-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,17 @@
-Metadata-Version: 2.1
-Name: manifest-ml
-Version: 0.1.2
-Summary: Manifest for Prompting Foundation Models.
-Home-page: https://github.com/HazyResearch/manifest
-Author: Laurel Orr
-Author-email: laurel.orr@numbersstation.ai
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: api
-Provides-Extra: app
-Provides-Extra: diffusers
-Provides-Extra: gcp
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
-
 # Manifest
 How to make prompt programming with Foundation Models a little easier.
 
 
 # Table of Contents
 - [Install](#install)
 - [Getting Started](#getting-started)
 - [Manifest](#manifest-components)
 - [Local HuggingFace Models](#local-huggingface-models)
+- [Embedding Models](#embedding-models)
 - [Development](#development)
 - [Cite](#cite)
 
 
 # Install
 Install:
 ```bash
@@ -67,14 +44,17 @@
 # Start a manifest session to OpenAI - default `engine=text-davinci-002`
 manifest = Manifest(
     client_name = "openai",
 )
 manifest.run("Why is the grass green?")
 ```
 
+## Examples
+We have example notebook and python scripts located at [examples](examples). These show how to use different models, model types (i.e. text, diffusers, or embedding models), and async running.
+
 # Manifest Components
 Manifest is meant to be a very light weight package to help with prompt design and iteration. Three key design decisions of Manifest are
 
 * All models are behind APIs
 * Supports caching of model inputs/outputs for iteration, reproducibility, and cost saving
 * Unified API of generate, score, and embed
 
@@ -132,14 +112,20 @@
 ```
 
 You can also run over multiple examples if supported by the client.
 ```python
 results = manifest.run(["Where are the cats?", "Where are the dogs?"])
 ```
 
+We support async queries as well via
+```python
+import asyncio
+results = asyncio.run(manifest.arun_batch(["Where are the cats?", "Where are the dogs?"]))
+```
+
 If something doesn't go right, you can also ask to get a raw manifest Response.
 ```python
 result_object = manifest.run(["Where are the cats?", "Where are the dogs?"], return_response=True)
 print(result_object.get_request())
 print(result_object.is_cached())
 print(result_object.get_json_response())
 ```
@@ -198,14 +184,31 @@
 python3 -m manifest.api.app \
     --model_type huggingface \
     --model_name_or_path bigscience/bloom \
     --use_bitsandbytes \
     --percent_max_gpu_mem_reduction 0.85
 ```
 
+# Embedding Models
+Manifest also supports getting embeddings from models and available APIs. We do this all through changing the `client_name` argument. You still use `run` and `abatch_run`.
+
+To use OpenAI's embedding models, simply run
+```python
+manifest = Manifest(client_name="openaiembedding")
+embedding_as_np = manifest.run("Get me an embedding for a bunny")
+```
+
+As explained above, you can load local HuggingFace models that give you embeddings, too. If you want to use a standard generative model, load the model as above use use `client_name="huggingfaceembedding"`. If you want to use a standard embedding model, like those from SentenceTransformers, load your local model via
+```bash
+python3 -m manifest.api.app \
+    --model_type sentence_transformers \
+    --model_name_or_path all-mpnet-base-v2 \
+    --device 0
+```
+
 # Development
 Before submitting a PR, run
 ```bash
 export REDIS_PORT="6379"  # or whatever PORT local redis is running for those tests
 cd <REDIS_PATH>
 docker run -d -p 127.0.0.1:${REDIS_PORT}:6379 -v `pwd`:`pwd` -w `pwd` --name manifest_redis_test redis
 make test
@@ -218,9 +221,7 @@
   author = {Orr, Laurel},
   title = {Manifest},
   year = {2022},
   publisher = {GitHub},
   howpublished = {\url{https://github.com/HazyResearch/manifest}},
 }
 ```
-
-
```

### Comparing `manifest-ml-0.1.2/manifest_ml.egg-info/SOURCES.txt` & `manifest-ml-0.1.3/manifest_ml.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 manifest/api/__init__.py
 manifest/api/app.py
 manifest/api/response.py
 manifest/api/models/__init__.py
 manifest/api/models/diffuser.py
 manifest/api/models/huggingface.py
 manifest/api/models/model.py
+manifest/api/models/sentence_transformer.py
 manifest/caches/__init__.py
 manifest/caches/array_cache.py
 manifest/caches/cache.py
 manifest/caches/noop.py
 manifest/caches/postgres.py
 manifest/caches/redis.py
 manifest/caches/serializers.py
@@ -25,16 +26,18 @@
 manifest/clients/__init__.py
 manifest/clients/ai21.py
 manifest/clients/client.py
 manifest/clients/cohere.py
 manifest/clients/diffuser.py
 manifest/clients/dummy.py
 manifest/clients/huggingface.py
+manifest/clients/huggingface_embedding.py
 manifest/clients/openai.py
-manifest/clients/openaichat.py
+manifest/clients/openai_chat.py
+manifest/clients/openai_embedding.py
 manifest/clients/toma.py
 manifest/clients/toma_diffuser.py
 manifest_ml.egg-info/PKG-INFO
 manifest_ml.egg-info/SOURCES.txt
 manifest_ml.egg-info/dependency_links.txt
 manifest_ml.egg-info/requires.txt
 manifest_ml.egg-info/top_level.txt
```

### Comparing `manifest-ml-0.1.2/manifest_ml.egg-info/requires.txt` & `manifest-ml-0.1.3/manifest_ml.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,59 +5,61 @@
 aiohttp>=3.8.0
 sqlitedict>=2.0.0
 tenacity>=8.2.0
 tiktoken>=0.3.0
 xxhash>=3.0.0
 
 [all]
-deepspeed>=0.7.0
-types-setuptools>=57.4.17
-fastapi>=0.70.0
-types-protobuf>=3.19.21
+types-xxhash>=3.0.0
+uvicorn>=0.18.0
+python-dotenv>=0.20.0
+types-requests>=2.27.29
 sphinx-rtd-theme>=0.5.1
+pre-commit>=2.14.0
+sphinx-autobuild
 sqlalchemy
-autopep8>=1.6.0
-docformatter>=1.4
-types-python-dateutil>=2.8.16
-recommonmark>=0.7.1
-uvicorn>=0.18.0
-diffusers>=0.6.0
 pg8000
-pre-commit>=2.14.0
-isort>=5.9.3
+pillow>=9.0.0
+types-protobuf>=3.19.21
+twine
+accelerate>=0.10.0
 flake8>=4.0.0
+cloud-sql-python-connector[pg8000]>=1.0.0
+pep8-naming>=0.12.1
+recommonmark>=0.7.1
+sentence_transformers>=2.2.0
+types-redis>=4.2.6
+pytest>=7.0.0
+types-pillow>=9.0.0
+torch>=1.8.0
+autopep8>=1.6.0
 nbsphinx>=0.8.0
+fastapi>=0.70.0
+types-python-dateutil>=2.8.16
+types-PyYAML>=6.0.7
 transformers<4.26.0,>=4.20.0
+Flask>=2.1.2
+deepspeed>=0.7.0
+pytest-cov>=3.0.0
+docformatter>=1.4
+types-setuptools>=57.4.17
+isort>=5.9.3
+diffusers>=0.6.0
 black>=22.3.0
 mypy>=0.950
-twine
-types-PyYAML>=6.0.7
-types-requests>=2.27.29
-pep8-naming>=0.12.1
-accelerate>=0.10.0
-torch>=1.8.0
-python-dotenv>=0.20.0
-Flask>=2.1.2
-types-xxhash>=3.0.0
 flake8-docstrings>=1.6.0
-cloud-sql-python-connector[pg8000]>=1.0.0
-pytest-cov>=3.0.0
-pillow>=9.0.0
-types-pillow>=9.0.0
-pytest>=7.0.0
-types-redis>=4.2.6
-sphinx-autobuild
 
 [api]
+accelerate>=0.10.0
 deepspeed>=0.7.0
 diffusers>=0.6.0
 Flask>=2.1.2
-accelerate>=0.10.0
-transformers<4.26.0,>=4.20.0
+sentence_transformers>=2.2.0
 torch>=1.8.0
+transformers<4.26.0,>=4.20.0
 
 [app]
 fastapi>=0.70.0
 uvicorn>=0.18.0
 
 [dev]
 autopep8>=1.6.0
```

### Comparing `manifest-ml-0.1.2/pyproject.toml` & `manifest-ml-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
   "deepspeed",
   "numpy",
   "diffusers",
+  "sentence_transformers",
   "sqlitedict",
   "dill",
   "accelerate",
   "accelerate.utils.modeling",
   "transformers",
   "flask",
   "torch",
```

### Comparing `manifest-ml-0.1.2/setup.py` & `manifest-ml-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,21 @@
     "tiktoken>=0.3.0",
     "xxhash>=3.0.0",
 ]
 
 # What packages are optional?
 EXTRAS = {
     "api": [
+        "accelerate>=0.10.0",
         "deepspeed>=0.7.0",
         "diffusers>=0.6.0",
         "Flask>=2.1.2",
-        "accelerate>=0.10.0",
-        "transformers>=4.20.0,<4.26.0",
+        "sentence_transformers>=2.2.0",
         "torch>=1.8.0",
+        "transformers>=4.20.0,<4.26.0",
     ],
     "app": [
         "fastapi>=0.70.0",
         "uvicorn>=0.18.0",
     ],
     "diffusers": [
         "pillow>=9.0.0",
```

### Comparing `manifest-ml-0.1.2/tests/test_array_cache.py` & `manifest-ml-0.1.3/tests/test_array_cache.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/tests/test_cache.py` & `manifest-ml-0.1.3/tests/test_cache.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """Cache test."""
-from typing import cast
+from typing import Dict, cast
 
 import numpy as np
 import pytest
 from redis import Redis
 from sqlitedict import SqliteDict
 
 from manifest.caches.cache import Cache
 from manifest.caches.noop import NoopCache
 from manifest.caches.postgres import PostgresCache
 from manifest.caches.redis import RedisCache
 from manifest.caches.sqlite import SQLiteCache
 
 
-def _get_postgres_cache(**kwargs) -> Cache:  # type: ignore
+def _get_postgres_cache(
+    client_name: str = "", cache_args: Dict = {}
+) -> Cache:  # type: ignore
     """Get postgres cache."""
+    cache_args.update({"cache_user": "", "cache_password": "", "cache_db": ""})
     return PostgresCache(
         "postgres",
-        cache_args={"cache_user": "", "cache_password": "", "cache_db": ""},
-        **kwargs,
+        client_name=client_name,
+        cache_args=cache_args,
     )
 
 
 @pytest.mark.usefixtures("sqlite_cache")
 @pytest.mark.usefixtures("redis_cache")
 @pytest.mark.usefixtures("postgres_cache")
 @pytest.mark.parametrize("cache_type", ["sqlite", "redis", "postgres"])
@@ -92,19 +95,19 @@
 
     cache.set(test_request, test_response)
     response = cache.get(test_request)
     assert response.get_response() == "hello"
     assert response.is_cached()
     assert response.get_request() == test_request
 
+    # Test array
     arr = np.random.rand(4, 4)
     test_request = {"test": "hello", "testA": "world of images"}
     compute_arr_response = {"choices": [{"array": arr}]}
 
-    # Test array
     if cache_type == "sqlite":
         cache = SQLiteCache(sqlite_cache, client_name="diffuser")
     elif cache_type == "redis":
         cache = RedisCache(redis_cache, client_name="diffuser")
     elif cache_type == "postgres":
         cache = _get_postgres_cache(client_name="diffuser")
 
@@ -113,14 +116,45 @@
 
     cache.set(test_request, compute_arr_response)
     response = cache.get(test_request)
     assert np.allclose(response.get_response(), arr)
     assert response.is_cached()
     assert response.get_request() == test_request
 
+    # Test array byte string
+    arr = np.random.rand(4, 4)
+    test_request = {"test": "hello", "testA": "world of images 2"}
+    compute_arr_response = {"choices": [{"array": arr}]}
+
+    if cache_type == "sqlite":
+        cache = SQLiteCache(
+            sqlite_cache,
+            client_name="diffuser",
+            cache_args={"array_serializer": "byte_string"},
+        )
+    elif cache_type == "redis":
+        cache = RedisCache(
+            redis_cache,
+            client_name="diffuser",
+            cache_args={"array_serializer": "byte_string"},
+        )
+    elif cache_type == "postgres":
+        cache = _get_postgres_cache(
+            client_name="diffuser", cache_args={"array_serializer": "byte_string"}
+        )
+
+    response = cache.get(test_request)
+    assert response is None
+
+    cache.set(test_request, compute_arr_response)
+    response = cache.get(test_request)
+    assert np.allclose(response.get_response(), arr)
+    assert response.is_cached()
+    assert response.get_request() == test_request
+
 
 @pytest.mark.usefixtures("sqlite_cache")
 @pytest.mark.usefixtures("redis_cache")
 @pytest.mark.usefixtures("postgres_cache")
 @pytest.mark.parametrize("cache_type", ["sqlite", "redis", "postgres"])
 def test_get_batch_prompt(
     sqlite_cache: str, redis_cache: str, postgres_cache: str, cache_type: str
@@ -160,14 +194,47 @@
 
     response = cache.get(test_request)
     assert response is None
 
     cache.set(test_request, compute_arr_response)
     response = cache.get(test_request)
     assert np.allclose(response.get_response()[0], arr)
+    assert np.allclose(response.get_response()[1], arr2)
+    assert response.is_cached()
+    assert response.get_request() == test_request
+
+    # Test arrays byte serializer
+    arr = np.random.rand(4, 4)
+    arr2 = np.random.rand(4, 4)
+    test_request = {"test": ["hello", "goodbye"], "testA": "world of images 2"}
+    compute_arr_response = {"choices": [{"array": arr}, {"array": arr2}]}
+
+    if cache_type == "sqlite":
+        cache = SQLiteCache(
+            sqlite_cache,
+            client_name="diffuser",
+            cache_args={"array_serializer": "byte_string"},
+        )
+    elif cache_type == "redis":
+        cache = RedisCache(
+            redis_cache,
+            client_name="diffuser",
+            cache_args={"array_serializer": "byte_string"},
+        )
+    elif cache_type == "postgres":
+        cache = _get_postgres_cache(
+            client_name="diffuser", cache_args={"array_serializer": "byte_string"}
+        )
+
+    response = cache.get(test_request)
+    assert response is None
+
+    cache.set(test_request, compute_arr_response)
+    response = cache.get(test_request)
+    assert np.allclose(response.get_response()[0], arr)
     assert np.allclose(response.get_response()[1], arr2)
     assert response.is_cached()
     assert response.get_request() == test_request
 
 
 def test_noop_cache() -> None:
     """Test cache that is a no-op cache."""
```

### Comparing `manifest-ml-0.1.2/tests/test_client.py` & `manifest-ml-0.1.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/tests/test_huggingface_api.py` & `manifest-ml-0.1.3/tests/test_huggingface_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Test the HuggingFace API."""
 
 import math
 import os
 from subprocess import PIPE, Popen
 
+import numpy as np
 import pytest
 
 from manifest.api.models.huggingface import MODEL_REGISTRY, TextGenerationModel
+from manifest.api.models.sentence_transformer import SentenceTransformerModel
 
 NOCUDA = 0
 try:
     p = Popen(
         [
             "nvidia-smi",
             (
@@ -143,14 +145,45 @@
     assert len(result) == 2
     assert math.isclose(round(result[0][0], 3), -46.71)
     assert math.isclose(round(result[1][0], 3), -12.752)
     assert isinstance(result[0][1], list)
     assert isinstance(result[1][1], list)
 
 
+def test_embed() -> None:
+    """Test embedding pipeline."""
+    model = TextGenerationModel(
+        model_name_or_path="gpt2",
+        use_accelerate=False,
+        use_parallelize=False,
+        use_bitsandbytes=False,
+        use_deepspeed=False,
+        use_fp16=False,
+        device=-1,
+    )
+    inputs = ["Why is the sky green?", "Cats are butterflies"]
+    embeddings = model.embed(inputs)
+    assert isinstance(embeddings, np.ndarray)
+    assert embeddings.shape == (2, 768)
+
+    model2 = SentenceTransformerModel(
+        model_name_or_path="all-mpnet-base-v2",
+        use_accelerate=False,
+        use_parallelize=False,
+        use_bitsandbytes=False,
+        use_deepspeed=False,
+        use_fp16=False,
+        device=-1,
+    )
+    inputs = ["Why is the sky green?", "Cats are butterflies"]
+    embeddings = model2.embed(inputs)
+    assert isinstance(embeddings, np.ndarray)
+    assert embeddings.shape == (2, 768)
+
+
 def test_batch_gpt_generate() -> None:
     """Test pipeline generation from a gpt model."""
     model = TextGenerationModel(
         model_name_or_path="gpt2",
         use_accelerate=False,
         use_parallelize=False,
         use_bitsandbytes=False,
```

### Comparing `manifest-ml-0.1.2/tests/test_manifest.py` & `manifest-ml-0.1.3/tests/test_manifest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Manifest test."""
 import asyncio
 import os
 from typing import cast
 from unittest.mock import MagicMock, Mock, patch
 
+import numpy as np
 import pytest
 import requests
 from requests import HTTPError
 
 from manifest import Manifest, Response
 from manifest.caches.noop import NoopCache
 from manifest.caches.sqlite import SQLiteCache
@@ -546,14 +547,109 @@
         scores["response"]["choices"][0]["tokens"]
     )
     assert len(scores["response"]["choices"][0]["token_logprobs"]) == len(
         scores["response"]["choices"][0]["tokens"]
     )
 
 
+@pytest.mark.skipif(not MODEL_ALIVE, reason=f"No model at {URL}")
+@pytest.mark.usefixtures("sqlite_cache")
+def test_local_huggingfaceembedding(sqlite_cache: str) -> None:
+    """Test openaichat client."""
+    client = Manifest(
+        client_name="huggingfaceembedding",
+        client_connection=URL,
+        cache_name="sqlite",
+        cache_connection=sqlite_cache,
+    )
+
+    res = client.run("Why are there carrots?")
+    assert isinstance(res, np.ndarray)
+
+    response = cast(
+        Response, client.run("Why are there carrots?", return_response=True)
+    )
+    assert isinstance(response.get_response(), np.ndarray)
+    assert np.allclose(response.get_response(), res)
+
+    client = Manifest(
+        client_name="huggingfaceembedding",
+        client_connection=URL,
+        cache_name="sqlite",
+        cache_connection=sqlite_cache,
+    )
+
+    res = client.run("Why are there apples?")
+    assert isinstance(res, np.ndarray)
+
+    response = cast(Response, client.run("Why are there apples?", return_response=True))
+    assert isinstance(response.get_response(), np.ndarray)
+    assert np.allclose(response.get_response(), res)
+    assert response.is_cached() is True
+
+    response = cast(Response, client.run("Why are there apples?", return_response=True))
+    assert response.is_cached() is True
+
+    res_list = client.run(["Why are there apples?", "Why are there bananas?"])
+    assert (
+        isinstance(res_list, list)
+        and len(res_list) == 2
+        and isinstance(res_list[0], np.ndarray)
+    )
+
+    response = cast(
+        Response,
+        client.run(
+            ["Why are there apples?", "Why are there mangos?"], return_response=True
+        ),
+    )
+    assert (
+        isinstance(response.get_response(), list) and len(response.get_response()) == 2
+    )
+
+    response = cast(
+        Response, client.run("Why are there bananas?", return_response=True)
+    )
+    assert response.is_cached() is True
+
+    response = cast(
+        Response, client.run("Why are there oranges?", return_response=True)
+    )
+    assert response.is_cached() is False
+
+    res_list = asyncio.run(
+        client.arun_batch(["Why are there pears?", "Why are there oranges?"])
+    )
+    assert (
+        isinstance(res_list, list)
+        and len(res_list) == 2
+        and isinstance(res_list[0], np.ndarray)
+    )
+
+    response = cast(
+        Response,
+        asyncio.run(
+            client.arun_batch(
+                ["Why are there pinenuts?", "Why are there cocoa?"],
+                return_response=True,
+            )
+        ),
+    )
+    assert (
+        isinstance(response.get_response(), list)
+        and len(res_list) == 2
+        and isinstance(res_list[0], np.ndarray)
+    )
+
+    response = cast(
+        Response, client.run("Why are there oranges?", return_response=True)
+    )
+    assert response.is_cached() is True
+
+
 @pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
 @pytest.mark.usefixtures("sqlite_cache")
 def test_openai(sqlite_cache: str) -> None:
     """Test openai client."""
     client = Manifest(
         client_name="openai",
         engine="text-ada-001",
@@ -563,14 +659,15 @@
     )
 
     res = client.run("Why are there apples?")
     assert isinstance(res, str) and len(res) > 0
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert isinstance(response.get_response(), str) and len(response.get_response()) > 0
+    assert response.get_response() == res
     assert response.is_cached() is True
     assert "usage" in response.get_json_response()
     assert response.get_json_response()["usage"][0]["total_tokens"] == 15
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert response.is_cached() is True
 
@@ -639,14 +736,15 @@
     )
 
     res = client.run("Why are there apples?")
     assert isinstance(res, str) and len(res) > 0
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert isinstance(response.get_response(), str) and len(response.get_response()) > 0
+    assert response.get_response() == res
     assert response.is_cached() is True
     assert "usage" in response.get_json_response()
     assert response.get_json_response()["usage"][0]["total_tokens"] == 23
 
     response = cast(Response, client.run("Why are there apples?", return_response=True))
     assert response.is_cached() is True
 
@@ -681,14 +779,122 @@
 
     response = cast(
         Response, client.run("Why are there oranges?", return_response=True)
     )
     assert response.is_cached() is True
 
 
+@pytest.mark.skipif(not OPENAI_ALIVE, reason="No openai key set")
+@pytest.mark.usefixtures("sqlite_cache")
+def test_openaiembedding(sqlite_cache: str) -> None:
+    """Test openaichat client."""
+    client = Manifest(
+        client_name="openaiembedding",
+        cache_name="sqlite",
+        cache_connection=sqlite_cache,
+        array_serializer="local_file",
+    )
+
+    res = client.run("Why are there carrots?")
+    assert isinstance(res, np.ndarray)
+
+    response = cast(
+        Response, client.run("Why are there carrots?", return_response=True)
+    )
+    assert isinstance(response.get_response(), np.ndarray)
+    assert np.allclose(response.get_response(), res)
+
+    client = Manifest(
+        client_name="openaiembedding",
+        cache_name="sqlite",
+        cache_connection=sqlite_cache,
+    )
+
+    res = client.run("Why are there apples?")
+    assert isinstance(res, np.ndarray)
+
+    response = cast(Response, client.run("Why are there apples?", return_response=True))
+    assert isinstance(response.get_response(), np.ndarray)
+    assert np.allclose(response.get_response(), res)
+    assert response.is_cached() is True
+    assert "usage" in response.get_json_response()
+    assert response.get_json_response()["usage"][0]["total_tokens"] == 5
+
+    response = cast(Response, client.run("Why are there apples?", return_response=True))
+    assert response.is_cached() is True
+
+    res_list = client.run(["Why are there apples?", "Why are there bananas?"])
+    assert (
+        isinstance(res_list, list)
+        and len(res_list) == 2
+        and isinstance(res_list[0], np.ndarray)
+    )
+
+    response = cast(
+        Response,
+        client.run(
+            ["Why are there apples?", "Why are there mangos?"], return_response=True
+        ),
+    )
+    assert (
+        isinstance(response.get_response(), list) and len(response.get_response()) == 2
+    )
+    assert (
+        "usage" in response.get_json_response()
+        and len(response.get_json_response()["usage"]) == 2
+    )
+    assert response.get_json_response()["usage"][0]["total_tokens"] == 5
+    assert response.get_json_response()["usage"][1]["total_tokens"] == 6
+
+    response = cast(
+        Response, client.run("Why are there bananas?", return_response=True)
+    )
+    assert response.is_cached() is True
+
+    response = cast(
+        Response, client.run("Why are there oranges?", return_response=True)
+    )
+    assert response.is_cached() is False
+
+    res_list = asyncio.run(
+        client.arun_batch(["Why are there pears?", "Why are there oranges?"])
+    )
+    assert (
+        isinstance(res_list, list)
+        and len(res_list) == 2
+        and isinstance(res_list[0], np.ndarray)
+    )
+
+    response = cast(
+        Response,
+        asyncio.run(
+            client.arun_batch(
+                ["Why are there pinenuts?", "Why are there cocoa?"],
+                return_response=True,
+            )
+        ),
+    )
+    assert (
+        isinstance(response.get_response(), list)
+        and len(res_list) == 2
+        and isinstance(res_list[0], np.ndarray)
+    )
+    assert (
+        "usage" in response.get_json_response()
+        and len(response.get_json_response()["usage"]) == 2
+    )
+    assert response.get_json_response()["usage"][0]["total_tokens"] == 7
+    assert response.get_json_response()["usage"][1]["total_tokens"] == 5
+
+    response = cast(
+        Response, client.run("Why are there oranges?", return_response=True)
+    )
+    assert response.is_cached() is True
+
+
 def test_retry_handling() -> None:
     """Test retry handling."""
     # We'll mock the response so we won't need a real connection
     client = Manifest(client_name="openai", client_connection="fake")
     mock_create = MagicMock(
         side_effect=[
             # raise a 429 error
```

### Comparing `manifest-ml-0.1.2/tests/test_request.py` & `manifest-ml-0.1.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/tests/test_response.py` & `manifest-ml-0.1.3/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/tests/test_serializer.py` & `manifest-ml-0.1.3/tests/test_serializer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 """Cache test."""
 import json
 
 import numpy as np
 
-from manifest.caches.serializers import ArraySerializer
+from manifest.caches.serializers import ArraySerializer, NumpyByteSerializer
 
 
-def test_response_to_key() -> None:
+def test_response_to_key_array() -> None:
     """Test array serializer initialization."""
     serializer = ArraySerializer()
     arr = np.random.rand(4, 4)
     res = {"choices": [{"array": arr}]}
     key = serializer.response_to_key(res)
     key_dct = json.loads(key)
     assert isinstance(key_dct["choices"][0]["array"], str)
 
     res2 = serializer.key_to_response(key)
+    assert np.allclose(arr, res2["choices"][0]["array"])
+
+
+def test_response_to_key_numpybytes() -> None:
+    """Test array serializer initialization."""
+    serializer = NumpyByteSerializer()
+    arr = np.random.rand(4, 4)
+    res = {"choices": [{"array": arr}]}
+    key = serializer.response_to_key(res)
+    key_dct = json.loads(key)
+    assert isinstance(key_dct["choices"][0]["array"], str)
+
+    res2 = serializer.key_to_response(key)
     assert np.allclose(arr, res2["choices"][0]["array"])
```

### Comparing `manifest-ml-0.1.2/web_app/main.py` & `manifest-ml-0.1.3/web_app/main.py`

 * *Files identical despite different names*

### Comparing `manifest-ml-0.1.2/web_app/schemas.py` & `manifest-ml-0.1.3/web_app/schemas.py`

 * *Files identical despite different names*

