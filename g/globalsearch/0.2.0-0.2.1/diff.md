# Comparing `tmp/globalsearch-0.2.0.tar.gz` & `tmp/globalsearch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalsearch-0.2.0.tar", last modified: Tue Apr 11 15:49:44 2023, max compression
+gzip compressed data, was "globalsearch-0.2.1.tar", last modified: Tue Apr 11 22:08:24 2023, max compression
```

## Comparing `globalsearch-0.2.0.tar` & `globalsearch-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.032609 globalsearch-0.2.0/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-11 15:49:44.032669 globalsearch-0.2.0/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.0/README.md
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.027840 globalsearch-0.2.0/bin/
--rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.0/bin/gs_prepare
--rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.0/bin/gs_submit
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.027004 globalsearch-0.2.0/globalsearch/
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.029011 globalsearch-0.2.0/globalsearch/control/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.0/globalsearch/control/__init__.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.0/globalsearch/control/gs_prepare.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.032395 globalsearch-0.2.0/globalsearch/rnaseq/
--rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.0/globalsearch/rnaseq/__init__.py
--rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.2.0/globalsearch/rnaseq/find_files.py
--rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.0/globalsearch/rnaseq/index_star.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.0/globalsearch/rnaseq/make_kallisto_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.0/globalsearch/rnaseq/make_star_idx_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     6154 2023-04-07 20:18:38.000000 globalsearch-0.2.0/globalsearch/rnaseq/make_star_salmon_job.py
--rwxr-xr-x   0 weiju      (501) staff       (20)     1634 2023-02-09 22:31:19.000000 globalsearch-0.2.0/globalsearch/rnaseq/post_star_salmon.py
--rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.0/globalsearch/rnaseq/run_kallisto.py
--rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.2.0/globalsearch/rnaseq/run_spladder.py
--rwxr-xr-x   0 weiju      (501) staff       (20)    13266 2023-04-11 15:47:13.000000 globalsearch-0.2.0/globalsearch/rnaseq/run_star_salmon.py
--rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.2.0/globalsearch/rnaseq/trim_galore.py
-drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 15:49:44.028762 globalsearch-0.2.0/globalsearch.egg-info/
--rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/PKG-INFO
--rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/SOURCES.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/dependency_links.txt
--rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.0/globalsearch.egg-info/not-zip-safe
--rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/requires.txt
--rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-11 15:49:43.000000 globalsearch-0.2.0/globalsearch.egg-info/top_level.txt
--rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-11 15:49:44.032864 globalsearch-0.2.0/setup.cfg
--rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-11 15:48:05.000000 globalsearch-0.2.0/setup.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 22:08:24.340979 globalsearch-0.2.1/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-11 22:08:24.341048 globalsearch-0.2.1/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      252 2022-12-13 19:27:00.000000 globalsearch-0.2.1/README.md
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 22:08:24.337226 globalsearch-0.2.1/bin/
+-rwxr--r--   0 weiju      (501) staff       (20)      533 2023-01-09 18:49:49.000000 globalsearch-0.2.1/bin/gs_prepare
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1268 2023-02-09 22:31:19.000000 globalsearch-0.2.1/bin/gs_submit
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 22:08:24.336403 globalsearch-0.2.1/globalsearch/
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 22:08:24.338379 globalsearch-0.2.1/globalsearch/control/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-10 16:54:29.000000 globalsearch-0.2.1/globalsearch/control/__init__.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6635 2023-02-24 18:56:53.000000 globalsearch-0.2.1/globalsearch/control/gs_prepare.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 22:08:24.340762 globalsearch-0.2.1/globalsearch/rnaseq/
+-rw-r--r--   0 weiju      (501) staff       (20)        0 2022-12-09 00:21:15.000000 globalsearch-0.2.1/globalsearch/rnaseq/__init__.py
+-rw-r--r--   0 weiju      (501) staff       (20)     7034 2023-03-21 18:06:55.000000 globalsearch-0.2.1/globalsearch/rnaseq/find_files.py
+-rw-r--r--   0 weiju      (501) staff       (20)     2978 2023-04-07 20:18:38.000000 globalsearch-0.2.1/globalsearch/rnaseq/index_star.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     2130 2023-02-09 22:31:19.000000 globalsearch-0.2.1/globalsearch/rnaseq/make_kallisto_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     3120 2023-04-07 20:18:38.000000 globalsearch-0.2.1/globalsearch/rnaseq/make_star_idx_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     6330 2023-04-11 22:07:15.000000 globalsearch-0.2.1/globalsearch/rnaseq/make_star_salmon_job.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)     1634 2023-02-09 22:31:19.000000 globalsearch-0.2.1/globalsearch/rnaseq/post_star_salmon.py
+-rwxr--r--   0 weiju      (501) staff       (20)     5497 2023-01-06 20:10:59.000000 globalsearch-0.2.1/globalsearch/rnaseq/run_kallisto.py
+-rw-r--r--   0 weiju      (501) staff       (20)    14661 2023-03-10 21:10:17.000000 globalsearch-0.2.1/globalsearch/rnaseq/run_spladder.py
+-rwxr-xr-x   0 weiju      (501) staff       (20)    13278 2023-04-11 22:07:15.000000 globalsearch-0.2.1/globalsearch/rnaseq/run_star_salmon.py
+-rw-r--r--   0 weiju      (501) staff       (20)     3664 2023-03-21 18:06:55.000000 globalsearch-0.2.1/globalsearch/rnaseq/trim_galore.py
+drwxr-xr-x   0 weiju      (501) staff       (20)        0 2023-04-11 22:08:24.338153 globalsearch-0.2.1/globalsearch.egg-info/
+-rw-r--r--   0 weiju      (501) staff       (20)      951 2023-04-11 22:08:24.000000 globalsearch-0.2.1/globalsearch.egg-info/PKG-INFO
+-rw-r--r--   0 weiju      (501) staff       (20)      751 2023-04-11 22:08:24.000000 globalsearch-0.2.1/globalsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2023-04-11 22:08:24.000000 globalsearch-0.2.1/globalsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 weiju      (501) staff       (20)        1 2022-12-15 20:31:36.000000 globalsearch-0.2.1/globalsearch.egg-info/not-zip-safe
+-rw-r--r--   0 weiju      (501) staff       (20)       25 2023-04-11 22:08:24.000000 globalsearch-0.2.1/globalsearch.egg-info/requires.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       13 2023-04-11 22:08:24.000000 globalsearch-0.2.1/globalsearch.egg-info/top_level.txt
+-rw-r--r--   0 weiju      (501) staff       (20)       67 2023-04-11 22:08:24.341436 globalsearch-0.2.1/setup.cfg
+-rw-r--r--   0 weiju      (501) staff       (20)     1611 2023-04-11 22:08:06.000000 globalsearch-0.2.1/setup.py
```

### Comparing `globalsearch-0.2.0/PKG-INFO` & `globalsearch-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.0
+Version: 0.2.1
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.0/bin/gs_prepare` & `globalsearch-0.2.1/bin/gs_prepare`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/bin/gs_submit` & `globalsearch-0.2.1/bin/gs_submit`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/control/gs_prepare.py` & `globalsearch-0.2.1/globalsearch/control/gs_prepare.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/find_files.py` & `globalsearch-0.2.1/globalsearch/rnaseq/find_files.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/index_star.py` & `globalsearch-0.2.1/globalsearch/rnaseq/index_star.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/make_kallisto_job.py` & `globalsearch-0.2.1/globalsearch/rnaseq/make_kallisto_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/make_star_idx_job.py` & `globalsearch-0.2.1/globalsearch/rnaseq/make_star_idx_job.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/make_star_salmon_job.py` & `globalsearch-0.2.1/globalsearch/rnaseq/make_star_salmon_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,20 @@
         star_extra_options += ["--sjdbGTFtagExonParentTranscript", config['star_options']['sjdbGTFtagExonParentTranscript']]
     except:
         pass
     try:
         star_extra_options += ["--sjdbGTFtagExonParentGene", config['star_options']['sjdbGTFtagExonParentGene']]
     except:
         pass
+    try:
+        quantmode = config['star_options']['quantMode']
+        star_extra_options += ["--quantMode"]
+        star_extra_options += quantmode
+    except:
+        pass
     config['star_extra_options'] = ' '.join(star_extra_options)
 
     salmon_extra_options = []
     try:
         salmon_extra_options += ["--salmon_genome_fasta", config['salmon_options']['genome_fasta']]
     except:
         pass
```

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/post_star_salmon.py` & `globalsearch-0.2.1/globalsearch/rnaseq/post_star_salmon.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/run_kallisto.py` & `globalsearch-0.2.1/globalsearch/rnaseq/run_kallisto.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/run_spladder.py` & `globalsearch-0.2.1/globalsearch/rnaseq/run_spladder.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/run_star_salmon.py` & `globalsearch-0.2.1/globalsearch/rnaseq/run_star_salmon.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     # add more optional arguments
     if args.sjdbGTFfeatureExon is not None:
         command += ["--sjdbGTFfeatureExon", args.sjdbGTFfeatureExon]
     if args.sjdbGTFtagExonParentGene is not None:
         command += ["--sjdbGTFtagExonParentGene", args.sjdbGTFtagExonParentGene]
     if args.quantMode is not None:
-        command += ["--quantMode", args.quantMode]
+        command += ["--quantMode"] + args.quantMode
 
     cmd = ' '.join(command)
     compl_proc = subprocess.run(command, check=True, capture_output=False, cwd=results_dir)
 
 ####################### Deduplication (not in _old) ###############################
 def dedup(results_dir,folder_name):
     print('\033[33mRunning Deduplication! \033[0m', flush=True)
@@ -257,15 +257,15 @@
     parser.add_argument('--limitBAMsortRAM', type=int, default=5784458574)
     parser.add_argument('--sjdbGTFtagExonParentTranscript', default="Parent")
     parser.add_argument('--sjdbOverhang', type=int, default=None)
     parser.add_argument('--limitSjdbInsertNsj', type=int, default=1602710)
 
     parser.add_argument('--sjdbGTFfeatureExon')
     parser.add_argument('--sjdbGTFtagExonParentGene')
-    parser.add_argument('--quantMode')
+    parser.add_argument('--quantMode', nargs="+")
     parser.add_argument('--salmon_genome_fasta')
 
     args = parser.parse_args()
 
     now = datetime.datetime.now()
     timeprint = now.strftime("%Y-%m-%d %H:%M")
     data_folder = "%s/%s" % (args.dataroot, args.indir)
```

### Comparing `globalsearch-0.2.0/globalsearch/rnaseq/trim_galore.py` & `globalsearch-0.2.1/globalsearch/rnaseq/trim_galore.py`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/globalsearch.egg-info/PKG-INFO` & `globalsearch-0.2.1/globalsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalsearch
-Version: 0.2.0
+Version: 0.2.1
 Summary: globalsearch is a collection of Python modules and command tools for the Global Search pipeline.
 Home-page: https://github.com/baliga-lab/Global_Search
 Author: Wei-ju Wu
 Author-email: weiju.wu@gmail.com
 Maintainer: Wei-ju Wu
 Maintainer-email: weiju.wu@gmail.com
 License: LGPL V3
```

### Comparing `globalsearch-0.2.0/globalsearch.egg-info/SOURCES.txt` & `globalsearch-0.2.1/globalsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globalsearch-0.2.0/setup.py` & `globalsearch-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = 'globalsearch'
 PACKAGES = ['globalsearch.rnaseq', 'globalsearch.control']
 DESCRIPTION = 'globalsearch is a collection of Python modules and command tools for the Global Search pipeline.'
 LICENSE = 'LGPL V3'
 URI = 'https://github.com/baliga-lab/Global_Search'
 AUTHOR = 'Wei-ju Wu'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 KEYWORDS = ['global search', 'coral reef']
 
 # See trove classifiers
 # https://testpypi.python.org/pypi?%3Aaction=list_classifiers
 
 CLASSIFIERS = [
```

