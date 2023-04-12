# Comparing `tmp/multiPrime-2.3.6.tar.gz` & `tmp/multiPrime-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.3.6.tar", last modified: Wed Apr 12 07:44:56 2023, max compression
+gzip compressed data, was "multiPrime-2.3.7.tar", last modified: Wed Apr 12 10:01:32 2023, max compression
```

## Comparing `multiPrime-2.3.6.tar` & `multiPrime-2.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 07:44:56.890061 multiPrime-2.3.6/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.6/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 07:44:56.889061 multiPrime-2.3.6/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.6/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 07:44:56.854058 multiPrime-2.3.6/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-12 07:44:56.000000 multiPrime-2.3.6/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-12 07:44:56.890061 multiPrime-2.3.6/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.6/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 07:44:56.880060 multiPrime-2.3.6/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.6/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-12 07:44:50.000000 multiPrime-2.3.6/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-02-21 05:52:29.000000 multiPrime-2.3.6/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    83718 2023-04-12 07:44:03.000000 multiPrime-2.3.6/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24839 2023-03-29 01:44:02.000000 multiPrime-2.3.6/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 10:01:32.145124 multiPrime-2.3.7/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.7/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 10:01:32.145124 multiPrime-2.3.7/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.7/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 10:01:32.144123 multiPrime-2.3.7/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-12 10:01:32.000000 multiPrime-2.3.7/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-12 10:01:32.145124 multiPrime-2.3.7/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.7/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-12 10:01:32.144123 multiPrime-2.3.7/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.7/src/__init__.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-12 09:55:33.000000 multiPrime-2.3.7/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-12 10:01:12.000000 multiPrime-2.3.7/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    84362 2023-04-12 10:01:05.000000 multiPrime-2.3.7/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24853 2023-04-12 10:01:01.000000 multiPrime-2.3.7/src/utils.py
```

### Comparing `multiPrime-2.3.6/LICENSE` & `multiPrime-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.6/PKG-INFO` & `multiPrime-2.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.6
+Version: 2.3.7
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.3.6/README.md` & `multiPrime-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.6/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.3.7/multiPrime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.6
+Version: 2.3.7
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.3.6/setup.py` & `multiPrime-2.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.6/src/main.py` & `multiPrime-2.3.7/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.6/src/src.py` & `multiPrime-2.3.7/src/src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1200,15 +1200,15 @@
                 for start in range(len(candidate_position)):
                     new_p.submit(self.primer_pairs(start, adaptor, min_len, max_len, candidate_position, primer_pairs,
                                                    coverage_threshold))
                     # This will submit all tasks to one place without blocking, and then each
                     # thread in the thread pool will fetch tasks.
                 new_p.shutdown()
             ID = str(self.outfile)
-            primer_ID = str(self.outfile).split("/")[-1].rstrip("txt") + "fa"
+            primer_ID = str(self.outfile).split("/")[-1].rstrip(".txt")
             with open(self.outfile, "w") as fo:
                 # headers = ["Primer_F_seq", "Primer_R_seq", "Product length:Tm:coverage_percentage",
                 # "Target number", "Primer_start_end"]
                 # fo.write(ID + "\t" + "\t".join(headers) + "\t")
                 with open(self.outfile + ".fa", "w") as fa:
                     fo.write(ID + "\t")
                     primer_pairs_sort = sorted(primer_pairs, key=lambda k: k[3], reverse=True)
@@ -1430,14 +1430,27 @@
         with open(Output, "w") as fo:
             for seq in seq_ID.keys():
                 # print(">" + '_'.join(seq_ID[seq]))
                 # print(seq)
                 fo.write(">" + '_'.join(seq_ID[seq]) + "\n" + seq + "\n")
         return seq_ID
 
+    def Bowtie_index(self, Input):
+        Bowtie_file = Path(Input).parent.joinpath("Bowtie_DB")
+        Bowtie_prefix = Path(Bowtie_file).joinpath(Path(Input).stem)
+        if Bowtie_file.exists():
+            size = os.path.getsize(Bowtie_file)
+            if not size:
+                os.system("bowtie2-build {} {}".format(Input, Bowtie_prefix))
+            else:
+                pass
+        else:
+            os.mkdir(Bowtie_file)
+            os.system("bowtie2-build {} {}".format(Input, Bowtie_prefix))
+
     def build_dict(self, Input):
         Input_dict = defaultdict(list)
         threshold = self.term_threshold
         with open(Input, "r") as f:
             position_pattern_1 = re.compile('MD:Z:(\w+)')
             position_pattern = re.compile("[A-Z]?(\d+)")
             for i in f:
@@ -1454,15 +1467,15 @@
                         pass
                     else:
                         Input_dict[gene].append([primer_match_start, primer])
         return Input_dict
 
     def bowtie_map(self):
         fa = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".term.fa")
-        ref_index = self.reference_file
+        ref_index = Path(self.reference_file).parent.joinpath("Bowtie_DB").joinpath(Path(self.reference_file).stem)
         out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".sam")
         for_out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".for.sam")
         rev_out = Path(self.primer_file).parent.joinpath(Path(self.primer_file).stem).with_suffix(".rev.sam")
         nproc = self.nproc
         if for_out.exists() and rev_out.exists():
             pass
         else:
@@ -1534,14 +1547,15 @@
                             # still stored in that process. In fact, this variable in the main process is equivalent
                             # to not being modified. In order to synchronize the changes of other processes to the
                             # main process, you need to create variables that can be shared among multiple processes.
         self.resQ.put(None)
 
     def run(self):
         self.get_term()
+        self.Bowtie_index(self.reference_file)
         self.bowtie_map()
         target_gene, forward_dict, reverse_dict = self.build_dict_run()
         p = ProcessPoolExecutor(self.nproc)
         for gene in target_gene:
             p.submit(self.PCR_product(gene, forward_dict, reverse_dict))
         # This will submit all tasks to one place without blocking, and then each
         # thread in the thread pool will fetch tasks.
```

### Comparing `multiPrime-2.3.6/src/utils.py` & `multiPrime-2.3.7/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
 
     parser.add_option('-i', '--input',
                       dest='input_file',
                       help='input file: primer.fa.')
 
     parser.add_option('-r', '--ref',
                       dest='ref',
-                      help='reference file: bowtie index.')
+                      help='reference file: fasta file.')
 
     parser.add_option('-l', '--len',
                       dest='len',
                       default=18,
                       type="int",
                       help='Length of primer, which is used for mapping. Default: 18')
 
@@ -332,15 +332,15 @@
     elif options.out is None:
         parser.print_help()
         print("No output file provided !!!")
         sys.exit(1)
     return parser.parse_args()
 
 def main_Usage():
-    print('Usage: \n'
+    print('Usage (version 2.3.7): \n'
           'multiPrime DPrime:  Degenerate primer design through MD-DPD or MD-EDPD.\n'
           'multiPrime Ppair:   Primer pair selection from the result of multiPrime DPrime.\n'
           'multiPrime Perfect: Extract primer-contained sequences with non-mismatches.\n'
           'multiPrime Errors:  Extract primer-contained sequences with errors.\n')
 
 
 degenerate_base = {"-": ["-"], "A": ["A"], "G": ["G"], "C": ["C"], "T": ["T"], "R": ["A", "G"], "Y": ["C", "T"],
```

