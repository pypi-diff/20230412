# Comparing `tmp/hpcblast-1.0.0-py3-none-any.whl.zip` & `tmp/hpcblast-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8664 bytes, number of entries: 11
+Zip file size: 9008 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       34 b- defN 22-Sep-30 08:42 hpcblast/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Sep-30 08:42 hpcblast/_version.py
+-rw-r--r--  2.0 unx       22 b- defN 22-Dec-06 14:44 hpcblast/_version.py
 -rw-r--r--  2.0 unx      151 b- defN 22-Oct-07 09:48 hpcblast/main.py
--rw-r--r--  2.0 unx     4277 b- defN 22-Oct-07 09:50 hpcblast/src.py
--rw-r--r--  2.0 unx     6609 b- defN 22-Oct-07 08:50 hpcblast/utils.py
--rw-r--r--  2.0 unx     1094 b- defN 22-Oct-10 07:41 hpcblast-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5261 b- defN 22-Oct-10 07:41 hpcblast-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Oct-10 07:41 hpcblast-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 22-Oct-10 07:41 hpcblast-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 22-Oct-10 07:41 hpcblast-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 22-Oct-10 07:41 hpcblast-1.0.0.dist-info/RECORD
-11 files, 18453 bytes uncompressed, 7220 bytes compressed:  60.9%
+-rw-r--r--  2.0 unx     6204 b- defN 23-Apr-10 02:53 hpcblast/src.py
+-rw-r--r--  2.0 unx     6788 b- defN 23-Mar-30 08:39 hpcblast/utils.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-Apr-12 09:03 hpcblast-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5528 b- defN 23-Apr-12 09:03 hpcblast-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 09:03 hpcblast-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-12 09:03 hpcblast-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-12 09:03 hpcblast-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      855 b- defN 23-Apr-12 09:03 hpcblast-1.0.1.dist-info/RECORD
+11 files, 20844 bytes uncompressed, 7564 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: hpcblast/src.py
 Comment: 
 
 Filename: hpcblast/utils.py
 Comment: 
 
-Filename: hpcblast-1.0.0.dist-info/LICENSE
+Filename: hpcblast-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: hpcblast-1.0.0.dist-info/METADATA
+Filename: hpcblast-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: hpcblast-1.0.0.dist-info/WHEEL
+Filename: hpcblast-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: hpcblast-1.0.0.dist-info/entry_points.txt
+Filename: hpcblast-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: hpcblast-1.0.0.dist-info/top_level.txt
+Filename: hpcblast-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: hpcblast-1.0.0.dist-info/RECORD
+Filename: hpcblast-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpcblast/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

## hpcblast/src.py

```diff
@@ -2,55 +2,104 @@
 
 from .utils import *
 
 __all__ = ["HPCBlast", "HPCBlastArg"]
 
 
 class HPCBlast(object):
+
     def __init__(self, args=None, blast_options=None):
+        self.outfile = os.path.abspath(args.outfile)
+        temp = os.path.basename(tempfile.mktemp(prefix="hpc-blast_"))
+        self.outdir = os.path.abspath(args.output or os.path.join(
+            os.path.dirname(self.outfile), temp))
         self.args = args
-        self.outdir = args.output
-        self.args.mode = "sge"
-        if self.args.local:
-            self.args.mode = "local"
-        self.args.jobname = "hpc_blast_%d" % os.getpid()
-        self.args.logdir = os.path.join(self.outdir, "logs")
-        self.args.workdir = os.getcwd()
-        self.args.startline = 0
-        self.args.groups = 1
+        self._create_sge_args()
         self.btype = args.blast
         self.db = args.blast_db
         self.blast_exe = which(self.btype)
         self.query = args.query
-        self.outfile = args.outfile
         self.blast_options = blast_options
         self.chunk_files = {}
         self.chunk_res = []
         self.blast_scripts = ""
+        self.finished = False
         if not self.blast_exe or not "blast" in os.path.basename(self.blast_exe):
             raise ArgumentsError("blast not found or not exists in command")
+        self.cleandir = not args.output
+
+    def _create_sge_args(self):
+        self.args.mode = "sge"
+        if self.args.local:
+            self.args.mode = "local"
+        self.args.logdir = os.path.join(self.outdir, "logs")
+        self.args.workdir = os.getcwd()
+        self.args.startline = 0
+        self.args.groups = 1
+
+    def split_fastx_by_size(self, size=0):
+        self.chunk_files = {}
+        if size <= 0:
+            return
+        if os.path.isfile(self.query):
+            mkdir(os.path.join(self.outdir, "chunks"))
+        fx = get_fastx_type(self.query)
+        s = fh = 0
+        with Zopen(self.query, mode="rb") as fi:
+            if fx == "fasta":
+                for line in fi:
+                    if line.startswith(b">"):
+                        n, mod = divmod(s, size)
+                        s += 1
+                        if mod == 0:
+                            if fh:
+                                fh.close()
+                            fo = os.path.join(
+                                self.outdir, "chunks", "split.%05d.fa" % n)
+                            self.chunk_files[n] = fo
+                            fh = open(fo, "wb")
+                    fh.write(line)
+            elif fx == "fastq":
+                for i, line in enumerate(fi):
+                    x = i % 4
+                    if x == 0:
+                        n, mod = divmod(s, size)
+                        s += 1
+                        if mod == 0:
+                            if fh:
+                                fh.close()
+                            fo = os.path.join(
+                                self.outdir, "chunks", "split.%05d.fa" % n)
+                            self.chunk_files[n] = fo
+                            fh = open(fo, "wb")
+                        line = b">" + line[1:]
+                    elif x > 1:
+                        continue
+                    fh.write(line)
+        if fh:
+            fh.close()
 
-    def split_fastx(self, num=10):
+    def split_fastx_by_part(self, part=10):
         self.chunk_files = {str(i): os.path.join(
-            self.outdir, "chunks", "split.%05d.fa" % i) for i in range(num)}
+            self.outdir, "chunks", "split.%05d.fa" % i) for i in range(part)}
         if os.path.isfile(self.query):
             mkdir(os.path.join(self.outdir, "chunks"))
         fx = get_fastx_type(self.query)
         with Zopen(self.query, mode="rb") as fi, MultiFileOpen(mode="wb", **self.chunk_files) as fo:
             if fx == "fasta":
                 for line in fi:
                     if line.startswith(b">"):
-                        n = randrange(0, num)
+                        n = randrange(0, part)
                         fh = fo[n]
                     fh.write(line)
             elif fx == "fastq":
                 for i, line in enumerate(fi):
                     x = i % 4
                     if x == 0:
-                        n = randrange(0, num)
+                        n = randrange(0, part)
                         fh = fo[n]
                         line = b">" + line[1:]
                     elif x > 1:
                         continue
                     fh.write(line)
 
     @property
@@ -81,30 +130,37 @@
         mkdir(os.path.join(self.outdir, "results"))
         self.args.jobfile = self.blast_scripts
         self.args.force = True  # force to resubmit
         conf = Config()
         conf.update_dict(**self.args.__dict__)
         if os.path.isfile(self.blast_scripts):
             mkdir(os.path.join(self.outdir, "logs"))
-            runsge_loger = Mylog(self.args.log, "info", name=RunSge.__module__)
-            runsge = RunSge(config=conf)
-            h = ParseSingal(obj=runsge, name=self.args.jobname,
-                            mode=self.args.mode, conf=conf)
-            h.start()
-            runsge.run(times=0)
-            if not runsge.sumstatus():
-                os.kill(os.getpid(), signal.SIGTERM)
-            runsge_loger.info("hpc blast finished")
+            loger = log(self.args.log, "info", name=runsge.__module__)
+            job = runsge(config=conf)
+            job.set_rate(20)
+            job.run()
+            loger.info("hpc blast finished")
+            self.finished = True
 
     def mergs_res(self):
         if self.chunk_res:
             with open(self.outfile, "wb") as fo:
                 for f in self.chunk_res:
                     with open(f, "rb") as fi:
                         for line in fi:
                             fo.write(line)
 
     def run(self):
-        self.split_fastx(self.args.split)
+        if self.args.size:
+            self.split_fastx_by_size(self.args.size)
+        else:
+            self.split_fastx_by_part(self.args.split)
         self.write_blast_sh()
         self.run_blast()
         self.mergs_res()
+
+    def __del__(self):
+        try:
+            if self.cleandir:
+                shutil.rmtree(self.outdir)
+        except:
+            pass
```

## hpcblast/utils.py

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 
 import os
 import sys
 import gzip
 import shlex
+import shutil
 import signal
+import tempfile
 import argparse
 import subprocess
 
 from random import randrange
 
-from runjob.utils import Mylog
+from runjob import log, runsge
 from runjob.config import Config
-from runjob.sge_run import RunSge
-from runjob.sge import ParseSingal
 
 from ._version import __version__
 
 
 class Zopen(object):
     def __init__(self, name,  mode="rb"):
         self.name = name
@@ -66,17 +66,20 @@
 
 def mkdir(path):
     if not os.path.isdir(path):
         os.makedirs(path)
 
 
 def get_fastx_type(fastx):
-    if (fastx.lower().endswith(".fasta") or fastx.lower().endswith(".fa") or fastx.lower().endswith(".fasta.gz")):
+    fastx_ = fastx.lower()
+    if fastx_.endswith(".gz"):
+        fastx_ = fastx_[:-3]
+    if fastx_.endswith(".fasta") or fastx_.endswith(".fa"):
         return "fasta"
-    elif (fastx.lower().endswith(".fastq") or fastx.lower().endswith(".fq") or fastx.lower().endswith(".fastq.gz")):
+    elif fastx_.endswith(".fastq") or fastx_.endswith(".fq"):
         return "fastq"
     fastx_type = "fastq"
     with Zopen(fastx) as fi:
         curr_line = 0
         for line in fi:
             if line.startswith(b">"):
                 fastx_type = "fasta"
@@ -138,47 +141,52 @@
             subprocess.check_call(cmd, shell=True, stdout=fo, stderr=fo)
 
 
 def canonicalize(path):
     return os.path.abspath(os.path.expanduser(path))
 
 
-blast_dbtype = {"blastn": "nucl",
-                "blastp": "prot",
-                "blastx": "prot",
-                "tblastn": "nucl",
-                "tblastx": "nucl",
-                }
+blast_dbtype = {
+    "blastn": "nucl",
+    "blastp": "prot",
+    "blastx": "prot",
+    "tblastn": "nucl",
+    "tblastx": "nucl",
+}
 
 
 def HPCBlastArg():
     parser = argparse.ArgumentParser(
-        description="hpc-blast <OPTIONS> <blast commands>", add_help=False)
-    parser.add_argument("--split", type=int, default=10,
-                        help='split query into num of chunks, 10 by default', metavar="<int>")
-    parser.add_argument("--queue", type=str, default="all.q",
-                        help='sge queue, all.q by default, multi-queue can be sepreated by whitespace', nargs="*", metavar="<str>")
-    parser.add_argument("--cpu", type=int, default=1,
-                        help='cpu usage for sge, 1 by default, max(--cpu, -num_threads) will be used', metavar="<int>")
-    parser.add_argument("--memory", type=int, default=1,
-                        help='memory (GB) usage for sge, 1 by default', metavar="<int>")
+        description="hpc-blast <OPTIONS> <blast command>", add_help=False)
+    ex_args = parser.add_mutually_exclusive_group(required=False)
+    ex_args.add_argument("--split", type=int, default=10,
+                         help='split query into num of chunks, 10 by default', metavar="<int>")
+    ex_args.add_argument("--size", type=int,
+                         help='split query into multi chunks with N sequences', metavar="<int>")
     parser.add_argument("--num", type=int,
-                        help='max number of chunks run parallelly, default: all', metavar="<int>")
-    parser.add_argument("--output", type=str, required=True,
+                        help='max number of chunks run parallelly, all chunks by default', metavar="<int>")
+    parser.add_argument("--output", type=str, required=False,
                         help='hpc blast output directory', metavar="<str>")
     parser.add_argument("--log", type=str,
                         help='append hpc-blast log info to file, sys.stdout by default', metavar="<file>")
     parser.add_argument("--local", action='store_true',
                         help="run blast in localhost instead of sge", default=False)
     parser.add_argument('--version',
                         action='version', version="v" + __version__)
     parser.add_argument("-h", '--help',
                         action='help', help="show this help message and exit")
     parser.add_argument("blast", type=str,
-                        help='blast command', metavar="<blast command>")
+                        help='blast command, required', metavar="<blast command>")
+    sge_group = parser.add_argument_group("sge arguments")
+    sge_group.add_argument("--queue", type=str,
+                           help='sge queue, multi-queue can be sepreated by whitespace, all access queue by default', nargs="*", metavar="<str>")
+    sge_group.add_argument("--cpu", type=int, default=1,
+                           help='cpu usage for sge, 1 by default, max(--cpu, -num_threads) will be used', metavar="<int>")
+    sge_group.add_argument("--memory", type=int, default=1,
+                           help='memory (GB) usage for sge, 1 by default', metavar="<int>")
     args, unknown_args = parser.parse_known_args()
     c, o, d, q = 0, 0, 0, 0
     for a in sys.argv[1:]:
         if a == "-num_threads":
             c = 1
         elif a == "-out":
             unknown_args.remove(a)
```

## Comparing `hpcblast-1.0.0.dist-info/LICENSE` & `hpcblast-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hpcblast-1.0.0.dist-info/METADATA` & `hpcblast-1.0.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: hpcblast
-Version: 1.0.0
-Summary: UNKNOWN
+Version: 1.0.1
 Home-page: https://github.com/yodeng/hpc-blast
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cython
 Requires-Dist: runjob
 
 # hpcblast
 
-`hpcblast`软件用于在`HPC`环境下运行`NCBI-BLAST+`套件程序，提供了简单高效的方法，通过将比对输入文件进行拆分并利用`HPC`环境加速blast查找速度。当`blast`比对输入序列较多，运行速度较慢时使用`hpcblast`有明显的性能提升。
+`hpcblast`软件为在`HPC`环境`(Sun Grid Engine)`下运行`NCBI-BLAST+`套件程序提供了简单高效的方法，其通过将比对输入文件进行拆分并利用`HPC`环境加速blast查找速度。当`blast`比对输入文件序列较多，运行速度较慢时使用`hpcblast`有明显的性能提升。
 
 ### 1. 特性
 
 + `hpcblast`将比对序列随机拆分成小文件并将任务并发运行在`SGE`或本地环境中
 + `hpcblast`兼容全部的`NCBI-BLAST+`选项和命令，结果和`NCBI-BLAST+`相同
 + `hpcblast`支持`fa/fq`格式，支持`gz`压缩格式输入，无需将`fastq`解压并转为`fasta`步骤
 + `hpcblast`统一的任务管理调度，自动管理资源，当程序中断或报错情况，自动销毁运行中的任务
@@ -50,62 +48,66 @@
 pip3 install hpcblast -U
 ```
 
 ### 4. 使用
 
 ```
 $ hpc-blast -h 
-usage: hpc-blast [--split <int>] [--queue [<str> ...]] [--cpu <int>] [--memory <int>] [--num <int>] --output <str> [--log <file>] [--local] [--version] [-h] <blast command>
+usage: hpc-blast [--split <int> | --size <int>] [--num <int>] [--output <str>] [--log <file>] [--local] [--version] [-h] [--queue [<str> ...]]
+                 [--cpu <int>] [--memory <int>]
+                 <blast command>
 
-hpc-blast <OPTIONS> <blast commands>
+hpc-blast <OPTIONS> <blast command>
 
 positional arguments:
-  <blast command>      blast command
+  <blast command>      blast command, required
 
 optional arguments:
   --split <int>        split query into num of chunks, 10 by default
-  --queue [<str> ...]  sge queue, all.q by default, multi-queue can be sepreated by whitespace
-  --cpu <int>          cpu usage for sge, 1 by default, max(--cpu, -num_threads) will be used
-  --memory <int>       memory (GB) usage for sge, 1 by default
-  --num <int>          max number of chunks run parallelly, default: all
+  --size <int>         split query into multi chunks with N sequences
+  --num <int>          max number of chunks run parallelly, all chunks by default
   --output <str>       hpc blast output directory
   --log <file>         append hpc-blast log info to file, sys.stdout by default
   --local              run blast in localhost instead of sge
   --version            show program's version number and exit
   -h, --help           show this help message and exit
+
+sge arguments:
+  --queue [<str> ...]  sge queue, multi-queue can be sepreated by whitespace, all access queue by default
+  --cpu <int>          cpu usage for sge, 1 by default, max(--cpu, -num_threads) will be used
+  --memory <int>       memory (GB) usage for sge, 1 by default
 ```
 
 相关参数解释如下：
 
 | 参数       | 描述                                                         |
 | ---------- | ------------------------------------------------------------ |
 | --split    | 将输入序列拆分为多少份                                       |
-| --queue    | 如果运行在`sge`环境，则传入指定的队列名，多个队列用空白隔开，默认`all.q` |
-| --cpu      | 如果运行在`sge`环境，则任务申请的`cpu`资源数，默认1，会识别`blast`参数中的`-num_thread`参数，使用较大的值 |
-| --memory   | 如果运行在`sge`环境，则任务申请的内存，默认1，单位`GB`       |
+| --size     | 将输入序列拆分，每份指定多少序列条数                         |
 | --num      | `hpcblast`任务队列，将拆分的块发送到`hpcblast`任务队列中，代表同时运行的拆分块任务数，默认全部拆分块同时运行 |
 | --output   | `hpcblast`输出目录，不存在会自动创建                         |
 | --log      | `hpcblast`输出日志文件，默认标准输出                         |
 | --local    | 强制`hpcblast`本地并发运行，不使用`sge`运行。                |
 | --version  | 打印`hpcblast`版本并退出                                     |
 | -h, --help | 打印`hpcblast`帮助并退出                                     |
+| --queue    | 如果运行在`sge`环境，则传入指定的队列名，多个队列用空白隔开，默认全部可用队列 |
+| --cpu      | 如果运行在`sge`环境，则任务申请的`cpu`资源数，默认1，会识别`blast`参数中的`-num_thread`参数，使用较大的值 |
+| --memory   | 如果运行在`sge`环境，则任务申请的内存，默认1，单位`GB`       |
 
 **说明**：
 
 + `hpc-blast`选项使用两个中划线`--`，`blast`选项使用一个中划线`-`
-
 + `hpc-blast`命令和选项后面直接跟需要运行的blast命令即可，完全兼容，命令阻塞直到全部任务运行完成
-+ `hpcblast`任务队列为最大允许同时运行的任务快，当某个任务快运行完成时会立即添加一个任务块到任务队列中运行
++ `hpcblast`任务队列为最大允许同时运行的任务块，当某个任务块运行完成时会立即添加一个任务块到任务队列中并启动运行
 + `hpcblast`主线程管理各并发子任务块，主线程几乎不占用cpu和内存资源，主程序终止，其管理的本地或sge任务自动清空，无需手动销毁
 + `hpc-blast`识别`blast`命令中的`-query`和`-num_thread`参数，`-query`后面可直接跟`fa/fq`格式文件（支持`*.gz`压缩格式）
 + `hpc-blast`随机拆分输入文件，拆分过程无须将全部序列读入内存，无内存消耗，比对输出结果无序
 + 并发环境，需注意使用的`cpu`和内存资源
 
 ### 5. 示例
 
 以下命令表示将`test.fastq.gz`序列随机拆分成`200`份进行`blastn`比对，任务投递到`sge`集群中，投递队列为`all.q`和`test.q`，使用资源`virtual_free=1g,num_proc=4`，允许同时运行的最大任务数为`50`个，`blastn`输出结果文件为`test.blast.m6`，`hpc-blast`输出目录为当前目录下的`out`目录。
 
 ```
 hpc-blast --split 200 --queue all.q test.q --num 50 --output out blastn -query test.fastq.gz -db /data/refdb -num_threads 4 -out test.blast.m6 -outfmt "6 qseqid qlen qstart qend"
 ```
 
-
```

## Comparing `hpcblast-1.0.0.dist-info/RECORD` & `hpcblast-1.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 hpcblast/__init__.py,sha256=ZygAIkX6Nbjag1czWdQa-yP-GM1mBE_9ss21Xh__JFc,34
-hpcblast/_version.py,sha256=J-j-u0itpEFT6irdmWmixQqYMadNl1X91TxUmoiLHMI,22
+hpcblast/_version.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
 hpcblast/main.py,sha256=aoxML-Qo96y_2kWo_TKVkS9evKhriSDTzme56jIZN6s,151
-hpcblast/src.py,sha256=VvunwOpX1660Ex6o9dyK4qW1E16C7oWAP_COApBkSF4,4277
-hpcblast/utils.py,sha256=DV5Qqoqpt71s5Ft5P4-hhkmm1mihV3ugquhpsJoROLc,6609
-hpcblast-1.0.0.dist-info/LICENSE,sha256=NPhTiU6xEYnFPLB9rlmsTVfU7qLJHuBT6bmQ3KFkBgE,1094
-hpcblast-1.0.0.dist-info/METADATA,sha256=Vf_LafbOBXfD0ppNRiXCn3Wamlt7eoJQGIPqhZIs0AA,5261
-hpcblast-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-hpcblast-1.0.0.dist-info/entry_points.txt,sha256=_QQOruj9xQehF9RgdA-sLN7_gomdqQ4tdA_I6OVQ-8I,50
-hpcblast-1.0.0.dist-info/top_level.txt,sha256=6UT0wBs5o0FWZkuihpYrL-R5Y8e_93LrWRqpfEqDxR8,9
-hpcblast-1.0.0.dist-info/RECORD,,
+hpcblast/src.py,sha256=UPiw2BgX6EoI98o-GEbYFQm22HyfTXZoM6jqM-vnpdc,6204
+hpcblast/utils.py,sha256=pO3GKt5bISxBhrMZqqiXef-96NMybAMRApDYzgyo7gQ,6788
+hpcblast-1.0.1.dist-info/LICENSE,sha256=NPhTiU6xEYnFPLB9rlmsTVfU7qLJHuBT6bmQ3KFkBgE,1094
+hpcblast-1.0.1.dist-info/METADATA,sha256=ZsD_khwcxnZ8nDQ71aFM0vC3AmaxKDqoBLVCL1dOBMM,5528
+hpcblast-1.0.1.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
+hpcblast-1.0.1.dist-info/entry_points.txt,sha256=o3N7LuF2aVHfr5PjMkgUsZF8lL1xE61MAPdYRgmYETE,49
+hpcblast-1.0.1.dist-info/top_level.txt,sha256=6UT0wBs5o0FWZkuihpYrL-R5Y8e_93LrWRqpfEqDxR8,9
+hpcblast-1.0.1.dist-info/RECORD,,
```

