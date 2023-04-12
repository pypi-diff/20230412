# Comparing `tmp/openai_api_call-0.3.4.tar.gz` & `tmp/openai_api_call-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.3.4.tar", last modified: Mon Apr 10 08:31:09 2023, max compression
+gzip compressed data, was "openai_api_call-0.3.5.tar", last modified: Wed Apr 12 13:16:09 2023, max compression
```

## Comparing `openai_api_call-0.3.4.tar` & `openai_api_call-0.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 08:31:09.000000 openai_api_call-0.3.4/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:31:09.677534 openai_api_call-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-10 08:30:57.000000 openai_api_call-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:16:09.580229 openai_api_call-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-12 13:16:09.580229 openai_api_call-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:16:09.580229 openai_api_call-0.3.5/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:16:09.580229 openai_api_call-0.3.5/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-12 13:16:08.000000 openai_api_call-0.3.5/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 13:16:09.000000 openai_api_call-0.3.5/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:16:08.000000 openai_api_call-0.3.5/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 13:16:08.000000 openai_api_call-0.3.5/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:16:08.000000 openai_api_call-0.3.5/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 13:16:08.000000 openai_api_call-0.3.5/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 13:16:08.000000 openai_api_call-0.3.5/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:16:09.580229 openai_api_call-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-12 13:15:46.000000 openai_api_call-0.3.5/setup.py
```

### Comparing `openai_api_call-0.3.4/LICENSE` & `openai_api_call-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.4/PKG-INFO` & `openai_api_call-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.3.4
+Version: 0.3.5
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -37,14 +37,22 @@
         Or set `OPENAI_API_KEY` in `~/.bashrc` to avoid setting the API key every time:
         
         ```bash
         # Add the following code to ~/.bashrc
         export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         ```
         
+        Also, you might set different `api_key` for each `Chat` object:
+        
+        ```py
+        from openai_api_call import Chat
+        chat = Chat("hello")
+        chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        ```
+        
         ### Set Proxy (Optional)
         
         ```py
         from openai_api_call import proxy_on, proxy_off, proxy_status
         # Check the current proxy
         proxy_status()
         
@@ -60,16 +68,15 @@
         
         Alternatively, you can use a proxy URL to send requests from restricted network, as shown below:
         
         ```py
         from openai_api_call import request
         
         # set request url
-        alt_url = "https://api.example.com/v1/chat/completions"
-        request.url = alt_url
+        request.base_url = "https://api.example.com"
         ```
         
         ### Basic Usage
         
         Example 1, send prompt and return response:
         
         ```python
@@ -100,17 +107,15 @@
         # Set the number of retries to Inf
         # The timeout for each request is 10 seconds
         response = chat.getresponse(temperature=0.5, max_requests=-1, timeout=10)
         print("Number of consumed tokens: ", response.total_tokens)
         print("Returned content: ", response.content)
         ```
         
-        ### Advanced Usage
-        
-        Continue chatting based on the last response:
+        Example 3, continue chatting based on the last response:
         
         ```python
         # first call
         chat = Chat("Hello, GPT-3.5!")
         resp = chat.getresponse() # update chat history, default is True
         print(resp.content)
         
@@ -126,14 +131,26 @@
         # get the last result
         print(chat[-1])
         
         # print chat history
         chat.print_log()
         ```
         
+        Moreover, you can check the usage status of the API key:
+        
+        ```py
+        # show usage status of the default API key
+        chat = Chat()
+        chat.show_usage_status()
+        
+        # show usage status of the specified API key
+        chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        chat.show_usage_status()
+        ```
+        
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
```

### Comparing `openai_api_call-0.3.4/README.md` & `openai_api_call-0.3.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 Or set `OPENAI_API_KEY` in `~/.bashrc` to avoid setting the API key every time:
 
 ```bash
 # Add the following code to ~/.bashrc
 export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
 ```
 
+Also, you might set different `api_key` for each `Chat` object:
+
+```py
+from openai_api_call import Chat
+chat = Chat("hello")
+chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+```
+
 ### Set Proxy (Optional)
 
 ```py
 from openai_api_call import proxy_on, proxy_off, proxy_status
 # Check the current proxy
 proxy_status()
 
@@ -52,16 +60,15 @@
 
 Alternatively, you can use a proxy URL to send requests from restricted network, as shown below:
 
 ```py
 from openai_api_call import request
 
 # set request url
-alt_url = "https://api.example.com/v1/chat/completions"
-request.url = alt_url
+request.base_url = "https://api.example.com"
 ```
 
 ### Basic Usage
 
 Example 1, send prompt and return response:
 
 ```python
@@ -92,17 +99,15 @@
 # Set the number of retries to Inf
 # The timeout for each request is 10 seconds
 response = chat.getresponse(temperature=0.5, max_requests=-1, timeout=10)
 print("Number of consumed tokens: ", response.total_tokens)
 print("Returned content: ", response.content)
 ```
 
-### Advanced Usage
-
-Continue chatting based on the last response:
+Example 3, continue chatting based on the last response:
 
 ```python
 # first call
 chat = Chat("Hello, GPT-3.5!")
 resp = chat.getresponse() # update chat history, default is True
 print(resp.content)
 
@@ -118,14 +123,26 @@
 # get the last result
 print(chat[-1])
 
 # print chat history
 chat.print_log()
 ```
 
+Moreover, you can check the usage status of the API key:
+
+```py
+# show usage status of the default API key
+chat = Chat()
+chat.show_usage_status()
+
+# show usage status of the specified API key
+chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+chat.show_usage_status()
+```
+
 ## License
 
 This package is licensed under the MIT license. See the LICENSE file for more details.
 
 ## update log
 
 - Since version `0.2.0`, `Chat` type is used to handle data
```

### Comparing `openai_api_call-0.3.4/openai_api_call/__init__.py` & `openai_api_call-0.3.5/openai_api_call/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.3.4'
+__version__ = '0.3.5'
 
 import os
-from .chattool import Chat, Resp, chat_completion
+from .chattool import Chat, Resp, chat_completion, usage_status
 from .proxy import proxy_on, proxy_off, proxy_status
 
 # read API key from the environment variable
 if os.environ.get('OPENAI_API_KEY') is not None:
     api_key = os.environ.get('OPENAI_API_KEY')
     if not api_key.startswith("sk-"):
         print("Warning: The default environment variable `OPENAI_API_KEY` is not a valid API key.")
```

### Comparing `openai_api_call-0.3.4/openai_api_call/chattool.py` & `openai_api_call-0.3.5/openai_api_call/chattool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # The object that stores the chat log
 
 from typing import List, Dict, Union
 import openai_api_call
 from .response import Resp
-from .request import chat_completion
+from .request import chat_completion, usage_status
 import signal, time, random
+import datetime
 
 # timeout handler
 def handler(signum, frame):
     raise Exception("API call timed out!")
 
 class Chat():
     def __init__(self, msg:Union[List[Dict], None, str]=None) -> None:
@@ -89,14 +90,51 @@
         else:
             raise Exception("Failed to get the response!\nYou can try to update the API key"
                             + ", increase `max_requests` or set proxy.")
         if update: # update the chat log
             self.assistant(resp.content)
         return resp
 
+    def get_usage_status(self, recent:int=10, duration:int=99):
+        """Get the usage status
+        
+        Args:
+            recent (int, optional): number of the usage of recent days. Defaults to 10.
+            duration (int, optional): duration of the usage. Defaults to 99.
+        
+        Returns:
+            str: usage status
+        """
+        storage, usage, dailyusage = usage_status(self.api_key, duration=duration)
+        status = [storage, usage, storage-usage, {}]
+        if recent <= 0 or len(dailyusage) == 0: # no need to print the usage of recent days
+            return status
+        recent = min(recent, len(dailyusage)) # number of recent days
+        dailyusage = dailyusage[-recent:]
+        for day in dailyusage:
+            date = datetime.datetime.fromtimestamp(day.get("timestamp")).strftime("%Y-%m-%d")
+            line_items = day.get("line_items")
+            cost = sum([item.get("cost") for item in line_items]) / 100
+            status[-1].update({date: cost})
+        return status
+    
+    def show_usage_status(self, recent:int=10, duration:int=99):
+        """Show the usage status
+        
+        Args:
+            recent (int, optional): number of the usage of recent days. Defaults to 10.
+            duration (int, optional): duration of the usage. Defaults to 99.
+        """
+        storage, usage, rem, recent_usage = self.get_usage_status(recent=recent, duration=duration)
+        print(f"Total account: {storage:.4f}$")
+        print(f"Total usage: {usage:.4f}$")
+        print(f"Total remaining: {storage-usage:.4f}$")
+        for date, cost in recent_usage.items():
+            print(f"{date}: {cost:.4f}$")
+
     def add(self, role:str, msg:str):
         assert role in ['user', 'assistant', 'system'], "role should be 'user', 'assistant' or 'system'"
         self._chat_log.append({"role": role, "content": msg})
         return self
 
     def user(self, msg:str):
         """User message"""
```

### Comparing `openai_api_call-0.3.4/openai_api_call/proxy.py` & `openai_api_call-0.3.5/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.4/openai_api_call/response.py` & `openai_api_call-0.3.5/openai_api_call/response.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.3.4/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.3.5/openai_api_call.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.3.4
+Version: 0.3.5
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/RexWzh/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -37,14 +37,22 @@
         Or set `OPENAI_API_KEY` in `~/.bashrc` to avoid setting the API key every time:
         
         ```bash
         # Add the following code to ~/.bashrc
         export OPENAI_API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
         ```
         
+        Also, you might set different `api_key` for each `Chat` object:
+        
+        ```py
+        from openai_api_call import Chat
+        chat = Chat("hello")
+        chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        ```
+        
         ### Set Proxy (Optional)
         
         ```py
         from openai_api_call import proxy_on, proxy_off, proxy_status
         # Check the current proxy
         proxy_status()
         
@@ -60,16 +68,15 @@
         
         Alternatively, you can use a proxy URL to send requests from restricted network, as shown below:
         
         ```py
         from openai_api_call import request
         
         # set request url
-        alt_url = "https://api.example.com/v1/chat/completions"
-        request.url = alt_url
+        request.base_url = "https://api.example.com"
         ```
         
         ### Basic Usage
         
         Example 1, send prompt and return response:
         
         ```python
@@ -100,17 +107,15 @@
         # Set the number of retries to Inf
         # The timeout for each request is 10 seconds
         response = chat.getresponse(temperature=0.5, max_requests=-1, timeout=10)
         print("Number of consumed tokens: ", response.total_tokens)
         print("Returned content: ", response.content)
         ```
         
-        ### Advanced Usage
-        
-        Continue chatting based on the last response:
+        Example 3, continue chatting based on the last response:
         
         ```python
         # first call
         chat = Chat("Hello, GPT-3.5!")
         resp = chat.getresponse() # update chat history, default is True
         print(resp.content)
         
@@ -126,14 +131,26 @@
         # get the last result
         print(chat[-1])
         
         # print chat history
         chat.print_log()
         ```
         
+        Moreover, you can check the usage status of the API key:
+        
+        ```py
+        # show usage status of the default API key
+        chat = Chat()
+        chat.show_usage_status()
+        
+        # show usage status of the specified API key
+        chat.api_key = "sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
+        chat.show_usage_status()
+        ```
+        
         ## License
         
         This package is licensed under the MIT license. See the LICENSE file for more details.
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
```

### Comparing `openai_api_call-0.3.4/setup.py` & `openai_api_call-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 
 requirements = ['Click>=7.0', 'requests>=2.20']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
```

