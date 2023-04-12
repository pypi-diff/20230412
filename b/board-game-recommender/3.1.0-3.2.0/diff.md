# Comparing `tmp/board-game-recommender-3.1.0.tar.gz` & `tmp/board-game-recommender-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "board-game-recommender-3.1.0.tar", last modified: Wed Oct 26 19:57:04 2022, max compression
+gzip compressed data, was "board-game-recommender-3.2.0.tar", last modified: Wed Apr 12 18:48:02 2023, max compression
```

## Comparing `board-game-recommender-3.1.0.tar` & `board-game-recommender-3.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2022-10-26 19:57:04.637460 board-game-recommender-3.1.0/
--rw-r--r--   0 markus     (501) staff       (20)     1072 2020-09-18 05:15:08.000000 board-game-recommender-3.1.0/LICENSE
--rw-r--r--   0 markus     (501) staff       (20)       26 2021-11-28 20:14:53.000000 board-game-recommender-3.1.0/MANIFEST.in
--rw-r--r--   0 markus     (501) staff       (20)     4047 2022-10-26 19:57:04.637091 board-game-recommender-3.1.0/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)     2704 2021-05-19 13:26:08.000000 board-game-recommender-3.1.0/README.md
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2022-10-26 19:57:04.634272 board-game-recommender-3.1.0/board_game_recommender/
--rw-r--r--   0 markus     (501) staff       (20)      454 2022-10-24 07:53:40.000000 board-game-recommender-3.1.0/board_game_recommender/__init__.py
--rw-r--r--   0 markus     (501) staff       (20)     5103 2022-10-24 07:50:57.000000 board-game-recommender-3.1.0/board_game_recommender/__main__.py
--rw-r--r--   0 markus     (501) staff       (20)      103 2022-10-26 19:56:14.000000 board-game-recommender-3.1.0/board_game_recommender/__version__.py
--rw-r--r--   0 markus     (501) staff       (20)     1846 2022-10-24 07:53:40.000000 board-game-recommender-3.1.0/board_game_recommender/base.py
--rw-r--r--   0 markus     (501) staff       (20)     7420 2022-10-26 19:37:49.000000 board-game-recommender-3.1.0/board_game_recommender/light.py
--rw-r--r--   0 markus     (501) staff       (20)     4766 2022-10-24 07:54:43.000000 board-game-recommender-3.1.0/board_game_recommender/rankings.py
--rw-r--r--   0 markus     (501) staff       (20)    31633 2022-10-24 07:53:42.000000 board-game-recommender-3.1.0/board_game_recommender/recommend.py
--rw-r--r--   0 markus     (501) staff       (20)     2099 2022-10-24 07:53:12.000000 board-game-recommender-3.1.0/board_game_recommender/trust.py
--rw-r--r--   0 markus     (501) staff       (20)     3792 2021-10-14 03:42:57.000000 board-game-recommender-3.1.0/board_game_recommender/utils.py
-drwxr-xr-x   0 markus     (501) staff       (20)        0 2022-10-26 19:57:04.636449 board-game-recommender-3.1.0/board_game_recommender.egg-info/
--rw-r--r--   0 markus     (501) staff       (20)     4047 2022-10-26 19:57:04.000000 board-game-recommender-3.1.0/board_game_recommender.egg-info/PKG-INFO
--rw-r--r--   0 markus     (501) staff       (20)      573 2022-10-26 19:57:04.000000 board-game-recommender-3.1.0/board_game_recommender.egg-info/SOURCES.txt
--rw-r--r--   0 markus     (501) staff       (20)        1 2022-10-26 19:57:04.000000 board-game-recommender-3.1.0/board_game_recommender.egg-info/dependency_links.txt
--rw-r--r--   0 markus     (501) staff       (20)       65 2022-10-26 19:57:04.000000 board-game-recommender-3.1.0/board_game_recommender.egg-info/requires.txt
--rw-r--r--   0 markus     (501) staff       (20)       23 2022-10-26 19:57:04.000000 board-game-recommender-3.1.0/board_game_recommender.egg-info/top_level.txt
--rw-r--r--   0 markus     (501) staff       (20)       38 2022-10-26 19:57:04.637589 board-game-recommender-3.1.0/setup.cfg
--rwxr-xr-x   0 markus     (501) staff       (20)     4987 2022-10-24 07:52:41.000000 board-game-recommender-3.1.0/setup.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-04-12 18:48:02.374303 board-game-recommender-3.2.0/
+-rw-r--r--   0 markus     (501) staff       (20)     1072 2020-09-18 05:15:08.000000 board-game-recommender-3.2.0/LICENSE
+-rw-r--r--   0 markus     (501) staff       (20)       26 2021-11-28 20:14:53.000000 board-game-recommender-3.2.0/MANIFEST.in
+-rw-r--r--   0 markus     (501) staff       (20)     4047 2023-04-12 18:48:02.373755 board-game-recommender-3.2.0/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)     2704 2021-05-19 13:26:08.000000 board-game-recommender-3.2.0/README.md
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-04-12 18:48:02.370539 board-game-recommender-3.2.0/board_game_recommender/
+-rw-r--r--   0 markus     (501) staff       (20)      429 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/__init__.py
+-rw-r--r--   0 markus     (501) staff       (20)     5079 2023-04-11 10:26:21.000000 board-game-recommender-3.2.0/board_game_recommender/__main__.py
+-rw-r--r--   0 markus     (501) staff       (20)       78 2023-04-12 18:47:34.000000 board-game-recommender-3.2.0/board_game_recommender/__version__.py
+-rw-r--r--   0 markus     (501) staff       (20)     1846 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/base.py
+-rw-r--r--   0 markus     (501) staff       (20)     9358 2023-04-12 18:45:41.000000 board-game-recommender-3.2.0/board_game_recommender/light.py
+-rw-r--r--   0 markus     (501) staff       (20)     4766 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/rankings.py
+-rw-r--r--   0 markus     (501) staff       (20)    31608 2023-04-11 10:26:21.000000 board-game-recommender-3.2.0/board_game_recommender/recommend.py
+-rw-r--r--   0 markus     (501) staff       (20)     2099 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/board_game_recommender/trust.py
+-rw-r--r--   0 markus     (501) staff       (20)     3767 2023-04-11 10:26:21.000000 board-game-recommender-3.2.0/board_game_recommender/utils.py
+drwxr-xr-x   0 markus     (501) staff       (20)        0 2023-04-12 18:48:02.373036 board-game-recommender-3.2.0/board_game_recommender.egg-info/
+-rw-r--r--   0 markus     (501) staff       (20)     4047 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/PKG-INFO
+-rw-r--r--   0 markus     (501) staff       (20)      573 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/SOURCES.txt
+-rw-r--r--   0 markus     (501) staff       (20)        1 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/dependency_links.txt
+-rw-r--r--   0 markus     (501) staff       (20)       65 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/requires.txt
+-rw-r--r--   0 markus     (501) staff       (20)       23 2023-04-12 18:48:02.000000 board-game-recommender-3.2.0/board_game_recommender.egg-info/top_level.txt
+-rw-r--r--   0 markus     (501) staff       (20)       38 2023-04-12 18:48:02.374440 board-game-recommender-3.2.0/setup.cfg
+-rwxr-xr-x   0 markus     (501) staff       (20)     4947 2023-04-11 10:14:59.000000 board-game-recommender-3.2.0/setup.py
```

### Comparing `board-game-recommender-3.1.0/LICENSE` & `board-game-recommender-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.1.0/PKG-INFO` & `board-game-recommender-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-recommender
-Version: 3.1.0
+Version: 3.2.0
 Summary: Board games recommender engine
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-recommender/blob/master/README.md
 Project-URL: Funding, https://paypal.me/mschepke
```

### Comparing `board-game-recommender-3.1.0/README.md` & `board-game-recommender-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.1.0/board_game_recommender/__main__.py` & `board-game-recommender-3.2.0/board_game_recommender/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 
 """Main script & CLI entry point."""
 
 import argparse
 import logging
 import os
 import sys
```

### Comparing `board-game-recommender-3.1.0/board_game_recommender/base.py` & `board-game-recommender-3.2.0/board_game_recommender/base.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.1.0/board_game_recommender/light.py` & `board-game-recommender-3.2.0/board_game_recommender/light.py`

 * *Files 26% similar despite different names*

```diff
@@ -173,23 +173,73 @@
 
         return result[pd.MultiIndex.from_product([users, ["score", "rank"]])]
 
     def recommend_similar(
         self: "LightGamesRecommender",
         games: Iterable[int],
         **kwargs,
-    ):
-        raise NotImplementedError
+    ) -> pd.DataFrame:
+        """
+        Recommend games similar to the given games based on cosine similarity of latent factors.
+        """
+
+        games = list(games)
+        game_ids = np.array([self.items_indexes[game] for game in games])
+        game_factors = self.items_factors[:, game_ids]
+
+        scores = cosine_similarity(game_factors, self.items_factors).mean(axis=0)
+
+        result = pd.DataFrame(index=self.items_labels, data={"score": scores})
+        result["rank"] = result["score"].rank(method="min", ascending=False).astype(int)
+        result.sort_values("rank", inplace=True)
+
+        return result
 
     def similar_games(
         self: "LightGamesRecommender",
         games: Iterable[int],
         **kwargs,
-    ):
-        raise NotImplementedError
+    ) -> pd.DataFrame:
+        """Find games similar to the given games based on cosine similarity of latent factors."""
+
+        games = list(games)
+        game_ids = np.array([self.items_indexes[game] for game in games])
+        game_factors = self.items_factors[:, game_ids]
+
+        scores = cosine_similarity(game_factors, self.items_factors)
+
+        result = pd.DataFrame(
+            index=self.items_labels,
+            columns=pd.MultiIndex.from_product([games, ["score"]]),
+            data=scores.T,
+        )
+        result[pd.MultiIndex.from_product([games, ["rank"]])] = result.rank(
+            method="min",
+            ascending=False,
+        ).astype(int)
+
+        if len(games) == 1:
+            result.sort_values((games[0], "rank"), inplace=True)
+
+        return result[pd.MultiIndex.from_product([games, ["score", "rank"]])]
+
+
+def cosine_similarity(matrix_1: np.ndarray, matrix_2: np.ndarray) -> np.ndarray:
+    """
+    Calculates the cosine similarity between two matrices.
+
+    The input matrices need to be of shape (m,n) and (m,l); the result shape will be (n,l).
+    """
+
+    dot_product = matrix_1.T @ matrix_2  # (n,l)
+    matrix_1_norm = np.linalg.norm(matrix_1, axis=0)  # (n,)
+    matrix_2_norm = np.linalg.norm(matrix_2, axis=0)  # (l,)
+    outer_prod_norm = np.outer(matrix_1_norm, matrix_2_norm)  # (n,l)
+
+    return dot_product / outer_prod_norm  # (n,l)
 
 
 def turi_create_to_numpy(
     model: RecommenderModel,
     *,
     user_id: str = "bgg_user_name",
     item_id: str = "bgg_id",
```

### Comparing `board-game-recommender-3.1.0/board_game_recommender/rankings.py` & `board-game-recommender-3.2.0/board_game_recommender/rankings.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.1.0/board_game_recommender/recommend.py` & `board-game-recommender-3.2.0/board_game_recommender/recommend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """Board game recommenders."""
 
 import csv
 import logging
 import os
 import sys
 import tempfile
```

### Comparing `board-game-recommender-3.1.0/board_game_recommender/trust.py` & `board-game-recommender-3.2.0/board_game_recommender/trust.py`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.1.0/board_game_recommender/utils.py` & `board-game-recommender-3.2.0/board_game_recommender/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """Utility functions."""
 
 import csv
 import logging
 import os
 import sys
```

### Comparing `board-game-recommender-3.1.0/board_game_recommender.egg-info/PKG-INFO` & `board-game-recommender-3.2.0/board_game_recommender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: board-game-recommender
-Version: 3.1.0
+Version: 3.2.0
 Summary: Board games recommender engine
 Home-page: https://recommend.games/
 Author: Markus Shepherd
 Author-email: markus@recommend.games
 License: MIT
 Project-URL: Documentation, https://gitlab.com/recommend.games/board-game-recommender/blob/master/README.md
 Project-URL: Funding, https://paypal.me/mschepke
```

### Comparing `board-game-recommender-3.1.0/board_game_recommender.egg-info/SOURCES.txt` & `board-game-recommender-3.2.0/board_game_recommender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `board-game-recommender-3.1.0/setup.py` & `board-game-recommender-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """Setup."""
 
 # Template from https://github.com/navdeep-G/setup.py
 
-import io
 import os
 import sys
 from shutil import rmtree
 
-from setuptools import find_packages, setup, Command
+from setuptools import Command, find_packages, setup
 
 # Package meta-data.
 NAME = "board-game-recommender"
 DESCRIPTION = "Board games recommender engine"
 KEYWORDS = (
     "board games",
     "tabletop games",
@@ -63,15 +61,15 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
+    with open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 ABOUT = {}
 if not VERSION:
@@ -88,15 +86,15 @@
 
     description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(string):
         """Prints things in bold."""
-        print("\033[1m{0}\033[0m".format(string))
+        print("\033[1m{}\033[0m".format(string))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
@@ -104,21 +102,21 @@
         try:
             self.status("Removing previous builds…")
             rmtree(os.path.join(HERE, "dist"))
         except OSError:
             pass
 
         self.status("Building Source and Wheel (universal) distribution…")
-        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+        os.system("{} setup.py sdist bdist_wheel --universal".format(sys.executable))
 
         self.status("Uploading the package to PyPI via Twine…")
         os.system("twine upload dist/*")
 
         self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(ABOUT["__version__"]))
+        os.system("git tag v{}".format(ABOUT["__version__"]))
         os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
```

