# Comparing `tmp/llama-server-0.0.1.tar.gz` & `tmp/llama-server-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama-server-0.0.1.tar", last modified: Sun Apr  9 03:30:18 2023, max compression
+gzip compressed data, was "llama-server-0.1.0.tar", last modified: Wed Apr 12 04:39:21 2023, max compression
```

## Comparing `llama-server-0.0.1.tar` & `llama-server-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 yisu       (501) staff       (20)        0 2023-04-09 03:30:18.079564 llama-server-0.0.1/
--rw-r--r--   0 yisu       (501) staff       (20)     1062 2023-04-03 01:26:49.000000 llama-server-0.0.1/LICENSE
--rw-r--r--   0 yisu       (501) staff       (20)     3459 2023-04-09 03:30:18.079754 llama-server-0.0.1/PKG-INFO
--rw-r--r--   0 yisu       (501) staff       (20)     2616 2023-04-08 20:14:03.000000 llama-server-0.0.1/README.md
-drwxr-xr-x   0 yisu       (501) staff       (20)        0 2023-04-09 03:30:18.065972 llama-server-0.0.1/llama_server/
--rw-r--r--   0 yisu       (501) staff       (20)       22 2023-04-08 23:03:31.000000 llama-server-0.0.1/llama_server/__init__.py
-drwxr-xr-x   0 yisu       (501) staff       (20)        0 2023-04-09 03:30:18.078511 llama-server-0.0.1/llama_server/prompts/
--rw-r--r--   0 yisu       (501) staff       (20)      106 2023-04-08 20:02:05.000000 llama-server-0.0.1/llama_server/prompts/alpaca.txt
--rw-r--r--   0 yisu       (501) staff       (20)      387 2023-04-08 20:02:05.000000 llama-server-0.0.1/llama_server/prompts/chat-with-bob.txt
--rw-r--r--   0 yisu       (501) staff       (20)     1669 2023-04-09 00:04:28.000000 llama-server-0.0.1/llama_server/prompts/dan.txt
--rw-r--r--   0 yisu       (501) staff       (20)      759 2023-04-08 20:02:05.000000 llama-server-0.0.1/llama_server/prompts/reason-act.txt
--rw-r--r--   0 yisu       (501) staff       (20)     7200 2023-04-09 02:06:08.000000 llama-server-0.0.1/llama_server/server.py
-drwxr-xr-x   0 yisu       (501) staff       (20)        0 2023-04-09 03:30:18.072846 llama-server-0.0.1/llama_server.egg-info/
--rw-r--r--   0 yisu       (501) staff       (20)     3459 2023-04-09 03:30:18.000000 llama-server-0.0.1/llama_server.egg-info/PKG-INFO
--rw-r--r--   0 yisu       (501) staff       (20)      438 2023-04-09 03:30:18.000000 llama-server-0.0.1/llama_server.egg-info/SOURCES.txt
--rw-r--r--   0 yisu       (501) staff       (20)        1 2023-04-09 03:30:18.000000 llama-server-0.0.1/llama_server.egg-info/dependency_links.txt
--rw-r--r--   0 yisu       (501) staff       (20)       58 2023-04-09 03:30:18.000000 llama-server-0.0.1/llama_server.egg-info/entry_points.txt
--rw-r--r--   0 yisu       (501) staff       (20)      106 2023-04-09 03:30:18.000000 llama-server-0.0.1/llama_server.egg-info/requires.txt
--rw-r--r--   0 yisu       (501) staff       (20)       20 2023-04-09 03:30:18.000000 llama-server-0.0.1/llama_server.egg-info/top_level.txt
--rw-r--r--   0 yisu       (501) staff       (20)      392 2023-04-09 03:30:18.080675 llama-server-0.0.1/setup.cfg
--rw-r--r--   0 yisu       (501) staff       (20)     2445 2023-04-09 01:33:25.000000 llama-server-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 04:39:09.000000 llama-server-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-12 04:39:21.288362 llama-server-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-12 04:39:09.000000 llama-server-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/llama_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/llama_server/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/alpaca.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/chat-with-bob.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/dan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/prompts/reason-act.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-12 04:39:09.000000 llama-server-0.1.0/llama_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 04:39:21.288362 llama-server-0.1.0/llama_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-12 04:39:21.000000 llama-server-0.1.0/llama_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-12 04:39:21.288362 llama-server-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-12 04:39:09.000000 llama-server-0.1.0/setup.py
```

### Comparing `llama-server-0.0.1/LICENSE` & `llama-server-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llama-server-0.0.1/PKG-INFO` & `llama-server-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,16 @@
-Metadata-Version: 2.1
-Name: llama-server
-Version: 0.0.1
-Summary: LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.
-Home-page: https://github.com/nuance1979/llama-server
-Author: Yi Su
-Author-email: nuance@gmail.com
-License: MIT
-Keywords: llama llama.cpp chatbot-ui chatbot
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # LLaMA Server
 
-LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
+[![PyPI version](https://img.shields.io/pypi/v/llama-server)](https://pypi.org/project/llama-server/)[![Unit test](https://github.com/nuance1979/llama-server/actions/workflows/test.yml/badge.svg?branch=main&&event=push)](https://github.com/nuance1979/llama-server/actions)[![GitHub stars](https://img.shields.io/github/stars/nuance1979/llama-server)](https://star-history.com/#nuance1979/llama-server&Date)[![GitHub license](https://img.shields.io/github/license/nuance1979/llama-server)](https://github.com/nuance1979/llama-server/blob/master/LICENSE)
+
+LLaMA Server combines the power of [LLaMA C++](https://github.com/ggerganov/llama.cpp) (via [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)) with the beauty of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui).
 
-🦙LLaMA C++ ➕ 🤖Chatbot UI ➕ 🔗LLaMA Server 🟰 😊
+🦙LLaMA C++ (via 🐍PyLLaMACpp) ➕ 🤖Chatbot UI ➕ 🔗LLaMA Server 🟰 😊
 
-**UPDATE**: Now supports Windows through [pyllamacpp](https://github.com/nomic-ai/pyllamacpp)! And better streaming!
+**UPDATE**: Now supports better streaming through [PyLLaMACpp](https://github.com/nomic-ai/pyllamacpp)!
 
 **UPDATE**: Now supports streaming!
 
 ## Demo
 - Streaming
 
 https://user-images.githubusercontent.com/10931178/229980159-61546fa6-2985-4cdc-8230-5dcb6a69c559.mov
@@ -42,27 +22,49 @@
 
 ## Setup
 
 - Get your favorite LLaMA models by
   - Download from [🤗Hugging Face](https://huggingface.co/models?sort=downloads&search=ggml);
   - Or follow instructions at [LLaMA C++](https://github.com/ggerganov/llama.cpp);
   - Make sure models are converted and quantized;
-  - Copy models to the folders with correct name, e.g., `models/7B/ggml-model-q4_0.bin`;
+
+- Create a `models.yml` file to provide your `model_home` directory and add your favorite [South American camelids](https://en.wikipedia.org/wiki/Lama_(genus)), e.g.:
+```yaml
+model_home: /path/to/your/models
+models:
+  llama-7b:
+    name: LLAMA-7B
+    path: 7B/ggml-model-q4_0.bin  # relative to `model_home` or an absolute path
+```
+See [models.yml](https://github.com/nuance1979/llama-server/blob/main/models.yml) for an example.
 
 - Set up python environment:
 ```bash
 conda create -n llama python=3.9
 conda activate llama
-python -m pip install -r requirements.txt
 ```
 
-- Start LLaMA Server:
+- Install LLaMA Server:
+  - From PyPI:
+  ```bash
+  python -m pip install llama-server
+  ```
+  - Or from source:
+  ```bash
+  python -m pip install git+https://github.com/nuance1979/llama-server.git
+  ```
+
+- Install a patched version of PyLLaMACpp: (*Note:* this step will not be needed **after** PyLLaMACpp makes a new release.)
+```bash
+python -m pip install git+https://github.com/nuance1979/pyllamacpp.git@dev --upgrade
+```
+
+- Start LLaMA Server with your `models.yml` file:
 ```bash
-export LLAMA_SERVER_HOME=$(git rev-parse --show-toplevel)  # path to this repo
-python -m llama_server
+llama-server --models-yml models.yml --model-id llama-7b
 ```
 
 - Check out [my fork](https://github.com/nuance1979/chatbot-ui) of Chatbot UI and start the app;
 ```bash
 git clone https://github.com/nuance1979/chatbot-ui
 cd chatbot-ui
 git checkout llama
@@ -78,19 +80,18 @@
   ```
 - Enjoy!
 
 ## More
 
 - Try a larger model if you have it:
 ```bash
-export LLAMA_MODEL_ID=llama-13b  # llama-7b/llama-33b/llama-65b
-python -m llama_server
+llama-server --models-yml models.yml --model-id llama-13b  # or any `model_id` defined in `models.yml`
 ```
 
-- Try streaming mode by restarting Chatbot UI:
+- Try non-streaming mode by restarting Chatbot UI:
 ```bash
 export LLAMA_STREAM_MODE=1  # 0 to disable streaming
 npm run dev
 ```
 
 ## Limitations
```

### Comparing `llama-server-0.0.1/llama_server/prompts/dan.txt` & `llama-server-0.1.0/llama_server/prompts/dan.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.0.1/llama_server/prompts/reason-act.txt` & `llama-server-0.1.0/llama_server/prompts/reason-act.txt`

 * *Files identical despite different names*

### Comparing `llama-server-0.0.1/llama_server/server.py` & `llama-server-0.1.0/llama_server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from fastapi import FastAPI
 from pydantic import BaseModel
 from pyllamacpp.model import Model
 from sse_starlette import EventSourceResponse
 
 
 PROMPT_PATH = Path(__file__).parent / "prompts" / "chat-with-bob.txt"
-PROMPT = PROMPT_PATH.read_text().strip()
+PROMPT = PROMPT_PATH.read_text(encoding="utf-8").strip()
 PROMPT_SIZE = len(PROMPT)
 REVERSE_PROMPT = "User:"
 REPLY_PREFIX = "Bob: "
 
 
 class Message(BaseModel):
     role: str
```

### Comparing `llama-server-0.0.1/setup.py` & `llama-server-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 
 def get_version() -> str:
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    init = (Path("llama_server") / "__init__.py").read_text().split()
+    init = (Path("llama_server") / "__init__.py").read_text(encoding="utf-8").split()
     return init[init.index("__version__") + 2][1:-1]
 
 
 def get_install_requires() -> str:
     return [
         "pyllamacpp",
         "fastapi",
@@ -36,15 +36,15 @@
     return req
 
 
 setup(
     name="llama-server",
     version=get_version(),
     description="LLaMA Server combines the power of LLaMA C++ with the beauty of Chatbot UI.",
-    long_description=Path("README.md").read_text(),
+    long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/nuance1979/llama-server",
     author="Yi Su",
     author_email="nuance@gmail.com",
     license="MIT",
     python_requires=">=3.8",
     classifiers=[
```

