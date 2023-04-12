# Comparing `tmp/talkwave-0.0.4.tar.gz` & `tmp/talkwave-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkwave-0.0.4.tar", last modified: Tue Apr 11 20:45:27 2023, max compression
+gzip compressed data, was "talkwave-0.0.5.tar", last modified: Wed Apr 12 13:45:39 2023, max compression
```

## Comparing `talkwave-0.0.4.tar` & `talkwave-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:45:27.681444 talkwave-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-11 20:45:19.000000 talkwave-0.0.4/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-11 20:45:19.000000 talkwave-0.0.4/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 20:45:19.000000 talkwave-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 20:45:27.681444 talkwave-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-11 20:45:19.000000 talkwave-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 20:45:19.000000 talkwave-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-11 20:45:27.685444 talkwave-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-11 20:45:19.000000 talkwave-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:45:27.681444 talkwave-0.0.4/talkwave/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-11 20:45:19.000000 talkwave-0.0.4/talkwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-11 20:45:19.000000 talkwave-0.0.4/talkwave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-11 20:45:19.000000 talkwave-0.0.4/talkwave/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-11 20:45:19.000000 talkwave-0.0.4/talkwave/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:45:27.681444 talkwave-0.0.4/talkwave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-11 20:45:27.000000 talkwave-0.0.4/talkwave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 20:45:27.000000 talkwave-0.0.4/talkwave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:45:27.000000 talkwave-0.0.4/talkwave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-11 20:45:27.000000 talkwave-0.0.4/talkwave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 20:45:27.000000 talkwave-0.0.4/talkwave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:45:27.681444 talkwave-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-11 20:45:19.000000 talkwave-0.0.4/tests/test_curl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-11 20:45:19.000000 talkwave-0.0.4/tests/test_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-11 20:45:19.000000 talkwave-0.0.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10870 2023-04-12 13:45:29.000000 talkwave-0.0.5/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-12 13:45:29.000000 talkwave-0.0.5/LICENSE-MIT
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-12 13:45:29.000000 talkwave-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-12 13:45:39.099635 talkwave-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-12 13:45:29.000000 talkwave-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-12 13:45:29.000000 talkwave-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-12 13:45:39.099635 talkwave-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-12 13:45:29.000000 talkwave-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/talkwave/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-12 13:45:29.000000 talkwave-0.0.5/talkwave/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/talkwave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 13:45:39.000000 talkwave-0.0.5/talkwave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:45:39.099635 talkwave-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-12 13:45:29.000000 talkwave-0.0.5/tests/test_main.py
```

### Comparing `talkwave-0.0.4/LICENSE-APACHE` & `talkwave-0.0.5/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.4/LICENSE-MIT` & `talkwave-0.0.5/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.4/PKG-INFO` & `talkwave-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkwave
-Version: 0.0.4
+Version: 0.0.5
 Summary: TalkWave is an AI chatbot for developers written in Python.
 Home-page: https://github.com/sebastienrousseau/talkwave
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache License 2.0
 Keywords: talkwave,chatbot,AI,machine learningnatural language processing OpenAI GPT-3 GPT3 GPT python
 Classifier: Development Status :: 4 - Beta
@@ -63,25 +63,27 @@
 ```bash
 pip install openai tabulate python-dotenv
 ```
 
 1. Clone the TalkWave repository:
 
 ```bash
-git clone https://github.com/yourusername/talkwave.git
+git clone https://github.com/sebastienrousseau/talkwave.git
 ```
 
 1. Add your OpenAI API key to a `.env` file in the project directory:
 
 ```bash
 OPENAI_API_KEY="your_api_key_here"
 ```
 
 ## Usage 🚀
 
+### Command Line Interface
+
 To use TalkWave, navigate to the project directory in your terminal and
 run the following command:
 
 ```bash
 python talkwave -p "Your prompt here"
 ```
 
@@ -95,14 +97,27 @@
 
 For more information on the available options, run:
 
 ```bash
 python talkwave --help
 ```
 
+### Web Frontend
+
+To use the web frontend, navigate to the project directory in your
+terminal and run the following command:
+
+```bash
+python talkwave/frontend.py
+```
+
+Then, open your browser and navigate to `http://127.0.0.1:5000`. This
+will open the TalkWave web frontend, which you can use to generate
+responses.
+
 ## File Structure 📁
 
 ```bash
 .
 ├── talkwave
 │   ├── data
 │   ├── templates
```

### Comparing `talkwave-0.0.4/README.md` & `talkwave-0.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,25 +38,27 @@
 ```bash
 pip install openai tabulate python-dotenv
 ```
 
 1. Clone the TalkWave repository:
 
 ```bash
-git clone https://github.com/yourusername/talkwave.git
+git clone https://github.com/sebastienrousseau/talkwave.git
 ```
 
 1. Add your OpenAI API key to a `.env` file in the project directory:
 
 ```bash
 OPENAI_API_KEY="your_api_key_here"
 ```
 
 ## Usage 🚀
 
+### Command Line Interface
+
 To use TalkWave, navigate to the project directory in your terminal and
 run the following command:
 
 ```bash
 python talkwave -p "Your prompt here"
 ```
 
@@ -70,14 +72,27 @@
 
 For more information on the available options, run:
 
 ```bash
 python talkwave --help
 ```
 
+### Web Frontend
+
+To use the web frontend, navigate to the project directory in your
+terminal and run the following command:
+
+```bash
+python talkwave/frontend.py
+```
+
+Then, open your browser and navigate to `http://127.0.0.1:5000`. This
+will open the TalkWave web frontend, which you can use to generate
+responses.
+
 ## File Structure 📁
 
 ```bash
 .
 ├── talkwave
 │   ├── data
 │   ├── templates
```

### Comparing `talkwave-0.0.4/pyproject.toml` & `talkwave-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "talkwave"
-version = "0.0.4"
+version = "0.0.5"
 description = "TalkWave is an AI chatbot for developers written in Python."
 authors = ["Sebastien Rousseau <sebastian.rousseau at gmail.com>"]
 license = "Apache Software License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `talkwave-0.0.4/setup.cfg` & `talkwave-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = talkwave
-version = 0.0.4
+version = 0.0.5
 author = Sebastian Rousseau
 author_email = sebastian.rousseau@gmail.com
 description = TalkWave is an AI chatbot for developers written in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sebastienrousseau/talkwave
 license = Apache Software License
```

### Comparing `talkwave-0.0.4/setup.py` & `talkwave-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 TEST_DEPENDENCIES = [
     "coverage>=7.2.3",
     "pytest-cov>=4.0.0",
     "pytest>=7.3.0",
 ]
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 URL = 'https://github.com/sebastienrousseau/talkwave'
 
 setup(
     name='talkwave',
     version=VERSION,
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
@@ -64,12 +64,14 @@
         'Operating System :: OS Independent',
     ],
     keywords=(
         'talkwave, chatbot, AI, machine learning'
         'natural language processing '
         'OpenAI GPT-3 GPT3 GPT python'
     ),
-    packages=['talkwave'],
+    packages=[
+
+    ],
     install_requires=DEPENDENCIES,
     tests_require=TEST_DEPENDENCIES,
     python_requires='>=3.9',
 )
```

### Comparing `talkwave-0.0.4/talkwave/__init__.py` & `talkwave-0.0.5/talkwave/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,26 +13,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 
 # TalkWave
 
 
-TalkWave is a Python package that provides an easy-to-use command-line
-interface for interacting with OpenAI's GPT-powered language models.
+TalkWave is an AI chatbot for developers written in Python. It features
+a simple HTML frontend and is designed to be accessible across various
+browsers and devices. TalkWave supports asynchronous operations and can
+handle multiple requests simultaneously.
 
 ## Features
 
-- Supports multiple GPT models for generating responses.
-- Accepts a range of parameters to customize the response, such as max
-tokens, temperature, and stopping conditions.
-- Stores responses in log files, JSON, and Markdown formats for easy
+- [x] Accepts a range of parameters to customize the response, such as
+max tokens, temperature, and stopping conditions.
+- [x] Accessible design for cross-browser and device compatibility
+(Chrome, Firefox, Safari, Edge, and mobile).
+- [x] Accurately limits billing with limits and ID binding to prevent
+exceeding API limits and incurring charges.
+- [x] Implements rate limiting functionality to prevent exceeding API
+limits and incurring charges.
+- [x] Plain Python implementation with a limited number of dependencies
+for easy installation and use.
+- [x] Stores responses in log files, JSON, and Markdown formats for easy
 analysis and sharing.
-- Provides rate limiting functionality to prevent exceeding API limits
-and incurring charges.
+- [x] Supports multiple GPT models for generating responses, including
+`gpt-3.5-turbo`,`text-davinci-002`,`text-curie-001`,`text-babbage-001`,
+`text-ada-001`.
 
 ## Requirements
 
 - Python 3.6 or higher
 - The `openai`, `tabulate`, and `python-dotenv` packages
 - An OpenAI API key (get one [here](https://openai.com/))
 
@@ -43,18 +53,18 @@
 ```bash
 pip install openai tabulate python-dotenv
 ```
 
 1. Clone the TalkWave repository:
 
 ```bash
-git clone https://github.com/yourusername/talkwave.git
+git clone https://github.com/sebastienrousseau/talkwave.git
 ```
 
-3. Add your OpenAI API key to a `.env` file in the project directory:
+1. Add your OpenAI API key to a `.env` file in the project directory:
 
 ```bash
 OPENAI_API_KEY="your_api_key_here"
 ```
 
 ## Usage
 
@@ -72,15 +82,16 @@
 python talkwave\n
     -m 1\n
     -p "Tell me a joke"\n
     -t 50\n
     -T 0.5\n
     -u "test@test.com"\n
     -r 5\n
-    -s "."
+    -s\n
+    -o "json"\n
 ```
 
 For more information on the available options, run:
 
 ```bash
 python talkwave --help
 ```
@@ -91,12 +102,7 @@
 The project is licensed under the terms of both the MIT license and the
 Apache License (Version 2.0).
 
 - [Apache License, Version 2.0](https://opensource.org/license/apache-2-0/)
 - [MIT license](https://opensource.org/licenses/MIT)
 
 """
-
-"""The Python talkwave module."""
-__all__ = ["__version__"]
-
-__version__ = "0.0.4"
```

### Comparing `talkwave-0.0.4/talkwave/__main__.py` & `talkwave-0.0.5/talkwave/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,40 +11,44 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Enables use of Python TalkWave as a "main" function (i.e.
-"python3 -m talkwave").
+"python3 talkwave").
 
 This allows using TalkWave with third-party libraries without modifying
 their code.
 """
-# '
 
 from core import main
+from parse import parse_args
 from tabulate import tabulate
-from utils.parse import parse_args
 import os
 import sys
-
+from __version__ import (
+    __description__,
+    __title__,
+    __version__,
+)
 
 # set the directory where the data is stored, value is a string from an
 # environment variable "DIR_PATH" (required).
 dir_path = os.path.join(os.path.dirname(os.path.realpath(
     __file__)), os.environ.get('DIR_PATH', 'data'))
 
 if __name__ == "__main__":
     # Set the title and description of the program
-    title = "TalkWave 🐍 (v0.0.4)"
-    description = "An AI chatbot for developers"
+    title = __title__ + " (v" + __version__ + ")"
+    description = __description__
 
     # Print the title and description of the program
-    title_table = tabulate([[title], [description]], tablefmt="rounded_grid")
+    title_table = tabulate([[title], [description]],
+                           tablefmt="rounded_grid")
     print()
     print(title_table)
     print()
 
     # Parse the command-line arguments
     args = parse_args()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `talkwave-0.0.4/talkwave/core.py` & `talkwave-0.0.5/talkwave/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,37 +13,55 @@
 # implied.
 #
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # '
 from datetime import datetime
-from utils.curl import send_request
+
+try:
+    from talkwave.__version__ import (
+        __logo__,
+        __title__,
+        __version__,
+    )
+except ModuleNotFoundError:
+    from __version__ import (
+        __logo__,
+        __title__,
+        __version__,
+    )
+
+
 import dotenv
 import json
 import os
-import sys
 import sqlite3
+import sys
 
-# set the timeout for the API call to a string value from an environment
-timeout = os.environ.get('TIMEOUT', '90')
+try:
+    from talkwave.curl import send_request
+except ModuleNotFoundError:
+    from curl import send_request
 
 # set the directory where the data is stored, value is a string from an
 # environment variable "DATA_DIR" (required).
 data_dir = os.path.join(os.path.dirname(os.path.realpath(
     __file__)), os.environ.get('DATA_DIR', 'data'))
 
 # set the timestamp for the API call in ISO
 timestamp = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
 
 # Function Name: write_response_to_log_file
 '''
 Write the response to a log file.
 '''
 
+data_dir = "data"  # Define the data directory or pass it as an argument
+
 
 def write_response_to_log_file(response, prompt, timestamp):
     """
     Write the response and prompt to a log file.
     """
     if data_dir is None:
         print("Error: Directory path is not provided.")
@@ -59,15 +77,22 @@
 
 # List of valid file formats for text files
 text = ["csv", "xls", "html", "txt", "text",
         "log", "json", "xml", "yaml", "yml"]
 database = ["db", "sqlite", "sqlite3", "db3", "s3db", "sl3"]
 markdown = ["md", "markdown"]
 html = ["html", "htm"]
-VERSION = '0.0.4'
+# pdf = ["pdf"]
+# image = ["png", "jpg", "jpeg", "gif", "bmp", "tiff", "tif"]
+
+
+# Function Name: write_response_to_file
+'''
+Write the response to a file.
+'''
 
 
 def write_response_to_file(
     response,
     prompt,
     file_format,
     timestamp,
@@ -100,46 +125,45 @@
 <meta name=\"viewport\" content=\"width=device-width, initial-scale=1\">\n
 """)
                 f.write("""
 <meta name=\"theme-color\" content=\"#e82440\"/>\n
 """)
                 f.write("""
 <link rel=\"stylesheet\"
-      href=\"https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css\"
-      integrity=\"sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65\"
-      crossorigin=\"anonymous\" />\n""")
+href=\"https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css\"
+integrity=\"sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65\"
+crossorigin=\"anonymous\" />\n""")
                 f.write(
                     """
                         <style>
                             .wrap-code {
                                 white-space: pre-wrap;
                                 word-wrap: break-word;
                             }
                         </style>\n
                     """)
-                f.write("<title>TalkWave 🐍 Log Analysis</title>\n")
+                f.write("<title>"+__title__+"</title>\n")
                 f.write("</head>\n")
                 f.write("<body>\n")
                 f.write(
                     """
 <header class=\"bd-header bg-dark py-3 d-flex align-items-stretch
 border-bottom border-dark\">""")
                 f.write("""
 <div class=\"container-fluid d-flex align-items-center\">
 """)
                 f.write(
                     """
 <h1 class=\"d-flex align-items-center fs-4 text-white mb-0\">
 """)
-                f.write("""
-<img src=\"https://raw.githubusercontent.com/sebastienrousseau/vault/
-main/assets/talkwave/icon/ico-talkwave.svg\"
-width=\"33\"
-height=\"33\"
-class=\"me-3\" alt=\"TalkWave\" />TalkWave</h1>""")
+                f.write(f"""
+<img src="{__logo__}"
+width="33"
+height="33"
+class="me-3" alt="{__title__}" />{__title__}</h1>""")
                 f.write("</div>")
                 f.write("""
 <div class=\"container d-flex flex-wrap justify-content-end\">
 """)
                 f.write("</div>")
                 f.write("</header>")
                 f.write("  <main>\n")
@@ -181,15 +205,15 @@
                 f.write("</body>\n")
                 f.write("</html>\n")
     elif file_format in markdown:
         with open(
             os.path.join(data_dir, f"{timestamp}_log.md"),
             "a"
         ) as f:
-            f.write(f"# TalkWave 🐍 (v{VERSION})\n\n")
+            f.write(f"# {__title__} (v{__version__})\n\n")
             f.write(f"## {timestamp}\n\n")
             f.write(f"```bash\n{prompt}\n```\n\n")
             f.write(f"```bash\n{response}\n```\n")
     elif file_format in text:
         # elif file_format in ["csv", "xls", "html", "txt", "text"]:
         with open(
             os.path.join(data_dir, f"{timestamp}_log.{file_format}"),
@@ -257,14 +281,17 @@
     }
 
     model_str = model_dict.get(model)
     if model_str is None:
         print("Invalid model")
         sys.exit()
 
+    # Create the timestamp
+    timestamp = datetime.now().strftime("%Y-%m-%dT%H:%M:%SZ")
+
     json_resp = send_request(
         key,
         model_str,
         prompt,
         max_tokens,
         temperature,
         user_id,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `talkwave-0.0.4/talkwave/frontend.py` & `talkwave-0.0.5/talkwave/frontend.py`

 * *Files identical despite different names*

### Comparing `talkwave-0.0.4/talkwave.egg-info/PKG-INFO` & `talkwave-0.0.5/talkwave.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkwave
-Version: 0.0.4
+Version: 0.0.5
 Summary: TalkWave is an AI chatbot for developers written in Python.
 Home-page: https://github.com/sebastienrousseau/talkwave
 Author: Sebastien Rousseau
 Author-email: sebastian.rousseau@gmail.com
 License: Apache License 2.0
 Keywords: talkwave,chatbot,AI,machine learningnatural language processing OpenAI GPT-3 GPT3 GPT python
 Classifier: Development Status :: 4 - Beta
@@ -63,25 +63,27 @@
 ```bash
 pip install openai tabulate python-dotenv
 ```
 
 1. Clone the TalkWave repository:
 
 ```bash
-git clone https://github.com/yourusername/talkwave.git
+git clone https://github.com/sebastienrousseau/talkwave.git
 ```
 
 1. Add your OpenAI API key to a `.env` file in the project directory:
 
 ```bash
 OPENAI_API_KEY="your_api_key_here"
 ```
 
 ## Usage 🚀
 
+### Command Line Interface
+
 To use TalkWave, navigate to the project directory in your terminal and
 run the following command:
 
 ```bash
 python talkwave -p "Your prompt here"
 ```
 
@@ -95,14 +97,27 @@
 
 For more information on the available options, run:
 
 ```bash
 python talkwave --help
 ```
 
+### Web Frontend
+
+To use the web frontend, navigate to the project directory in your
+terminal and run the following command:
+
+```bash
+python talkwave/frontend.py
+```
+
+Then, open your browser and navigate to `http://127.0.0.1:5000`. This
+will open the TalkWave web frontend, which you can use to generate
+responses.
+
 ## File Structure 📁
 
 ```bash
 .
 ├── talkwave
 │   ├── data
 │   ├── templates
```

### Comparing `talkwave-0.0.4/tests/test_curl.py` & `talkwave-0.0.5/tests/test_curl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from unittest import TestCase
 from unittest.mock import MagicMock, patch
 from requests.exceptions import Timeout
 
-from curl import send_request
+from talkwave.curl import send_request
 
 
 class TestSendRequest(TestCase):
 
     # test case for missing user_id
     def test_missing_user_id(self):
         api_key = 'test_api_key'
@@ -128,29 +128,48 @@
                 user_id,
                 rate_limit_seconds,
                 stop
             )
             self.assertEqual(response, None)
             self.assertEqual(mock_post.call_count, 1)
 
-    # test case for stop
-
     @patch('requests.post')
-    def test_stop(self, mock_post):
+    def test_stop_message(self, mock_post):
         api_key = 'test_api_key'
         model = 'test_model'
         prompt = 'test_prompt'
         max_tokens = 10
         temperature = 0.5
         user_id = 'test_user'
         rate_limit_seconds = 5
-        stop = 'test_stop'
+        stop = 'stop'
+
+        # Mock response with stop message
+        mock_response = MagicMock()
+        mock_response.status_code = 200
+        mock_response.json.return_value = {
+            'choices': [
+                {
+                    'text': 'This is a stop message.',
+                    'index': 0,
+                    'logprobs': None,
+                    'finish_reason': 'stop'
+                }
+            ]
+        }
+        mock_post.return_value = mock_response
+
+        # Test that StopIteration is raised when stop message is received
+        with self.assertRaises(StopIteration):
+            send_request(api_key, model, prompt, max_tokens,
+                         temperature, user_id, rate_limit_seconds, stop)
 
-        # First call to send_request should return a response without
+        # Second call to send_request should return a response without
         # raising an exception
+
         mock_response = MagicMock()
         mock_response.status_code = 200
         mock_response.json.return_value = {
             'choices': [
                 {
                     'text': 'test_text',
                     'index': 0,
@@ -177,17 +196,18 @@
                     'index': 0,
                     'logprobs': None,
                     'finish_reason': 'test_reason'
                 }
             ]
         }
         self.assertEqual(response, expected_response)
-        self.assertEqual(mock_post.call_count, 1)
+        self.assertEqual(mock_post.call_count, 2)
 
     # test case for rate limit
+
     @patch('requests.post')
     def test_rate_limit(self, mock_post):
         api_key = 'test_api_key'
         model = 'test_model'
         prompt = 'test_prompt'
         max_tokens = 10
         temperature = 0.5
```

### Comparing `talkwave-0.0.4/tests/test_dir.py` & `talkwave-0.0.5/tests/test_dir.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 import unittest
 from unittest import TestCase
-from dir import set_data_directory
+from talkwave.dir import set_data_directory
 
 
 class TestDataDirectory(TestCase):
 
     # test case for setting the data directory
     def test_set_data_directory(self):
-        path = "/tests/test_data"
+        path = "/data"
         expected_location = os.path.join(os.path.dirname(__file__), path)
         actual_location = set_data_directory(path)
         self.assertEqual(actual_location, expected_location)
 
     # test case for setting the data directory to a non-existent directory
     def test_set_data_directory_non_existent(self):
         path = "/tests/non_existent"
         expected_location = os.path.join(os.path.dirname(__file__), path)
         actual_location = set_data_directory(path)
         self.assertEqual(actual_location, expected_location)
 
     # test case for setting the data directory to a file
     def test_set_data_directory_file(self):
-        path = "/tests/test_data/test_file.txt"
+        path = "/data/test_file.txt"
         expected_location = os.path.join(os.path.dirname(__file__), path)
         actual_location = set_data_directory(path)
         self.assertEqual(actual_location, expected_location)
 
     # test case for setting the data directory to a directory
     def test_set_data_directory_directory(self):
-        path = "/tests/test_data/test_directory"
+        path = "/data/test_directory"
         expected_location = os.path.join(os.path.dirname(__file__), path)
         actual_location = set_data_directory(path)
         self.assertEqual(actual_location, expected_location)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `talkwave-0.0.4/tests/test_main.py` & `talkwave-0.0.5/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 from unittest import TestCase, main as unittest_main
 from unittest.mock import patch
-
-from parse import parse_args
+from talkwave.parse import parse_args
 
 # Add the path to the 'utils' directory to sys.path
 # utils_path = os.path.abspath(os.path.join(
 #     os.path.dirname(__file__), '..', 'talkwave', 'utils'))
 # if not os.path.isdir(utils_path):
 #     raise ValueError(f"Cannot find 'utils' directory at {utils_path}")
 # sys.path.insert(0, utils_path)
```

