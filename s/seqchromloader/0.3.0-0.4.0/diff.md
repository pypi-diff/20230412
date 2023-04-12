# Comparing `tmp/seqchromloader-0.3.0.tar.gz` & `tmp/seqchromloader-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.3.0.tar", last modified: Mon Mar 27 20:08:40 2023, max compression
+gzip compressed data, was "seqchromloader-0.4.0.tar", last modified: Wed Apr 12 20:59:39 2023, max compression
```

## Comparing `seqchromloader-0.3.0.tar` & `seqchromloader-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-03-27 20:08:40.947665 seqchromloader-0.3.0/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-03-27 20:08:40.947198 seqchromloader-0.3.0/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.3.0/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-03-27 20:08:40.941918 seqchromloader-0.3.0/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      151 2023-03-27 19:30:37.000000 seqchromloader-0.3.0/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12246 2023-03-27 19:48:26.000000 seqchromloader-0.3.0/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14355 2022-10-21 21:55:06.000000 seqchromloader-0.3.0/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     4399 2023-03-27 19:08:58.000000 seqchromloader-0.3.0/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-03-27 20:08:40.946254 seqchromloader-0.3.0/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-03-27 20:08:40.000000 seqchromloader-0.3.0/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-03-27 20:08:40.000000 seqchromloader-0.3.0/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-03-27 20:08:40.000000 seqchromloader-0.3.0/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-03-27 20:08:40.000000 seqchromloader-0.3.0/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-03-27 20:08:40.000000 seqchromloader-0.3.0/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-03-27 20:08:40.947768 seqchromloader-0.3.0/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-03-27 20:04:32.000000 seqchromloader-0.3.0/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-04-12 20:59:39.821490 seqchromloader-0.4.0/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-04-12 20:59:39.820919 seqchromloader-0.4.0/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.4.0/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-04-12 20:59:39.812257 seqchromloader-0.4.0/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      176 2023-04-12 20:00:32.000000 seqchromloader-0.4.0/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-04-12 19:57:21.000000 seqchromloader-0.4.0/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14355 2022-10-21 21:55:06.000000 seqchromloader-0.4.0/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6248 2023-04-12 20:33:18.000000 seqchromloader-0.4.0/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-04-12 20:59:39.819836 seqchromloader-0.4.0/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-04-12 20:59:39.821658 seqchromloader-0.4.0/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-04-12 20:58:23.000000 seqchromloader-0.4.0/setup.py
```

### Comparing `seqchromloader-0.3.0/PKG-INFO` & `seqchromloader-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.3.0/README.md` & `seqchromloader-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.3.0/seqchromloader/loader.py` & `seqchromloader-0.4.0/seqchromloader/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,21 @@
 class _SeqChromDatasetByWds(IterableDataset):
     """
     :param wds: list of webdataset files to get samples from
     :type wds: list of str
     :param transforms: A dictionary of functions to transform the output data, accepted keys are **["seq", "chrom", "target", "label"]**
     :type transforms: dict of functions
     """
-    def __init__(self, wds, transforms:dict=None, rank=0, world_size=1):
+    def __init__(self, wds, transforms:dict=None, rank=0, world_size=1, keep_key=False):
         self.wds = wds
         self.transforms = transforms
 
         self.rank = rank
         self.world_size = world_size
+        self.keep_key = keep_key
 
     def initialize(self):
         # this function will be called by worker_init_function in DataLoader
         pass
 
     def __iter__(self):
         pipeline = [
@@ -81,15 +82,18 @@
                        label="label.npy")
         ]
         
         # transform
         if self.transforms is not None: 
             pipeline.append(wds.map_dict(**self.transforms))
 
-        pipeline.append(wds.to_tuple("seq", "chrom", "target", "label"))
+        if self.keep_key:
+            pipeline.append(wds.to_tuple("__key__", "seq", "chrom", "target", "label"))
+        else:
+            pipeline.append(wds.to_tuple("seq", "chrom", "target", "label"))
             
         ds = wds.DataPipeline(*pipeline)
 
         return iter(ds)
 
 SeqChromDatasetByWds = seqChromLoaderCurry(_SeqChromDatasetByWds)
```

### Comparing `seqchromloader-0.3.0/seqchromloader/utils.py` & `seqchromloader-0.4.0/seqchromloader/utils.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.3.0/seqchromloader/writer.py` & `seqchromloader-0.4.0/seqchromloader/writer.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,22 +13,51 @@
 from multiprocessing import Pool
 
 import pyfasta
 import pysam
 import pyBigWig
 import webdataset as wds
 
-from seqchromloader import utils
+from . import utils
+from .loader import _SeqChromDatasetByWds
 
+def convert_data_webdataset(wds_in, wds_out, transforms=None, compress=False):
+    """
+    Transform the provided webdataset
+    
+    :param wds_in: input webdataset file
+    :type wds_in: string
+    :param wds_out: output webdataset file
+    :type wds_out: string
+    :param transforms: A dictionary of functions to transform the output data, accepted keys are *["seq", "chrom", "target", "label"]*
+    :type transforms: dict of functions
+    :param compress: whether to compress the output file
+    :type compress: boolean
+    """
+    
+    ds = _SeqChromDatasetByWds(wds_in, transforms=transforms, keep_key=True)
+    sink = wds.TarWriter(wds_out, compress=compress)
+    for (key, seq, chrom, target, label) in ds:
+        feature_dict = defaultdict()
+        feature_dict["__key__"] = key
+        
+        feature_dict["seq.npy"] = seq
+        feature_dict["chrom.npy"] = chrom
+        feature_dict["target.npy"] = target
+        feature_dict["label.npy"] = label
+        sink.write(feature_dict)
+    sink.close()
+    
 def dump_data_webdataset(coords, genome_fasta, bigwig_filelist,
                         target_bam=None, 
                         outdir="dataset/", outprefix="seqchrom", 
                         compress=True, 
                         numProcessors=1,
-                        transforms=None):
+                        transforms=None,
+                        DALI=False):
     """
     Given coordinates dataframe, extract the sequence and chromatin signal, save in webdataset format
 
     :param coords: pandas DataFrame containing genomic coordinates with columns **[chrom, start, end, label]**
     :type coords: pandas DataFrame
     :param genome_fasta: Genome fasta file.
     :type genome_fasta: str
@@ -42,14 +71,16 @@
     :type outdir: str
     :param outprefix: prefix of output files
     :type outprefix: str
     :param compress: whether to compress the output files
     :type compress: boolean
     :param numProcessors: number of processors
     :type numProcessors: int
+    :param DALI: Set to True if you want to use the dataset for NVIDIA DALI, it would save all arrays in bytes, which results in losing the array shape info
+    :param DALI: boolean
     """
 
     # split coordinates and assign chunks to workers
     num_chunks = math.ceil(len(coords) / 7000)
     chunks = np.array_split(coords, num_chunks)
 
     # freeze the common parameters
@@ -57,30 +88,37 @@
     ## also create a multiprocessing lock
     dump_data_worker_freeze = functools.partial(dump_data_webdataset_worker, 
                                                     fasta=genome_fasta, 
                                                     bigwig_files=bigwig_filelist,
                                                     target_bam=target_bam,
                                                     compress=compress,
                                                     outdir=outdir,
-                                                    transforms=transforms)
+                                                    transforms=transforms,
+                                                    DALI=DALI)
+    
+    count_of_digits = 0
+    while num_chunks > 0:
+       num_chunks = int(num_chunks/10)
+       count_of_digits += 1
 
     pool = Pool(numProcessors)
-    res = pool.starmap_async(dump_data_worker_freeze, zip(chunks, [outprefix + "_" + str(i) for i in range(num_chunks)]))
+    res = pool.starmap_async(dump_data_worker_freeze, zip(chunks, [outprefix + "_" + format(i, f'0{count_of_digits}d') for i in range(num_chunks)]))
     files = res.get()
 
     return files
 
 def dump_data_webdataset_worker(coords, 
                                 outprefix, 
                                 fasta, 
                                 bigwig_files,
                                 target_bam=None, 
                                 outdir="dataset/", 
                                 compress=True,
-                                transforms=None):
+                                transforms=None,
+                                DALI=False):
     # get handlers
     genome_pyfasta = pyfasta.Fasta(fasta)
     bigwigs = [pyBigWig.open(bw) for bw in bigwig_files]
     target_pysam = pysam.AlignmentFile(target_bam) if target_bam is not None else None
 
     # iterate all records
     filename = os.path.join(outdir, f"{outprefix}.tar.gz" if compress else f"{outprefix}.tar")
@@ -99,19 +137,25 @@
                 bigwigs=bigwigs,
                 target_bam=target_pysam,
                 strand=item.strand,
                 transforms=transforms,
             )
         except utils.BigWigInaccessible as e:
             continue
-
-        feature_dict["seq.npy"] = feature['seq']
-        feature_dict["chrom.npy"] = feature['chrom']
-        feature_dict["target.npy"] = feature['target']
-        feature_dict["label.npy"] = feature['label']
+        
+        if not DALI:
+            feature_dict["seq.npy"] = feature['seq']
+            feature_dict["chrom.npy"] = feature['chrom']
+            feature_dict["target.npy"] = feature['target']
+            feature_dict["label.npy"] = feature['label']
+        else:
+            feature_dict["seq.npy"] = feature['seq'].tobytes()
+            feature_dict["chrom.npy"] = feature['chrom'].tobytes()
+            feature_dict["target.npy"] = feature['target'].tobytes()
+            feature_dict["label.npy"] = feature['label'].tobytes()
 
         sink.write(feature_dict)
 
     sink.close()
     for bw in bigwigs: bw.close()
 
     return filename
```

### Comparing `seqchromloader-0.3.0/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.4.0/seqchromloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.3.0/setup.py` & `seqchromloader-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.3.0",
+    version="0.4.0",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

