# Comparing `tmp/multiPrime-2.3.5.tar.gz` & `tmp/multiPrime-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.3.5.tar", last modified: Wed Mar 29 01:45:05 2023, max compression
+gzip compressed data, was "multiPrime-2.3.6.tar", last modified: Wed Apr 12 07:44:56 2023, max compression
```

## Comparing `multiPrime-2.3.5.tar` & `multiPrime-2.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-03-29 01:45:05.671498 multiPrime-2.3.5/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.5/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-03-29 01:45:05.671498 multiPrime-2.3.5/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.5/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-03-29 01:45:05.670498 multiPrime-2.3.5/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-03-29 01:45:05.000000 multiPrime-2.3.5/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-03-29 01:45:05.000000 multiPrime-2.3.5/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-03-29 01:45:05.000000 multiPrime-2.3.5/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-03-29 01:45:05.000000 multiPrime-2.3.5/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-03-29 01:45:05.000000 multiPrime-2.3.5/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-03-29 01:45:05.671498 multiPrime-2.3.5/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.5/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-03-29 01:45:05.670498 multiPrime-2.3.5/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.5/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-03-29 01:44:55.000000 multiPrime-2.3.5/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-02-21 05:52:29.000000 multiPrime-2.3.5/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    83283 2023-03-13 01:24:21.000000 multiPrime-2.3.5/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24839 2023-03-29 01:44:02.000000 multiPrime-2.3.5/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 07:44:56.890061 multiPrime-2.3.6/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.6/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 07:44:56.889061 multiPrime-2.3.6/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.6/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 07:44:56.854058 multiPrime-2.3.6/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-12 07:44:56.890061 multiPrime-2.3.6/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.6/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 07:44:56.880060 multiPrime-2.3.6/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.6/src/__init__.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-12 07:44:50.000000 multiPrime-2.3.6/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-02-21 05:52:29.000000 multiPrime-2.3.6/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    83718 2023-04-12 07:44:03.000000 multiPrime-2.3.6/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24839 2023-03-29 01:44:02.000000 multiPrime-2.3.6/src/utils.py
```

### Comparing `multiPrime-2.3.5/LICENSE` & `multiPrime-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.5/PKG-INFO` & `multiPrime-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.5
+Version: 2.3.6
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.3.5/README.md` & `multiPrime-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.5/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.3.6/multiPrime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.5
+Version: 2.3.6
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.3.5/setup.py` & `multiPrime-2.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.5/src/main.py` & `multiPrime-2.3.6/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.5/src/src.py` & `multiPrime-2.3.6/src/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -1200,27 +1200,32 @@
                 for start in range(len(candidate_position)):
                     new_p.submit(self.primer_pairs(start, adaptor, min_len, max_len, candidate_position, primer_pairs,
                                                    coverage_threshold))
                     # This will submit all tasks to one place without blocking, and then each
                     # thread in the thread pool will fetch tasks.
                 new_p.shutdown()
             ID = str(self.outfile)
+            primer_ID = str(self.outfile).split("/")[-1].rstrip("txt") + "fa"
             with open(self.outfile, "w") as fo:
                 # headers = ["Primer_F_seq", "Primer_R_seq", "Product length:Tm:coverage_percentage",
                 # "Target number", "Primer_start_end"]
                 # fo.write(ID + "\t" + "\t".join(headers) + "\t")
-                fo.write(ID + "\t")
-                primer_pairs_sort = sorted(primer_pairs, key=lambda k: k[3], reverse=True)
-                for i in primer_pairs_sort:
-                    fo.write("\t".join(map(str, i)) + "\t")
-                # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
-                # but slow.
-                fo.write("\n")
-                fo.close()
-
+                with open(self.outfile + ".fa", "w") as fa:
+                    fo.write(ID + "\t")
+                    primer_pairs_sort = sorted(primer_pairs, key=lambda k: k[3], reverse=True)
+                    for i in primer_pairs_sort:
+                        fo.write("\t".join(map(str, i)) + "\t")
+                        start_stop = i[4].split(":")
+                        fa.write(primer_ID + "_" + start_stop[0] + "F\n" + i[0] + "\n" + primer_ID + "_" + start_stop[1]
+                                 + "R\n" + i[1] + "\n")
+                    # get results before shutdown. Synchronous call mode: call, wait for the return value, decouple,
+                    # but slow.
+                    fo.write("\n")
+                    fo.close()
+                    fa.close()
 
 class Product_perfect(object):
     def __init__(self, primer_file="", output_file="", ref_file="", file_format="fa", coverage="", nproc=10):
         self.nproc = nproc
         self.primers_file = primer_file
         self.ref_file = ref_file
         self.output_file = Path(output_file)
```

### Comparing `multiPrime-2.3.5/src/utils.py` & `multiPrime-2.3.6/src/utils.py`

 * *Files identical despite different names*

