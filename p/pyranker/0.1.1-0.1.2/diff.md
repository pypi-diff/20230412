# Comparing `tmp/pyranker-0.1.1-py3-none-any.whl.zip` & `tmp/pyranker-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 5966 bytes, number of entries: 13
+Zip file size: 5970 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 10:50 pyranker/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 18:01 pyranker/preprocessing/__init__.py
 -rw-r--r--  2.0 unx      507 b- defN 23-Apr-12 11:00 pyranker/preprocessing/normalizer.py
 -rw-r--r--  2.0 unx      216 b- defN 23-Apr-12 11:00 pyranker/preprocessing/tokenizer.py
 -rw-r--r--  2.0 unx     1274 b- defN 23-Apr-12 11:00 pyranker/rankers/__init__.py
--rw-r--r--  2.0 unx     1611 b- defN 23-Apr-12 11:17 pyranker/rankers/bm25.py
+-rw-r--r--  2.0 unx     1611 b- defN 23-Apr-12 11:52 pyranker/rankers/bm25.py
 -rw-r--r--  2.0 unx      801 b- defN 23-Apr-12 11:00 pyranker/rankers/tf_idf.py
 -rw-r--r--  2.0 unx     1172 b- defN 23-Apr-12 11:00 pyranker/rankers/vspace.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-12 11:22 pyranker-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1139 b- defN 23-Apr-12 11:22 pyranker-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 11:22 pyranker-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-12 11:22 pyranker-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-12 11:22 pyranker-0.1.1.dist-info/RECORD
-13 files, 8959 bytes uncompressed, 4170 bytes compressed:  53.5%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1139 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-12 11:54 pyranker-0.1.2.dist-info/RECORD
+13 files, 8959 bytes uncompressed, 4174 bytes compressed:  53.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pyranker/rankers/tf_idf.py
 Comment: 
 
 Filename: pyranker/rankers/vspace.py
 Comment: 
 
-Filename: pyranker-0.1.1.dist-info/LICENSE
+Filename: pyranker-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyranker-0.1.1.dist-info/METADATA
+Filename: pyranker-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pyranker-0.1.1.dist-info/WHEEL
+Filename: pyranker-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyranker-0.1.1.dist-info/top_level.txt
+Filename: pyranker-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyranker-0.1.1.dist-info/RECORD
+Filename: pyranker-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyranker/rankers/bm25.py

```diff
@@ -29,21 +29,22 @@
         """
         Gets the tf-idf of all documents w.r.t. query
         The function doesn't normalize the scores
         """
         score = np.zeros(self.corpus_size)
         avg_dl = sum(self.doc_len) / self.corpus_size
         for word in self.tokenizer(query):
-            if self.idf.get(word, 0) >= prune:
-                q_freq = np.array([doc.get(word, 0) for doc in self.doc_freqs])
-                score += self.idf.get(word, 0) * (
-                    q_freq
-                    * (self.k1 + 1)
-                    / (q_freq + self.k1 * (1 - self.b + self.b * self.doc_len / avg_dl))
-                )
+            if self.idf.get(word, 0) < prune:
+                continue
+            q_freq = np.array([doc.get(word, 0) for doc in self.doc_freqs])
+            score += self.idf.get(word, 0) * (
+                q_freq
+                * (self.k1 + 1)
+                / (q_freq + self.k1 * (1 - self.b + self.b * self.doc_len / avg_dl))
+            )
         return score
 
     def get_top_n(self, query, prune=0, n=5):
         """
         Get top n documents ranked by tf-idf
         """
         scores = self.get_scores(query, prune)
```

## Comparing `pyranker-0.1.1.dist-info/LICENSE` & `pyranker-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyranker-0.1.1.dist-info/METADATA` & `pyranker-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyranker
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python based package consisiting of BM25 and         Vector Space Rankers for Information Retrieval
 Home-page: https://github.com/AvishrantsSh/PyRanker
 Author: AvishrantSh (Avishrant Sharma)
 Author-email: <avishrants@gmail.com>
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AvishrantsSh/PyRanker/issues
 Platform: UNKNOWN
```

## Comparing `pyranker-0.1.1.dist-info/RECORD` & `pyranker-0.1.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pyranker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyranker/preprocessing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pyranker/preprocessing/normalizer.py,sha256=9VMOgBU0k4fo-06GMWHCLZHWOwN1a9LdBtO6tUDzwcw,507
 pyranker/preprocessing/tokenizer.py,sha256=GeS6SjmgIxXOnjATMkQSU1rFgFZfnPZABo4eJDwMfbg,216
 pyranker/rankers/__init__.py,sha256=HpfP50YusSq4fohtLLwSXGl0XDd5kWVHgdBMkaQKajk,1274
-pyranker/rankers/bm25.py,sha256=08DQwGNZN350H1b4BAKAdRMxdIjVyEBLbNSYUThVFio,1611
+pyranker/rankers/bm25.py,sha256=koZmYYe_R89UoY1KExyWyCbn9upKApbVQWmPCVcCMUk,1611
 pyranker/rankers/tf_idf.py,sha256=N8Z8SaX32Rmn-JPSXUJZakr44KmzuWClJmTjzXX7lgU,801
 pyranker/rankers/vspace.py,sha256=XXn0lqSwteU7-eKQ-Mw0ndOVnd408_9Sv82D8KHeYIE,1172
-pyranker-0.1.1.dist-info/LICENSE,sha256=5-dETpK1DgmAC-cXgfwkldJnpVpdt_U0f32yQ3lRBCQ,1072
-pyranker-0.1.1.dist-info/METADATA,sha256=6-YQbqYS6yrA9O6FcqE22whDrdvHKcMM3jSiF_JaRqY,1139
-pyranker-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyranker-0.1.1.dist-info/top_level.txt,sha256=oJAiLyQwtBSkOcLtjGX9bR5qQwmCiSk2DxIXyxzvr6w,9
-pyranker-0.1.1.dist-info/RECORD,,
+pyranker-0.1.2.dist-info/LICENSE,sha256=5-dETpK1DgmAC-cXgfwkldJnpVpdt_U0f32yQ3lRBCQ,1072
+pyranker-0.1.2.dist-info/METADATA,sha256=OPx9y500j74-Y3SY83dDrNWPNzI0lqkEDdpCpqY1z1g,1139
+pyranker-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyranker-0.1.2.dist-info/top_level.txt,sha256=oJAiLyQwtBSkOcLtjGX9bR5qQwmCiSk2DxIXyxzvr6w,9
+pyranker-0.1.2.dist-info/RECORD,,
```

