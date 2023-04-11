# Comparing `tmp/sleepyask-4.3.2.tar.gz` & `tmp/sleepyask-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyask-4.3.2.tar", last modified: Sun Mar 26 23:32:36 2023, max compression
+gzip compressed data, was "sleepyask-4.4.0.tar", last modified: Tue Apr 11 22:13:32 2023, max compression
```

## Comparing `sleepyask-4.3.2.tar` & `sleepyask-4.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:32:36.562601 sleepyask-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-26 23:32:25.000000 sleepyask-4.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-26 23:32:36.562601 sleepyask-4.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-03-26 23:32:25.000000 sleepyask-4.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-26 23:32:25.000000 sleepyask-4.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 23:32:36.562601 sleepyask-4.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:32:36.562601 sleepyask-4.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:32:36.562601 sleepyask-4.3.2/src/sleepyask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:32:36.562601 sleepyask-4.3.2/src/sleepyask/openai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 23:32:25.000000 sleepyask-4.3.2/src/sleepyask/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-26 23:32:25.000000 sleepyask-4.3.2/src/sleepyask/openai/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-26 23:32:25.000000 sleepyask-4.3.2/src/sleepyask/openai/chatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 23:32:36.562601 sleepyask-4.3.2/src/sleepyask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-26 23:32:36.000000 sleepyask-4.3.2/src/sleepyask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-26 23:32:36.000000 sleepyask-4.3.2/src/sleepyask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 23:32:36.000000 sleepyask-4.3.2/src/sleepyask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-26 23:32:36.000000 sleepyask-4.3.2/src/sleepyask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-26 23:32:36.000000 sleepyask-4.3.2/src/sleepyask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.552820 sleepyask-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 22:13:21.000000 sleepyask-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-11 22:13:32.552820 sleepyask-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-11 22:13:21.000000 sleepyask-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-11 22:13:21.000000 sleepyask-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 22:13:32.552820 sleepyask-4.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.548820 sleepyask-4.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.548820 sleepyask-4.4.0/src/sleepyask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.552820 sleepyask-4.4.0/src/sleepyask/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:21.000000 sleepyask-4.4.0/src/sleepyask/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-11 22:13:21.000000 sleepyask-4.4.0/src/sleepyask/openai/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-11 22:13:21.000000 sleepyask-4.4.0/src/sleepyask/openai/chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:13:32.552820 sleepyask-4.4.0/src/sleepyask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 22:13:32.000000 sleepyask-4.4.0/src/sleepyask.egg-info/top_level.txt
```

### Comparing `sleepyask-4.3.2/LICENSE` & `sleepyask-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepyask-4.3.2/PKG-INFO` & `sleepyask-4.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 4.3.2
+Version: 4.4.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227806954-ee58434a-c782-4c79-901a-5ca8db264bfd.png" width=450/>
+  <img src="https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-48d8-b17a-4e4126ddd245.png" width=450/>
 </p>
 
 <p align="center">
-  A small tool for automating collecting data from ChatGPT over long periods of time.
+  A small tool for collecting data from ChatGPT over long periods of time.
 </p>
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-4470-bb8d-738e9269ccae.png" width="900" />
+  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
 </p>
 
 <p align="center">
 	<a href="https://github.com/hwelsters/sleepyask/stargazers">
-		<img alt="Stargazers" src="https://img.shields.io/github/stars/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=342430"></a>
+		<img alt="Stargazers" src="https://img.shields.io/github/stars/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=5f8872"></a>
 	<a href="https://github.com/hwelsters/sleepyask/releases/latest">
-		<img alt="Releases" src="https://img.shields.io/github/release/hwelsters/sleepyask.svg?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=342430"/></a>
+		<img alt="Releases" src="https://img.shields.io/github/release/hwelsters/sleepyask.svg?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=5f8872"/></a>
 	<a href="https://github.com/hwelsters/sleepyask/issues">
-		<img alt="Issues" src="https://img.shields.io/github/issues/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=342430"></a>
+		<img alt="Issues" src="https://img.shields.io/github/issues/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=5f8872"></a>
 </p>
 
-## What does it do?
-ChatGPT currently limits the number of questions that users may ask per hour. The goal of this project is to allow users to just leave their computers on for extended periods of time to collect large amounts of responses from ChatGPT. There might not be a lot of practical use for this. Its main use is in research or data analysis.
+## 💬 What does it do?
+ChatGPT rate limits the number of questions users may ask. The goal of this project is to allow users to just leave their computers on for extended periods of time to collect large amounts of responses from ChatGPT. Contributions are welcome! 🤗
 
-## Installation
+## 💬 Installation
 To install sleepyask, do one of the following:
 ```bash
 > pip install sleepyask
 > py -m pip install sleepyask
 > python -m pip install sleepyask
 ```
 This project also depends on the following packages
 ```bash
 > openai
 ```
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-4470-bb8d-738e9269ccae.png" width="900" />
+  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
 </p>
 
-## Usage
+## 💬 Usage
 
 ### Authentication
 You are required to provide an organization as well as an API Key  
-`organization` - Your organization ID. Get it here: https://platform.openai.com/account/org-settings  
-`api_key` - You create an API Key on OpenAI by. Get it here: https://platform.openai.com/account/api-keys
+- `organization` - Your OpenAI organization ID. Get it here: https://platform.openai.com/account/org-settings  
+- `api_key` - You OpenAI API Key. To get it:
 ```bash
-> Clicking on your profile picture on the top-right 
+> Go to https://platform.openai.com/account/api-keys
+> Login (if it is required)
+> Click on your profile picture on the top-right 
 > View API Keys 
 > Create new secret key.  
 ```
-`count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
+- `count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
 	
-Sample config
-```python
-config = {
-	"organization": "Your OpenAI organization",
-	"api_key": "Your OpenAI api key",
-	"count": 1 
-}
-```
 ### Sample code
+It is recommended that you do not store your user credentials directly in your code. Instead, use something like `python-dotenv` to store your credentials in another file.
 ```python
+from dotenv import load_dotenv
 from sleepyask.openai import chat
 
-# Your ChatGPT login information
-config_1 = {
-	"organization": "Your ChatGPT organization",
-	"api_key": "Your ChatGPT api key",
-	"count": 1
-}
+load_dotenv()  # take environment variables from .env.
 
-config_2 = {
-	"organization": "Your ChatGPT organization",
-	"api_key": "Your ChatGPT api key",
+# Your ChatGPT authentication configs
+config = {
+	"organization": os.getenv('OPENAI_ORGANIZATION_1'),
+	"api_key": os.getenv('OPENAI_API_KEY_1'),
 	"count": 1
 }
 
-configs = [config_1, config_2]
+# List of authentication configs
+configs = [config]
 
-## List of questions you would like to ask ChatGPT
-question_list = [
-  'What is 1 + 1?',
-  'What is 1 + 2?',
-  'What is 1 + 3?'
-]
+# List of questions you would like to ask ChatGPT
+question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?']
 
 # The filename in which you would like your responses to be stored.
 # sleepyask will create this file for you. If you create it yourself, there might be some problems.
 output_file_path = 'draw.json'  
 
 # Run sleepy_ask
 chat.ask(configs=configs,
            questions=question_list,
            output_file_path=output_file_path,
            verbose=True)
-
-# chat.ask has the following optional parameters:
-# verbose : bool = Whether or not sleepyask should print its prompts. It is False by default.
-# model: str = The ChatGPT model to ask. This is "gpt-3.5-turbo" by default.
-# system_text: str | None = System text to prime ChatGPT. This is None by default.
-# temperature: float | None = Defines how non-deterministic ChatGPT is. Ranges from 0 - 2. Lower values are more deterministic. This is 1 by default
-# max_tokens: int | None = Defines the maximum number of tokens in ChatGPT's response. This is 2048 by default.
 ```
 
-## Get involved
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
+</p>
+
+### Parameters
+`sleepyask.openai.ask` has the following parameters:
+#### Required
+- `configs` :: **(required)** - should be a list of dicts containing `organization` (your OpenAI organization ID), `api key` (your OpenAI api key) and the `count` (the number of instances to spin up for asking questions)
+- `questions` :: **(required)** - should be a list of strings containing questions you would like to ask ChatGPT.
+- `output_file_path` :: **(required)** - should be a valid file path where you would like your responses to be stored. sleepyask will create this file for you. If you create this file yourself, there might be some problems.
+
+#### Optional
+- `verbose` :: **(optional)** - a boolean which specifies whether or not sleepyask should print its progress to the console. It is `False` by default
+- `model` :: **(optional)** - to specify which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default
+- `system_text` :: **(optional)** - to specify system text. It is `
+- `temperature` :: **(optional)** - to specify how deterministic ChatGPT's responses are. Ranges from `0-2` where higher numbers represent increased randomness. It is `1` by default.
+- `max_tokens` :: **(optional)** - to specify the maximum number of tokens in ChatGPT's response. This is `2048` by default
+
+## 💬 Get involved
 - 🐛 **Found a bug or interested in adding a feature?** - Create an [issue][issue]  
 - 🤗 **Want to help?** - Create a pull-request!  
 
 [issue]: https://github.com/hwelsters/sleepyask/issues
```

#### html2text {}

```diff
@@ -1,52 +1,64 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 4.3.2 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 4.4.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
- [https://user-images.githubusercontent.com/84760072/227806954-ee58434a-c782-
-                          4c79-901a-5ca8db264bfd.png]
- A small tool for automating collecting data from ChatGPT over long periods of
-                                     time.
- [https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-
-                          4470-bb8d-738e9269ccae.png]
+ [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
+                          48d8-b17a-4e4126ddd245.png]
+   A small tool for collecting data from ChatGPT over long periods of time.
+ [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
+                          4ddd-a99d-019566cce0c5.png]
                        [Stargazers] [Releases] [Issues]
-## What does it do? ChatGPT currently limits the number of questions that users
-may ask per hour. The goal of this project is to allow users to just leave
-their computers on for extended periods of time to collect large amounts of
-responses from ChatGPT. There might not be a lot of practical use for this. Its
-main use is in research or data analysis. ## Installation To install sleepyask,
-do one of the following: ```bash > pip install sleepyask > py -m pip install
-sleepyask > python -m pip install sleepyask ``` This project also depends on
-the following packages ```bash > openai ```
- [https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-
-                          4470-bb8d-738e9269ccae.png]
-## Usage ### Authentication You are required to provide an organization as well
-as an API Key `organization` - Your organization ID. Get it here: https://
-platform.openai.com/account/org-settings `api_key` - You create an API Key on
-OpenAI by. Get it here: https://platform.openai.com/account/api-keys ```bash >
-Clicking on your profile picture on the top-right > View API Keys > Create new
-secret key. ``` `count` - This specifies the number of workers to create for
-asking questions. You can have multiple workers asking questions in parallel.
-Sample config ```python config = { "organization": "Your OpenAI organization",
-"api_key": "Your OpenAI api key", "count": 1 } ``` ### Sample code ```python
-from sleepyask.openai import chat # Your ChatGPT login information config_1 =
-{ "organization": "Your ChatGPT organization", "api_key": "Your ChatGPT api
-key", "count": 1 } config_2 = { "organization": "Your ChatGPT organization",
-"api_key": "Your ChatGPT api key", "count": 1 } configs = [config_1, config_2]
-## List of questions you would like to ask ChatGPT question_list = [ 'What is 1
-+ 1?', 'What is 1 + 2?', 'What is 1 + 3?' ] # The filename in which you would
-like your responses to be stored. # sleepyask will create this file for you. If
-you create it yourself, there might be some problems. output_file_path =
-'draw.json' # Run sleepy_ask chat.ask(configs=configs, questions=question_list,
-output_file_path=output_file_path, verbose=True) # chat.ask has the following
-optional parameters: # verbose : bool = Whether or not sleepyask should print
-its prompts. It is False by default. # model: str = The ChatGPT model to ask.
-This is "gpt-3.5-turbo" by default. # system_text: str | None = System text to
-prime ChatGPT. This is None by default. # temperature: float | None = Defines
-how non-deterministic ChatGPT is. Ranges from 0 - 2. Lower values are more
-deterministic. This is 1 by default # max_tokens: int | None = Defines the
-maximum number of tokens in ChatGPT's response. This is 2048 by default. ``` ##
-Get involved - ð **Found a bug or interested in adding a feature?** - Create
-an [issue][issue] - ð¤ **Want to help?** - Create a pull-request! [issue]:
-https://github.com/hwelsters/sleepyask/issues
+## ð¬ What does it do? ChatGPT rate limits the number of questions users may
+ask. The goal of this project is to allow users to just leave their computers
+on for extended periods of time to collect large amounts of responses from
+ChatGPT. Contributions are welcome! ð¤ ## ð¬ Installation To install
+sleepyask, do one of the following: ```bash > pip install sleepyask > py -m pip
+install sleepyask > python -m pip install sleepyask ``` This project also
+depends on the following packages ```bash > openai ```
+ [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
+                          4ddd-a99d-019566cce0c5.png]
+## ð¬ Usage ### Authentication You are required to provide an organization as
+well as an API Key - `organization` - Your OpenAI organization ID. Get it here:
+https://platform.openai.com/account/org-settings - `api_key` - You OpenAI API
+Key. To get it: ```bash > Go to https://platform.openai.com/account/api-keys >
+Login (if it is required) > Click on your profile picture on the top-right >
+View API Keys > Create new secret key. ``` - `count` - This specifies the
+number of workers to create for asking questions. You can have multiple workers
+asking questions in parallel. ### Sample code It is recommended that you do not
+store your user credentials directly in your code. Instead, use something like
+`python-dotenv` to store your credentials in another file. ```python from
+dotenv import load_dotenv from sleepyask.openai import chat load_dotenv() #
+take environment variables from .env. # Your ChatGPT authentication configs
+config = { "organization": os.getenv('OPENAI_ORGANIZATION_1'), "api_key":
+os.getenv('OPENAI_API_KEY_1'), "count": 1 } # List of authentication configs
+configs = [config] # List of questions you would like to ask ChatGPT
+question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?'] # The
+filename in which you would like your responses to be stored. # sleepyask will
+create this file for you. If you create it yourself, there might be some
+problems. output_file_path = 'draw.json' # Run sleepy_ask chat.ask
+(configs=configs, questions=question_list, output_file_path=output_file_path,
+verbose=True) ```
+ [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
+                          4ddd-a99d-019566cce0c5.png]
+### Parameters `sleepyask.openai.ask` has the following parameters: ####
+Required - `configs` :: **(required)** - should be a list of dicts containing
+`organization` (your OpenAI organization ID), `api key` (your OpenAI api key)
+and the `count` (the number of instances to spin up for asking questions) -
+`questions` :: **(required)** - should be a list of strings containing
+questions you would like to ask ChatGPT. - `output_file_path` :: **(required)**
+- should be a valid file path where you would like your responses to be stored.
+sleepyask will create this file for you. If you create this file yourself,
+there might be some problems. #### Optional - `verbose` :: **(optional)** - a
+boolean which specifies whether or not sleepyask should print its progress to
+the console. It is `False` by default - `model` :: **(optional)** - to specify
+which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default - `system_text`
+:: **(optional)** - to specify system text. It is ` - `temperature` :: **
+(optional)** - to specify how deterministic ChatGPT's responses are. Ranges
+from `0-2` where higher numbers represent increased randomness. It is `1` by
+default. - `max_tokens` :: **(optional)** - to specify the maximum number of
+tokens in ChatGPT's response. This is `2048` by default ## ð¬ Get involved -
+ð **Found a bug or interested in adding a feature?** - Create an [issue]
+[issue] - ð¤ **Want to help?** - Create a pull-request! [issue]: https://
+github.com/hwelsters/sleepyask/issues
```

### Comparing `sleepyask-4.3.2/pyproject.toml` & `sleepyask-4.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sleepyask"
-version = "4.3.2"
+version = "4.4.0"
 authors = [
   { name="hwelsters", email="redacted@redacted.redacted" },
 ]
 description = "A small tool for automating collecting data from ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = []
```

### Comparing `sleepyask-4.3.2/src/sleepyask/openai/chat.py` & `sleepyask-4.4.0/src/sleepyask/openai/chat.py`

 * *Files identical despite different names*

### Comparing `sleepyask-4.3.2/src/sleepyask/openai/chatgpt.py` & `sleepyask-4.4.0/src/sleepyask/openai/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     with open(output_file_path, 'a') as outfile:
         outfile.write(json.dumps(data))
         outfile.write("\n")
         outfile.close()
 
 
 def __clean_str_for_json(text: str):
+    return text
     return text.replace("\"", "\'")
 
 
 def ask_questions(configs : list, questions : list, output_file_path : str, verbose: bool = False, model : str = "gpt-3.5-turbo", system_text : str | None = None, temperature : float | None = 1, max_tokens : int | None = 2048) -> None:
     question_queue = queue.Queue()
     save_queue = queue.Queue()
```

### Comparing `sleepyask-4.3.2/src/sleepyask.egg-info/PKG-INFO` & `sleepyask-4.4.0/src/sleepyask.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,121 @@
 Metadata-Version: 2.1
 Name: sleepyask
-Version: 4.3.2
+Version: 4.4.0
 Summary: A small tool for automating collecting data from ChatGPT
 Author-email: hwelsters <redacted@redacted.redacted>
 Project-URL: Homepage, https://github.com/hwelsters/sleepyask
 Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227806954-ee58434a-c782-4c79-901a-5ca8db264bfd.png" width=450/>
+  <img src="https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-48d8-b17a-4e4126ddd245.png" width=450/>
 </p>
 
 <p align="center">
-  A small tool for automating collecting data from ChatGPT over long periods of time.
+  A small tool for collecting data from ChatGPT over long periods of time.
 </p>
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-4470-bb8d-738e9269ccae.png" width="900" />
+  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
 </p>
 
 <p align="center">
 	<a href="https://github.com/hwelsters/sleepyask/stargazers">
-		<img alt="Stargazers" src="https://img.shields.io/github/stars/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=342430"></a>
+		<img alt="Stargazers" src="https://img.shields.io/github/stars/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=5f8872"></a>
 	<a href="https://github.com/hwelsters/sleepyask/releases/latest">
-		<img alt="Releases" src="https://img.shields.io/github/release/hwelsters/sleepyask.svg?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=342430"/></a>
+		<img alt="Releases" src="https://img.shields.io/github/release/hwelsters/sleepyask.svg?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=5f8872"/></a>
 	<a href="https://github.com/hwelsters/sleepyask/issues">
-		<img alt="Issues" src="https://img.shields.io/github/issues/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=342430"></a>
+		<img alt="Issues" src="https://img.shields.io/github/issues/hwelsters/sleepyask?style=for-the-badge&logo=starship&color=f9e1cb&logoColor=ffffff&labelColor=5f8872"></a>
 </p>
 
-## What does it do?
-ChatGPT currently limits the number of questions that users may ask per hour. The goal of this project is to allow users to just leave their computers on for extended periods of time to collect large amounts of responses from ChatGPT. There might not be a lot of practical use for this. Its main use is in research or data analysis.
+## 💬 What does it do?
+ChatGPT rate limits the number of questions users may ask. The goal of this project is to allow users to just leave their computers on for extended periods of time to collect large amounts of responses from ChatGPT. Contributions are welcome! 🤗
 
-## Installation
+## 💬 Installation
 To install sleepyask, do one of the following:
 ```bash
 > pip install sleepyask
 > py -m pip install sleepyask
 > python -m pip install sleepyask
 ```
 This project also depends on the following packages
 ```bash
 > openai
 ```
 
 <p align="center">
-  <img src="https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-4470-bb8d-738e9269ccae.png" width="900" />
+  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
 </p>
 
-## Usage
+## 💬 Usage
 
 ### Authentication
 You are required to provide an organization as well as an API Key  
-`organization` - Your organization ID. Get it here: https://platform.openai.com/account/org-settings  
-`api_key` - You create an API Key on OpenAI by. Get it here: https://platform.openai.com/account/api-keys
+- `organization` - Your OpenAI organization ID. Get it here: https://platform.openai.com/account/org-settings  
+- `api_key` - You OpenAI API Key. To get it:
 ```bash
-> Clicking on your profile picture on the top-right 
+> Go to https://platform.openai.com/account/api-keys
+> Login (if it is required)
+> Click on your profile picture on the top-right 
 > View API Keys 
 > Create new secret key.  
 ```
-`count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
+- `count` - This specifies the number of workers to create for asking questions. You can have multiple workers asking questions in parallel.  
 	
-Sample config
-```python
-config = {
-	"organization": "Your OpenAI organization",
-	"api_key": "Your OpenAI api key",
-	"count": 1 
-}
-```
 ### Sample code
+It is recommended that you do not store your user credentials directly in your code. Instead, use something like `python-dotenv` to store your credentials in another file.
 ```python
+from dotenv import load_dotenv
 from sleepyask.openai import chat
 
-# Your ChatGPT login information
-config_1 = {
-	"organization": "Your ChatGPT organization",
-	"api_key": "Your ChatGPT api key",
-	"count": 1
-}
+load_dotenv()  # take environment variables from .env.
 
-config_2 = {
-	"organization": "Your ChatGPT organization",
-	"api_key": "Your ChatGPT api key",
+# Your ChatGPT authentication configs
+config = {
+	"organization": os.getenv('OPENAI_ORGANIZATION_1'),
+	"api_key": os.getenv('OPENAI_API_KEY_1'),
 	"count": 1
 }
 
-configs = [config_1, config_2]
+# List of authentication configs
+configs = [config]
 
-## List of questions you would like to ask ChatGPT
-question_list = [
-  'What is 1 + 1?',
-  'What is 1 + 2?',
-  'What is 1 + 3?'
-]
+# List of questions you would like to ask ChatGPT
+question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?']
 
 # The filename in which you would like your responses to be stored.
 # sleepyask will create this file for you. If you create it yourself, there might be some problems.
 output_file_path = 'draw.json'  
 
 # Run sleepy_ask
 chat.ask(configs=configs,
            questions=question_list,
            output_file_path=output_file_path,
            verbose=True)
-
-# chat.ask has the following optional parameters:
-# verbose : bool = Whether or not sleepyask should print its prompts. It is False by default.
-# model: str = The ChatGPT model to ask. This is "gpt-3.5-turbo" by default.
-# system_text: str | None = System text to prime ChatGPT. This is None by default.
-# temperature: float | None = Defines how non-deterministic ChatGPT is. Ranges from 0 - 2. Lower values are more deterministic. This is 1 by default
-# max_tokens: int | None = Defines the maximum number of tokens in ChatGPT's response. This is 2048 by default.
 ```
 
-## Get involved
+<p align="center">
+  <img src="https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-4ddd-a99d-019566cce0c5.png" width="900" />
+</p>
+
+### Parameters
+`sleepyask.openai.ask` has the following parameters:
+#### Required
+- `configs` :: **(required)** - should be a list of dicts containing `organization` (your OpenAI organization ID), `api key` (your OpenAI api key) and the `count` (the number of instances to spin up for asking questions)
+- `questions` :: **(required)** - should be a list of strings containing questions you would like to ask ChatGPT.
+- `output_file_path` :: **(required)** - should be a valid file path where you would like your responses to be stored. sleepyask will create this file for you. If you create this file yourself, there might be some problems.
+
+#### Optional
+- `verbose` :: **(optional)** - a boolean which specifies whether or not sleepyask should print its progress to the console. It is `False` by default
+- `model` :: **(optional)** - to specify which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default
+- `system_text` :: **(optional)** - to specify system text. It is `
+- `temperature` :: **(optional)** - to specify how deterministic ChatGPT's responses are. Ranges from `0-2` where higher numbers represent increased randomness. It is `1` by default.
+- `max_tokens` :: **(optional)** - to specify the maximum number of tokens in ChatGPT's response. This is `2048` by default
+
+## 💬 Get involved
 - 🐛 **Found a bug or interested in adding a feature?** - Create an [issue][issue]  
 - 🤗 **Want to help?** - Create a pull-request!  
 
 [issue]: https://github.com/hwelsters/sleepyask/issues
```

#### html2text {}

```diff
@@ -1,52 +1,64 @@
-Metadata-Version: 2.1 Name: sleepyask Version: 4.3.2 Summary: A small tool for
+Metadata-Version: 2.1 Name: sleepyask Version: 4.4.0 Summary: A small tool for
 automating collecting data from ChatGPT Author-email: hwelsters
 redacted.redacted> Project-URL: Homepage, https://github.com/hwelsters/
 sleepyask Project-URL: Bug Tracker, https://github.com/hwelsters/sleepyask/
 issues Requires-Python: >=3.7 Description-Content-Type: text/markdown License-
 File: LICENSE
- [https://user-images.githubusercontent.com/84760072/227806954-ee58434a-c782-
-                          4c79-901a-5ca8db264bfd.png]
- A small tool for automating collecting data from ChatGPT over long periods of
-                                     time.
- [https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-
-                          4470-bb8d-738e9269ccae.png]
+ [https://user-images.githubusercontent.com/84760072/227817729-098182f3-6916-
+                          48d8-b17a-4e4126ddd245.png]
+   A small tool for collecting data from ChatGPT over long periods of time.
+ [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
+                          4ddd-a99d-019566cce0c5.png]
                        [Stargazers] [Releases] [Issues]
-## What does it do? ChatGPT currently limits the number of questions that users
-may ask per hour. The goal of this project is to allow users to just leave
-their computers on for extended periods of time to collect large amounts of
-responses from ChatGPT. There might not be a lot of practical use for this. Its
-main use is in research or data analysis. ## Installation To install sleepyask,
-do one of the following: ```bash > pip install sleepyask > py -m pip install
-sleepyask > python -m pip install sleepyask ``` This project also depends on
-the following packages ```bash > openai ```
- [https://user-images.githubusercontent.com/84760072/227807017-21bcda58-4e89-
-                          4470-bb8d-738e9269ccae.png]
-## Usage ### Authentication You are required to provide an organization as well
-as an API Key `organization` - Your organization ID. Get it here: https://
-platform.openai.com/account/org-settings `api_key` - You create an API Key on
-OpenAI by. Get it here: https://platform.openai.com/account/api-keys ```bash >
-Clicking on your profile picture on the top-right > View API Keys > Create new
-secret key. ``` `count` - This specifies the number of workers to create for
-asking questions. You can have multiple workers asking questions in parallel.
-Sample config ```python config = { "organization": "Your OpenAI organization",
-"api_key": "Your OpenAI api key", "count": 1 } ``` ### Sample code ```python
-from sleepyask.openai import chat # Your ChatGPT login information config_1 =
-{ "organization": "Your ChatGPT organization", "api_key": "Your ChatGPT api
-key", "count": 1 } config_2 = { "organization": "Your ChatGPT organization",
-"api_key": "Your ChatGPT api key", "count": 1 } configs = [config_1, config_2]
-## List of questions you would like to ask ChatGPT question_list = [ 'What is 1
-+ 1?', 'What is 1 + 2?', 'What is 1 + 3?' ] # The filename in which you would
-like your responses to be stored. # sleepyask will create this file for you. If
-you create it yourself, there might be some problems. output_file_path =
-'draw.json' # Run sleepy_ask chat.ask(configs=configs, questions=question_list,
-output_file_path=output_file_path, verbose=True) # chat.ask has the following
-optional parameters: # verbose : bool = Whether or not sleepyask should print
-its prompts. It is False by default. # model: str = The ChatGPT model to ask.
-This is "gpt-3.5-turbo" by default. # system_text: str | None = System text to
-prime ChatGPT. This is None by default. # temperature: float | None = Defines
-how non-deterministic ChatGPT is. Ranges from 0 - 2. Lower values are more
-deterministic. This is 1 by default # max_tokens: int | None = Defines the
-maximum number of tokens in ChatGPT's response. This is 2048 by default. ``` ##
-Get involved - ð **Found a bug or interested in adding a feature?** - Create
-an [issue][issue] - ð¤ **Want to help?** - Create a pull-request! [issue]:
-https://github.com/hwelsters/sleepyask/issues
+## ð¬ What does it do? ChatGPT rate limits the number of questions users may
+ask. The goal of this project is to allow users to just leave their computers
+on for extended periods of time to collect large amounts of responses from
+ChatGPT. Contributions are welcome! ð¤ ## ð¬ Installation To install
+sleepyask, do one of the following: ```bash > pip install sleepyask > py -m pip
+install sleepyask > python -m pip install sleepyask ``` This project also
+depends on the following packages ```bash > openai ```
+ [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
+                          4ddd-a99d-019566cce0c5.png]
+## ð¬ Usage ### Authentication You are required to provide an organization as
+well as an API Key - `organization` - Your OpenAI organization ID. Get it here:
+https://platform.openai.com/account/org-settings - `api_key` - You OpenAI API
+Key. To get it: ```bash > Go to https://platform.openai.com/account/api-keys >
+Login (if it is required) > Click on your profile picture on the top-right >
+View API Keys > Create new secret key. ``` - `count` - This specifies the
+number of workers to create for asking questions. You can have multiple workers
+asking questions in parallel. ### Sample code It is recommended that you do not
+store your user credentials directly in your code. Instead, use something like
+`python-dotenv` to store your credentials in another file. ```python from
+dotenv import load_dotenv from sleepyask.openai import chat load_dotenv() #
+take environment variables from .env. # Your ChatGPT authentication configs
+config = { "organization": os.getenv('OPENAI_ORGANIZATION_1'), "api_key":
+os.getenv('OPENAI_API_KEY_1'), "count": 1 } # List of authentication configs
+configs = [config] # List of questions you would like to ask ChatGPT
+question_list = ['What is 1 + 1?', 'What is 1 + 2?', 'What is 1 + 3?'] # The
+filename in which you would like your responses to be stored. # sleepyask will
+create this file for you. If you create it yourself, there might be some
+problems. output_file_path = 'draw.json' # Run sleepy_ask chat.ask
+(configs=configs, questions=question_list, output_file_path=output_file_path,
+verbose=True) ```
+ [https://user-images.githubusercontent.com/84760072/227817860-f4aef84b-9992-
+                          4ddd-a99d-019566cce0c5.png]
+### Parameters `sleepyask.openai.ask` has the following parameters: ####
+Required - `configs` :: **(required)** - should be a list of dicts containing
+`organization` (your OpenAI organization ID), `api key` (your OpenAI api key)
+and the `count` (the number of instances to spin up for asking questions) -
+`questions` :: **(required)** - should be a list of strings containing
+questions you would like to ask ChatGPT. - `output_file_path` :: **(required)**
+- should be a valid file path where you would like your responses to be stored.
+sleepyask will create this file for you. If you create this file yourself,
+there might be some problems. #### Optional - `verbose` :: **(optional)** - a
+boolean which specifies whether or not sleepyask should print its progress to
+the console. It is `False` by default - `model` :: **(optional)** - to specify
+which ChatGPT model to use. It is `"gpt-3.5-turbo"` by default - `system_text`
+:: **(optional)** - to specify system text. It is ` - `temperature` :: **
+(optional)** - to specify how deterministic ChatGPT's responses are. Ranges
+from `0-2` where higher numbers represent increased randomness. It is `1` by
+default. - `max_tokens` :: **(optional)** - to specify the maximum number of
+tokens in ChatGPT's response. This is `2048` by default ## ð¬ Get involved -
+ð **Found a bug or interested in adding a feature?** - Create an [issue]
+[issue] - ð¤ **Want to help?** - Create a pull-request! [issue]: https://
+github.com/hwelsters/sleepyask/issues
```

