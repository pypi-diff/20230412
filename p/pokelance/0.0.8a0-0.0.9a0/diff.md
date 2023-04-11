# Comparing `tmp/pokelance-0.0.8a0.tar.gz` & `tmp/pokelance-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokelance-0.0.8a0.tar", max compression
+gzip compressed data, was "pokelance-0.0.9a0.tar", max compression
```

## Comparing `pokelance-0.0.8a0.tar` & `pokelance-0.0.9a0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1089 2022-12-10 11:13:03.511548 pokelance-0.0.8a0/LICENSE
--rw-r--r--   0        0        0      113 2023-01-15 15:16:02.656449 pokelance-0.0.8a0/pokelance/__init__.py
--rw-r--r--   0        0        0      440 2022-12-11 17:08:17.590957 pokelance-0.0.8a0/pokelance/cache/__init__.py
--rw-r--r--   0        0        0    11402 2022-12-20 18:48:39.115038 pokelance-0.0.8a0/pokelance/cache/cache.py
--rw-r--r--   0        0        0    13281 2022-12-11 17:08:17.582941 pokelance-0.0.8a0/pokelance/cache/cache_manager.py
--rw-r--r--   0        0        0     7220 2022-12-20 12:38:38.895456 pokelance-0.0.8a0/pokelance/client.py
--rw-r--r--   0        0        0     4007 2023-01-15 15:14:32.922033 pokelance-0.0.8a0/pokelance/exceptions.py
--rw-r--r--   0        0        0      557 2022-12-11 13:38:48.112513 pokelance-0.0.8a0/pokelance/ext/__init__.py
--rw-r--r--   0        0        0     2752 2022-12-16 15:19:02.709295 pokelance-0.0.8a0/pokelance/ext/_base.py
--rw-r--r--   0        0        0     8283 2022-12-12 08:19:49.122292 pokelance-0.0.8a0/pokelance/ext/berry.py
--rw-r--r--   0        0        0     8305 2022-12-12 08:50:00.325832 pokelance-0.0.8a0/pokelance/ext/contest.py
--rw-r--r--   0        0        0     8518 2022-12-12 08:19:49.153538 pokelance-0.0.8a0/pokelance/ext/encounter.py
--rw-r--r--   0        0        0     5848 2022-12-12 09:36:06.045977 pokelance-0.0.8a0/pokelance/ext/evolution.py
--rw-r--r--   0        0        0     9663 2022-12-12 08:19:49.122292 pokelance-0.0.8a0/pokelance/ext/game.py
--rw-r--r--   0        0        0    12868 2022-12-12 08:19:49.137914 pokelance-0.0.8a0/pokelance/ext/item.py
--rw-r--r--   0        0        0    10380 2022-12-12 08:19:49.106655 pokelance-0.0.8a0/pokelance/ext/location.py
--rw-r--r--   0        0        0     3218 2022-12-12 08:19:49.137914 pokelance-0.0.8a0/pokelance/ext/machine.py
--rw-r--r--   0        0        0    17794 2022-12-12 08:19:49.153538 pokelance-0.0.8a0/pokelance/ext/move.py
--rw-r--r--   0        0        0    37654 2022-12-16 15:22:25.618475 pokelance-0.0.8a0/pokelance/ext/pokemon.py
--rw-r--r--   0        0        0     4915 2023-01-15 15:14:32.904490 pokelance-0.0.8a0/pokelance/http/__init__.py
--rw-r--r--   0        0        0    20788 2023-01-15 14:53:37.103076 pokelance-0.0.8a0/pokelance/http/endpoints.py
--rw-r--r--   0        0        0     8879 2023-01-12 15:18:29.781435 pokelance-0.0.8a0/pokelance/languages.py
--rw-r--r--   0        0        0     3705 2022-12-20 18:51:58.101341 pokelance-0.0.8a0/pokelance/logger.py
--rw-r--r--   0        0        0     2026 2023-01-11 15:01:47.770702 pokelance-0.0.8a0/pokelance/models/__init__.py
--rw-r--r--   0        0        0      553 2022-12-11 20:07:41.544812 pokelance-0.0.8a0/pokelance/models/_base.py
--rw-r--r--   0        0        0     1953 2022-12-14 07:51:07.459692 pokelance-0.0.8a0/pokelance/models/abstract/__init__.py
--rw-r--r--   0        0        0     5673 2022-12-12 10:01:29.037738 pokelance-0.0.8a0/pokelance/models/abstract/berry.py
--rw-r--r--   0        0        0     4198 2022-12-12 10:01:29.005834 pokelance-0.0.8a0/pokelance/models/abstract/contest.py
--rw-r--r--   0        0        0     3612 2022-12-12 10:01:29.045625 pokelance-0.0.8a0/pokelance/models/abstract/encounter.py
--rw-r--r--   0        0        0     2477 2022-12-12 09:29:14.458132 pokelance-0.0.8a0/pokelance/models/abstract/evolution.py
--rw-r--r--   0        0        0     7819 2022-12-12 10:01:29.030788 pokelance-0.0.8a0/pokelance/models/abstract/game.py
--rw-r--r--   0        0        0     9018 2022-12-12 10:07:49.062544 pokelance-0.0.8a0/pokelance/models/abstract/item.py
--rw-r--r--   0        0        0     6884 2022-12-12 10:01:29.017252 pokelance-0.0.8a0/pokelance/models/abstract/location.py
--rw-r--r--   0        0        0     1261 2022-12-12 10:02:12.153337 pokelance-0.0.8a0/pokelance/models/abstract/machine.py
--rw-r--r--   0        0        0    13071 2022-12-12 10:07:49.076966 pokelance-0.0.8a0/pokelance/models/abstract/move.py
--rw-r--r--   0        0        0    36150 2023-01-12 15:16:55.376161 pokelance-0.0.8a0/pokelance/models/abstract/pokemon.py
--rw-r--r--   0        0        0    20518 2022-12-14 07:45:21.884450 pokelance-0.0.8a0/pokelance/models/abstract/showdown.py
--rw-r--r--   0        0        0     2601 2022-12-11 11:50:28.534022 pokelance-0.0.8a0/pokelance/models/abstract/utils/__init__.py
--rw-r--r--   0        0        0     1539 2022-12-11 18:59:05.329462 pokelance-0.0.8a0/pokelance/models/abstract/utils/berries.py
--rw-r--r--   0        0        0      978 2022-12-12 10:07:49.053540 pokelance-0.0.8a0/pokelance/models/abstract/utils/contests.py
--rw-r--r--   0        0        0     6291 2022-12-15 17:00:51.853687 pokelance-0.0.8a0/pokelance/models/abstract/utils/evolutions.py
--rw-r--r--   0        0        0      921 2022-12-12 10:07:49.024480 pokelance-0.0.8a0/pokelance/models/abstract/utils/games.py
--rw-r--r--   0        0        0     2362 2022-12-12 10:07:49.068442 pokelance-0.0.8a0/pokelance/models/abstract/utils/items.py
--rw-r--r--   0        0        0     3655 2022-12-12 10:07:49.084482 pokelance-0.0.8a0/pokelance/models/abstract/utils/locations.py
--rw-r--r--   0        0        0     7275 2022-12-12 10:07:49.031476 pokelance-0.0.8a0/pokelance/models/abstract/utils/moves.py
--rw-r--r--   0        0        0    43239 2023-01-12 15:16:55.402704 pokelance-0.0.8a0/pokelance/models/abstract/utils/pokemons.py
--rw-r--r--   0        0        0      684 2023-01-11 15:01:47.945064 pokelance-0.0.8a0/pokelance/models/common/__init__.py
--rw-r--r--   0        0        0    11207 2023-01-11 15:09:24.211629 pokelance-0.0.8a0/pokelance/models/common/models.py
--rw-r--r--   0        0        0     1112 2022-12-11 18:59:05.425975 pokelance-0.0.8a0/pokelance/models/common/resources.py
--rw-r--r--   0        0        0        0 2022-12-10 11:13:00.835196 pokelance-0.0.8a0/pokelance/py.typed
--rw-r--r--   0        0        0     1169 2023-01-15 15:15:40.916571 pokelance-0.0.8a0/pyproject.toml
--rw-r--r--   0        0        0     3762 2023-01-15 15:14:39.817070 pokelance-0.0.8a0/README.md
--rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 pokelance-0.0.8a0/setup.py
--rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 pokelance-0.0.8a0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2022-12-10 11:13:03.511548 pokelance-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0      113 2023-01-15 15:29:42.503617 pokelance-0.0.9a0/pokelance/__init__.py
+-rw-r--r--   0        0        0      440 2022-12-11 17:08:17.590957 pokelance-0.0.9a0/pokelance/cache/__init__.py
+-rw-r--r--   0        0        0    11402 2022-12-20 18:48:39.115038 pokelance-0.0.9a0/pokelance/cache/cache.py
+-rw-r--r--   0        0        0    13281 2022-12-11 17:08:17.582941 pokelance-0.0.9a0/pokelance/cache/cache_manager.py
+-rw-r--r--   0        0        0     7220 2022-12-20 12:38:38.895456 pokelance-0.0.9a0/pokelance/client.py
+-rw-r--r--   0        0        0     4029 2023-01-15 15:29:04.733511 pokelance-0.0.9a0/pokelance/exceptions.py
+-rw-r--r--   0        0        0      557 2022-12-11 13:38:48.112513 pokelance-0.0.9a0/pokelance/ext/__init__.py
+-rw-r--r--   0        0        0     2752 2022-12-16 15:19:02.709295 pokelance-0.0.9a0/pokelance/ext/_base.py
+-rw-r--r--   0        0        0     8283 2022-12-12 08:19:49.122292 pokelance-0.0.9a0/pokelance/ext/berry.py
+-rw-r--r--   0        0        0     8305 2022-12-12 08:50:00.325832 pokelance-0.0.9a0/pokelance/ext/contest.py
+-rw-r--r--   0        0        0     8518 2022-12-12 08:19:49.153538 pokelance-0.0.9a0/pokelance/ext/encounter.py
+-rw-r--r--   0        0        0     5848 2022-12-12 09:36:06.045977 pokelance-0.0.9a0/pokelance/ext/evolution.py
+-rw-r--r--   0        0        0     9663 2022-12-12 08:19:49.122292 pokelance-0.0.9a0/pokelance/ext/game.py
+-rw-r--r--   0        0        0    12868 2022-12-12 08:19:49.137914 pokelance-0.0.9a0/pokelance/ext/item.py
+-rw-r--r--   0        0        0    10380 2022-12-12 08:19:49.106655 pokelance-0.0.9a0/pokelance/ext/location.py
+-rw-r--r--   0        0        0     3218 2022-12-12 08:19:49.137914 pokelance-0.0.9a0/pokelance/ext/machine.py
+-rw-r--r--   0        0        0    17794 2022-12-12 08:19:49.153538 pokelance-0.0.9a0/pokelance/ext/move.py
+-rw-r--r--   0        0        0    37654 2022-12-16 15:22:25.618475 pokelance-0.0.9a0/pokelance/ext/pokemon.py
+-rw-r--r--   0        0        0     4915 2023-01-15 15:14:32.904490 pokelance-0.0.9a0/pokelance/http/__init__.py
+-rw-r--r--   0        0        0    20788 2023-01-15 14:53:37.103076 pokelance-0.0.9a0/pokelance/http/endpoints.py
+-rw-r--r--   0        0        0     8879 2023-01-12 15:18:29.781435 pokelance-0.0.9a0/pokelance/languages.py
+-rw-r--r--   0        0        0     3705 2022-12-20 18:51:58.101341 pokelance-0.0.9a0/pokelance/logger.py
+-rw-r--r--   0        0        0     2026 2023-01-11 15:01:47.770702 pokelance-0.0.9a0/pokelance/models/__init__.py
+-rw-r--r--   0        0        0      553 2022-12-11 20:07:41.544812 pokelance-0.0.9a0/pokelance/models/_base.py
+-rw-r--r--   0        0        0     1953 2022-12-14 07:51:07.459692 pokelance-0.0.9a0/pokelance/models/abstract/__init__.py
+-rw-r--r--   0        0        0     5673 2022-12-12 10:01:29.037738 pokelance-0.0.9a0/pokelance/models/abstract/berry.py
+-rw-r--r--   0        0        0     4198 2022-12-12 10:01:29.005834 pokelance-0.0.9a0/pokelance/models/abstract/contest.py
+-rw-r--r--   0        0        0     3612 2022-12-12 10:01:29.045625 pokelance-0.0.9a0/pokelance/models/abstract/encounter.py
+-rw-r--r--   0        0        0     2477 2022-12-12 09:29:14.458132 pokelance-0.0.9a0/pokelance/models/abstract/evolution.py
+-rw-r--r--   0        0        0     7819 2022-12-12 10:01:29.030788 pokelance-0.0.9a0/pokelance/models/abstract/game.py
+-rw-r--r--   0        0        0     9018 2022-12-12 10:07:49.062544 pokelance-0.0.9a0/pokelance/models/abstract/item.py
+-rw-r--r--   0        0        0     6884 2022-12-12 10:01:29.017252 pokelance-0.0.9a0/pokelance/models/abstract/location.py
+-rw-r--r--   0        0        0     1261 2022-12-12 10:02:12.153337 pokelance-0.0.9a0/pokelance/models/abstract/machine.py
+-rw-r--r--   0        0        0    13071 2022-12-12 10:07:49.076966 pokelance-0.0.9a0/pokelance/models/abstract/move.py
+-rw-r--r--   0        0        0    36150 2023-01-12 15:16:55.376161 pokelance-0.0.9a0/pokelance/models/abstract/pokemon.py
+-rw-r--r--   0        0        0    20518 2022-12-14 07:45:21.884450 pokelance-0.0.9a0/pokelance/models/abstract/showdown.py
+-rw-r--r--   0        0        0     2601 2022-12-11 11:50:28.534022 pokelance-0.0.9a0/pokelance/models/abstract/utils/__init__.py
+-rw-r--r--   0        0        0     1539 2022-12-11 18:59:05.329462 pokelance-0.0.9a0/pokelance/models/abstract/utils/berries.py
+-rw-r--r--   0        0        0      978 2022-12-12 10:07:49.053540 pokelance-0.0.9a0/pokelance/models/abstract/utils/contests.py
+-rw-r--r--   0        0        0     6291 2022-12-15 17:00:51.853687 pokelance-0.0.9a0/pokelance/models/abstract/utils/evolutions.py
+-rw-r--r--   0        0        0      921 2022-12-12 10:07:49.024480 pokelance-0.0.9a0/pokelance/models/abstract/utils/games.py
+-rw-r--r--   0        0        0     2362 2022-12-12 10:07:49.068442 pokelance-0.0.9a0/pokelance/models/abstract/utils/items.py
+-rw-r--r--   0        0        0     3655 2022-12-12 10:07:49.084482 pokelance-0.0.9a0/pokelance/models/abstract/utils/locations.py
+-rw-r--r--   0        0        0     7275 2022-12-12 10:07:49.031476 pokelance-0.0.9a0/pokelance/models/abstract/utils/moves.py
+-rw-r--r--   0        0        0    43239 2023-01-12 15:16:55.402704 pokelance-0.0.9a0/pokelance/models/abstract/utils/pokemons.py
+-rw-r--r--   0        0        0      684 2023-01-11 15:01:47.945064 pokelance-0.0.9a0/pokelance/models/common/__init__.py
+-rw-r--r--   0        0        0    11207 2023-01-11 15:09:24.211629 pokelance-0.0.9a0/pokelance/models/common/models.py
+-rw-r--r--   0        0        0     1112 2022-12-11 18:59:05.425975 pokelance-0.0.9a0/pokelance/models/common/resources.py
+-rw-r--r--   0        0        0        0 2022-12-10 11:13:00.835196 pokelance-0.0.9a0/pokelance/py.typed
+-rw-r--r--   0        0        0     1169 2023-01-15 15:29:42.494758 pokelance-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0     3762 2023-01-15 15:14:39.817070 pokelance-0.0.9a0/README.md
+-rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 pokelance-0.0.9a0/setup.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 pokelance-0.0.9a0/PKG-INFO
```

### Comparing `pokelance-0.0.8a0/LICENSE` & `pokelance-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/cache/cache.py` & `pokelance-0.0.9a0/pokelance/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/cache/cache_manager.py` & `pokelance-0.0.9a0/pokelance/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/client.py` & `pokelance-0.0.9a0/pokelance/client.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/exceptions.py` & `pokelance-0.0.9a0/pokelance/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     from pokelance.http import Route
 
 
 __all__: t.Tuple[str, ...] = (
     "PokeLanceException",
     "HTTPException",
     "ResourceNotFound",
+    "ImageNotFound",
 )
 
 
 class PokeLanceException(Exception):
     """Base exception class for PokeLance.
 
     Parameters
```

### Comparing `pokelance-0.0.8a0/pokelance/ext/__init__.py` & `pokelance-0.0.9a0/pokelance/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/_base.py` & `pokelance-0.0.9a0/pokelance/ext/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/berry.py` & `pokelance-0.0.9a0/pokelance/ext/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/contest.py` & `pokelance-0.0.9a0/pokelance/ext/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/encounter.py` & `pokelance-0.0.9a0/pokelance/ext/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/evolution.py` & `pokelance-0.0.9a0/pokelance/ext/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/game.py` & `pokelance-0.0.9a0/pokelance/ext/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/item.py` & `pokelance-0.0.9a0/pokelance/ext/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/location.py` & `pokelance-0.0.9a0/pokelance/ext/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/machine.py` & `pokelance-0.0.9a0/pokelance/ext/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/move.py` & `pokelance-0.0.9a0/pokelance/ext/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/ext/pokemon.py` & `pokelance-0.0.9a0/pokelance/ext/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/http/__init__.py` & `pokelance-0.0.9a0/pokelance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/http/endpoints.py` & `pokelance-0.0.9a0/pokelance/http/endpoints.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/languages.py` & `pokelance-0.0.9a0/pokelance/languages.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/logger.py` & `pokelance-0.0.9a0/pokelance/logger.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/__init__.py` & `pokelance-0.0.9a0/pokelance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/_base.py` & `pokelance-0.0.9a0/pokelance/models/_base.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/__init__.py` & `pokelance-0.0.9a0/pokelance/models/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/berry.py` & `pokelance-0.0.9a0/pokelance/models/abstract/berry.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/contest.py` & `pokelance-0.0.9a0/pokelance/models/abstract/contest.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/encounter.py` & `pokelance-0.0.9a0/pokelance/models/abstract/encounter.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/evolution.py` & `pokelance-0.0.9a0/pokelance/models/abstract/evolution.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/game.py` & `pokelance-0.0.9a0/pokelance/models/abstract/game.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/item.py` & `pokelance-0.0.9a0/pokelance/models/abstract/item.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/location.py` & `pokelance-0.0.9a0/pokelance/models/abstract/location.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/machine.py` & `pokelance-0.0.9a0/pokelance/models/abstract/machine.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/move.py` & `pokelance-0.0.9a0/pokelance/models/abstract/move.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/pokemon.py` & `pokelance-0.0.9a0/pokelance/models/abstract/pokemon.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/showdown.py` & `pokelance-0.0.9a0/pokelance/models/abstract/showdown.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/__init__.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/berries.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/berries.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/contests.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/contests.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/evolutions.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/evolutions.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/games.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/games.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/items.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/items.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/locations.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/locations.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/moves.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/moves.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/abstract/utils/pokemons.py` & `pokelance-0.0.9a0/pokelance/models/abstract/utils/pokemons.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/common/__init__.py` & `pokelance-0.0.9a0/pokelance/models/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/common/models.py` & `pokelance-0.0.9a0/pokelance/models/common/models.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pokelance/models/common/resources.py` & `pokelance-0.0.9a0/pokelance/models/common/resources.py`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/pyproject.toml` & `pokelance-0.0.9a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokelance"
-version = "0.0.8a"
+version = "0.0.9a"
 description = "A flexible and easy to use pokemon library."
 authors = ["FallenDeity <61227305+FallenDeity@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pokelance-0.0.8a0/README.md` & `pokelance-0.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `pokelance-0.0.8a0/setup.py` & `pokelance-0.0.9a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiofiles>=22.1.0,<23.0.0',
  'aiohttp>=3.8.3,<4.0.0',
  'attrs>=22.1.0,<23.0.0',
  'types-aiofiles>=22.1.0.4,<23.0.0.0']
 
 setup_kwargs = {
     'name': 'pokelance',
-    'version': '0.0.8a0',
+    'version': '0.0.9a0',
     'description': 'A flexible and easy to use pokemon library.',
     'long_description': '<h1 align="center"><b>PokeLance</b></h1>\n<p align="center">\n<img src="https://raw.githubusercontent.com/FallenDeity/PokeLance/master/docs/assets/pokelance.png" width=450 alt="logo"><br><br>\n<img src="https://img.shields.io/github/license/FallenDeity/PokeLance?style=flat-square" alt="license">\n<img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n<img src="https://img.shields.io/badge/%20type_checker-mypy-%231674b1?style=flat-square" alt="mypy">\n<img src="https://img.shields.io/badge/%20linter-ruff-%231674b1?style=flat-square" alt="ruff">\n<img src="https://img.shields.io/github/stars/FallenDeity/PokeLance?style=flat-square" alt="stars">\n<img src="https://img.shields.io/github/last-commit/FallenDeity/PokeLance?style=flat-square" alt="commits">\n<img src="https://img.shields.io/pypi/pyversions/PokeLance?style=flat-square" alt="py">\n<img src="https://img.shields.io/pypi/v/PokeLance?style=flat-square" alt="versions">\n<br><br>\nA flexible, statically typed and easy to use pokeapi wrapper for python 🚀\n</p>\n\n---\n\n\nFeatures:\n- Modern and pythonic API asynchronously built on top of aiohttp\n- Flexible and easy to use\n- Statically typed with mypy\n- Linted with ruff\n- Well documented\n- Optimized for speed and performance\n- Automatically caches data for faster access\n- Caches endpoints for user convenience\n\n---\n\n## Installation\n\n```bash\n$ python -m pip install PokeLance\n```\n\n---\n\n## Usage\n\n```python\nimport asyncio\n\nfrom pokelance import PokeLance\n\nclient = PokeLance()  # Create a client instance\n\n\nasync def main() -> None:\n    print(await client.ping())  # Ping the pokeapi\n    print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi\n    print(await client.berry.fetch_berry_flavor("spicy"))\n    print(await client.berry.fetch_berry_firmness("very-soft"))\n    print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn\'t exist\n    print(client.berry.get_berry_flavor("spicy"))\n    print(client.berry.get_berry_firmness("very-soft"))\n    await client.close()  # Close the client\n    return None\n\n\nasyncio.run(main())\n```\n\n## With Async Context Manager\n\n```python\nimport asyncio\n\nimport aiohttp\nfrom pokelance import PokeLance\n\n\nasync def main() -> None:\n    # Use an async context manager to create a client instance\n    async with aiohttp.ClientSession() as session, PokeLance(session=session) as client:\n        print(await client.ping())  # Ping the pokeapi\n        print(await client.berry.fetch_berry("cheri"))  # Fetch a berry from the pokeapi\n        print(await client.berry.fetch_berry_flavor("spicy"))\n        print(await client.berry.fetch_berry_firmness("very-soft"))\n        print(client.berry.get_berry("cheri"))  # Get a cached berry it will return None if it doesn\'t exist\n        print(client.berry.get_berry_flavor("spicy"))\n        print(client.berry.get_berry_firmness("very-soft"))\n        # The client will be closed automatically when the async context manager exits\n    return None\n\nasyncio.run(main())\n```\n\n## Important Links\n\n\n- [PokeAPI](https://pokeapi.co/)\n- [PokeAPI Documentation](https://pokeapi.co/docs/v2)\n- [PokeLance Documentation](https://FallenDeity.github.io/PokeLance/)\n- [PokeLance ReadTheDocs](https://pokelance.readthedocs.io/en/latest/)\n- [PokeLance GitHub](https://github.com/FallenDeity/PokeLance)\n- [PokeLance PyPI](https://pypi.org/project/PokeLance/)\n- [PokeLance Discord](https://discord.gg/yeyEvT5V2J)\n\n---\n\n!!! note "Note"\n    This is a work in progress. If you find any bugs or have any suggestions, please open an issue [here](https://github.com/FallenDeity/PokeLance/issues/new).\n\n---\n',
     'author': 'FallenDeity',
     'author_email': '61227305+FallenDeity@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pokelance-0.0.8a0/PKG-INFO` & `pokelance-0.0.9a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokelance
-Version: 0.0.8a0
+Version: 0.0.9a0
 Summary: A flexible and easy to use pokemon library.
 License: MIT
 Author: FallenDeity
 Author-email: 61227305+FallenDeity@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

