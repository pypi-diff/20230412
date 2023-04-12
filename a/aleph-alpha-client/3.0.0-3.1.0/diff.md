# Comparing `tmp/aleph-alpha-client-3.0.0.tar.gz` & `tmp/aleph-alpha-client-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-alpha-client-3.0.0.tar", last modified: Tue Apr  4 08:52:58 2023, max compression
+gzip compressed data, was "aleph-alpha-client-3.1.0.tar", last modified: Wed Apr 12 13:49:55 2023, max compression
```

## Comparing `aleph-alpha-client-3.0.0.tar` & `aleph-alpha-client-3.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:52:58.869219 aleph-alpha-client-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-04 08:52:58.869219 aleph-alpha-client-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:52:58.865219 aleph-alpha-client-3.0.0/aleph_alpha_client/
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33904 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/aleph_alpha_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/detokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/summarization.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/aleph_alpha_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:52:58.865219 aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-04 08:52:58.000000 aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-04 08:52:58.000000 aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 08:52:58.000000 aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-04 08:52:58.000000 aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 08:52:58.000000 aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 08:52:58.869219 aleph-alpha-client-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 08:52:58.869219 aleph-alpha-client-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_detokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-04 08:52:47.000000 aleph-alpha-client-3.0.0/tests/test_tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.834322 aleph-alpha-client-3.1.0/aleph_alpha_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/aleph_alpha_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/detokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18677 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/summarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/aleph_alpha_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.834322 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 13:49:55.000000 aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:49:55.838322 aleph-alpha-client-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_detokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-12 13:49:43.000000 aleph-alpha-client-3.1.0/tests/test_tokenize.py
```

### Comparing `aleph-alpha-client-3.0.0/LICENSE` & `aleph-alpha-client-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/PKG-INFO` & `aleph-alpha-client-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.0.0
+Version: 3.1.0
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.0.0/README.md` & `aleph-alpha-client-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/__init__.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/aleph_alpha_client.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/aleph_alpha_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
     ) -> EvaluationResponse:
         """Evaluates the model's likelihood to produce a completion given a prompt.
 
         Parameters:
             request (EvaluationRequest, required):
                 Parameters for the requested evaluation.
 
-            model (string, optional, default None):
+            model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> request = EvaluationRequest(
                     prompt=Prompt.from_text("hello"), completion_expected=" world"
                 )
@@ -447,19 +447,37 @@
         """
         response = self._post_request(
             "summarize",
             request,
         )
         return SummarizationResponse.from_json(response)
 
-    def _explain(
+    def explain(
         self,
         request: ExplanationRequest,
         model: str,
     ) -> ExplanationResponse:
+        """Better understand the source of a completion, specifically on how much each section of a
+        prompt impacts each token of the completion.
+
+        Parameters:
+            request (ExplanationRequest, required):
+                Parameters for the requested explanation.
+
+            model (string, required):
+                Name of model to use. A model name refers to a model architecture (number of parameters among others).
+                Always the latest version of model is used.
+
+        Examples:
+            >>> request = ExplanationRequest(
+                    prompt=Prompt.from_text("Andreas likes"),
+                    target=" pizza."
+                )
+            >>> response = client.explain(request, model="luminous-extended")
+        """
         response = self._post_request(
             "explain",
             request,
             model,
         )
         return ExplanationResponse.from_json(response)
 
@@ -696,15 +714,15 @@
     ) -> TokenizationResponse:
         """Tokenizes the given prompt for the given model.
 
         Parameters:
             request (TokenizationRequest, required):
                 Parameters for the requested tokenization.
 
-            model (string, optional, default None):
+            model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> request = TokenizationRequest(prompt="hello", token_ids=True, tokens=True)
             >>> response = await client.tokenize(request, model=model_name)
         """
@@ -722,15 +740,15 @@
     ) -> DetokenizationResponse:
         """Detokenizes the given prompt for the given model.
 
         Parameters:
             request (DetokenizationRequest, required):
                 Parameters for the requested detokenization.
 
-            model (string, optional, default None):
+            model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> request = DetokenizationRequest(token_ids=[2, 3, 4])
             >>> response = await client.detokenize(request, model=model_name)
         """
@@ -748,15 +766,15 @@
     ) -> EmbeddingResponse:
         """Embeds a text and returns vectors that can be used for downstream tasks (e.g. semantic similarity) and models (e.g. classifiers).
 
         Parameters:
             request (EmbeddingRequest, required):
                 Parameters for the requested embedding.
 
-            model (string, optional, default None):
+            model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> request = EmbeddingRequest(prompt=Prompt.from_text("This is an example."), layers=[-1], pooling=["mean"])
             >>> result = await client.embed(request, model=model_name)
         """
@@ -775,15 +793,15 @@
         """Embeds a text and returns vectors that can be used for downstream tasks
         (e.g. semantic similarity) and models (e.g. classifiers).
 
         Parameters:
             request (SemanticEmbeddingRequest, required):
                 Parameters for the requested semnatic embedding.
 
-            model (string, optional, default None):
+            model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> # function for symmetric embedding
             >>> async def embed_symmetric(text: str):
                     # Create an embeddingrequest with the type set to symmetric
@@ -824,15 +842,15 @@
     ) -> EvaluationResponse:
         """Evaluates the model's likelihood to produce a completion given a prompt.
 
         Parameters:
             request (EvaluationRequest, required):
                 Parameters for the requested evaluation.
 
-            model (string, optional, default None):
+            model (string, required):
                 Name of model to use. A model name refers to a model architecture (number of parameters among others).
                 Always the latest version of model is used.
 
         Examples:
             >>> request = EvaluationRequest(
                     prompt=Prompt.from_text("hello"), completion_expected=" world"
                 )
@@ -867,36 +885,49 @@
         request: SummarizationRequest,
     ) -> SummarizationResponse:
         """Summarizes a document.
 
         Parameters:
             request (SummarizationRequest, required):
                 Parameters for the requested summarization.
-
-            model (string, optional, default None):
-                Name of model to use. A model name refers to a model architecture (number of parameters among others).
-                Always the latest version of model is used.
-
         Examples:
             >>> request = SummarizationRequest(
                     document=Document.from_text("Andreas likes pizza."),
                 )
             >>> response = await client.summarize(request, model="luminous-extended")
         """
         response = await self._post_request(
             "summarize",
             request,
         )
         return SummarizationResponse.from_json(response)
 
-    async def _explain(
+    async def explain(
         self,
         request: ExplanationRequest,
         model: str,
     ) -> ExplanationResponse:
+        """Better understand the source of a completion, specifically on how much each section of a
+        prompt impacts each token of the completion.
+
+        Parameters:
+            request (ExplanationRequest, required):
+                Parameters for the requested explanation.
+
+            model (string, required):
+                Name of model to use. A model name refers to a model architecture (number of parameters among others).
+                Always the latest version of model is used.
+
+        Examples:
+            >>> request = ExplanationRequest(
+                    prompt=Prompt.from_text("Andreas likes"),
+                    target=" pizza."
+                )
+            >>> response = await client.explain(request, model="luminous-extended")
+        """
         response = await self._post_request(
             "explain",
             request,
             model,
         )
         return ExplanationResponse.from_json(response)
```

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/completion.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/completion.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/detokenization.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/detokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/document.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/document.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/embedding.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/embedding.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/evaluation.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/evaluation.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/explanation.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/explanation.py`

 * *Files 5% similar despite different names*

```diff
@@ -202,29 +202,31 @@
     def from_json(score: Any) -> "TextScore":
         return TextScore(
             start=score["start"],
             length=score["length"],
             score=score["score"],
         )
 
+
 class TextScoreWithRaw(NamedTuple):
     start: int
     length: int
     score: float
     text: str
 
     @staticmethod
     def from_text_score(score: TextScore, prompt: Text) -> "TextScoreWithRaw":
         return TextScoreWithRaw(
             start=score.start,
             length=score.length,
             score=score.score,
-            text=prompt.text[score.start:score.start + score.length],
+            text=prompt.text[score.start : score.start + score.length],
         )
 
+
 class ImageScore(NamedTuple):
     left: float
     top: float
     width: float
     height: float
     score: float
 
@@ -248,40 +250,49 @@
     def from_json(score: Any) -> "TargetScore":
         return TargetScore(
             start=score["start"],
             length=score["length"],
             score=score["score"],
         )
 
+
 class TargetScoreWithRaw(NamedTuple):
     start: int
     length: int
     score: float
     text: str
 
     @staticmethod
     def from_target_score(score: TargetScore, target: str) -> "TargetScoreWithRaw":
         return TargetScoreWithRaw(
             start=score.start,
             length=score.length,
             score=score.score,
-            text=target[score.start:score.start + score.length],
+            text=target[score.start : score.start + score.length],
         )
 
+
 class TokenScore(NamedTuple):
     score: float
 
     @staticmethod
     def from_json(score: Any) -> "TokenScore":
         return TokenScore(
             score=score,
         )
 
 
 class ImagePromptItemExplanation(NamedTuple):
+    """
+    Explains the importance of an image prompt item.
+    The amount of items in the "scores" array depends on the granularity setting.
+    Each score object contains the top-left corner of a rectangular area in the image prompt.
+    The coordinates are all between 0 and 1 in terms of the total image size
+    """
+
     scores: List[ImageScore]
 
     @staticmethod
     def from_json(item: Dict[str, Any]) -> "ImagePromptItemExplanation":
         return ImagePromptItemExplanation(
             scores=[ImageScore.from_json(score) for score in item["scores"]]
         )
@@ -301,58 +312,93 @@
                 )
                 for score in self.scores
             ]
         )
 
 
 class TextPromptItemExplanation(NamedTuple):
+    """
+    Explains the importance of a text prompt item.
+    The amount of items in the "scores" array depends on the granularity setting.
+    Each score object contains an inclusive start character and a length of the substring plus
+    a floating point score value.
+    """
+
     scores: List[Union[TextScore, TextScoreWithRaw]]
 
     @staticmethod
     def from_json(item: Dict[str, Any]) -> "TextPromptItemExplanation":
         return TextPromptItemExplanation(
             scores=[TextScore.from_json(score) for score in item["scores"]]
         )
-    
+
     def with_text(self, prompt: Text) -> "TextPromptItemExplanation":
         return TextPromptItemExplanation(
-            scores=[TextScoreWithRaw.from_text_score(score, prompt) if isinstance(score, TextScore) else score for score in self.scores]
+            scores=[
+                TextScoreWithRaw.from_text_score(score, prompt)
+                if isinstance(score, TextScore)
+                else score
+                for score in self.scores
+            ]
         )
 
 
-
 class TargetPromptItemExplanation(NamedTuple):
+    """
+    Explains the importance of text in the target string that came before the currently
+    to-be-explained target token. The amount of items in the "scores" array depends on the
+    granularity setting.
+    Each score object contains an inclusive start character and a length of the substring plus
+    a floating point score value.
+    """
+
     scores: List[Union[TargetScore, TargetScoreWithRaw]]
 
     @staticmethod
     def from_json(item: Dict[str, Any]) -> "TargetPromptItemExplanation":
         return TargetPromptItemExplanation(
             scores=[TargetScore.from_json(score) for score in item["scores"]]
         )
-    
+
     def with_text(self, prompt: str) -> "TargetPromptItemExplanation":
         return TargetPromptItemExplanation(
-            scores=[TargetScoreWithRaw.from_target_score(score, prompt) if isinstance(score, TargetScore) else score for score in self.scores]
+            scores=[
+                TargetScoreWithRaw.from_target_score(score, prompt)
+                if isinstance(score, TargetScore)
+                else score
+                for score in self.scores
+            ]
         )
-    
-
-
 
 
 class TokenPromptItemExplanation(NamedTuple):
+    """Explains the importance of a request prompt item of type "token_ids".
+    Will contain one floating point importance value for each token in the same order as in the original prompt.
+    """
+
     scores: List[TokenScore]
 
     @staticmethod
     def from_json(item: Dict[str, Any]) -> "TokenPromptItemExplanation":
         return TokenPromptItemExplanation(
             scores=[TokenScore.from_json(score) for score in item["scores"]]
         )
 
 
 class Explanation(NamedTuple):
+    """
+    Explanations for a given portion of the target.
+
+    Parameters:
+        target (str, required)
+            If target_granularity was set to "complete", then this will be the entire target. If it was set to "token", this will be a single target token.
+        items (List[Union[TextPromptItemExplanation, TargetPromptItemExplanation, TokenPromptItemExplanation, ImagePromptItemExplanation], required)
+            Contains one item for each prompt item (in order), and the last item refers to the target.
+    """
+
     target: str
     items: List[
         Union[
             TextPromptItemExplanation,
             TargetPromptItemExplanation,
             TokenPromptItemExplanation,
             ImagePromptItemExplanation,
@@ -393,40 +439,51 @@
                 if isinstance(item, ImagePromptItemExplanation)
                 else item
                 for item_index, item in enumerate(self.items)
             ],
         )
 
     def with_text_from_prompt(self, prompt: Prompt, target: str) -> "Explanation":
-        items: List[Union[
-            TextPromptItemExplanation,
-            ImagePromptItemExplanation,
-            TargetPromptItemExplanation,
-            TokenPromptItemExplanation,
-        ]] = []
-        for item_index, item in enumerate(self.items): 
+        items: List[
+            Union[
+                TextPromptItemExplanation,
+                ImagePromptItemExplanation,
+                TargetPromptItemExplanation,
+                TokenPromptItemExplanation,
+            ]
+        ] = []
+        for item_index, item in enumerate(self.items):
             if isinstance(item, TextPromptItemExplanation):
                 # separate variable to fix linting error
                 prompt_item = prompt.items[item_index]
-                if isinstance(prompt_item, Text): 
+                if isinstance(prompt_item, Text):
                     items.append(item.with_text(prompt_item))
                 else:
                     items.append(item)
             elif isinstance(item, TargetPromptItemExplanation):
                 items.append(item.with_text(target))
             else:
                 items.append(item)
         return Explanation(
             target=self.target,
             items=items,
         )
 
 
-
 class ExplanationResponse(NamedTuple):
+    """
+    The top-level response data structure that will be returned from an explanation request.
+
+    Parameters:
+        model_version (str, required)
+            Version of the model used to generate the explanation.
+        explanations (List[Explanation], required)
+            This array will contain one explanation object for each portion of the target.
+    """
+
     model_version: str
     explanations: List[Explanation]
 
     @staticmethod
     def from_json(json: Dict[str, Any]) -> "ExplanationResponse":
         return ExplanationResponse(
             model_version=json["model_version"],
@@ -440,15 +497,15 @@
         self, prompt: Prompt
     ) -> "ExplanationResponse":
         mapped_explanations = [
             explanation.with_image_prompt_items_in_pixels(prompt)
             for explanation in self.explanations
         ]
         return ExplanationResponse(self.model_version, mapped_explanations)
-    
+
     def with_text_from_prompt(
         self, request: ExplanationRequest
     ) -> "ExplanationResponse":
         mapped_explanations = [
             explanation.with_text_from_prompt(request.prompt, request.target)
             for explanation in self.explanations
         ]
```

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/prompt.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/qa.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/search.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/summarization.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/summarization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client/tokenization.py` & `aleph-alpha-client-3.1.0/aleph_alpha_client/tokenization.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/PKG-INFO` & `aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleph-alpha-client
-Version: 3.0.0
+Version: 3.1.0
 Summary: python client to interact with Aleph Alpha api endpoints
 Home-page: https://github.com/Aleph-Alpha/aleph-alpha-client
 Author: Aleph Alpha
 Author-email: support@aleph-alpha.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `aleph-alpha-client-3.0.0/aleph_alpha_client.egg-info/SOURCES.txt` & `aleph-alpha-client-3.1.0/aleph_alpha_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/setup.py` & `aleph-alpha-client-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_clients.py` & `aleph-alpha-client-3.1.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_complete.py` & `aleph-alpha-client-3.1.0/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_detokenize.py` & `aleph-alpha-client-3.1.0/tests/test_detokenize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_embed.py` & `aleph-alpha-client-3.1.0/tests/test_embed.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_error_handling.py` & `aleph-alpha-client-3.1.0/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_evaluate.py` & `aleph-alpha-client-3.1.0/tests/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_explanation.py` & `aleph-alpha-client-3.1.0/tests/test_explanation.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             ]
         ),
         target=" pizza with cheese",
         prompt_granularity=CustomGranularity("###"),
         target_granularity=TargetGranularity.Token,
     )
 
-    explanation = await async_client._explain(request, model=model_name)
+    explanation = await async_client.explain(request, model=model_name)
 
     assert len(explanation.explanations) == 3
     assert all([len(exp.items) == 3 for exp in explanation.explanations])
     assert len(explanation.explanations[0].items[0].scores) == 4
 
 
 # Client
@@ -72,15 +72,15 @@
         prompt_granularity="sentence",
         postprocessing=ExplanationPostprocessing.Absolute,
         normalize=True,
         target_granularity=TargetGranularity.Token,
         control_token_overlap=ControlTokenOverlap.Complete,
     )
 
-    explanation = sync_client._explain(request, model=model_name)
+    explanation = sync_client.explain(request, model=model_name)
 
     assert len(explanation.explanations) == 3
     assert all([len(exp.items) == 4 for exp in explanation.explanations])
     # At least one of the following options must be set in the request
     # to make all scores positive (or zero):
     # postprocessing=ExplanationPostProcessing.Absolute
     # postprocessing=ExplanationPostProcessing.Square
@@ -103,15 +103,15 @@
                 Tokens.from_token_ids([4014, 36316, 5681, 387]),
             ]
         ),
         target=" pizza with cheese",
         prompt_granularity=None,
     )
 
-    explanation = sync_client._explain(request, model=model_name)
+    explanation = sync_client.explain(request, model=model_name)
 
     assert len(explanation.explanations) == 1
     assert all([len(exp.items) == 4 for exp in explanation.explanations])
 
 
 def test_explanation_of_image_in_pixels(sync_client: Client, model_name: str):
     image_source_path = Path(__file__).parent / "dog-and-cat-cover.jpg"
@@ -126,15 +126,15 @@
                 Tokens.from_token_ids([4014, 36316, 5681, 387]),
             ]
         ),
         target=" pizza with cheese",
         prompt_granularity=None,
     )
 
-    explanation = sync_client._explain(request, model=model_name)
+    explanation = sync_client.explain(request, model=model_name)
 
     explanation = explanation.with_image_prompt_items_in_pixels(request.prompt)
     assert len(explanation.explanations) == 1
     assert all([len(exp.items) == 4 for exp in explanation.explanations])
     assert all(
         [
             isinstance(image_score, ImageScore) and isinstance(image_score.left, int)
@@ -146,34 +146,35 @@
 def test_explanation_of_text_in_prompt_relativ_indeces(
     sync_client: Client, model_name: str
 ):
     request = ExplanationRequest(
         prompt=Prompt(
             [
                 Text.from_text("I am a programmer and French. My favourite food is"),
-
                 # " My favorite food is"
                 Tokens.from_token_ids([4014, 36316, 5681, 387]),
             ]
         ),
         target=" pizza with cheese",
         prompt_granularity=None,
         target_granularity=TargetGranularity.Token,
     )
 
-    explanation = sync_client._explain(request, model=model_name)
+    explanation = sync_client.explain(request, model=model_name)
 
     explanation = explanation.with_text_from_prompt(request)
     assert len(explanation.explanations) == 3
     assert all([len(exp.items) == 3 for exp in explanation.explanations])
     assert all(
         [
-            isinstance(raw_text_score, TextScoreWithRaw) and isinstance(raw_text_score.text, str)
+            isinstance(raw_text_score, TextScoreWithRaw)
+            and isinstance(raw_text_score.text, str)
             for raw_text_score in explanation.explanations[0].items[0].scores
         ]
     )
     assert all(
         [
-            isinstance(raw_text_score, TargetScoreWithRaw) and isinstance(raw_text_score.text, str)
+            isinstance(raw_text_score, TargetScoreWithRaw)
+            and isinstance(raw_text_score.text, str)
             for raw_text_score in explanation.explanations[1].items[2].scores
         ]
     )
```

### Comparing `aleph-alpha-client-3.0.0/tests/test_image.py` & `aleph-alpha-client-3.1.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_prompt.py` & `aleph-alpha-client-3.1.0/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_qa.py` & `aleph-alpha-client-3.1.0/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_search.py` & `aleph-alpha-client-3.1.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_summarize.py` & `aleph-alpha-client-3.1.0/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `aleph-alpha-client-3.0.0/tests/test_tokenize.py` & `aleph-alpha-client-3.1.0/tests/test_tokenize.py`

 * *Files identical despite different names*

