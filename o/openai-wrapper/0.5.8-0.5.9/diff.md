# Comparing `tmp/openai_wrapper-0.5.8.tar.gz` & `tmp/openai_wrapper-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_wrapper-0.5.8.tar", max compression
+gzip compressed data, was "openai_wrapper-0.5.9.tar", max compression
```

## Comparing `openai_wrapper-0.5.8.tar` & `openai_wrapper-0.5.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      134 2022-11-29 21:37:02.139266 openai_wrapper-0.5.8/openai_wrapper/__init__.py
--rw-r--r--   0        0        0    13180 2022-11-29 21:37:02.139266 openai_wrapper-0.5.8/openai_wrapper/completion.py
--rw-r--r--   0        0        0     2053 2022-11-29 21:37:02.139266 openai_wrapper-0.5.8/openai_wrapper/config.py
--rw-r--r--   0        0        0      729 2022-11-29 21:37:02.143266 openai_wrapper-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 openai_wrapper-0.5.8/setup.py
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      134 2022-11-29 21:49:50.056076 openai_wrapper-0.5.9/openai_wrapper/__init__.py
+-rw-r--r--   0        0        0    13150 2022-11-29 21:49:50.056076 openai_wrapper-0.5.9/openai_wrapper/completion.py
+-rw-r--r--   0        0        0     2053 2022-11-29 21:49:50.056076 openai_wrapper-0.5.9/openai_wrapper/config.py
+-rw-r--r--   0        0        0      729 2022-11-29 21:49:50.060076 openai_wrapper-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 openai_wrapper-0.5.9/setup.py
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.5.9/PKG-INFO
```

### Comparing `openai_wrapper-0.5.8/openai_wrapper/completion.py` & `openai_wrapper-0.5.9/openai_wrapper/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,34 +222,31 @@
             A dictionary containing the completion request and response
         """
         if preprocess_prompt_args is None:
             preprocess_prompt_args = {}
         if process_response_args is None:
             process_response_args = {}
 
+        logging.info(f"Sending async request to OpenAI with params: {self.model_params}")
         preprocessed_prompt = preprocess_prompt(prompt, **preprocess_prompt_args)
         self.model_params["prompt"] = preprocessed_prompt
         request_headers = {"Authorization": f"Bearer {self.openai_client.api_key}",
                            "Content-Type": "application/json"}
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.post("https://api.openai.com/v1/completions",
                                         headers=request_headers,
                                         json=self.model_params) as resp:
                     response = await resp.json()
+                    logging.info(f"Response: {response}")
 
                     if process_response is not None:
                         response = process_response(response, **process_response_args)
 
-                    logging.debug(f"Response: {response}")
-
-                    if "usage" in response:
-                        request_costs = self._calculate_request_costs(response["usage"]["total_tokens"])
-                    else:
-                        request_costs = 0.0
+                    request_costs = self._calculate_request_costs(response["usage"]["total_tokens"])
 
                     document = {
                         "prompt": preprocessed_prompt,
                         "prompt_version": prompt_version,
                         "prompt_version_description": prompt_version_description,
                         "completion_text": response["choices"][0]["text"],
                         "openai_response": response,
```

### Comparing `openai_wrapper-0.5.8/openai_wrapper/config.py` & `openai_wrapper-0.5.9/openai_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.5.8/pyproject.toml` & `openai_wrapper-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-wrapper"
-version = "0.5.8"
+version = "0.5.9"
 description = "A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models."
 authors = ["AI Team <datascience@prosus.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 openai = "^0.25.0"
```

### Comparing `openai_wrapper-0.5.8/setup.py` & `openai_wrapper-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'motor>=3.1.1,<4.0.0',
  'openai>=0.25.0,<0.26.0',
  'pymongo>=4.2.0,<5.0.0',
  'typeguard>=2.13.3,<3.0.0']
 
 setup_kwargs = {
     'name': 'openai-wrapper',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': "A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models.",
     'long_description': 'None',
     'author': 'AI Team',
     'author_email': 'datascience@prosus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `openai_wrapper-0.5.8/PKG-INFO` & `openai_wrapper-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-wrapper
-Version: 0.5.8
+Version: 0.5.9
 Summary: A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models.
 License: MIT
 Author: AI Team
 Author-email: datascience@prosus.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

