# Comparing `tmp/kami_messenger-0.1.0.tar.gz` & `tmp/kami_messenger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kami_messenger-0.1.0.tar", max compression
+gzip compressed data, was "kami_messenger-0.2.0.tar", max compression
```

## Comparing `kami_messenger-0.1.0.tar` & `kami_messenger-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    35149 2023-03-13 16:03:45.862136 kami_messenger-0.1.0/LICENSE
--rw-r--r--   0        0        0     4650 2023-03-19 05:35:50.210163 kami_messenger-0.1.0/README.md
--rw-r--r--   0        0        0      217 2023-03-19 04:09:19.232696 kami_messenger-0.1.0/kami_messenger/__init__.py
--rw-r--r--   0        0        0       64 2023-03-19 04:09:19.232696 kami_messenger-0.1.0/kami_messenger/botconversa/__init__.py
--rw-r--r--   0        0        0     2429 2023-03-19 03:42:48.694310 kami_messenger-0.1.0/kami_messenger/botconversa/botconversa.py
--rw-r--r--   0        0        0        0 2023-03-19 03:42:48.694310 kami_messenger-0.1.0/kami_messenger/botconversa/test/__init__.py
--rw-r--r--   0        0        0     1786 2023-03-19 04:09:19.232696 kami_messenger-0.1.0/kami_messenger/botconversa/test/test_botconversa.py
--rw-r--r--   0        0        0      107 2023-03-19 04:09:19.232696 kami_messenger-0.1.0/kami_messenger/contact/__init__.py
--rw-r--r--   0        0        0     1741 2023-03-14 07:58:07.715711 kami_messenger-0.1.0/kami_messenger/contact/contact.py
--rw-r--r--   0        0        0        0 2023-03-13 16:03:45.886136 kami_messenger-0.1.0/kami_messenger/contact/test/__init__.py
--rw-r--r--   0        0        0      629 2023-03-13 16:28:12.863088 kami_messenger-0.1.0/kami_messenger/contact/test/test_contact.py
--rw-r--r--   0        0        0       81 2023-03-19 04:09:19.236696 kami_messenger-0.1.0/kami_messenger/email_messenger/__init__.py
--rw-r--r--   0        0        0     2448 2023-03-19 04:09:19.236696 kami_messenger-0.1.0/kami_messenger/email_messenger/email_messenger.py
--rw-r--r--   0        0        0        0 2023-03-13 16:03:45.902136 kami_messenger-0.1.0/kami_messenger/email_messenger/test/__init__.py
--rw-r--r--   0        0        0     1724 2023-03-14 16:44:44.787426 kami_messenger-0.1.0/kami_messenger/email_messenger/test/test_email.py
--rw-r--r--   0        0        0     1962 2023-03-14 08:00:37.521846 kami_messenger-0.1.0/kami_messenger/kami_messenger.py
--rw-r--r--   0        0        0      139 2023-03-19 04:09:19.236696 kami_messenger-0.1.0/kami_messenger/messenger/__init__.py
--rw-r--r--   0        0        0     5015 2023-03-19 04:09:19.236696 kami_messenger-0.1.0/kami_messenger/messenger/messenger.py
--rw-r--r--   0        0        0        0 2023-03-13 16:03:45.914137 kami_messenger-0.1.0/kami_messenger/messenger/test/__init__.py
--rw-r--r--   0        0        0      659 2023-03-14 07:54:17.168425 kami_messenger-0.1.0/kami_messenger/messenger/test/test_message.py
--rw-r--r--   0        0        0    17687 2023-03-13 16:03:45.930137 kami_messenger-0.1.0/kami_messenger/static/img/icon.png
--rw-r--r--   0        0        0     1911 2023-03-13 16:03:45.938137 kami_messenger-0.1.0/kami_messenger/templates/overdue_weekly.html
--rw-r--r--   0        0        0     1862 2023-03-13 16:03:45.938137 kami_messenger-0.1.0/kami_messenger/templates/sales_montly.html
--rw-r--r--   0        0        0     1906 2023-03-13 16:03:45.942137 kami_messenger-0.1.0/kami_messenger/templates/sales_weekly.html
--rw-r--r--   0        0        0      282 2023-03-19 04:09:19.236696 kami_messenger-0.1.0/kami_messenger/validator/__init__.py
--rw-r--r--   0        0        0      597 2023-03-13 16:28:12.327080 kami_messenger-0.1.0/kami_messenger/validator/custom_html_parser.py
--rw-r--r--   0        0        0        0 2023-03-13 16:03:45.962137 kami_messenger-0.1.0/kami_messenger/validator/test/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 16:03:45.966138 kami_messenger-0.1.0/kami_messenger/validator/test/test_custom_html_parser.py
--rw-r--r--   0        0        0        0 2023-03-13 16:03:45.966138 kami_messenger-0.1.0/kami_messenger/validator/test/test_validator.py
--rw-r--r--   0        0        0     2403 2023-03-19 03:42:48.694310 kami_messenger-0.1.0/kami_messenger/validator/validator.py
--rw-r--r--   0        0        0       31 2023-03-19 03:42:48.694310 kami_messenger-0.1.0/kami_messenger/whatsapp/__init__.py
--rw-r--r--   0        0        0        0 2023-03-19 03:42:48.694310 kami_messenger-0.1.0/kami_messenger/whatsapp/tests/__init__.py
--rw-r--r--   0        0        0     1710 2023-03-19 04:09:19.236696 kami_messenger-0.1.0/kami_messenger/whatsapp/tests/test_whatsapp.py
--rw-r--r--   0        0        0     2355 2023-03-19 03:42:48.694310 kami_messenger-0.1.0/kami_messenger/whatsapp/whatsapp.py
--rw-r--r--   0        0        0     1174 2023-03-19 03:35:09.535802 kami_messenger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5196 1970-01-01 00:00:00.000000 kami_messenger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 07:22:43.455976 kami_messenger-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4550 2023-04-12 21:21:58.803352 kami_messenger-0.2.0/README.md
+-rw-r--r--   0        0        0      217 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/botconversa/__init__.py
+-rw-r--r--   0        0        0     4462 2023-04-12 18:15:04.107703 kami_messenger-0.2.0/kami_messenger/botconversa/botconversa.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/botconversa/test/__init__.py
+-rw-r--r--   0        0        0     1268 2023-04-12 18:39:57.659656 kami_messenger-0.2.0/kami_messenger/botconversa/test/test_botconversa.py
+-rw-r--r--   0        0        0      107 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/contact/__init__.py
+-rw-r--r--   0        0        0     1741 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/contact/contact.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/contact/test/__init__.py
+-rw-r--r--   0        0        0      629 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/contact/test/test_contact.py
+-rw-r--r--   0        0        0       81 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/email_messenger/__init__.py
+-rw-r--r--   0        0        0     2448 2023-04-12 17:21:13.963804 kami_messenger-0.2.0/kami_messenger/email_messenger/email_messenger.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/email_messenger/test/__init__.py
+-rw-r--r--   0        0        0     1823 2023-04-12 18:39:57.475656 kami_messenger-0.2.0/kami_messenger/email_messenger/test/test_email.py
+-rw-r--r--   0        0        0     1962 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/kami_messenger.py
+-rw-r--r--   0        0        0      208 2023-04-12 17:31:49.731784 kami_messenger-0.2.0/kami_messenger/messenger/__init__.py
+-rw-r--r--   0        0        0     5312 2023-04-12 21:29:04.435339 kami_messenger-0.2.0/kami_messenger/messenger/messenger.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/messenger/test/__init__.py
+-rw-r--r--   0        0        0      682 2023-04-12 17:31:49.731784 kami_messenger-0.2.0/kami_messenger/messenger/test/test_message.py
+-rw-r--r--   0        0        0    17687 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/static/img/icon.png
+-rw-r--r--   0        0        0     1911 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/templates/overdue_weekly.html
+-rw-r--r--   0        0        0     1862 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/templates/sales_montly.html
+-rw-r--r--   0        0        0     1906 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/templates/sales_weekly.html
+-rw-r--r--   0        0        0      282 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/validator/__init__.py
+-rw-r--r--   0        0        0      597 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/validator/custom_html_parser.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/validator/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/validator/test/test_custom_html_parser.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/validator/test/test_validator.py
+-rw-r--r--   0        0        0     2875 2023-04-12 18:13:02.375707 kami_messenger-0.2.0/kami_messenger/validator/validator.py
+-rw-r--r--   0        0        0       31 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/whatsapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/whatsapp/tests/__init__.py
+-rw-r--r--   0        0        0     1783 2023-04-12 17:31:49.731784 kami_messenger-0.2.0/kami_messenger/whatsapp/tests/test_whatsapp.py
+-rw-r--r--   0        0        0     2355 2023-04-10 07:22:43.459976 kami_messenger-0.2.0/kami_messenger/whatsapp/whatsapp.py
+-rw-r--r--   0        0        0     1632 2023-04-12 21:34:57.603328 kami_messenger-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5638 1970-01-01 00:00:00.000000 kami_messenger-0.2.0/PKG-INFO
```

### Comparing `kami_messenger-0.1.0/LICENSE` & `kami_messenger-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/README.md` & `kami_messenger-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 <h3 align="center">Kami Messenger</h3>
 
 <div align="center">
 
 [![GitHub release](https://img.shields.io/github/release/devkami/kami-messenger.svg)](https://GitHub.com/devkami/kami-messenger/releases/)
 [![GitHub issues](https://badgen.net/github/issues/devkami/kami-messenger/)](https://github.com/devkami/kami-messenger/issues/)
 [![License](https://img.shields.io/badge/License-GNU-blue)](/LICENSE)
-
+[![Documentation Status](https://readthedocs.org/projects/kami-messenger/badge/?version=latest)](https://kami-messenger.readthedocs.io/en/latest/?badge=latest)
+![CI](https://github.com/devkami/kami-messenger/actions/workflows/pipeline.yml/badge.svg)
 
 </div>
 
 ---
 
 <p align="center"> Aggregator of Digital Channels For Sending Messages
     <br> 
@@ -49,20 +50,16 @@
 ### Prerequisites
 
 To run this package you only need a [python 3.x](https://www.python.org/downloads/) compiler and [poetry](https://python-poetry.org/) on your dev enviroment.
 
 
 ### Installing
 
-If you still don't have poetry installed in your development environment follow [this tutorial](https://python-poetry.org/docs/#installation) and install the latest version
-
-After the repository has already been cloned to your local development environment, it's time to install the project's dependencies using the command below in the root of the project
-
 ```bash
-poetry install
+pip install kami-messenger
 ```
 
 Then, after installing the dependencies, just activate the development environment with the following command:
 
 ```bash
 poetry shell
 ```
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
                                 [Project logo]
                            **** Kami Messenger ****
     [![GitHub release](https://img.shields.io/github/release/devkami/kami-
 messenger.svg)](https://GitHub.com/devkami/kami-messenger/releases/) [![GitHub
   issues](https://badgen.net/github/issues/devkami/kami-messenger/)](https://
 github.com/devkami/kami-messenger/issues/) [![License](https://img.shields.io/
-                      badge/License-GNU-blue)](/LICENSE)
+     badge/License-GNU-blue)](/LICENSE) [![Documentation Status](https://
+ readthedocs.org/projects/kami-messenger/badge/?version=latest)](https://kami-
+  messenger.readthedocs.io/en/latest/?badge=latest) ![CI](https://github.com/
+       devkami/kami-messenger/actions/workflows/pipeline.yml/badge.svg)
 ---
              Aggregator of Digital Channels For Sending Messages
 ## ð Table of Contents - [About](#about) - [Getting Started]
 (#getting_started) - [Deployment](#deployment) - [Usage](#usage) - [Built
 Using](#built_using) - [TODO](../TODO.md) - [Contributing](../CONTRIBUTING.md)
 - [Authors](#authors) - [Acknowledgments](#acknowledgement) ## ð§ About  Kami
 Messenger is a tool for aggregating several messaging platforms into a single
@@ -18,40 +21,36 @@
 addresses for different messaging platforms); - Messenger(An object that
 instantiates, connects, and provides message push service of a specific
 platform) ## ð Getting Started  These instructions will get you a copy of
 the project up and running on your local machine for development and testing
 purposes. See [deployment](#deployment) for notes on how to deploy the project
 on a live system. ### Prerequisites To run this package you only need a [python
 3.x](https://www.python.org/downloads/) compiler and [poetry](https://python-
-poetry.org/) on your dev enviroment. ### Installing If you still don't have
-poetry installed in your development environment follow [this tutorial](https:/
-/python-poetry.org/docs/#installation) and install the latest version After the
-repository has already been cloned to your local development environment, it's
-time to install the project's dependencies using the command below in the root
-of the project ```bash poetry install ``` Then, after installing the
-dependencies, just activate the development environment with the following
-command: ```bash poetry shell ``` Ready now you start developing and testing!
-## ð§ Running the tests  The project already has some of the main unit tests
-for each of the entities present in the code, but you can add your own tests in
-the respective directories 'test' of each entity. ### Break down into end to
-end tests Each entity has its own tests folder with the most elementary unit
-tests and to run them just run the command below in the entity folder you want
-to test or in the root folder to test all project codes ```terminal task test
-``` >Note that when executing this command, before actually testing the code, a
-code review will be performed using the lint-review task and after the
-execution of the test, an html file with the full coverage of the test will be
-available in the htmlcov folder created in the folder where the command was
-run. was executed ### And coding style tests In addition, the project already
-has automated tasks for review and correcting the code style following pep8
-standards To just review the code run the command below in the folder you want
-to analyze: ```terminal task lint-review ``` If you want to automatically
-review and correct the code, run this command in the desired directory
-```terminal task lint-fix ``` ## ð Usage  Add notes about how to use the
-system. ## ð Deployment  Add additional notes about how to deploy this on a
-live system. ## âï¸ Built Using  - [Python 3.x](https://www.python.org/
-downloads/) - [Python email built-in lib](https://docs.python.org/3/library/
-email.examples.html) ## âï¸ Authors  - [@maicondmenezes](https://github.com/
-maicondmenezes) - Idea & Initial work See also the list of [contributors]
-(https://github.com/devkami/kami_messenger/contributors) who participated in
-this project. ## ð Acknowledgements  - The main references for this project
-can be found in the Python topic of [this repository](https://github.com/
-devkami/kami_wiki/blob/main/python_estudies.md)
+poetry.org/) on your dev enviroment. ### Installing ```bash pip install kami-
+messenger ``` Then, after installing the dependencies, just activate the
+development environment with the following command: ```bash poetry shell ```
+Ready now you start developing and testing! ## ð§ Running the tests  The
+project already has some of the main unit tests for each of the entities
+present in the code, but you can add your own tests in the respective
+directories 'test' of each entity. ### Break down into end to end tests Each
+entity has its own tests folder with the most elementary unit tests and to run
+them just run the command below in the entity folder you want to test or in the
+root folder to test all project codes ```terminal task test ``` >Note that when
+executing this command, before actually testing the code, a code review will be
+performed using the lint-review task and after the execution of the test, an
+html file with the full coverage of the test will be available in the htmlcov
+folder created in the folder where the command was run. was executed ### And
+coding style tests In addition, the project already has automated tasks for
+review and correcting the code style following pep8 standards To just review
+the code run the command below in the folder you want to analyze: ```terminal
+task lint-review ``` If you want to automatically review and correct the code,
+run this command in the desired directory ```terminal task lint-fix ``` ## ð
+Usage  Add notes about how to use the system. ## ð Deployment  Add
+additional notes about how to deploy this on a live system. ## âï¸ Built
+Using  - [Python 3.x](https://www.python.org/downloads/) - [Python email built-
+in lib](https://docs.python.org/3/library/email.examples.html) ## âï¸
+Authors  - [@maicondmenezes](https://github.com/maicondmenezes) - Idea &
+Initial work See also the list of [contributors](https://github.com/devkami/
+kami_messenger/contributors) who participated in this project. ## ð
+Acknowledgements  - The main references for this project can be found in the
+Python topic of [this repository](https://github.com/devkami/kami_wiki/blob/
+main/python_estudies.md)
```

### Comparing `kami_messenger-0.1.0/kami_messenger/botconversa/test/test_botconversa.py` & `kami_messenger-0.2.0/kami_messenger/botconversa/test/test_botconversa.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,40 @@
 # -*- coding: utf-8 -*-
 import json
-from os import getenv
 
 from dotenv import load_dotenv
+from pytest import mark
 
 from kami_messenger.botconversa import Botconversa
 
 load_dotenv()
 
 
+@mark.skip(reason='Defined but not implemented')
 class TestBotconversa:
     data = f"""{{
       "name":"Botconversa",
       "messages":[{{
-          "sender":"124707269",
-          "recipients":["124707269"],
+          "sender":"+5511916654692",
+          "recipients":["+5521983144824"],
           "subject":"Teste",
-          "body":"<p>Teste de mensagem</p>"
-        }}],
-      "credentials":{{" implementar o dicionário das credenciais necessárias para acessar o botconversa usando getenv() para proteção dos dados ": "valor"}},
+          "body":"<p>Teste de mensagem</p>",
+          "type":"text"
+          }}],          
+      "credentials":{{"api-key": "b6ba8d5c-19a1-4c38-8f5b-3966f11f2bbe"}},
       "engine":null
     }}"""
 
     def test_when_email_get_valid_json_data_then_returns_new_botconversa_messenger(
         self,
     ):
         json_data = json.loads(self.data)
         new_botconversa_messenger = Botconversa(**json_data)
         assert json_data == new_botconversa_messenger.dict()
 
-    def test_when_botconversa_sucess_connect_should_returns_200(self):
-        json_data = json.loads(self.data)
-        new_botconversa_messenger = Botconversa(**json_data)
-        status = new_botconversa_messenger.connect()
-
-        assert status == 200
-
-    def test_when_connect_botconversa_should_update_engine(self):
-        json_data = json.loads(self.data)
-        new_botconversa_messenger = Botconversa(**json_data)
-        new_botconversa_messenger.connect()
-
-        assert new_botconversa_messenger.engine != None
-
     def test_when_send_message_by_botconversa_should_return_sent_messages_quantity(
         self,
     ):
         json_data = json.loads(self.data)
         new_botconversa_messenger = Botconversa(**json_data)
         messages_to_send = len(new_botconversa_messenger.messages)
         sent_messages = new_botconversa_messenger.sendMessage()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kami_messenger-0.1.0/kami_messenger/contact/contact.py` & `kami_messenger-0.2.0/kami_messenger/contact/contact.py`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/contact/test/test_contact.py` & `kami_messenger-0.2.0/kami_messenger/contact/test/test_contact.py`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/email_messenger/email_messenger.py` & `kami_messenger-0.2.0/kami_messenger/email_messenger/email_messenger.py`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/email_messenger/test/test_email.py` & `kami_messenger-0.2.0/kami_messenger/email_messenger/test/test_email.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 from pytest import mark
 
 from kami_messenger.email_messenger import EmailMessenger
 
 load_dotenv()
 
 
+@mark.skip(reason='Needs to create fixtures to test without real values')
 class TestEmailMessenger:
     data = f"""{{
       "name":"Gmail",
       "messages":[{{
           "sender":"dev@kamico.com.br",
           "recipients":["maicon@kamico.com.br"],
           "subject":"Teste",
-          "body":"<p>Teste de mensagem</p>"
+          "body":"<p>Teste de mensagem</p>",
+          "type":"text"
         }}],
       "credentials":{{
           "login":"{getenv("EMAIL_USER")}",
           "password":"{getenv("EMAIL_PASSWORD")}"
       }},
       "engine":""
     }}"""
```

### Comparing `kami_messenger-0.1.0/kami_messenger/kami_messenger.py` & `kami_messenger-0.2.0/kami_messenger/kami_messenger.py`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/messenger/messenger.py` & `kami_messenger-0.2.0/kami_messenger/messenger/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,23 @@
 
     def __init__(self, value: str, message: str) -> None:
         self.value = value
         self.message = message
         super().__init__(message)
 
 
+class MessageNotSendError(Exception):
+    """Custom error that is raised when a message is not sended to a recipient."""
+
+    def __init__(self, value: str, message: str) -> None:
+        self.value = value
+        self.message = message
+        super().__init__(message)
+
+
 class Message(BaseModel):
     """
     Represents a generic message used in all messengers.
 
     Attributes:
         sender: Contact of the sender of the message
         recipients: List of contacts who will receive the message
@@ -40,14 +49,15 @@
         body: message body, content that will be sent to recipients
     """
 
     sender: str
     recipients: List[str]
     subject: Optional[str]
     body: str
+    type: str = 'text'
 
 
 class Messenger(ABC, BaseModel):
     """
     Represents a generic messaging service, used to abstract the characteristics common to all messaging services used in the project.
 
     Attributes:
```

### Comparing `kami_messenger-0.1.0/kami_messenger/messenger/test/test_message.py` & `kami_messenger-0.2.0/kami_messenger/messenger/test/test_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 
 class TestMessage:
     data = """{
         "sender":"dev@kamico.com.br",
         "recipients":["maicon@kamico.com.br"],
         "subject":"Teste",
-        "body":"<p>Teste de mensagem</p>"
+        "body":"<p>Teste de mensagem</p>",
+        "type":"text"
     }"""
 
     def test_when_message_get_valid_json_data_then_returns_new_message(self):
         json_data = json.loads(self.data)
         new_message = Message(**json_data)
         assert json_data == new_message.dict()
```

### Comparing `kami_messenger-0.1.0/kami_messenger/static/img/icon.png` & `kami_messenger-0.2.0/kami_messenger/static/img/icon.png`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/templates/overdue_weekly.html` & `kami_messenger-0.2.0/kami_messenger/templates/overdue_weekly.html`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/templates/sales_montly.html` & `kami_messenger-0.2.0/kami_messenger/templates/sales_montly.html`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/templates/sales_weekly.html` & `kami_messenger-0.2.0/kami_messenger/templates/sales_weekly.html`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/validator/custom_html_parser.py` & `kami_messenger-0.2.0/kami_messenger/validator/custom_html_parser.py`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/kami_messenger/validator/validator.py` & `kami_messenger-0.2.0/kami_messenger/validator/validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import re
+from os import getenv
+from urllib.parse import urljoin
 
 import phonenumbers as phonevalidator
+import requests
+from dotenv import load_dotenv
 
 from .custom_html_parser import MyHTMLParser
 
+load_dotenv()
+
 
 class PhoneFormatError(Exception):
     """Custom error that is raised when a phone number doesn't have the rigth format."""
 
     def __init__(self, value: str, message: str) -> None:
         self.value = value
         self.message = message
@@ -70,9 +76,22 @@
             raise HTMLFormatError(
                 value=self.value, message="It's Not A Valid HTML document."
             )
 
         return True
 
     def _isIdBotconversa(self):
-        # Implementar uma função que verifica se self.value é um id de contato do botconversa válido e caso contrário levanta uma exceção do tipo IdBotconversaMissingError, utilizar os métodos anteriores como exemplo
-        ...
+        api_url = f'https://backend.botconversa.com.br/api/v1/webhook/subscriber/get_by_phone/{self.value}/'
+
+        headers = {
+            'accept': 'application/json',
+            'api-key': getenv('BOTCONVERSA_API_TOKEN'),
+            'Content-Type': 'application/json',
+        }
+        response = requests.get(api_url, headers=headers)
+        if response.status_code < 200 or response.status_code >= 400:
+            raise IdBotconversaMissingError(
+                value=self.value,
+                message="It's Not A Valid IdBotconversa User.",
+            )
+
+        return True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kami_messenger-0.1.0/kami_messenger/whatsapp/tests/test_whatsapp.py` & `kami_messenger-0.2.0/kami_messenger/whatsapp/tests/test_whatsapp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 import json
 from os import getenv
 
 from dotenv import load_dotenv
+from pytest import mark
 
 from kami_messenger.whatsapp import Whatsapp
 
 load_dotenv()
 
 
+@mark.skip(reason='Defined but not implemented')
 class TestWhatsapp:
     data = f"""{{
       "name":"Whatsapp",
       "messages":[{{
           "sender":"",
           "recipients":["21983144824"],
           "subject":"Teste",
```

### Comparing `kami_messenger-0.1.0/kami_messenger/whatsapp/whatsapp.py` & `kami_messenger-0.2.0/kami_messenger/whatsapp/whatsapp.py`

 * *Files identical despite different names*

### Comparing `kami_messenger-0.1.0/PKG-INFO` & `kami_messenger-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 Metadata-Version: 2.1
 Name: kami-messenger
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library to aggregate multiple messengers services
+License: GNU 3.0
 Author: Maicon de Menezes
 Author-email: maicondmenezes@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: Other/Proprietary License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Communications :: Email
+Classifier: Topic :: Communications :: Telephony
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: kami-logging (>=0.2.0,<0.3.0)
 Requires-Dist: phonenumbers (>=8.13.7,<9.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/devkami/kami-messenger/issues
+Project-URL: Docs, https://kami-messenger.readthedocs.io/en/latest/
+Project-URL: Source, https://github.com/devkami/kami-messenger
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="" rel="noopener">
  <img width=200px height=200px src="static/logo/icon.jpg" alt="Project logo"></a>
 </p>
 
 <h3 align="center">Kami Messenger</h3>
 
 <div align="center">
 
 [![GitHub release](https://img.shields.io/github/release/devkami/kami-messenger.svg)](https://GitHub.com/devkami/kami-messenger/releases/)
 [![GitHub issues](https://badgen.net/github/issues/devkami/kami-messenger/)](https://github.com/devkami/kami-messenger/issues/)
 [![License](https://img.shields.io/badge/License-GNU-blue)](/LICENSE)
-
+[![Documentation Status](https://readthedocs.org/projects/kami-messenger/badge/?version=latest)](https://kami-messenger.readthedocs.io/en/latest/?badge=latest)
+![CI](https://github.com/devkami/kami-messenger/actions/workflows/pipeline.yml/badge.svg)
 
 </div>
 
 ---
 
 <p align="center"> Aggregator of Digital Channels For Sending Messages
     <br> 
@@ -67,20 +79,16 @@
 ### Prerequisites
 
 To run this package you only need a [python 3.x](https://www.python.org/downloads/) compiler and [poetry](https://python-poetry.org/) on your dev enviroment.
 
 
 ### Installing
 
-If you still don't have poetry installed in your development environment follow [this tutorial](https://python-poetry.org/docs/#installation) and install the latest version
-
-After the repository has already been cloned to your local development environment, it's time to install the project's dependencies using the command below in the root of the project
-
 ```bash
-poetry install
+pip install kami-messenger
 ```
 
 Then, after installing the dependencies, just activate the development environment with the following command:
 
 ```bash
 poetry shell
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,34 @@
-Metadata-Version: 2.1 Name: kami-messenger Version: 0.1.0 Summary: Library to
-aggregate multiple messengers services Author: Maicon de Menezes Author-email:
-maicondmenezes@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-
+Metadata-Version: 2.1 Name: kami-messenger Version: 0.2.0 Summary: Library to
+aggregate multiple messengers services License: GNU 3.0 Author: Maicon de
+Menezes Author-email: maicondmenezes@gmail.com Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
+Proprietary License Classifier: Natural Language :: English Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 Classifier: Topic :: Communications :: Email Classifier: Topic ::
+Communications :: Telephony Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-
 Dist: kami-logging (>=0.2.0,<0.3.0) Requires-Dist: phonenumbers
 (>=8.13.7,<9.0.0) Requires-Dist: pydantic (>=1.10.6,<2.0.0) Requires-Dist:
-python-dotenv (>=1.0.0,<2.0.0) Description-Content-Type: text/markdown
+python-dotenv (>=1.0.0,<2.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0)
+Project-URL: Bug Tracker, https://github.com/devkami/kami-messenger/issues
+Project-URL: Docs, https://kami-messenger.readthedocs.io/en/latest/ Project-
+URL: Source, https://github.com/devkami/kami-messenger Description-Content-
+Type: text/markdown
                                 [Project logo]
                            **** Kami Messenger ****
     [![GitHub release](https://img.shields.io/github/release/devkami/kami-
 messenger.svg)](https://GitHub.com/devkami/kami-messenger/releases/) [![GitHub
   issues](https://badgen.net/github/issues/devkami/kami-messenger/)](https://
 github.com/devkami/kami-messenger/issues/) [![License](https://img.shields.io/
-                      badge/License-GNU-blue)](/LICENSE)
+     badge/License-GNU-blue)](/LICENSE) [![Documentation Status](https://
+ readthedocs.org/projects/kami-messenger/badge/?version=latest)](https://kami-
+  messenger.readthedocs.io/en/latest/?badge=latest) ![CI](https://github.com/
+       devkami/kami-messenger/actions/workflows/pipeline.yml/badge.svg)
 ---
              Aggregator of Digital Channels For Sending Messages
 ## ð Table of Contents - [About](#about) - [Getting Started]
 (#getting_started) - [Deployment](#deployment) - [Usage](#usage) - [Built
 Using](#built_using) - [TODO](../TODO.md) - [Contributing](../CONTRIBUTING.md)
 - [Authors](#authors) - [Acknowledgments](#acknowledgement) ## ð§ About  Kami
 Messenger is a tool for aggregating several messaging platforms into a single
@@ -27,40 +38,36 @@
 addresses for different messaging platforms); - Messenger(An object that
 instantiates, connects, and provides message push service of a specific
 platform) ## ð Getting Started  These instructions will get you a copy of
 the project up and running on your local machine for development and testing
 purposes. See [deployment](#deployment) for notes on how to deploy the project
 on a live system. ### Prerequisites To run this package you only need a [python
 3.x](https://www.python.org/downloads/) compiler and [poetry](https://python-
-poetry.org/) on your dev enviroment. ### Installing If you still don't have
-poetry installed in your development environment follow [this tutorial](https:/
-/python-poetry.org/docs/#installation) and install the latest version After the
-repository has already been cloned to your local development environment, it's
-time to install the project's dependencies using the command below in the root
-of the project ```bash poetry install ``` Then, after installing the
-dependencies, just activate the development environment with the following
-command: ```bash poetry shell ``` Ready now you start developing and testing!
-## ð§ Running the tests  The project already has some of the main unit tests
-for each of the entities present in the code, but you can add your own tests in
-the respective directories 'test' of each entity. ### Break down into end to
-end tests Each entity has its own tests folder with the most elementary unit
-tests and to run them just run the command below in the entity folder you want
-to test or in the root folder to test all project codes ```terminal task test
-``` >Note that when executing this command, before actually testing the code, a
-code review will be performed using the lint-review task and after the
-execution of the test, an html file with the full coverage of the test will be
-available in the htmlcov folder created in the folder where the command was
-run. was executed ### And coding style tests In addition, the project already
-has automated tasks for review and correcting the code style following pep8
-standards To just review the code run the command below in the folder you want
-to analyze: ```terminal task lint-review ``` If you want to automatically
-review and correct the code, run this command in the desired directory
-```terminal task lint-fix ``` ## ð Usage  Add notes about how to use the
-system. ## ð Deployment  Add additional notes about how to deploy this on a
-live system. ## âï¸ Built Using  - [Python 3.x](https://www.python.org/
-downloads/) - [Python email built-in lib](https://docs.python.org/3/library/
-email.examples.html) ## âï¸ Authors  - [@maicondmenezes](https://github.com/
-maicondmenezes) - Idea & Initial work See also the list of [contributors]
-(https://github.com/devkami/kami_messenger/contributors) who participated in
-this project. ## ð Acknowledgements  - The main references for this project
-can be found in the Python topic of [this repository](https://github.com/
-devkami/kami_wiki/blob/main/python_estudies.md)
+poetry.org/) on your dev enviroment. ### Installing ```bash pip install kami-
+messenger ``` Then, after installing the dependencies, just activate the
+development environment with the following command: ```bash poetry shell ```
+Ready now you start developing and testing! ## ð§ Running the tests  The
+project already has some of the main unit tests for each of the entities
+present in the code, but you can add your own tests in the respective
+directories 'test' of each entity. ### Break down into end to end tests Each
+entity has its own tests folder with the most elementary unit tests and to run
+them just run the command below in the entity folder you want to test or in the
+root folder to test all project codes ```terminal task test ``` >Note that when
+executing this command, before actually testing the code, a code review will be
+performed using the lint-review task and after the execution of the test, an
+html file with the full coverage of the test will be available in the htmlcov
+folder created in the folder where the command was run. was executed ### And
+coding style tests In addition, the project already has automated tasks for
+review and correcting the code style following pep8 standards To just review
+the code run the command below in the folder you want to analyze: ```terminal
+task lint-review ``` If you want to automatically review and correct the code,
+run this command in the desired directory ```terminal task lint-fix ``` ## ð
+Usage  Add notes about how to use the system. ## ð Deployment  Add
+additional notes about how to deploy this on a live system. ## âï¸ Built
+Using  - [Python 3.x](https://www.python.org/downloads/) - [Python email built-
+in lib](https://docs.python.org/3/library/email.examples.html) ## âï¸
+Authors  - [@maicondmenezes](https://github.com/maicondmenezes) - Idea &
+Initial work See also the list of [contributors](https://github.com/devkami/
+kami_messenger/contributors) who participated in this project. ## ð
+Acknowledgements  - The main references for this project can be found in the
+Python topic of [this repository](https://github.com/devkami/kami_wiki/blob/
+main/python_estudies.md)
```

