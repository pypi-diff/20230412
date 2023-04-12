# Comparing `tmp/langchain_utils-0.3.7.tar.gz` & `tmp/langchain_utils-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.3.7.tar", max compression
+gzip compressed data, was "langchain_utils-0.3.8.tar", max compression
```

## Comparing `langchain_utils-0.3.7.tar` & `langchain_utils-0.3.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     4808 2023-04-12 04:43:07.091701 langchain_utils-0.3.7/README.md
--rw-r--r--   0        0        0       22 2023-04-12 05:23:27.126659 langchain_utils-0.3.7/langchain_utils/__init__.py
--rw-r--r--   0        0        0      168 2023-04-12 04:44:56.762320 langchain_utils-0.3.7/langchain_utils/config.py
--rwxr-xr-x   0        0        0     3373 2023-04-12 04:42:32.076969 langchain_utils-0.3.7/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     2644 2023-04-12 05:22:36.130523 langchain_utils-0.3.7/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     2528 2023-04-12 05:21:34.707838 langchain_utils-0.3.7/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.7/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     1922 2023-04-12 05:00:54.153184 langchain_utils-0.3.7/langchain_utils/loaders.py
--rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.7/langchain_utils/prompts.py
--rw-r--r--   0        0        0     7622 2023-04-12 05:22:23.854783 langchain_utils-0.3.7/langchain_utils/utils.py
--rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.7/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     1623 2023-04-12 05:23:27.126197 langchain_utils-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     5810 1970-01-01 00:00:00.000000 langchain_utils-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     7895 2023-04-12 05:34:44.784594 langchain_utils-0.3.8/README.md
+-rw-r--r--   0        0        0       22 2023-04-12 05:34:49.338575 langchain_utils-0.3.8/langchain_utils/__init__.py
+-rw-r--r--   0        0        0      222 2023-04-12 05:33:55.491462 langchain_utils-0.3.8/langchain_utils/config.py
+-rwxr-xr-x   0        0        0     2630 2023-04-12 05:34:17.215880 langchain_utils-0.3.8/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     3373 2023-04-12 04:42:32.076969 langchain_utils-0.3.8/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     2660 2023-04-12 05:30:43.018177 langchain_utils-0.3.8/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     2528 2023-04-12 05:21:34.707838 langchain_utils-0.3.8/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     2111 2023-04-10 07:40:28.101477 langchain_utils-0.3.8/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     1922 2023-04-12 05:00:54.153184 langchain_utils-0.3.8/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      445 2023-04-09 14:48:21.143127 langchain_utils-0.3.8/langchain_utils/prompts.py
+-rw-r--r--   0        0        0     7841 2023-04-12 05:25:48.783743 langchain_utils-0.3.8/langchain_utils/utils.py
+-rw-r--r--   0        0        0     1467 2023-04-10 07:33:58.876416 langchain_utils-0.3.8/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     1747 2023-04-12 05:34:49.338114 langchain_utils-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     8933 1970-01-01 00:00:00.000000 langchain_utils-0.3.8/PKG-INFO
```

### Comparing `langchain_utils-0.3.7/README.md` & `langchain_utils-0.3.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 - [langchain-utils](#langchain-utils)
   - [Prompt generation using LangChain document loaders](#prompt-generation-using-langchain-document-loaders)
     - [`urlprompt`](#urlprompt)
     - [`pdfprompt`](#pdfprompt)
     - [`ytprompt`](#ytprompt)
+    - [`textprompt`](#textprompt)
+    - [`htmlprompt`](#htmlprompt)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Develop](#develop)
 
 
 ## Prompt generation using LangChain document loaders
@@ -112,15 +114,90 @@
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split (default: 2000)
   -n, --dry-run         Dry run (default: False)
 
 ```
 
+### `textprompt`
 
+```
+$ textprompt --help
+
+usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                  [-P PARTS [PARTS ...]] [-n] [-w WHAT] [-M]
+                  [PATH ...]
+
+Get a prompt from text files
+
+positional arguments:
+  PATH                  Paths to the text files, or stdin if not provided
+                        (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -c, --copy            Copy the prompt to clipboard (default: False)
+  -e, --edit            Edit the prompt and copy manually (default: False)
+  -m model, --model model
+                        Model to use (default: gpt-3.5-turbo)
+  -S, --split           Split the prompt into multiple parts (default: False)
+  -s chunk_size, --chunk-size chunk_size
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split (default: 2000)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -n, --dry-run         Dry run (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the content of a
+                        document)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+```
+
+
+### `htmlprompt`
+
+```
+$ htmlprompt --help
+
+usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                  [-P PARTS [PARTS ...]] [-n] [-w WHAT] [-M]
+                  [PATH ...]
+
+Get a prompt from html files
+
+positional arguments:
+  PATH                  Paths to the html files, or stdin if not provided
+                        (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -c, --copy            Copy the prompt to clipboard (default: False)
+  -e, --edit            Edit the prompt and copy manually (default: False)
+  -m model, --model model
+                        Model to use (default: gpt-3.5-turbo)
+  -S, --split           Split the prompt into multiple parts (default: False)
+  -s chunk_size, --chunk-size chunk_size
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split (default: 2000)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -n, --dry-run         Dry run (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the text content of a
+                        html file)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+
+
+```
 ## Installation
 
 ### pipx
 
 This is the recommended installation method.
 
 ```
```

### Comparing `langchain_utils-0.3.7/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.3.8/langchain_utils/get_pdf_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.7/langchain_utils/get_text_prompt.py` & `langchain_utils-0.3.8/langchain_utils/get_text_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """Get command-line arguments"""
 
     parser = get_get_prompt_base_arg_parser(
         description='Get a prompt from text files'
     )
 
     parser.add_argument(
-        'path', help='Paths to the text files, or stdin if not provided', metavar='Path', type=str, default=None, nargs='*'
+        'path', help='Paths to the text files, or stdin if not provided', metavar='PATH', type=str, default=None, nargs='*'
     )
 
     parser.add_argument(
         '-w',
         '--what',
         help='Initial knowledge you want to insert before the PDF content in the prompt',
         type=str,
@@ -52,15 +52,15 @@
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
     print(f'Loading text file(s) from {args.path} ...', file=sys.stderr)
-    docs = load_text(args.path)
+    docs = [load_text(p)[0] for p in args.path]
     texts = [doc.page_content for doc in docs]
     all_text = '\n'.join(texts)
     word_count = get_word_count((all_text))
     print(
         f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
         file=sys.stderr,
     )
```

### Comparing `langchain_utils-0.3.7/langchain_utils/get_url_prompt.py` & `langchain_utils-0.3.8/langchain_utils/get_url_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.7/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.3.8/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.7/langchain_utils/loaders.py` & `langchain_utils-0.3.8/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.7/langchain_utils/utils.py` & `langchain_utils-0.3.8/langchain_utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,21 @@
     metadata = document.metadata
     if 'page_number' in metadata:
         return f', Page {metadata["page_number"]}/{metadata["total_pages"]}'
     else:
         return ''
 
 
+def html_source_info(document: 'Document') -> str:
+    metadata = document.metadata
+    if 'source' in metadata:
+        return f', Title: {metadata["title"]}, Source: {metadata["source"]}'
+    else:
+        return ''
+
 def general_document_source_info(document: 'Document') -> str:
     metadata = document.metadata
     if 'source' in metadata:
         return f', Source: {metadata["source"]}'
     else:
         return ''
```

### Comparing `langchain_utils-0.3.7/langchain_utils/utils_argparse.py` & `langchain_utils-0.3.8/langchain_utils/utils_argparse.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.3.7/pyproject.toml` & `langchain_utils-0.3.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.3.7"
+version = "0.3.8"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
@@ -14,14 +14,16 @@
 [tool.poetry.scripts]
 get-youtube-transcript-prompt = "langchain_utils.get_youtube_transcript_prompt:main"
 ytprompt = "langchain_utils.get_youtube_transcript_prompt:main"
 get-url-prompt = "langchain_utils.get_url_prompt:main"
 urlprompt = "langchain_utils.get_url_prompt:main"
 get-text-prompt = "langchain_utils.get_text_prompt:main"
 textprompt = "langchain_utils.get_text_prompt:main"
+get-html-prompt = "langchain_utils.get_html_prompt:main"
+htmlprompt = "langchain_utils.get_html_prompt:main"
 get-pdf-prompt = "langchain_utils.get_pdf_prompt:main"
 pdfprompt = "langchain_utils.get_pdf_prompt:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/langchain-utils/issues"
 
 [tool.poetry.dependencies]
@@ -31,14 +33,15 @@
 pytube = "^12.1.3"
 pyperclip = "^1.8.2"
 tiktoken = "^0.3.3"
 pymupdf = "^1.21.1"
 # must use this version of unstructured, or it won't be able to parse certain htmls
 unstructured = "0.5.2"
 selenium = "^4.8.3"
+bs4 = "^0.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 better-exceptions = "^0.3.3"
 ipython = "^8.12.0"
 ipykernel = "^6.22.0"
```

### Comparing `langchain_utils-0.3.7/PKG-INFO` & `langchain_utils-0.3.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.3.7
+Version: 0.3.8
 Summary: 
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: langchain (>=0.0.135,<0.0.136)
 Requires-Dist: pymupdf (>=1.21.1,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pytube (>=12.1.3,<13.0.0)
 Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: unstructured (==0.5.2)
@@ -30,14 +31,16 @@
 
 
 - [langchain-utils](#langchain-utils)
   - [Prompt generation using LangChain document loaders](#prompt-generation-using-langchain-document-loaders)
     - [`urlprompt`](#urlprompt)
     - [`pdfprompt`](#pdfprompt)
     - [`ytprompt`](#ytprompt)
+    - [`textprompt`](#textprompt)
+    - [`htmlprompt`](#htmlprompt)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [Develop](#develop)
 
 
 ## Prompt generation using LangChain document loaders
@@ -138,15 +141,90 @@
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split (default: 2000)
   -n, --dry-run         Dry run (default: False)
 
 ```
 
+### `textprompt`
 
+```
+$ textprompt --help
+
+usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                  [-P PARTS [PARTS ...]] [-n] [-w WHAT] [-M]
+                  [PATH ...]
+
+Get a prompt from text files
+
+positional arguments:
+  PATH                  Paths to the text files, or stdin if not provided
+                        (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -c, --copy            Copy the prompt to clipboard (default: False)
+  -e, --edit            Edit the prompt and copy manually (default: False)
+  -m model, --model model
+                        Model to use (default: gpt-3.5-turbo)
+  -S, --split           Split the prompt into multiple parts (default: False)
+  -s chunk_size, --chunk-size chunk_size
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split (default: 2000)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -n, --dry-run         Dry run (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the content of a
+                        document)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+```
+
+
+### `htmlprompt`
+
+```
+$ htmlprompt --help
+
+usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                  [-P PARTS [PARTS ...]] [-n] [-w WHAT] [-M]
+                  [PATH ...]
+
+Get a prompt from html files
+
+positional arguments:
+  PATH                  Paths to the html files, or stdin if not provided
+                        (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -c, --copy            Copy the prompt to clipboard (default: False)
+  -e, --edit            Edit the prompt and copy manually (default: False)
+  -m model, --model model
+                        Model to use (default: gpt-3.5-turbo)
+  -S, --split           Split the prompt into multiple parts (default: False)
+  -s chunk_size, --chunk-size chunk_size
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split (default: 2000)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -n, --dry-run         Dry run (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the text content of a
+                        html file)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+
+
+```
 ## Installation
 
 ### pipx
 
 This is the recommended installation method.
 
 ```
```

