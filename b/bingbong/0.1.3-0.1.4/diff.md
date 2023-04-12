# Comparing `tmp/bingbong-0.1.3.tar.gz` & `tmp/bingbong-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingbong-0.1.3.tar", last modified: Wed Apr 12 06:06:50 2023, max compression
+gzip compressed data, was "bingbong-0.1.4.tar", last modified: Wed Apr 12 15:50:15 2023, max compression
```

## Comparing `bingbong-0.1.3.tar` & `bingbong-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 06:06:50.572730 bingbong-0.1.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1.3/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2458 2023-04-12 06:06:50.572730 bingbong-0.1.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1851 2023-04-12 05:11:48.000000 bingbong-0.1.3/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 06:06:50.572730 bingbong-0.1.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      971 2023-04-12 06:06:26.000000 bingbong-0.1.3/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 06:06:50.544729 bingbong-0.1.3/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 06:06:50.564730 bingbong-0.1.3/src/bingbong.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2458 2023-04-12 06:06:50.000000 bingbong-0.1.3/src/bingbong.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      371 2023-04-12 06:06:50.000000 bingbong-0.1.3/src/bingbong.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 06:06:50.000000 bingbong-0.1.3/src/bingbong.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1.3/src/bingbong.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 06:06:50.000000 bingbong-0.1.3/src/bingbong.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 06:06:50.568730 bingbong-0.1.3/src/pingpong/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-04-12 06:06:22.000000 bingbong-0.1.3/src/pingpong/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      853 2023-04-12 04:50:42.000000 bingbong-0.1.3/src/pingpong/alpaca.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      583 2023-04-12 04:44:04.000000 bingbong-0.1.3/src/pingpong/gradio.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      662 2023-04-12 04:40:43.000000 bingbong-0.1.3/src/pingpong/pingpong.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 06:06:50.568730 bingbong-0.1.3/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 03:28:01.000000 bingbong-0.1.3/tests/test_pingpong.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-04-12 04:54:28.000000 bingbong-0.1.3/tests/test_scenarios.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2686 2023-04-12 04:54:13.000000 bingbong-0.1.3/tests/test_strategy.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 15:50:15.838457 bingbong-0.1.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1.4/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3346 2023-04-12 15:50:15.834457 bingbong-0.1.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2740 2023-04-12 07:46:43.000000 bingbong-0.1.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 15:50:15.838457 bingbong-0.1.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      991 2023-04-12 15:49:41.000000 bingbong-0.1.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 15:50:15.806456 bingbong-0.1.4/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 15:50:15.818456 bingbong-0.1.4/src/bingbong.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3346 2023-04-12 15:50:15.000000 bingbong-0.1.4/src/bingbong.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      575 2023-04-12 15:50:15.000000 bingbong-0.1.4/src/bingbong.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 15:50:15.000000 bingbong-0.1.4/src/bingbong.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1.4/src/bingbong.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 15:50:15.000000 bingbong-0.1.4/src/bingbong.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 15:50:15.822456 bingbong-0.1.4/src/pingpong/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-04-12 15:50:11.000000 bingbong-0.1.4/src/pingpong/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      853 2023-04-12 04:50:42.000000 bingbong-0.1.4/src/pingpong/alpaca.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 15:50:15.830457 bingbong-0.1.4/src/pingpong/context/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      173 2023-04-12 04:36:28.000000 bingbong-0.1.4/src/pingpong/context/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      589 2023-04-12 00:59:39.000000 bingbong-0.1.4/src/pingpong/context/auto_summary_strategy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      502 2023-04-12 04:51:09.000000 bingbong-0.1.4/src/pingpong/context/last_window_strategy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      840 2023-04-12 04:54:35.000000 bingbong-0.1.4/src/pingpong/context/search_window_strategy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2023-04-11 14:54:21.000000 bingbong-0.1.4/src/pingpong/context/strategy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      583 2023-04-12 04:44:04.000000 bingbong-0.1.4/src/pingpong/gradio.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      662 2023-04-12 04:40:43.000000 bingbong-0.1.4/src/pingpong/pingpong.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 15:50:15.834457 bingbong-0.1.4/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 03:28:01.000000 bingbong-0.1.4/tests/test_pingpong.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-04-12 04:54:28.000000 bingbong-0.1.4/tests/test_scenarios.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2686 2023-04-12 04:54:13.000000 bingbong-0.1.4/tests/test_strategy.py
```

### Comparing `bingbong-0.1.3/LICENSE` & `bingbong-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.3/PKG-INFO` & `bingbong-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-Metadata-Version: 2.1
-Name: bingbong
-Version: 0.1.3
-Summary: Ping pong management library for LLM applied application
-Home-page: https://github.com/deep-diver/PingPong
-Author: chansung park
-Author-email: deep.diver.csp@gmail.com
-Keywords: LLM,pingpong,prompt,context,management
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PingPong
 
 <p align="center">
     <img width="200" src="https://raw.githubusercontent.com/deep-diver/PingPong/main/assets/logo.png">
 </p>
 
 PingPong is a simple library to manage pings(prompt) and pongs(response). The main purpose of this library is to manage histories and contexts in LLM applied applications such as ChatGPT.
 
 The basic motivations behind this project are:
-- Abstract prompt and response so that any UIs and Prompt formats can be adopted
-- Abstract context management strategies to apply any number of context managements
+- **Abstract prompt and response so that any UIs and Prompt formats can be adopted**
+  - There are a number of instruction-following finetuned language models, but they are fine-tuned with differently crafted datasets. For instance, the Alpaca dataset works when `### Insturction:`, `### Response:`, and `### Input:` are given while StackLLaMA works when `Question:` and `Answer` are given even though the underlying pre-trained LLM is the same LLaMA.
+  - THere are a number of UIs built to interact with language model such as Chatbot. Even with a single example of Chatbot, one could use Gradio while other could use JavaScript based tools, and they represents prompt histories in different data structure. 
+- **Abstract context management strategies to apply any number of context managements**
+  - There could be a number of strategies to effectively handle context due to the limit of the number of input tokens in language model(usually 4096). It is also possible to mix different strategies.
 
 ## Installation
 
 ```shell
 $ pip install bingbong
 ```
 
@@ -37,15 +24,14 @@
 ```python
 from pingpong import PingPong
 from pingpong.gradio import GradioAlpacaChatPPManager
 from pingpong.context import CtxAutoSummaryStrategy
 from pingpong.context import CtxLastWindowStrategy
 from pingpong.context import CtxSearchWindowStrategy
 
-```python
 ppmanager = GradioAlpacaChatPPManager()
 strategies = [
     CtxAutoSummaryStrategy(2),
     CtxLastWindowStrategy(1),
     CtxSearchWindowStrategy(1)
 ]
 
@@ -67,7 +53,11 @@
         elif isinstanceof(strategy, CtxSearchWindowStrategy):
             for cur_win in strategy(ppmanager):
                 # looking the entire conversation through
                 # a sliding window, size of 1
                 # find out relevant history to the recent conversation
                 ...
 ```
+
+## Todos
+
+- [ ] Add an working example with Gradio application
```

### Comparing `bingbong-0.1.3/setup.py` & `bingbong-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='bingbong',
-    version='0.1.3',
+    version='0.1.4',
     description='Ping pong management library for LLM applied application',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='chansung park',
     author_email='deep.diver.csp@gmail.com',
     url='https://github.com/deep-diver/PingPong',
     install_requires=[],
-    packages=['pingpong'],
+    packages=['pingpong', 'pingpong.context'],
     package_dir={'':'src'},
     keywords=['LLM', 'pingpong', 'prompt', 'context', 'management'],
     python_reuqires='>=3.8',
     package_data={},
     zip_safe=False,
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `bingbong-0.1.3/src/bingbong.egg-info/PKG-INFO` & `bingbong-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,16 +19,19 @@
 <p align="center">
     <img width="200" src="https://raw.githubusercontent.com/deep-diver/PingPong/main/assets/logo.png">
 </p>
 
 PingPong is a simple library to manage pings(prompt) and pongs(response). The main purpose of this library is to manage histories and contexts in LLM applied applications such as ChatGPT.
 
 The basic motivations behind this project are:
-- Abstract prompt and response so that any UIs and Prompt formats can be adopted
-- Abstract context management strategies to apply any number of context managements
+- **Abstract prompt and response so that any UIs and Prompt formats can be adopted**
+  - There are a number of instruction-following finetuned language models, but they are fine-tuned with differently crafted datasets. For instance, the Alpaca dataset works when `### Insturction:`, `### Response:`, and `### Input:` are given while StackLLaMA works when `Question:` and `Answer` are given even though the underlying pre-trained LLM is the same LLaMA.
+  - THere are a number of UIs built to interact with language model such as Chatbot. Even with a single example of Chatbot, one could use Gradio while other could use JavaScript based tools, and they represents prompt histories in different data structure. 
+- **Abstract context management strategies to apply any number of context managements**
+  - There could be a number of strategies to effectively handle context due to the limit of the number of input tokens in language model(usually 4096). It is also possible to mix different strategies.
 
 ## Installation
 
 ```shell
 $ pip install bingbong
 ```
 
@@ -37,15 +40,14 @@
 ```python
 from pingpong import PingPong
 from pingpong.gradio import GradioAlpacaChatPPManager
 from pingpong.context import CtxAutoSummaryStrategy
 from pingpong.context import CtxLastWindowStrategy
 from pingpong.context import CtxSearchWindowStrategy
 
-```python
 ppmanager = GradioAlpacaChatPPManager()
 strategies = [
     CtxAutoSummaryStrategy(2),
     CtxLastWindowStrategy(1),
     CtxSearchWindowStrategy(1)
 ]
 
@@ -67,7 +69,11 @@
         elif isinstanceof(strategy, CtxSearchWindowStrategy):
             for cur_win in strategy(ppmanager):
                 # looking the entire conversation through
                 # a sliding window, size of 1
                 # find out relevant history to the recent conversation
                 ...
 ```
+
+## Todos
+
+- [ ] Add an working example with Gradio application
```

### Comparing `bingbong-0.1.3/src/pingpong/alpaca.py` & `bingbong-0.1.4/src/pingpong/alpaca.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.3/src/pingpong/gradio.py` & `bingbong-0.1.4/src/pingpong/gradio.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.3/src/pingpong/pingpong.py` & `bingbong-0.1.4/src/pingpong/pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.3/tests/test_pingpong.py` & `bingbong-0.1.4/tests/test_pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.3/tests/test_scenarios.py` & `bingbong-0.1.4/tests/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1.3/tests/test_strategy.py` & `bingbong-0.1.4/tests/test_strategy.py`

 * *Files identical despite different names*

