# Comparing `tmp/bingbong-0.1.tar.gz` & `tmp/bingbong-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingbong-0.1.tar", last modified: Wed Apr 12 01:31:44 2023, max compression
+gzip compressed data, was "bingbong-0.1.1.tar", last modified: Wed Apr 12 04:57:44 2023, max compression
```

## Comparing `bingbong-0.1.tar` & `bingbong-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.815587 bingbong-0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      563 2023-04-12 01:31:44.815587 bingbong-0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1105 2023-04-11 13:40:02.000000 bingbong-0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 01:31:44.815587 bingbong-0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      794 2023-04-12 01:31:34.000000 bingbong-0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.807587 bingbong-0.1/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.811587 bingbong-0.1/src/bingbong.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      563 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      347 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1/src/bingbong.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 01:31:44.000000 bingbong-0.1/src/bingbong.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.815587 bingbong-0.1/src/pingpong/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2023-04-12 01:31:41.000000 bingbong-0.1/src/pingpong/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      756 2023-04-11 23:29:23.000000 bingbong-0.1/src/pingpong/alpaca.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      471 2023-04-11 14:52:10.000000 bingbong-0.1/src/pingpong/gradio.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      636 2023-04-11 23:32:31.000000 bingbong-0.1/src/pingpong/pingpong.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 01:31:44.815587 bingbong-0.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 01:05:54.000000 bingbong-0.1/tests/test_pingpong.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1909 2023-04-12 01:05:44.000000 bingbong-0.1/tests/test_strategy.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.005177 bingbong-0.1.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-04-11 05:49:32.000000 bingbong-0.1.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      565 2023-04-12 04:57:44.005177 bingbong-0.1.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1105 2023-04-11 13:40:02.000000 bingbong-0.1.1/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-12 04:57:44.005177 bingbong-0.1.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      796 2023-04-12 04:57:34.000000 bingbong-0.1.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:43.997177 bingbong-0.1.1/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.001177 bingbong-0.1.1/src/bingbong.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      565 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      371 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-12 01:31:19.000000 bingbong-0.1.1/src/bingbong.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-04-12 04:57:43.000000 bingbong-0.1.1/src/bingbong.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.005177 bingbong-0.1.1/src/pingpong/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-04-12 04:57:40.000000 bingbong-0.1.1/src/pingpong/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      853 2023-04-12 04:50:42.000000 bingbong-0.1.1/src/pingpong/alpaca.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      583 2023-04-12 04:44:04.000000 bingbong-0.1.1/src/pingpong/gradio.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      662 2023-04-12 04:40:43.000000 bingbong-0.1.1/src/pingpong/pingpong.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-12 04:57:44.005177 bingbong-0.1.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1733 2023-04-12 03:28:01.000000 bingbong-0.1.1/tests/test_pingpong.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3055 2023-04-12 04:54:28.000000 bingbong-0.1.1/tests/test_scenarios.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2686 2023-04-12 04:54:13.000000 bingbong-0.1.1/tests/test_strategy.py
```

### Comparing `bingbong-0.1/LICENSE` & `bingbong-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bingbong-0.1/PKG-INFO` & `bingbong-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1
+Version: 0.1.1
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bingbong-0.1/README.md` & `bingbong-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bingbong-0.1/setup.py` & `bingbong-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bingbong',
-    version='0.1',
+    version='0.1.1',
     description='Ping pong management library for LLM applied application',
     author='chansung park',
     author_email='deep.diver.csp@gmail.com',
     url='https://github.com/deep-diver/PingPong',
     install_requires=[],
     packages=['pingpong'],
     package_dir={'':'src'},
```

### Comparing `bingbong-0.1/src/bingbong.egg-info/PKG-INFO` & `bingbong-0.1.1/src/bingbong.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1
+Version: 0.1.1
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `bingbong-0.1/src/pingpong/alpaca.py` & `bingbong-0.1.1/src/pingpong/alpaca.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,23 @@
   @classmethod
   def prompt(cls, pingpong):
     return f"""### Instruction: {pingpong.ping}
 
 ### Response: {pingpong.pong}"""
 
 class AlpacaChatPPManager(PPManager):
-  def build_prompts(self, from_idx: int=0, fmt: PromptFmt=AlpacaPromptFmt):
+  def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt):
+    if to_idx == -1 or to_idx >= len(self.pingpongs):
+      to_idx = len(self.pingpongs)
+
     results = fmt.ctx(self.ctx)
 
-    for idx, pingpong in enumerate(self.pingpongs[from_idx:]):
+    for idx, pingpong in enumerate(self.pingpongs[from_idx:to_idx]):
       print(idx)
       results += fmt.prompt(pingpong)
 
-      if idx != len(self.pingpongs[from_idx:])-1:
+      if from_idx+idx != to_idx-1:
         results += """
 
 """
 
     return results
```

### Comparing `bingbong-0.1/src/pingpong/pingpong.py` & `bingbong-0.1.1/src/pingpong/pingpong.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 
   def add_pingpong(self, pingpong):
     self.pingpongs.append(pingpong)
 
   def pop_pingpong(self):
     return self.pingpongs.pop()
 
-  def build_prompts(self, from_idx: int, fmt: PromptFmt):
+  def build_prompts(self, from_idx: int, to_idx: int, fmt: PromptFmt):
     pass
 
-  def build_uis(self, from_idx: int, fmt: UIFmt):
+  def build_uis(self, from_idx: int, to_idx: int, fmt: UIFmt):
     pass
```

### Comparing `bingbong-0.1/tests/test_pingpong.py` & `bingbong-0.1.1/tests/test_pingpong.py`

 * *Files identical despite different names*

### Comparing `bingbong-0.1/tests/test_strategy.py` & `bingbong-0.1.1/tests/test_strategy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,72 @@
 from pingpong import PingPong
 from pingpong.gradio import GradioAlpacaChatPPManager
 from pingpong.context import CtxAutoSummaryStrategy
 from pingpong.context import CtxLastWindowStrategy
+from pingpong.context import CtxSearchWindowStrategy
 
 
 class TestStrategy():
+	def test_search_window_strategy(self):
+		pp_manager = GradioAlpacaChatPPManager()
+		strategy = CtxSearchWindowStrategy(2)
+
+		for i in range(5):
+			pp = PingPong(f"ping-{i}", f"pong-{i}")
+			pp_manager.add_pingpong(pp)
+
+		answer1 = """### Instruction: ping-0
+
+### Response: pong-0
+
+### Instruction: ping-1
+
+### Response: pong-1"""
+
+		answer2 = """### Instruction: ping-2
+
+### Response: pong-2
+
+### Instruction: ping-3
+
+### Response: pong-3"""
+
+		answer3 = """### Instruction: ping-4
+
+### Response: pong-4"""
+
+		for idx, win in enumerate(strategy(pp_manager)):
+			if idx == 0:
+				assert win == answer1
+			elif idx == 1:
+				assert win == answer2
+			elif idx == 2:
+				assert win == answer3
+			else:
+				assert True is False
+
 	def test_last_window_strategy(self):
 		pp_manager = GradioAlpacaChatPPManager()
 		strategy = CtxLastWindowStrategy(2)
 
 		for i in range(1):
 			pp = PingPong(f"ping-{i}", f"pong-{i}")
 			pp_manager.add_pingpong(pp)
 
-		answers = f"""### Instruction: ping-0
+		answers = """### Instruction: ping-0
 
 ### Response: pong-0"""
 		assert strategy(pp_manager) == answers
 
 		pp_manager = GradioAlpacaChatPPManager()
 		for i in range(3):
 			pp = PingPong(f"ping-{i}", f"pong-{i}")
 			pp_manager.add_pingpong(pp)
 
-		answers = f"""### Instruction: ping-1
+		answers = """### Instruction: ping-1
 
 ### Response: pong-1
 
 ### Instruction: ping-2
 
 ### Response: pong-2"""
 		assert strategy(pp_manager) == answers		
@@ -37,44 +76,45 @@
 		pp_manager = GradioAlpacaChatPPManager()
 		strategy = CtxAutoSummaryStrategy(2)
 
 		pp = PingPong("hello", "world")
 		pp_manager.add_pingpong(pp)
 
 		sum_req, to_summarize = strategy(pp_manager)
-		assert sum_req == False
+		assert sum_req is False
 
 		pp = PingPong("hello2", "world2")
 		pp_manager.add_pingpong(pp)
 
 		sum_req, to_summarize = strategy(pp_manager)
 		to_summarize_answer = """### Instruction: hello
 
 ### Response: world
 
 ### Instruction: hello2
 
 ### Response: world2"""
-		assert sum_req == True
+		assert sum_req is True
 		assert to_summarize == to_summarize_answer
 		assert strategy.last_idx == 2
 
 		pp = PingPong("hello3", "world3")
 		pp_manager.add_pingpong(pp)
 
 		sum_req, to_summarize = strategy(pp_manager)
-		assert sum_req == False
+		assert sum_req is False
 
 		pp = PingPong("hello4", "world4")
 		pp_manager.add_pingpong(pp)
 
 		sum_req, to_summarize = strategy(pp_manager)
 		to_summarize_answer = """### Instruction: hello3
 
 ### Response: world3
 
 ### Instruction: hello4
 
 ### Response: world4"""
-		assert sum_req == True
+
+		assert sum_req is True
 		assert to_summarize == to_summarize_answer
 		assert strategy.last_idx == 4
```

