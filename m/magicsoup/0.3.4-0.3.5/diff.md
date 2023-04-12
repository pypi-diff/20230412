# Comparing `tmp/magicsoup-0.3.4.tar.gz` & `tmp/magicsoup-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.3.4.tar", last modified: Tue Apr 11 15:53:30 2023, max compression
+gzip compressed data, was "magicsoup-0.3.5.tar", last modified: Wed Apr 12 15:01:06 2023, max compression
```

## Comparing `magicsoup-0.3.4.tar` & `magicsoup-0.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.4/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-11 15:53:30.558584 magicsoup-0.3.4/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.4/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.4/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-11 15:53:30.558584 magicsoup-0.3.4/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.554584 magicsoup-0.3.4/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.554584 magicsoup-0.3.4/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-11 15:53:18.000000 magicsoup-0.3.4/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.4/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.4/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.4/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.4/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.4/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.4/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    11993 2023-04-06 09:43:57.000000 magicsoup-0.3.4/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    28797 2023-04-07 15:20:43.000000 magicsoup-0.3.4/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4140 2023-03-31 15:15:22.000000 magicsoup-0.3.4/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.4/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    43105 2023-04-11 15:46:53.000000 magicsoup-0.3.4/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-11 15:53:30.000000 magicsoup-0.3.4/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-11 15:53:30.558584 magicsoup-0.3.4/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.4/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.4/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.4/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.4/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.4/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.880493 magicsoup-0.3.5/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.5/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-12 15:01:06.880493 magicsoup-0.3.5/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.5/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.5/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-12 15:01:06.880493 magicsoup-0.3.5/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-12 15:00:55.000000 magicsoup-0.3.5/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.5/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.5/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.5/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.5/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.5/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.5/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    11993 2023-04-06 09:43:57.000000 magicsoup-0.3.5/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    28797 2023-04-07 15:20:43.000000 magicsoup-0.3.5/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-12 14:59:48.000000 magicsoup-0.3.5/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.5/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    43105 2023-04-11 15:46:53.000000 magicsoup-0.3.5/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.880493 magicsoup-0.3.5/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.5/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.5/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.5/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.5/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.5/tests/test_world.py
```

### Comparing `magicsoup-0.3.4/LICENSE` & `magicsoup-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/PKG-INFO` & `magicsoup-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.4/README.md` & `magicsoup-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/pyproject.toml` & `magicsoup-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/constants.py` & `magicsoup-0.3.5/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/containers.py` & `magicsoup-0.3.5/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.3.5/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.3.5/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.3.5/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/genetics.py` & `magicsoup-0.3.5/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/kinetics.py` & `magicsoup-0.3.5/src/magicsoup/kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/mutations.py` & `magicsoup-0.3.5/src/magicsoup/mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     E.g. if it's 5, it means `seq_pairs[5]` was mutated and the resulting sequences are in this 3-tuple.
     """
     n = len(seq_pairs)
     if n == 0:
         return []
 
     combined_seqs = [(a + b, len(a)) for a, b in seq_pairs]
-    lens = [len(d) for d in combined_seqs]
+    lens = [len(d[0]) for d in combined_seqs]
     s_max = max(lens)
 
     mask = torch.zeros(n, s_max)
     for i, s in enumerate(lens):
         mask[i, :s] = True
 
     probs = torch.full((n, s_max), p)
```

### Comparing `magicsoup-0.3.4/src/magicsoup/util.py` & `magicsoup-0.3.5/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup/world.py` & `magicsoup-0.3.5/src/magicsoup/world.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.3.5/src/magicsoup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.4/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.3.5/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/tests/test_containers.py` & `magicsoup-0.3.5/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/tests/test_genetics.py` & `magicsoup-0.3.5/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/tests/test_kinetics.py` & `magicsoup-0.3.5/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/tests/test_util.py` & `magicsoup-0.3.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.4/tests/test_world.py` & `magicsoup-0.3.5/tests/test_world.py`

 * *Files identical despite different names*

