# Comparing `tmp/fastq_handler-0.1.3.tar.gz` & `tmp/fastq_handler-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastq_handler-0.1.3.tar", max compression
+gzip compressed data, was "fastq_handler-0.2.0.tar", max compression
```

## Comparing `fastq_handler-0.1.3.tar` & `fastq_handler-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    31904 2023-04-08 10:54:25.406907 fastq_handler-0.1.3/LICENSE
--rw-r--r--   0        0        0     2393 2023-04-11 23:25:16.755777 fastq_handler-0.1.3/README.md
--rw-r--r--   0        0        0      708 2023-04-11 23:23:04.423006 fastq_handler-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 23:12:44.814007 fastq_handler-0.1.3/src/fastq_handler/__init__.py
--rw-r--r--   0        0        0     1609 2023-04-11 23:22:46.582883 fastq_handler-0.1.3/src/fastq_handler/__main__.py
--rw-r--r--   0        0        0     1488 2023-04-11 23:12:44.810006 fastq_handler-0.1.3/src/fastq_handler/actions.py
--rw-r--r--   0        0        0     1068 2023-04-11 23:12:44.810006 fastq_handler-0.1.3/src/fastq_handler/configs.py
--rw-r--r--   0        0        0    12595 2023-04-11 23:12:44.810006 fastq_handler-0.1.3/src/fastq_handler/fastq_handler.py
--rw-r--r--   0        0        0     6758 2023-04-11 23:12:44.814007 fastq_handler-0.1.3/src/fastq_handler/records.py
--rw-r--r--   0        0        0     3984 2023-04-11 23:12:44.814007 fastq_handler-0.1.3/src/fastq_handler/utilities.py
--rw-r--r--   0        0        0     3414 2023-04-11 23:25:20.344028 fastq_handler-0.1.3/setup.py
--rw-r--r--   0        0        0     3086 2023-04-11 23:25:20.344427 fastq_handler-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    31904 2023-04-08 10:54:25.406907 fastq_handler-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2550 2023-04-12 13:41:44.822767 fastq_handler-0.2.0/README.md
+-rw-r--r--   0        0        0      834 2023-04-12 13:45:45.504468 fastq_handler-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 13:11:04.485704 fastq_handler-0.2.0/src/fastq_handler/__init__.py
+-rw-r--r--   0        0        0     2121 2023-04-12 13:28:10.461007 fastq_handler-0.2.0/src/fastq_handler/__main__.py
+-rw-r--r--   0        0        0     3535 2023-04-12 13:16:46.900154 fastq_handler-0.2.0/src/fastq_handler/actions.py
+-rw-r--r--   0        0        0     1068 2023-04-12 13:11:04.481704 fastq_handler-0.2.0/src/fastq_handler/configs.py
+-rw-r--r--   0        0        0    11309 2023-04-12 13:18:03.328698 fastq_handler-0.2.0/src/fastq_handler/fastq_handler.py
+-rw-r--r--   0        0        0     6758 2023-04-12 13:11:04.485704 fastq_handler-0.2.0/src/fastq_handler/records.py
+-rw-r--r--   0        0        0     4588 2023-04-12 13:11:04.485704 fastq_handler-0.2.0/src/fastq_handler/utilities.py
+-rw-r--r--   0        0        0     3632 2023-04-12 13:45:57.601206 fastq_handler-0.2.0/setup.py
+-rw-r--r--   0        0        0     3402 2023-04-12 13:45:57.601651 fastq_handler-0.2.0/PKG-INFO
```

### Comparing `fastq_handler-0.1.3/LICENSE` & `fastq_handler-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.3/README.md` & `fastq_handler-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # Fastq Handler
 
 [![PyPI version](https://badge.fury.io/py/fastq-handler.svg)](https://badge.fury.io/py/fastq-handler)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
 [![PyPI license](https://img.shields.io/pypi/l/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
-[![PyPI status](https://img.shields.io/pypi/status/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
 [![PyPI format](https://img.shields.io/pypi/format/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
 
-A python module to process ONT fastq files by concatenating reads as they are generated during a sequencing run
+_A python module to process ONT fastq files by concatenating reads as they are generated during a sequencing run_
 
 ## INTRODUCTION
 
 The _fastqc-handler_ module screens folders and subfolders for fastq (fastq or fastq.gz format) files and concatenates them iteratively. This is useful for merging same-sample reads that are split into multiple files, as commonly obtained in ONT sequencing. The output is a one file per
 output fastq.gz, containing all reads from the previous files. The output directory structure is maintained.
 
 ## INPUT
 
 A directory containing fastq files. The files can be in subfolders (each representing a different sample). The files can be gzipped or not.
 
-## USAGE
+## API
 
 ```bash
-usage: fastq_handler [-h] [-i INPUT] [-o OUTPUT] [-n TAG] [--keep_names]
+usage: fastq_handler [-h] -i IN_DIR -o OUT_DIR [-s SLEEP] [-n TAG] [--keep_names] [--monitor] [--max-size MAX_SIZE] [--downsize] [--merge]
 
-parse arguments
+Process fastq files.
 
 optional arguments:
-    -h, --help            show this help message and exit
-    -i INPUT, --input INPUT
+  -h, --help            show this help message and exit
+  -i IN_DIR, --in_dir IN_DIR
                         Input directory
-    -o OUTPUT, --output OUTPUT
+  -o OUT_DIR, --out_dir OUT_DIR
                         Output directory
-    -n TAG, --tag TAG     Tag to add to output file name
-    --keep_names          Keep original file names in output file
-    --max-size MAX_SIZE   max size of the output file, in kilobytes
+  -s SLEEP, --sleep SLEEP
+                        Sleep time
+  -n TAG, --tag TAG     name tag, if given, will be added to the output file names
+  --keep_names          keep original file names
+  --monitor             run indefinitely
+  --max-size MAX_SIZE   max size of the output file, in kilobytes
+  --downsize            downsize fastq files to max-size
+  --merge               merge files
 ```
 
 ## REQUIREMENTS
 
 **Modules**
 
 - dataclasses==0.6
```

### Comparing `fastq_handler-0.1.3/pyproject.toml` & `fastq_handler-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [tool.poetry]
 name = "fastq_handler"
-version = "0.1.3"
+version = "0.2.0"
 description = "A python module to process minion fastq files by concatenating reads as they are generated"
 authors = ["SantosJGND <dourado.jns@gmail.com>", "Andre Santos <xiaodre2112@gmail.com>", "insapathogenomics <insapathogenomics@insa.min-saude.pt>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dataclasses = "0.6"
 natsort = "8.3.1"
 pandas = "1.5.3"
 pip = "21.2.3"
 setuptools = "57.4.0"
 xopen = "1.7.0"
+dnaio = "^0.10.0"
+fastq-filter = "^0.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 fastq_handler = "fastq_handler.__main__:main"
+
+[tool.poetry.urls]
+homepage = "https://github.com/insapathogenomics/fastq-handler"
```

### Comparing `fastq_handler-0.1.3/src/fastq_handler/__main__.py` & `fastq_handler-0.2.0/src/fastq_handler/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 
 from fastq_handler.fastq_handler import PreMain
 
-from fastq_handler.actions import ProcessActionMergeWithLast
+from fastq_handler.actions import ProcessActionMergeWithLast, ProcessActionDownsize
 from fastq_handler.configs import RunConfig
 
 
 def get_arguments():
     parser = argparse.ArgumentParser(description="Process fastq files.")
     parser.add_argument(
         "-i", "--in_dir", help="Input directory", required=True)
@@ -24,26 +24,43 @@
 
     parser.add_argument(
         "--monitor", help="run indefinitely", action="store_true")
 
     parser.add_argument(
         "--max-size", help="max size of the output file, in kilobytes", type=int, default=400000)
 
+    parser.add_argument(
+        "--downsize", help="downsize fastq files to max-size", action="store_true")
+
+    parser.add_argument("--merge", help="merge files", action="store_true")
+
     return parser.parse_args()
 
 
 def main():
 
     args = get_arguments()
 
+    actions = []
+
+    if args.merge:
+        actions.append(ProcessActionMergeWithLast())
+
+    if args.downsize:
+        actions.append(ProcessActionDownsize(args.max_size * 1000))
+
+    if not actions:
+        print("No actions specified, will merge files by default")
+        actions.append(ProcessActionMergeWithLast())
+
     run_metadata = RunConfig(
         fastq_dir=args.in_dir,
         output_dir=args.out_dir,
         name_tag=args.tag,
-        actions=[ProcessActionMergeWithLast],
+        actions=actions,
         keep_name=args.keep_names,
         sleep_time=args.sleep,
         max_size=(args.max_size * 1000),
     )
 
     compressor = PreMain(
         run_metadata,
```

### Comparing `fastq_handler-0.1.3/src/fastq_handler/configs.py` & `fastq_handler-0.2.0/src/fastq_handler/configs.py`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.3/src/fastq_handler/fastq_handler.py` & `fastq_handler-0.2.0/src/fastq_handler/fastq_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,30 +14,14 @@
 
 from fastq_handler.configs import RunConfig
 from fastq_handler.records import Processed
 from fastq_handler.utilities import Utils
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
-
-"""
-Notes:
-- Now automatically detects if there's barcoding or not and also the format.
-- Now it always creates .fastq.gz merged files.
-
-TO DO:
-- de sleep em sleep fazer uma pasta com 'lattest_compilation_to_upload' todos os últimos concatenados por amostra
-(barcode10, barcode11, etc) + um ficheiro de metadata com todos os dados respetivos dos concatenados totais.
-
-"""
-
-HELP = " _________________________________________________\n | mfmc.py - MERGING FASTQ AND METADATA CREATION | \n _________________________________________________\nExample of usage:\npython mfmc.py --in_dir C:\\users\\samples --out_dir C:\\users\processed_files --tsv_t_name template.tsv --tsv_t_dir C:\\users\\templates \n\nOptions and arguments:\n--in_dir [DIRECTORY OF THE FAST_PASS] : directory of the files being produced by the sequencing machine (typically the 'fast_pass' folder).\n--out_dir [OUTPUT DIRECTORY or 'q' for the default] : desired directory to storage the output files\n--tsv_t_n [TSV TEMPLATE FILE NAME] : name of the tsv template\n--tsv_t_dir [TSV TEMPLATE DIRECTORY] : directory of the tsv template file\n--sleep [TIME SLEEP] : amount of time (in seconds) for the script to hold, between search cycles"
-ARGUMENT_OPTIONS = ["--in_dir", "--out_dir", "--tsv_t_n", "--tsv_t_dir"]
-
-
 ####################         5 - Main functions          #####################
 
 
 class PreMain:
 
     start_time: float
     folder_files: list = []
@@ -392,29 +376,30 @@
         destination_file = fastq_file
 
         if self.run_metadata.actions:
 
             destination_file = self.set_destination_filepath(
                 fastq_file, self.fastq_dir)
 
-            self.append_to_file(fastq_file, destination_file)
-
             sample_id = self.processed.get_sample_id_from_merged(
                 destination_file)
 
+            ###########################################
+
             projected_size = self.estimate_actions_size(
-                destination_file, sample_id)
+                fastq_file, sample_id)
 
             if projected_size > self.run_metadata.max_size:
-                os.remove(destination_file)
                 self.processed.ignore_this(
                     fastq_file
                 )
                 return self
 
+            self.append_to_file(fastq_file, destination_file)
+
             for process_action in self.run_metadata.actions:
 
                 process_action.process(
                     destination_file, sample_id, self.processed)
 
         self.update_processed(fastq_file, self.fastq_dir,
                               destination_file)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastq_handler-0.1.3/src/fastq_handler/records.py` & `fastq_handler-0.2.0/src/fastq_handler/records.py`

 * *Files identical despite different names*

### Comparing `fastq_handler-0.1.3/src/fastq_handler/utilities.py` & `fastq_handler-0.2.0/src/fastq_handler/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,40 @@
         ):
             os.makedirs(
                 os.path.dirname(destination)
             )
 
         shutil.copy(input_file, destination)
 
+    def temp_fastq_file(self, fastq_file: str):
+        """
+        get temp fastq file
+        """
+
+        if fastq_file.endswith(".gz"):
+            temp_fastq_file = fastq_file[:-3] + ".temp.gz"
+        else:
+            temp_fastq_file = fastq_file + ".temp"
+
+        return temp_fastq_file
+
+    def move_file(self, input_file, destination):
+        """
+        move file
+        """
+
+        if not os.path.exists(
+            os.path.dirname(destination)
+        ):
+            os.makedirs(
+                os.path.dirname(destination)
+            )
+
+        shutil.move(input_file, destination)
+
     def seqs_in_dir(self, fastq_dir: str):
         """
         Check if there are any fastq files in the directory
         """
         ext = ""
         constans = ConstantsSettings()
```

### Comparing `fastq_handler-0.1.3/setup.py` & `fastq_handler-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 ['fastq_handler']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['dataclasses==0.6',
+ 'dnaio>=0.10.0,<0.11.0',
+ 'fastq-filter>=0.3.0,<0.4.0',
  'natsort==8.3.1',
  'pandas==1.5.3',
  'pip==21.2.3',
  'setuptools==57.4.0',
  'xopen==1.7.0']
 
 entry_points = \
 {'console_scripts': ['fastq_handler = fastq_handler.__main__:main']}
 
 setup_kwargs = {
     'name': 'fastq-handler',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': 'A python module to process minion fastq files by concatenating reads as they are generated',
-    'long_description': '# Fastq Handler\n\n[![PyPI version](https://badge.fury.io/py/fastq-handler.svg)](https://badge.fury.io/py/fastq-handler)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n[![PyPI license](https://img.shields.io/pypi/l/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n[![PyPI status](https://img.shields.io/pypi/status/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n[![PyPI format](https://img.shields.io/pypi/format/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n\nA python module to process ONT fastq files by concatenating reads as they are generated during a sequencing run\n\n## INTRODUCTION\n\nThe _fastqc-handler_ module screens folders and subfolders for fastq (fastq or fastq.gz format) files and concatenates them iteratively. This is useful for merging same-sample reads that are split into multiple files, as commonly obtained in ONT sequencing. The output is a one file per\noutput fastq.gz, containing all reads from the previous files. The output directory structure is maintained.\n\n## INPUT\n\nA directory containing fastq files. The files can be in subfolders (each representing a different sample). The files can be gzipped or not.\n\n## USAGE\n\n```bash\nusage: fastq_handler [-h] [-i INPUT] [-o OUTPUT] [-n TAG] [--keep_names]\n\nparse arguments\n\noptional arguments:\n    -h, --help            show this help message and exit\n    -i INPUT, --input INPUT\n                        Input directory\n    -o OUTPUT, --output OUTPUT\n                        Output directory\n    -n TAG, --tag TAG     Tag to add to output file name\n    --keep_names          Keep original file names in output file\n    --max-size MAX_SIZE   max size of the output file, in kilobytes\n```\n\n## REQUIREMENTS\n\n**Modules**\n\n- dataclasses==0.6\n- natsort==8.3.1\n- pandas==1.5.3\n- setuptools==57.4.0\n- xopen==1.7.0\n\n## INSTALLATION\n\n```bash\npython -m venv .venv\nsource .venv/bin/activate\npython -m pip install fastq-handler\n```\n\n## MAIN OUTPUTS\n\n> **Note:** The output directory structure is maintained.\n\n- **fastq.gz** files containing all reads from the previous files.\n- **log.txt** file containing the concatenation process.\n\n## Maintainers\n\n- [**@xiaodre21**](https://github.com/xiaodre21)\n- [**@santosjgnd**](https://github.com/SantosJGND)\n- [**@insaflu**](https://github.com/insapathogenomics)\n',
+    'long_description': '# Fastq Handler\n\n[![PyPI version](https://badge.fury.io/py/fastq-handler.svg)](https://badge.fury.io/py/fastq-handler)\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n[![PyPI license](https://img.shields.io/pypi/l/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n[![PyPI format](https://img.shields.io/pypi/format/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)\n\n_A python module to process ONT fastq files by concatenating reads as they are generated during a sequencing run_\n\n## INTRODUCTION\n\nThe _fastqc-handler_ module screens folders and subfolders for fastq (fastq or fastq.gz format) files and concatenates them iteratively. This is useful for merging same-sample reads that are split into multiple files, as commonly obtained in ONT sequencing. The output is a one file per\noutput fastq.gz, containing all reads from the previous files. The output directory structure is maintained.\n\n## INPUT\n\nA directory containing fastq files. The files can be in subfolders (each representing a different sample). The files can be gzipped or not.\n\n## API\n\n```bash\nusage: fastq_handler [-h] -i IN_DIR -o OUT_DIR [-s SLEEP] [-n TAG] [--keep_names] [--monitor] [--max-size MAX_SIZE] [--downsize] [--merge]\n\nProcess fastq files.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -i IN_DIR, --in_dir IN_DIR\n                        Input directory\n  -o OUT_DIR, --out_dir OUT_DIR\n                        Output directory\n  -s SLEEP, --sleep SLEEP\n                        Sleep time\n  -n TAG, --tag TAG     name tag, if given, will be added to the output file names\n  --keep_names          keep original file names\n  --monitor             run indefinitely\n  --max-size MAX_SIZE   max size of the output file, in kilobytes\n  --downsize            downsize fastq files to max-size\n  --merge               merge files\n```\n\n## REQUIREMENTS\n\n**Modules**\n\n- dataclasses==0.6\n- natsort==8.3.1\n- pandas==1.5.3\n- setuptools==57.4.0\n- xopen==1.7.0\n\n## INSTALLATION\n\n```bash\npython -m venv .venv\nsource .venv/bin/activate\npython -m pip install fastq-handler\n```\n\n## MAIN OUTPUTS\n\n> **Note:** The output directory structure is maintained.\n\n- **fastq.gz** files containing all reads from the previous files.\n- **log.txt** file containing the concatenation process.\n\n## Maintainers\n\n- [**@xiaodre21**](https://github.com/xiaodre21)\n- [**@santosjgnd**](https://github.com/SantosJGND)\n- [**@insaflu**](https://github.com/insapathogenomics)\n',
     'author': 'SantosJGND',
     'author_email': 'dourado.jns@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `fastq_handler-0.1.3/PKG-INFO` & `fastq_handler-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 Metadata-Version: 2.1
 Name: fastq-handler
-Version: 0.1.3
+Version: 0.2.0
 Summary: A python module to process minion fastq files by concatenating reads as they are generated
 License: MIT
 Author: SantosJGND
 Author-email: dourado.jns@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: dataclasses (==0.6)
+Requires-Dist: dnaio (>=0.10.0,<0.11.0)
+Requires-Dist: fastq-filter (>=0.3.0,<0.4.0)
 Requires-Dist: natsort (==8.3.1)
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pip (==21.2.3)
 Requires-Dist: setuptools (==57.4.0)
 Requires-Dist: xopen (==1.7.0)
+Project-URL: homepage, https://github.com/insapathogenomics/fastq-handler
 Description-Content-Type: text/markdown
 
 # Fastq Handler
 
 [![PyPI version](https://badge.fury.io/py/fastq-handler.svg)](https://badge.fury.io/py/fastq-handler)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
 [![PyPI license](https://img.shields.io/pypi/l/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
-[![PyPI status](https://img.shields.io/pypi/status/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
 [![PyPI format](https://img.shields.io/pypi/format/fastq-handler.svg)](https://pypi.python.org/pypi/fastq-handler/)
 
-A python module to process ONT fastq files by concatenating reads as they are generated during a sequencing run
+_A python module to process ONT fastq files by concatenating reads as they are generated during a sequencing run_
 
 ## INTRODUCTION
 
 The _fastqc-handler_ module screens folders and subfolders for fastq (fastq or fastq.gz format) files and concatenates them iteratively. This is useful for merging same-sample reads that are split into multiple files, as commonly obtained in ONT sequencing. The output is a one file per
 output fastq.gz, containing all reads from the previous files. The output directory structure is maintained.
 
 ## INPUT
 
 A directory containing fastq files. The files can be in subfolders (each representing a different sample). The files can be gzipped or not.
 
-## USAGE
+## API
 
 ```bash
-usage: fastq_handler [-h] [-i INPUT] [-o OUTPUT] [-n TAG] [--keep_names]
+usage: fastq_handler [-h] -i IN_DIR -o OUT_DIR [-s SLEEP] [-n TAG] [--keep_names] [--monitor] [--max-size MAX_SIZE] [--downsize] [--merge]
 
-parse arguments
+Process fastq files.
 
 optional arguments:
-    -h, --help            show this help message and exit
-    -i INPUT, --input INPUT
+  -h, --help            show this help message and exit
+  -i IN_DIR, --in_dir IN_DIR
                         Input directory
-    -o OUTPUT, --output OUTPUT
+  -o OUT_DIR, --out_dir OUT_DIR
                         Output directory
-    -n TAG, --tag TAG     Tag to add to output file name
-    --keep_names          Keep original file names in output file
-    --max-size MAX_SIZE   max size of the output file, in kilobytes
+  -s SLEEP, --sleep SLEEP
+                        Sleep time
+  -n TAG, --tag TAG     name tag, if given, will be added to the output file names
+  --keep_names          keep original file names
+  --monitor             run indefinitely
+  --max-size MAX_SIZE   max size of the output file, in kilobytes
+  --downsize            downsize fastq files to max-size
+  --merge               merge files
 ```
 
 ## REQUIREMENTS
 
 **Modules**
 
 - dataclasses==0.6
```

