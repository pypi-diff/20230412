# Comparing `tmp/langchain_utils-0.3.5.tar.gz` & `tmp/langchain_utils-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.3.5.tar", max compression
+gzip compressed data, was "langchain_utils-0.3.6.tar", max compression
```

## Comparing `langchain_utils-0.3.5.tar` & `langchain_utils-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4589 2023-04-10 07:12:43.729444 langchain_utils-0.3.5/README.md
--rw-r--r--   0        0        0       22 2023-04-12 04:41:37.095785 langchain_utils-0.3.5/langchain_utils/__init__.py
--rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.3.5/langchain_utils/config.py
--rwxr-xr-x   0        0        0     3346 2023-04-12 04:39:19.926241 langchain_utils-0.3.5/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2502 2023-04-10 07:36:50.130151 langchain_utils-0.3.5/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.5/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.3.5/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.5/langchain_utils/prompts.py
--rw-r--r--   0        0        0     7217 2023-04-12 04:36:41.629692 langchain_utils-0.3.5/langchain_utils/utils.py
--rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.5/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     1514 2023-04-12 04:41:37.094933 langchain_utils-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5591 1970-01-01 00:00:00.000000 langchain_utils-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     4808 2023-04-12 04:43:07.091701 langchain_utils-0.3.6/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 04:43:14.887039 langchain_utils-0.3.6/langchain_utils/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:46:38.293069 langchain_utils-0.3.6/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     3373 2023-04-12 04:42:32.076969 langchain_utils-0.3.6/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2502 2023-04-10 07:36:50.130151 langchain_utils-0.3.6/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.6/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1410 2023-04-10 04:52:53.679712 langchain_utils-0.3.6/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.6/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     7217 2023-04-12 04:36:41.629692 langchain_utils-0.3.6/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.6/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     1514 2023-04-12 04:43:14.886412 langchain_utils-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5810 1970-01-01 00:00:00.000000 langchain_utils-0.3.6/PKG-INFO
```

### Comparing `langchain_utils-0.3.5/README.md` & `langchain_utils-0.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,15 @@
 ```
 
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
-usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n]
-                 [-p PAGES [PAGES ...]] [-M] [-w WHAT]
+usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-P PARTS [PARTS ...]] [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -72,25 +71,24 @@
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
   -S, --split           Split the prompt into multiple parts (default: False)
   -s chunk_size, --chunk-size chunk_size
-                        Chunk size when splitting transcript, also used to
-                        determine whether to split (default: 2000)
+                        Chunk size when splitting transcript, also used to determine whether to split (default: 2000)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents (default: None)
   -n, --dry-run         Dry run (default: False)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
-  -M, --merge           Merge contents of all pages before processing
-                        (default: False)
-  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
-                        content in the prompt (default: the content of a PDF
-                        file)
-
+  -l PAGE_SLICE, --page-slice PAGE_SLICE
+                        Use Python slice syntax to select page numbers (e.g. 1:3, 1:10:2, etc.) (default: None)
+  -M, --merge           Merge contents of all pages before processing (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a PDF file)
 
 ```
 
 ### `ytprompt`
 
 ```
 $ ytprompt --help
```

### Comparing `langchain_utils-0.3.5/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.3.6/langchain_utils/get_pdf_prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         type=int,
         nargs='+',
         default=None,
     )
     parser.add_argument(
         '-l',
         '--page-slice',
-        help='Use Python list slice to select page numbers',
+        help='Use Python slice syntax to select page numbers (e.g. 1:3, 1:10:2, etc.)',
         type=str,
         default=None,
     )
     parser.add_argument(
         '-M',
         '--merge',
         help='Merge contents of all pages before processing',
```

### Comparing `langchain_utils-0.3.5/langchain_utils/get_url_prompt.py` & `langchain_utils-0.3.6/langchain_utils/get_url_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.5/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.3.6/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.5/langchain_utils/loaders.py` & `langchain_utils-0.3.6/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.5/langchain_utils/utils.py` & `langchain_utils-0.3.6/langchain_utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.5/langchain_utils/utils_argparse.py` & `langchain_utils-0.3.6/langchain_utils/utils_argparse.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.5/pyproject.toml` & `langchain_utils-0.3.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.3.5/PKG-INFO` & `langchain_utils-0.3.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -80,16 +80,15 @@
 ```
 
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
-usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-n]
-                 [-p PAGES [PAGES ...]] [-M] [-w WHAT]
+usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size] [-P PARTS [PARTS ...]] [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -98,25 +97,24 @@
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
                         Model to use (default: gpt-3.5-turbo)
   -S, --split           Split the prompt into multiple parts (default: False)
   -s chunk_size, --chunk-size chunk_size
-                        Chunk size when splitting transcript, also used to
-                        determine whether to split (default: 2000)
+                        Chunk size when splitting transcript, also used to determine whether to split (default: 2000)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents (default: None)
   -n, --dry-run         Dry run (default: False)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
-  -M, --merge           Merge contents of all pages before processing
-                        (default: False)
-  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
-                        content in the prompt (default: the content of a PDF
-                        file)
-
+  -l PAGE_SLICE, --page-slice PAGE_SLICE
+                        Use Python slice syntax to select page numbers (e.g. 1:3, 1:10:2, etc.) (default: None)
+  -M, --merge           Merge contents of all pages before processing (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF content in the prompt (default: the content of a PDF file)
 
 ```
 
 ### `ytprompt`
 
 ```
 $ ytprompt --help
```

