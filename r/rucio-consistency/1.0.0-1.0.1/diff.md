# Comparing `tmp/rucio-consistency-1.0.0.tar.gz` & `tmp/rucio-consistency-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.0.tar", last modified: Tue Apr 11 19:26:57 2023, max compression
+gzip compressed data, was "rucio-consistency-1.0.1.tar", last modified: Wed Apr 12 14:58:27 2023, max compression
```

## Comparing `rucio-consistency-1.0.0.tar` & `rucio-consistency-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-11 19:26:57.446349 rucio-consistency-1.0.0/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.0/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-11 19:26:57.446103 rucio-consistency-1.0.0/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.0/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-11 19:26:57.442697 rucio-consistency-1.0.0/rucio_ce/
--rw-r--r--   0 ivm        (501) staff       (20)      356 2023-04-11 19:20:50.000000 rucio-consistency-1.0.0/rucio_ce/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-01-26 19:54:24.000000 rucio-consistency-1.0.0/rucio_ce/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-01-31 18:55:50.000000 rucio-consistency-1.0.0/rucio_ce/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-01-26 19:54:24.000000 rucio-consistency-1.0.0/rucio_ce/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-01-26 19:54:24.000000 rucio-consistency-1.0.0/rucio_ce/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-11 19:26:57.444097 rucio-consistency-1.0.0/rucio_ce/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3436 2023-01-26 19:54:24.000000 rucio-consistency-1.0.0/rucio_ce/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3577 2023-01-31 19:05:18.000000 rucio-consistency-1.0.0/rucio_ce/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4318 2023-01-31 19:05:20.000000 rucio-consistency-1.0.0/rucio_ce/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9453 2023-01-31 19:06:53.000000 rucio-consistency-1.0.0/rucio_ce/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2743 2023-01-31 19:04:04.000000 rucio-consistency-1.0.0/rucio_ce/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3500 2023-01-26 19:54:24.000000 rucio-consistency-1.0.0/rucio_ce/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-11 19:19:16.000000 rucio-consistency-1.0.0/rucio_ce/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-11 19:26:57.445801 rucio-consistency-1.0.0/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      578 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      148 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       11 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)        9 2023-04-11 19:26:57.000000 rucio-consistency-1.0.0/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-11 19:26:57.446424 rucio-consistency-1.0.0/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1022 2023-04-11 19:26:23.000000 rucio-consistency-1.0.0/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.487654 rucio-consistency-1.0.1/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.1/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-12 14:58:27.487347 rucio-consistency-1.0.1/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.1/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.481781 rucio-consistency-1.0.1/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11324 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.485429 rucio-consistency-1.0.1/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9447 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3500 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-12 14:57:22.000000 rucio-consistency-1.0.1/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.486825 rucio-consistency-1.0.1/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9440 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27539 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-12 14:58:27.483859 rucio-consistency-1.0.1/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      808 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      325 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-12 14:58:27.000000 rucio-consistency-1.0.1/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-12 14:58:27.487736 rucio-consistency-1.0.1/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1313 2023-04-12 14:55:53.000000 rucio-consistency-1.0.1/setup.py
```

### Comparing `rucio-consistency-1.0.0/LICENSE` & `rucio-consistency-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.0/rucio_ce/cmplib.py` & `rucio-consistency-1.0.1/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.0/rucio_ce/config.py` & `rucio-consistency-1.0.1/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.0/rucio_ce/part.py` & `rucio-consistency-1.0.1/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.0/rucio_ce/scripts/cmp2.py` & `rucio-consistency-1.0.1/rucio_consistency/scripts/cmp2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys, glob, time, os
 
-from consistency_enforcement import PartitionedList, Stats
+from rucio_consistency import PartitionedList, Stats
 
 Version = "1.0"
 
 Usage = """
 python cmp2.py [-z] [-s <stats file> [-S <stats key>]]    (join|minus|xor|or) <A prefix> <B prefix> <output prefix>
 python cmp2.py [-z] [-s <stats file> [-S <stats key>]] -f (join|minus|xor|or) <A file> <B file> <output file>
 """
```

### Comparing `rucio-consistency-1.0.0/rucio_ce/scripts/cmp3.py` & `rucio-consistency-1.0.1/rucio_consistency/scripts/cmp3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random, string, sys, glob, time, gzip, os
 
-from consistency_enforcement import PartitionedList, cmp3_generator, Stats
+from rucio_consistency import PartitionedList, cmp3_generator, Stats
 
 Version = "1.1"
 
 Usage = """
 %s [-z] [-s <stats file> [-S <stats key>]] <b prefix> <r prefix> <a prefix> <dark output> <missing output>
 """
 
@@ -31,14 +31,15 @@
         opts = dict(opts)
 
         if len(args) < 5:
             cmd = sys.argv[0].rsplit("/", 1)[-1]
             if cmd.endswith(".py"):
                 cmd = "python " + cmd
             print(Usage % (cmd,))
+            sys.exit(2)
         compress = "-z" in opts
         stats_file = opts.get("-s")
         stats_key = opts.get("-S", "cmp3")
         stats = Stats(stats_file) if stats_file else None
 
         b_prefix, r_prefix, a_prefix, out_dark, out_missing = args
```

### Comparing `rucio-consistency-1.0.0/rucio_ce/scripts/cmp5.py` & `rucio-consistency-1.0.1/rucio_consistency/scripts/cmp5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random, string, sys, glob, time, gzip, os
-from consistency_enforcement import PartitionedList, cmp3_generator, Stats
+from rucio_consistency import PartitionedList, cmp3_generator, Stats
 
 Version = "cmp5 1.1"
 
 Usage = """
 %s [-z] [-s <stats file> [-S <stats key>]] <b m prefix> <b d prefix> <r prefix> <a m prefix> <a d prefix> <dark output> <missing output>
 """
```

### Comparing `rucio-consistency-1.0.0/rucio_ce/scripts/db_dump.py` & `rucio-consistency-1.0.1/rucio_consistency/scripts/db_dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import getopt, os, time, re, gzip, json, traceback
 import sys, uuid
 
-from consistency_enforcement import PartitionedList, DBConfig, CEConfiguration, Stats
+from rucio_consistency import PartitionedList, DBConfig, CEConfiguration, Stats
 
 from sqlalchemy import create_engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, Integer, String
 from sqlalchemy.orm import sessionmaker
 
 from sqlalchemy.dialects.postgresql import UUID, JSONB
```

### Comparing `rucio-consistency-1.0.0/rucio_ce/scripts/partition.py` & `rucio-consistency-1.0.1/rucio_consistency/scripts/partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from consistency_enforcement import PartitionedList, CEConfiguration
+from rucio_consistency import PartitionedList, CEConfiguration
 import sys, getopt, re, gzip
 try:
     import tqdm
     Use_tqdm = True
 except:
     Use_tqdm = False
```

### Comparing `rucio-consistency-1.0.0/rucio_ce/stats.py` & `rucio-consistency-1.0.1/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.0/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.0.1/rucio_consistency.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENSE
 README.rst
 setup.py
-rucio_ce/__init__.py
-rucio_ce/cmplib.py
-rucio_ce/config.py
-rucio_ce/part.py
-rucio_ce/py3.py
-rucio_ce/stats.py
-rucio_ce/version.py
-rucio_ce/scripts/cmp2.py
-rucio_ce/scripts/cmp3.py
-rucio_ce/scripts/cmp5.py
-rucio_ce/scripts/db_dump.py
-rucio_ce/scripts/partition.py
+rucio_consistency/__init__.py
+rucio_consistency/cmplib.py
+rucio_consistency/config.py
+rucio_consistency/part.py
+rucio_consistency/py3.py
+rucio_consistency/stats.py
+rucio_consistency/version.py
 rucio_consistency.egg-info/PKG-INFO
 rucio_consistency.egg-info/SOURCES.txt
 rucio_consistency.egg-info/dependency_links.txt
 rucio_consistency.egg-info/entry_points.txt
 rucio_consistency.egg-info/not-zip-safe
 rucio_consistency.egg-info/requires.txt
-rucio_consistency.egg-info/top_level.txt
+rucio_consistency.egg-info/top_level.txt
+rucio_consistency/scripts/cmp2.py
+rucio_consistency/scripts/cmp3.py
+rucio_consistency/scripts/cmp5.py
+rucio_consistency/scripts/db_dump.py
+rucio_consistency/scripts/partition.py
+rucio_consistency/xrootd/__init__.py
+rucio_consistency/xrootd/xrootd_client.py
+rucio_consistency/xrootd/xrootd_scanner.py
```

