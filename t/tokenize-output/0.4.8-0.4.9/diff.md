# Comparing `tmp/tokenize-output-0.4.8.tar.gz` & `tmp/tokenize-output-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenize-output-0.4.8.tar", last modified: Thu Mar 23 23:12:01 2023, max compression
+gzip compressed data, was "tokenize-output-0.4.9.tar", last modified: Fri Mar 24 08:38:06 2023, max compression
```

## Comparing `tokenize-output-0.4.8.tar` & `tokenize-output-0.4.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:12:01.333754 tokenize-output-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-23 23:12:01.333754 tokenize-output-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 23:12:01.333754 tokenize-output-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/tokenize-output
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:12:01.333754 tokenize-output-0.4.8/tokenize_output/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/tokenize_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-03-23 23:11:48.000000 tokenize-output-0.4.8/tokenize_output/tokenize_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:12:01.333754 tokenize-output-0.4.8/tokenize_output.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-23 23:12:01.000000 tokenize-output-0.4.8/tokenize_output.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 23:12:01.000000 tokenize-output-0.4.8/tokenize_output.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 23:12:01.000000 tokenize-output-0.4.8/tokenize_output.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-23 23:12:01.000000 tokenize-output-0.4.8/tokenize_output.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 23:12:01.000000 tokenize-output-0.4.8/tokenize_output.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:38:06.300525 tokenize-output-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-03-24 08:38:06.300525 tokenize-output-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 08:38:06.300525 tokenize-output-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/tokenize-output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:38:06.300525 tokenize-output-0.4.9/tokenize_output/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/tokenize_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-03-24 08:37:54.000000 tokenize-output-0.4.9/tokenize_output/tokenize_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 08:38:06.300525 tokenize-output-0.4.9/tokenize_output.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-03-24 08:38:06.000000 tokenize-output-0.4.9/tokenize_output.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-24 08:38:06.000000 tokenize-output-0.4.9/tokenize_output.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 08:38:06.000000 tokenize-output-0.4.9/tokenize_output.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 08:38:06.000000 tokenize-output-0.4.9/tokenize_output.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 08:38:06.000000 tokenize-output-0.4.9/tokenize_output.egg-info/top_level.txt
```

### Comparing `tokenize-output-0.4.8/LICENSE` & `tokenize-output-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenize-output-0.4.8/PKG-INFO` & `tokenize-output-0.4.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: tokenize-output
-Version: 0.4.8
-Summary: Get identifiers, names, paths, URLs and words from the command output.
-Home-page: https://github.com/anki-code/tokenize-output
-Author: anki-code
-Author-email: author@example.com
-License: BSD
-Project-URL: Documentation, https://github.com/anki-code/tokenize-output/blob/master/README.md
-Project-URL: Code, https://github.com/anki-code/tokenize-output
-Project-URL: Issue tracker, https://github.com/anki-code/tokenize-output/issues
-Platform: any
-Classifier: Programming Language :: Python
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <p align="center">
 Get identifiers, names, paths, URLs and words from the command output.<br> 
 The <a href="https://github.com/anki-code/xontrib-output-search">xontrib-output-search</a> for <a href="https://xon.sh/">xonsh shell</a> is using this library.
 </p>
 
 <p align="center">  
 If you like the idea click ⭐ on the repo and stay tuned by watching releases.
@@ -28,37 +10,44 @@
 ## Install
 ```shell script
 pip install -U tokenize-output
 ```
 
 ## Usage
 
+You can use `tokenize-output` command as well as export the tokenizers in Python:
+```python
+from tokenize_output.tokenize_output import *
+tokenizer_split("Hello world!")
+# {'final': set(), 'new': {'Hello', 'world!'}}
+```
+
 #### Words tokenizing
 ```shell script
-$ echo "Try https://github.com/xxh/xxh" | tokenize-output -p
-Try
-https://github.com/xxh/xxh
+echo "Try https://github.com/xxh/xxh" | tokenize-output -p
+# Try
+# https://github.com/xxh/xxh
 ```
 
 #### JSON, Python dict and JavaScript object tokenizing
 ```shell script
-$ echo '{"Try": "xonsh shell"}' | tokenize-output -p
-Try
-shell
-xonsh
-xonsh shell
+echo '{"Try": "xonsh shell"}' | tokenize-output -p
+# Try
+# shell
+# xonsh
+# xonsh shell
 ```    
 
 #### env tokenizing
 ```shell script
-$  echo 'PATH=/one/two:/three/four' | tokenize-output -p
-/one/two
-/one/two:/three/four
-/three/four
-PATH
+echo 'PATH=/one/two:/three/four' | tokenize-output -p
+# /one/two
+# /one/two:/three/four
+# /three/four
+# PATH
 ```    
 
 ## Development
 
 ### Tokenizers
 Tokenizer is a functions which extract tokens from the text.
 
@@ -72,14 +61,24 @@
 You can create your tokenizer and add it to `tokenizers_all` in `tokenize_output.py`.
 
 Tokenizing is a recursive process where every tokenizer returns `final` and `new` tokens. 
 The `final` tokens directly go to the result list of tokens. The `new` tokens go to all 
 tokenizers again to find new tokens. As result if there is a mix of json and env data 
 in the output it will be found and tokenized in appropriate way.  
 
+### How to add tokenizer
+
+You can start from `env` tokenizer:
+
+1. [Prepare regexp](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L10)
+2. [Prepare tokenizer function](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L57-L70)
+3. [Add the function to the list](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L139-L144) and [to the preset](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L147).
+4. [Add test](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tests/test_tokenize.py#L34-L35).
+5. Now you can test and debug (see below).
+
 ### Test and debug
 Run tests:
 ```shell script
 cd ~
 git clone https://github.com/anki-code/tokenize-output
 cd tokenize-output
 python -m pytest tests/
```

#### html2text {}

```diff
@@ -1,36 +1,43 @@
-Metadata-Version: 2.1 Name: tokenize-output Version: 0.4.8 Summary: Get
-identifiers, names, paths, URLs and words from the command output. Home-page:
-https://github.com/anki-code/tokenize-output Author: anki-code Author-email:
-author@example.com License: BSD Project-URL: Documentation, https://github.com/
-anki-code/tokenize-output/blob/master/README.md Project-URL: Code, https://
-github.com/anki-code/tokenize-output Project-URL: Issue tracker, https://
-github.com/anki-code/tokenize-output/issues Platform: any Classifier:
-Programming Language :: Python Requires-Python: >=3.6 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE
     Get identifiers, names, paths, URLs and words from the command output.
        The xontrib-output-search for xonsh_shell is using this library.
 If you like the idea click â­ on the repo and stay tuned by watching releases.
-## Install ```shell script pip install -U tokenize-output ``` ## Usage ####
-Words tokenizing ```shell script $ echo "Try https://github.com/xxh/xxh" |
-tokenize-output -p Try https://github.com/xxh/xxh ``` #### JSON, Python dict
-and JavaScript object tokenizing ```shell script $ echo '{"Try": "xonsh
-shell"}' | tokenize-output -p Try shell xonsh xonsh shell ``` #### env
-tokenizing ```shell script $ echo 'PATH=/one/two:/three/four' | tokenize-output
--p /one/two /one/two:/three/four /three/four PATH ``` ## Development ###
+## Install ```shell script pip install -U tokenize-output ``` ## Usage You can
+use `tokenize-output` command as well as export the tokenizers in Python:
+```python from tokenize_output.tokenize_output import * tokenizer_split("Hello
+world!") # {'final': set(), 'new': {'Hello', 'world!'}} ``` #### Words
+tokenizing ```shell script echo "Try https://github.com/xxh/xxh" | tokenize-
+output -p # Try # https://github.com/xxh/xxh ``` #### JSON, Python dict and
+JavaScript object tokenizing ```shell script echo '{"Try": "xonsh shell"}' |
+tokenize-output -p # Try # shell # xonsh # xonsh shell ``` #### env tokenizing
+```shell script echo 'PATH=/one/two:/three/four' | tokenize-output -p # /one/
+two # /one/two:/three/four # /three/four # PATH ``` ## Development ###
 Tokenizers Tokenizer is a functions which extract tokens from the text. |
 Priority | Tokenizer | Text | Tokens | | ---------| ---------- | ----- | -----
 - | | 1 | **dict** | `{"key": "val as str"}` | `key`, `val as str` | | 2 |
 **env** | `PATH=/bin:/etc` | `PATH`, `/bin:/etc`, `/bin`, `/etc` | | 3 |
 **split** | `Split me \n now!` | `Split`, `me`, `now!` | | 4 | **strip** | `
 {Hello}` | `Hello` | You can create your tokenizer and add it to
 `tokenizers_all` in `tokenize_output.py`. Tokenizing is a recursive process
 where every tokenizer returns `final` and `new` tokens. The `final` tokens
 directly go to the result list of tokens. The `new` tokens go to all tokenizers
 again to find new tokens. As result if there is a mix of json and env data in
-the output it will be found and tokenized in appropriate way. ### Test and
-debug Run tests: ```shell script cd ~ git clone https://github.com/anki-code/
-tokenize-output cd tokenize-output python -m pytest tests/ ``` To debug the
-tokenizer: ```shell script echo "Hello world" | ./tokenize-output -p ``` ##
+the output it will be found and tokenized in appropriate way. ### How to add
+tokenizer You can start from `env` tokenizer: 1. [Prepare regexp](https://
+github.com/tokenizer/tokenize-output/blob/
+25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/
+tokenize_output.py#L10) 2. [Prepare tokenizer function](https://github.com/
+tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/
+tokenize_output/tokenize_output.py#L57-L70) 3. [Add the function to the list]
+(https://github.com/tokenizer/tokenize-output/blob/
+25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/
+tokenize_output.py#L139-L144) and [to the preset](https://github.com/tokenizer/
+tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/
+tokenize_output.py#L147). 4. [Add test](https://github.com/tokenizer/tokenize-
+output/blob/25b930cfadf8291e72a72144962e411e47d28139/tests/
+test_tokenize.py#L34-L35). 5. Now you can test and debug (see below). ### Test
+and debug Run tests: ```shell script cd ~ git clone https://github.com/anki-
+code/tokenize-output cd tokenize-output python -m pytest tests/ ``` To debug
+the tokenizer: ```shell script echo "Hello world" | ./tokenize-output -p ``` ##
 Related projects * [xontrib-output-search][XONTRIB_OUTPUT_SEARCH] for [xonsh
 shell][XONSH] [XONTRIB_OUTPUT_SEARCH]: https://github.com/anki-code/xontrib-
 output-search [XONSH]: https://xon.sh/
```

### Comparing `tokenize-output-0.4.8/setup.py` & `tokenize-output-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `tokenize-output-0.4.8/tokenize-output` & `tokenize-output-0.4.9/tokenize-output`

 * *Files identical despite different names*

### Comparing `tokenize-output-0.4.8/tokenize_output/tokenize_output.py` & `tokenize-output-0.4.9/tokenize_output/tokenize_output.py`

 * *Files identical despite different names*

### Comparing `tokenize-output-0.4.8/tokenize_output.egg-info/PKG-INFO` & `tokenize-output-0.4.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenize-output
-Version: 0.4.8
+Version: 0.4.9
 Summary: Get identifiers, names, paths, URLs and words from the command output.
 Home-page: https://github.com/anki-code/tokenize-output
 Author: anki-code
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/tokenize-output/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/tokenize-output
@@ -28,37 +28,44 @@
 ## Install
 ```shell script
 pip install -U tokenize-output
 ```
 
 ## Usage
 
+You can use `tokenize-output` command as well as export the tokenizers in Python:
+```python
+from tokenize_output.tokenize_output import *
+tokenizer_split("Hello world!")
+# {'final': set(), 'new': {'Hello', 'world!'}}
+```
+
 #### Words tokenizing
 ```shell script
-$ echo "Try https://github.com/xxh/xxh" | tokenize-output -p
-Try
-https://github.com/xxh/xxh
+echo "Try https://github.com/xxh/xxh" | tokenize-output -p
+# Try
+# https://github.com/xxh/xxh
 ```
 
 #### JSON, Python dict and JavaScript object tokenizing
 ```shell script
-$ echo '{"Try": "xonsh shell"}' | tokenize-output -p
-Try
-shell
-xonsh
-xonsh shell
+echo '{"Try": "xonsh shell"}' | tokenize-output -p
+# Try
+# shell
+# xonsh
+# xonsh shell
 ```    
 
 #### env tokenizing
 ```shell script
-$  echo 'PATH=/one/two:/three/four' | tokenize-output -p
-/one/two
-/one/two:/three/four
-/three/four
-PATH
+echo 'PATH=/one/two:/three/four' | tokenize-output -p
+# /one/two
+# /one/two:/three/four
+# /three/four
+# PATH
 ```    
 
 ## Development
 
 ### Tokenizers
 Tokenizer is a functions which extract tokens from the text.
 
@@ -72,14 +79,24 @@
 You can create your tokenizer and add it to `tokenizers_all` in `tokenize_output.py`.
 
 Tokenizing is a recursive process where every tokenizer returns `final` and `new` tokens. 
 The `final` tokens directly go to the result list of tokens. The `new` tokens go to all 
 tokenizers again to find new tokens. As result if there is a mix of json and env data 
 in the output it will be found and tokenized in appropriate way.  
 
+### How to add tokenizer
+
+You can start from `env` tokenizer:
+
+1. [Prepare regexp](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L10)
+2. [Prepare tokenizer function](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L57-L70)
+3. [Add the function to the list](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L139-L144) and [to the preset](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/tokenize_output.py#L147).
+4. [Add test](https://github.com/tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tests/test_tokenize.py#L34-L35).
+5. Now you can test and debug (see below).
+
 ### Test and debug
 Run tests:
 ```shell script
 cd ~
 git clone https://github.com/anki-code/tokenize-output
 cd tokenize-output
 python -m pytest tests/
```

#### html2text {}

```diff
@@ -1,36 +1,52 @@
-Metadata-Version: 2.1 Name: tokenize-output Version: 0.4.8 Summary: Get
+Metadata-Version: 2.1 Name: tokenize-output Version: 0.4.9 Summary: Get
 identifiers, names, paths, URLs and words from the command output. Home-page:
 https://github.com/anki-code/tokenize-output Author: anki-code Author-email:
 author@example.com License: BSD Project-URL: Documentation, https://github.com/
 anki-code/tokenize-output/blob/master/README.md Project-URL: Code, https://
 github.com/anki-code/tokenize-output Project-URL: Issue tracker, https://
 github.com/anki-code/tokenize-output/issues Platform: any Classifier:
 Programming Language :: Python Requires-Python: >=3.6 Description-Content-Type:
 text/markdown Provides-Extra: dev License-File: LICENSE
     Get identifiers, names, paths, URLs and words from the command output.
        The xontrib-output-search for xonsh_shell is using this library.
 If you like the idea click â­ on the repo and stay tuned by watching releases.
-## Install ```shell script pip install -U tokenize-output ``` ## Usage ####
-Words tokenizing ```shell script $ echo "Try https://github.com/xxh/xxh" |
-tokenize-output -p Try https://github.com/xxh/xxh ``` #### JSON, Python dict
-and JavaScript object tokenizing ```shell script $ echo '{"Try": "xonsh
-shell"}' | tokenize-output -p Try shell xonsh xonsh shell ``` #### env
-tokenizing ```shell script $ echo 'PATH=/one/two:/three/four' | tokenize-output
--p /one/two /one/two:/three/four /three/four PATH ``` ## Development ###
+## Install ```shell script pip install -U tokenize-output ``` ## Usage You can
+use `tokenize-output` command as well as export the tokenizers in Python:
+```python from tokenize_output.tokenize_output import * tokenizer_split("Hello
+world!") # {'final': set(), 'new': {'Hello', 'world!'}} ``` #### Words
+tokenizing ```shell script echo "Try https://github.com/xxh/xxh" | tokenize-
+output -p # Try # https://github.com/xxh/xxh ``` #### JSON, Python dict and
+JavaScript object tokenizing ```shell script echo '{"Try": "xonsh shell"}' |
+tokenize-output -p # Try # shell # xonsh # xonsh shell ``` #### env tokenizing
+```shell script echo 'PATH=/one/two:/three/four' | tokenize-output -p # /one/
+two # /one/two:/three/four # /three/four # PATH ``` ## Development ###
 Tokenizers Tokenizer is a functions which extract tokens from the text. |
 Priority | Tokenizer | Text | Tokens | | ---------| ---------- | ----- | -----
 - | | 1 | **dict** | `{"key": "val as str"}` | `key`, `val as str` | | 2 |
 **env** | `PATH=/bin:/etc` | `PATH`, `/bin:/etc`, `/bin`, `/etc` | | 3 |
 **split** | `Split me \n now!` | `Split`, `me`, `now!` | | 4 | **strip** | `
 {Hello}` | `Hello` | You can create your tokenizer and add it to
 `tokenizers_all` in `tokenize_output.py`. Tokenizing is a recursive process
 where every tokenizer returns `final` and `new` tokens. The `final` tokens
 directly go to the result list of tokens. The `new` tokens go to all tokenizers
 again to find new tokens. As result if there is a mix of json and env data in
-the output it will be found and tokenized in appropriate way. ### Test and
-debug Run tests: ```shell script cd ~ git clone https://github.com/anki-code/
-tokenize-output cd tokenize-output python -m pytest tests/ ``` To debug the
-tokenizer: ```shell script echo "Hello world" | ./tokenize-output -p ``` ##
+the output it will be found and tokenized in appropriate way. ### How to add
+tokenizer You can start from `env` tokenizer: 1. [Prepare regexp](https://
+github.com/tokenizer/tokenize-output/blob/
+25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/
+tokenize_output.py#L10) 2. [Prepare tokenizer function](https://github.com/
+tokenizer/tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/
+tokenize_output/tokenize_output.py#L57-L70) 3. [Add the function to the list]
+(https://github.com/tokenizer/tokenize-output/blob/
+25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/
+tokenize_output.py#L139-L144) and [to the preset](https://github.com/tokenizer/
+tokenize-output/blob/25b930cfadf8291e72a72144962e411e47d28139/tokenize_output/
+tokenize_output.py#L147). 4. [Add test](https://github.com/tokenizer/tokenize-
+output/blob/25b930cfadf8291e72a72144962e411e47d28139/tests/
+test_tokenize.py#L34-L35). 5. Now you can test and debug (see below). ### Test
+and debug Run tests: ```shell script cd ~ git clone https://github.com/anki-
+code/tokenize-output cd tokenize-output python -m pytest tests/ ``` To debug
+the tokenizer: ```shell script echo "Hello world" | ./tokenize-output -p ``` ##
 Related projects * [xontrib-output-search][XONTRIB_OUTPUT_SEARCH] for [xonsh
 shell][XONSH] [XONTRIB_OUTPUT_SEARCH]: https://github.com/anki-code/xontrib-
 output-search [XONSH]: https://xon.sh/
```

