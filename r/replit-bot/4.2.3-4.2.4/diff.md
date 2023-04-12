# Comparing `tmp/replit-bot-4.2.3.tar.gz` & `tmp/replit-bot-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit-bot-4.2.3.tar", max compression
+gzip compressed data, was "replit-bot-4.2.4.tar", max compression
```

## Comparing `replit-bot-4.2.3.tar` & `replit-bot-4.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.3/LICENSE
--rw-r--r--   0        0        0      822 2023-04-11 18:24:41.452411 replit-bot-4.2.3/pyproject.toml
--rw-r--r--   0        0        0    35477 2023-04-11 18:25:13.346789 replit-bot-4.2.3/replit_bot/AsyncBot.py
--rw-r--r--   0        0        0    50177 2023-04-11 18:25:00.917862 replit-bot-4.2.3/replit_bot/AsyncClient.py
--rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.3/replit_bot/AsyncPost_ql.py
--rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.3/replit_bot/LICENSE
--rw-r--r--   0        0        0      292 2023-04-11 18:24:38.508192 replit-bot-4.2.3/replit_bot/__init__.py
--rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.3/replit_bot/bot.py
--rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.3/replit_bot/client.py
--rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.3/replit_bot/colors.py
--rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.3/replit_bot/exceptions.py
--rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.3/replit_bot/html_default_templates.py
--rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.3/replit_bot/links.py
--rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.3/replit_bot/param.py
--rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.3/replit_bot/post_ql.py
--rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.3/replit_bot/queries.js
--rw-r--r--   0        0        0    66318 2023-04-09 17:33:34.445917 replit-bot-4.2.3/replit_bot/queries.py
--rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.3/replit_bot/templates/index.html
--rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.3/replit_bot/utils/EventEmitter.py
--rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.3/replit_bot/utils/JSDict.py
--rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.3/replit_bot/utils/_uuid.py
--rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.3/replit_bot/utils/lines.py
--rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.3/replit_bot/utils/switch.py
--rw-r--r--   0        0        0      823 2023-04-11 18:25:17.754156 replit-bot-4.2.3/setup.py
--rw-r--r--   0        0        0      674 2023-04-11 18:25:17.754523 replit-bot-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-03-18 03:10:39.175601 replit-bot-4.2.4/LICENSE
+-rw-r--r--   0        0        0      858 2023-04-12 02:20:19.691873 replit-bot-4.2.4/pyproject.toml
+-rw-r--r--   0        0        0    35555 2023-04-12 02:20:29.103860 replit-bot-4.2.4/replit_bot/AsyncBot.py
+-rw-r--r--   0        0        0    50369 2023-04-12 02:20:29.827859 replit-bot-4.2.4/replit_bot/AsyncClient.py
+-rw-r--r--   0        0        0     4849 2023-03-27 19:47:43.541064 replit-bot-4.2.4/replit_bot/AsyncPost_ql.py
+-rw-r--r--   0        0        0     1052 2022-09-27 15:16:43.952285 replit-bot-4.2.4/replit_bot/LICENSE
+-rw-r--r--   0        0        0      292 2023-04-12 02:20:13.555882 replit-bot-4.2.4/replit_bot/__init__.py
+-rw-r--r--   0        0        0    18869 2023-03-28 03:01:12.062609 replit-bot-4.2.4/replit_bot/bot.py
+-rw-r--r--   0        0        0    40595 2023-03-27 04:53:44.611007 replit-bot-4.2.4/replit_bot/client.py
+-rw-r--r--   0        0        0      402 2022-10-16 23:52:32.225067 replit-bot-4.2.4/replit_bot/colors.py
+-rw-r--r--   0        0        0      417 2022-10-31 16:25:47.277382 replit-bot-4.2.4/replit_bot/exceptions.py
+-rw-r--r--   0        0        0      978 2023-03-28 14:54:09.153939 replit-bot-4.2.4/replit_bot/html_default_templates.py
+-rw-r--r--   0        0        0      337 2022-11-01 05:08:17.261306 replit-bot-4.2.4/replit_bot/links.py
+-rw-r--r--   0        0        0     1079 2023-03-18 17:19:56.099076 replit-bot-4.2.4/replit_bot/param.py
+-rw-r--r--   0        0        0     4622 2023-03-17 18:28:40.859392 replit-bot-4.2.4/replit_bot/post_ql.py
+-rw-r--r--   0        0        0    33930 2022-12-04 18:15:07.036375 replit-bot-4.2.4/replit_bot/queries.js
+-rw-r--r--   0        0        0    66619 2023-04-12 02:20:28.443861 replit-bot-4.2.4/replit_bot/queries.py
+-rw-r--r--   0        0        0      392 2022-10-25 21:03:02.210745 replit-bot-4.2.4/replit_bot/templates/index.html
+-rw-r--r--   0        0        0     4592 2023-03-17 18:28:40.863392 replit-bot-4.2.4/replit_bot/utils/EventEmitter.py
+-rw-r--r--   0        0        0      323 2022-10-17 16:19:01.766353 replit-bot-4.2.4/replit_bot/utils/JSDict.py
+-rw-r--r--   0        0        0      333 2022-09-29 01:59:37.161531 replit-bot-4.2.4/replit_bot/utils/_uuid.py
+-rw-r--r--   0        0        0     1055 2022-11-30 23:00:18.573144 replit-bot-4.2.4/replit_bot/utils/lines.py
+-rw-r--r--   0        0        0      172 2022-10-17 16:19:01.778353 replit-bot-4.2.4/replit_bot/utils/switch.py
+-rw-r--r--   0        0        0      879 2023-04-12 02:20:31.351770 replit-bot-4.2.4/setup.py
+-rw-r--r--   0        0        0      758 2023-04-12 02:20:31.352069 replit-bot-4.2.4/PKG-INFO
```

### Comparing `replit-bot-4.2.3/LICENSE` & `replit-bot-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/pyproject.toml` & `replit-bot-4.2.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "replit-bot"
-version = "4.2.3"
+version = "4.2.4"
 description = "make discord.py like bots on replit and/or do replapi-it style replit interactions"
 authors = ["bigminboss <you@example.com>"]
 
 [tool.poetry.dependencies]
 # python ver
 python = ">=3.6.1,<4.0.0"
 # replit db I think I can't remember lol
@@ -19,14 +19,16 @@
 # docs
 # [tool.poetry.group.docs]
 # optional = true
 
 # [tool.poetry.group.docs.dependencies]
 Flask = "^2.2.0"
 waitress = "^2.1.2"
+quart="^0.18.4"
+hypercorn="^0.14.3"
 
 [tool.poetry.dev-dependencies]
 debugpy = "^1.6.2"
 python-lsp-server = {extras = ["yapf", "rope", "pyflakes"], version = "^1.5.0"}
 toml = "^0.10.2"
 Markdown = "^3.4.1"
```

### Comparing `replit-bot-4.2.3/replit_bot/AsyncBot.py` & `replit-bot-4.2.4/replit_bot/AsyncBot.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     HTML_LIST,
     BLOCKQUOTE,
     TEMPLATE,
 )
 from typing import Callable as Function, Any, Dict, Tuple, get_type_hints, List
 from flask import Flask, render_template_string, request
 from waitress import serve
+
+# from hypercorn.config import Config
+# from hypercorn.asyncio import serve
 from threading import Thread
 from time import sleep
 from .param import Param
 from .exceptions import NamesMustBeAlphanumeric, MustBeRunOnReplitForButtons
 from .utils._uuid import random_characters
 from .post_ql import post
 from .colors import green, blue, purple, red, end, bold_green, bold_blue
@@ -826,9 +829,10 @@
 
         if flask_app is not None:
             Thread(
                 target=serve,
                 kwargs={"app": flask_app, "host": "0.0.0.0", "port": 8080},
                 daemon=daemon,
             ).start()
+
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self.user.notifications.startEvents())
```

### Comparing `replit-bot-4.2.3/replit_bot/AsyncClient.py` & `replit-bot-4.2.4/replit_bot/AsyncClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1404,7 +1404,13 @@
             return None
         comment = Comment(self.c)
         await comment.update(res["createReplCommentReply"])
         if options.cache:
             if comment.id != None:
                 self.c.comments.cache[comment.id] = comment
         return comment
+
+    async def edit(self, body: str):
+        """edit comment"""
+        await self.c.gql("editComment", {"input": {"id": self.id, "body": body}})
+        self.body = body
+        return self
```

### Comparing `replit-bot-4.2.3/replit_bot/AsyncPost_ql.py` & `replit-bot-4.2.4/replit_bot/AsyncPost_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/LICENSE` & `replit-bot-4.2.4/replit_bot/LICENSE`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/bot.py` & `replit-bot-4.2.4/replit_bot/bot.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/client.py` & `replit-bot-4.2.4/replit_bot/client.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/html_default_templates.py` & `replit-bot-4.2.4/replit_bot/html_default_templates.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/param.py` & `replit-bot-4.2.4/replit_bot/param.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/post_ql.py` & `replit-bot-4.2.4/replit_bot/post_ql.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/queries.js` & `replit-bot-4.2.4/replit_bot/queries.js`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/queries.py` & `replit-bot-4.2.4/replit_bot/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,15 @@
     }
   }
 }
 
 fragment ReplsDashboardReplItemRepl on Repl {
   id
 }""",
+    "editComment": "mutation ReplViewCommentsUpdateReplComment($input: UpdateReplCommentInput!) {\n  updateReplComment(input: $input) {\n    ... on ReplComment {\n      id\n      body\n      __typename\n    }\n    ... on UserError {\n      message\n      __typename\n    }\n    __typename\n  }\n}\n",
 }
 
 """
 import { GraphQL } from '@rayhanadev/replit-gql';
 import gql from 'graphql-tag';
 import * as fs from 'fs';
 const client = GraphQL()
```

### Comparing `replit-bot-4.2.3/replit_bot/utils/EventEmitter.py` & `replit-bot-4.2.4/replit_bot/utils/EventEmitter.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/replit_bot/utils/lines.py` & `replit-bot-4.2.4/replit_bot/utils/lines.py`

 * *Files identical despite different names*

### Comparing `replit-bot-4.2.3/setup.py` & `replit-bot-4.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 ['replit_bot', 'replit_bot.utils']
 
 package_data = \
 {'': ['*'], 'replit_bot': ['templates/*']}
 
 install_requires = \
 ['Flask>=2.2.0,<3.0.0',
+ 'hypercorn>=0.14.3,<0.15.0',
  'pyee>=9.0.4,<10.0.0',
+ 'quart>=0.18.4,<0.19.0',
  'replit>=3.2.4,<4.0.0',
  'requests>=2.28.1,<3.0.0',
  'waitress>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'replit-bot',
-    'version': '4.2.3',
+    'version': '4.2.4',
     'description': 'make discord.py like bots on replit and/or do replapi-it style replit interactions',
     'long_description': None,
     'author': 'bigminboss',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `replit-bot-4.2.3/PKG-INFO` & `replit-bot-4.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: replit-bot
-Version: 4.2.3
+Version: 4.2.4
 Summary: make discord.py like bots on replit and/or do replapi-it style replit interactions
 Author: bigminboss
 Author-email: you@example.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.2.0,<3.0.0)
+Requires-Dist: hypercorn (>=0.14.3,<0.15.0)
 Requires-Dist: pyee (>=9.0.4,<10.0.0)
+Requires-Dist: quart (>=0.18.4,<0.19.0)
 Requires-Dist: replit (>=3.2.4,<4.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: waitress (>=2.1.2,<3.0.0)
```

