# Comparing `tmp/eeisp-0.4.1-py3-none-any.whl.zip` & `tmp/eeisp-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 19450 bytes, number of entries: 8
--rw-rw-r--  2.0 unx       15 b- defN 22-May-01 05:43 eeisp/__init__.py
--rwxrwxr-x  2.0 unx     9775 b- defN 22-Jul-06 05:01 eeisp-0.4.1.data/scripts/eeisp
--rwxrwxr-x  2.0 unx     1268 b- defN 22-Jul-06 05:01 eeisp-0.4.1.data/scripts/eeisp_add_genename_from_geneid
--rw-rw-r--  2.0 unx    35149 b- defN 22-Jul-06 05:01 eeisp-0.4.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6309 b- defN 22-Jul-06 05:01 eeisp-0.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Jul-06 05:01 eeisp-0.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 22-Jul-06 05:01 eeisp-0.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      647 b- defN 22-Jul-06 05:01 eeisp-0.4.1.dist-info/RECORD
-8 files, 53261 bytes uncompressed, 18318 bytes compressed:  65.6%
+Zip file size: 19370 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx       15 b- defN 22-Jul-06 05:05 eeisp/__init__.py
+-rwxrwxr-x  2.0 unx     9568 b- defN 23-Apr-12 06:09 eeisp-0.5.0.data/scripts/eeisp
+-rwxrwxr-x  2.0 unx     1268 b- defN 23-Apr-12 06:09 eeisp-0.5.0.data/scripts/eeisp_add_genename_from_geneid
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-12 06:09 eeisp-0.5.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6289 b- defN 23-Apr-12 06:09 eeisp-0.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 06:09 eeisp-0.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-12 06:09 eeisp-0.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      647 b- defN 23-Apr-12 06:09 eeisp-0.5.0.dist-info/RECORD
+8 files, 53034 bytes uncompressed, 18238 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: eeisp/__init__.py
 Comment: 
 
-Filename: eeisp-0.4.1.data/scripts/eeisp
+Filename: eeisp-0.5.0.data/scripts/eeisp
 Comment: 
 
-Filename: eeisp-0.4.1.data/scripts/eeisp_add_genename_from_geneid
+Filename: eeisp-0.5.0.data/scripts/eeisp_add_genename_from_geneid
 Comment: 
 
-Filename: eeisp-0.4.1.dist-info/LICENSE
+Filename: eeisp-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: eeisp-0.4.1.dist-info/METADATA
+Filename: eeisp-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: eeisp-0.4.1.dist-info/WHEEL
+Filename: eeisp-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: eeisp-0.4.1.dist-info/top_level.txt
+Filename: eeisp-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: eeisp-0.4.1.dist-info/RECORD
+Filename: eeisp-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `eeisp-0.4.1.data/scripts/eeisp` & `eeisp-0.5.0.data/scripts/eeisp`

 * *Files 5% similar despite different names*

```diff
@@ -5,60 +5,51 @@
 Copyright(c)  Ryuichiro Nakato <rnakato@iqb.u-tokyo.ac.jp>
 All rights reserved.
 '''
 
 import numpy as np
 import pandas as pd
 import sys
+import os
 import time
 from scipy.stats import binom
 import argparse
 import multiprocessing as mp
 import gc
 
 def argwrapper(args):
     return args[0](*args[1:])
 
 def calcCDI_eachrow(i, ProbArray, CountArray, ngene, ncell):
-    array = np.zeros(ngene)
-    for j in range(i + 1, ngene):
-        x = CountArray[j]
-        p = ProbArray[j]
-        # 生存関数 binom.sfを使う
-         # xが入っていないのでx-1に気をつけること
-        prob = binom.sf(x - 1, ncell, p)
-        if prob <= 0:
-            val = -10000000.0
-        else:
-            val = -(np.log10(prob))
-        array[j] = val
+    x = CountArray[i + 1:]
+    p = ProbArray[i + 1:]
+    prob = binom.sf(x - 1, ncell, p)
+    val = np.where(prob <= 0, -10000000.0, -(np.log10(prob)))
+    array = np.pad(val, (i + 1, 0), mode='constant', constant_values=0)
 
     del ProbArray
     del CountArray
     return array
 
 '''
 各遺伝子ペアで(gi,gj)=(0,1)となるサンプル数がCount_excl[j][i]回以上になるp値(prob1)と排他性スコアの計算
 各遺伝子ペアで(gi,gj)=(1,0)となるサンプル数がCount_excl[i][j]回以上になるp値(prob2)と排他性スコアの計算
 便宜的に2つのp値の平均を計算する
 '''
 def calcEEI_eachrow(i, ProbArray_i, CountArray_i, ProbArray_T_i, CountArray_T_i, ngene, ncell):
-    array = np.zeros(ngene)
-    for j in range(i + 1, ngene):
-        x1 = CountArray_T_i[j]
-        p1 = ProbArray_i[j]
-        prob1 = binom.sf(x1 - 1, ncell, p1)
-        x2 = CountArray_i[j]
-        p2 = ProbArray_T_i[j]
-        prob2 = binom.sf(x2 - 1, ncell, p2)
-        if prob1 <= 0 or prob2 <= 0:
-            val = -10000000.0
-        else:
-            val = ((-(np.log10(prob1))) + (-(np.log10(prob2)))) / 2
-        array[j] = val
+    x1 = CountArray_T_i[i + 1:]
+    p1 = ProbArray_i[i + 1:]
+    prob1 = binom.sf(x1 - 1, ncell, p1)
+
+    x2 = CountArray_i[i + 1:]
+    p2 = ProbArray_T_i[i + 1:]
+    prob2 = binom.sf(x2 - 1, ncell, p2)
+
+    val = np.where((prob1 <= 0) | (prob2 <= 0), -10000000.0, (-(np.log10(prob1)) + (-(np.log10(prob2)))) / 2)
+    array = np.pad(val, (i + 1, 0), mode='constant', constant_values=0)
     return array
 
 def genMatrix_MultiProcess(Prob_joint, Count_joint, MatType, ngene, ncell, *, ncore=4):
     p = mp.get_context('spawn').Pool(ncore)
     func_args = []
 
     for i in range(0, ngene):
@@ -224,15 +215,15 @@
     parser.add_argument("--threCDI", help="Threshold for CDI (default: 10.0)", type=float, default=10)
     parser.add_argument("--threEEI", help="Threshold for EEI (default: 5.0)", type=float, default=5)
     parser.add_argument("--tsv", help="Specify when the input file is tab-delimited (.tsv)", action="store_true")
     parser.add_argument("--gpu", help="GPU mode", action="store_true")
     parser.add_argument("--CDIonly", help="Calculate CDI only", action="store_true")
     parser.add_argument("--EEIonly", help="Calculate EEI only", action="store_true")
     parser.add_argument("-p", "--threads", help="number of threads (default: 2)", type=int, default=2)
-    parser.add_argument("-v", "--version", action='version', version='%(prog)s 0.4.1')
+    parser.add_argument("-v", "--version", action='version', version='%(prog)s 0.5.0')
 
     args = parser.parse_args()
     print(args)
 
     startt = time.time()
 
     if (args.tsv):
```

## Comparing `eeisp-0.4.1.data/scripts/eeisp_add_genename_from_geneid` & `eeisp-0.5.0.data/scripts/eeisp_add_genename_from_geneid`

 * *Files identical despite different names*

## Comparing `eeisp-0.4.1.dist-info/LICENSE` & `eeisp-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `eeisp-0.4.1.dist-info/METADATA` & `eeisp-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eeisp
-Version: 0.4.1
+Version: 0.5.0
 Summary: Identify gene pairs that are codependent and mutually exclusive from single-cell RNA-seq data.
 Home-page: https://github.com/nakatolab/EEISP
 Author: Natsu Nakajima, Ryuichiro Nakato
 Author-email: rnakato@iqb.u-tokyo.ac.jp
 License: GPL3.0
 Keywords: eeisp scRNA-seq
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.14.2)
 Requires-Dist: pandas (>=0.22.0)
@@ -133,9 +132,7 @@
    7       8       ESG000008       ESG000009       FO538757.3      FO538757.2      0.6852891560232545
    3       9       ESG000004       ESG000010       RP11-34P13.7    AP006222.2      0.6469554204484568
    4       6       ESG100005       ESG000007       RP11-34P13.8    RP11-34P13.9    0.5258703930217091
 ```
 
 ## Reference
 Nakajima N., Hayashi T., Fujiki K., Shirahige K., Akiyama T., Akutsu T. and Nakato R., [Codependency and mutual exclusivity for gene community detection from sparse single-cell transcriptome data](https://academic.oup.com/nar/advance-article/doi/10.1093/nar/gkab601/6324613), *Nucleic Acids Research*, 2021.
-
-
```

