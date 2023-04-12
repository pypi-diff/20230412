# Comparing `tmp/revChatGPT-4.1.6.tar.gz` & `tmp/revChatGPT-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.1.6.tar", last modified: Mon Apr 10 03:31:17 2023, max compression
+gzip compressed data, was "revChatGPT-4.2.0.tar", last modified: Wed Apr 12 03:12:27 2023, max compression
```

## Comparing `revChatGPT-4.1.6.tar` & `revChatGPT-4.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-10 03:31:16.000000 revChatGPT-4.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.140262 revChatGPT-4.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.144262 revChatGPT-4.1.6/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    34518 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23144 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-10 03:30:47.000000 revChatGPT-4.1.6/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 03:31:17.148262 revChatGPT-4.1.6/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-10 03:31:17.000000 revChatGPT-4.1.6/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.720898 revChatGPT-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-12 03:12:27.720898 revChatGPT-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-12 03:12:27.720898 revChatGPT-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.712898 revChatGPT-4.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.716898 revChatGPT-4.2.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    47327 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23144 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.716898 revChatGPT-4.2.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-12 03:11:50.000000 revChatGPT-4.2.0/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:12:27.716898 revChatGPT-4.2.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 03:12:27.000000 revChatGPT-4.2.0/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.1.6/LICENSE` & `revChatGPT-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/PKG-INFO` & `revChatGPT-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.6
+Version: 4.2.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,16 +26,14 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-[![](./view.gif)](https://pypi.python.org/pypi/revChatGPT)
-
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
@@ -53,24 +51,24 @@
 
 <details>
 
 <summary>
 
 # V1 Standard ChatGPT
 
-> > 3:35 PM - Rate limit at 5 requests / 10 seconds due to small server (I ran out of budget.)
-
-> ### [Privacy policy](./PRIVACY.md)
->
-> <br>
+This uses a reversed `chat.openai.com`'s API with a [cloudflare bypass server](https://github.com/acheong08/ChatGPT-Proxy-V4) to make programmatic ChatGPT usage free. This specific library is meant for personal use due to severe rate limits on OpenAI's side. It has not been optimized for use with mutliple accounts.
 
-> ### !!! Server is now open source at https://github.com/acheong08/ChatGPT-Proxy-V4 for personal use (requires ChatGPT plus)
+You can check out [this project](https://github.com/acheong08/ChatGPT-to-API) for well supported multi account cycling. It is compatible with the official API. Use [OpenAI's documentation](https://platform.openai.com/docs/guides/chat) as reference on usage. It carries conversations between accounts to ensure rate limits are not hit given a high number of accounts.
 
 </summary>
 
+## Rate limits
+- Proxy server: 5 requests / 10 seconds
+- OpenAI: 50 requests / hour for each account
+
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
@@ -84,14 +82,16 @@
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
 
+> Please this!
+
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
```

### Comparing `revChatGPT-4.1.6/README.md` & `revChatGPT-4.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-[![](./view.gif)](https://pypi.python.org/pypi/revChatGPT)
-
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
@@ -31,24 +29,24 @@
 
 <details>
 
 <summary>
 
 # V1 Standard ChatGPT
 
-> > 3:35 PM - Rate limit at 5 requests / 10 seconds due to small server (I ran out of budget.)
-
-> ### [Privacy policy](./PRIVACY.md)
->
-> <br>
+This uses a reversed `chat.openai.com`'s API with a [cloudflare bypass server](https://github.com/acheong08/ChatGPT-Proxy-V4) to make programmatic ChatGPT usage free. This specific library is meant for personal use due to severe rate limits on OpenAI's side. It has not been optimized for use with mutliple accounts.
 
-> ### !!! Server is now open source at https://github.com/acheong08/ChatGPT-Proxy-V4 for personal use (requires ChatGPT plus)
+You can check out [this project](https://github.com/acheong08/ChatGPT-to-API) for well supported multi account cycling. It is compatible with the official API. Use [OpenAI's documentation](https://platform.openai.com/docs/guides/chat) as reference on usage. It carries conversations between accounts to ensure rate limits are not hit given a high number of accounts.
 
 </summary>
 
+## Rate limits
+- Proxy server: 5 requests / 10 seconds
+- OpenAI: 50 requests / hour for each account
+
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
@@ -62,14 +60,16 @@
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
 
+> Please this!
+
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
```

### Comparing `revChatGPT-4.1.6/setup.py` & `revChatGPT-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.1.6",
+    version="4.2.0",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.1.6/src/revChatGPT/V3.py` & `revChatGPT-4.2.0/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/src/revChatGPT/__init__.py` & `revChatGPT-4.2.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/src/revChatGPT/__main__.py` & `revChatGPT-4.2.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.2.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/src/revChatGPT/typings.py` & `revChatGPT-4.2.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/src/revChatGPT/utils.py` & `revChatGPT-4.2.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.6/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.2.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.6
+Version: 4.2.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -26,16 +26,14 @@
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
 
-[![](./view.gif)](https://pypi.python.org/pypi/revChatGPT)
-
 > ## Support my work
 >
 > Make a pull request and fix my bad code.
 >
 > [![support](https://ko-fi.com/img/githubbutton_sm.svg)](https://www.youtube.com/watch?v=dQw4w9WgXcQ)
 
 > #### Discord Server: https://discord.gg/9K2BvbXEHT
@@ -53,24 +51,24 @@
 
 <details>
 
 <summary>
 
 # V1 Standard ChatGPT
 
-> > 3:35 PM - Rate limit at 5 requests / 10 seconds due to small server (I ran out of budget.)
-
-> ### [Privacy policy](./PRIVACY.md)
->
-> <br>
+This uses a reversed `chat.openai.com`'s API with a [cloudflare bypass server](https://github.com/acheong08/ChatGPT-Proxy-V4) to make programmatic ChatGPT usage free. This specific library is meant for personal use due to severe rate limits on OpenAI's side. It has not been optimized for use with mutliple accounts.
 
-> ### !!! Server is now open source at https://github.com/acheong08/ChatGPT-Proxy-V4 for personal use (requires ChatGPT plus)
+You can check out [this project](https://github.com/acheong08/ChatGPT-to-API) for well supported multi account cycling. It is compatible with the official API. Use [OpenAI's documentation](https://platform.openai.com/docs/guides/chat) as reference on usage. It carries conversations between accounts to ensure rate limits are not hit given a high number of accounts.
 
 </summary>
 
+## Rate limits
+- Proxy server: 5 requests / 10 seconds
+- OpenAI: 50 requests / hour for each account
+
 ## Configuration
 
 1. Create account on [OpenAI's ChatGPT](https://chat.openai.com/)
 2. Save your email and password
 
 ### Authentication method: (Choose 1)
 
@@ -84,14 +82,16 @@
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
 
+> Please this!
+
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
```

