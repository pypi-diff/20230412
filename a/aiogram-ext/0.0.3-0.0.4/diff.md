# Comparing `tmp/aiogram-ext-0.0.3.tar.gz` & `tmp/aiogram-ext-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.0.3.tar", last modified: Wed Apr 12 10:57:04 2023, max compression
+gzip compressed data, was "aiogram-ext-0.0.4.tar", last modified: Wed Apr 12 11:09:30 2023, max compression
```

## Comparing `aiogram-ext-0.0.3.tar` & `aiogram-ext-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      465 2023-04-12 10:53:39.977438 aiogram-ext-0.0.3/aiogram_ext/__init__.py
--rw-r--r--   0        0        0     6468 2023-04-12 10:34:24.416929 aiogram-ext-0.0.3/aiogram_ext/_currents.py
--rw-r--r--   0        0        0     2291 2023-04-12 10:34:24.385343 aiogram-ext-0.0.3/aiogram_ext/_questions.py
--rw-r--r--   0        0        0     5406 2023-04-11 11:53:07.707408 aiogram-ext-0.0.3/aiogram_ext/_states.py
--rw-r--r--   0        0        0     1170 2023-04-12 10:10:11.862874 aiogram-ext-0.0.3/aiogram_ext/buttons.py
--rw-r--r--   0        0        0     1665 2023-04-11 12:03:57.675683 aiogram-ext-0.0.3/aiogram_ext/context.py
--rw-r--r--   0        0        0     1066 2023-04-12 10:53:39.961747 aiogram-ext-0.0.3/aiogram_ext/deps.py
--rw-r--r--   0        0        0     5382 2023-04-11 12:09:03.428321 aiogram-ext-0.0.3/aiogram_ext/dispatcher.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.3/aiogram_ext/filters.py
--rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.3/aiogram_ext/helpers.py
--rw-r--r--   0        0        0      700 2023-04-12 10:34:05.006090 aiogram-ext-0.0.3/aiogram_ext/keyboards.py
--rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.3/aiogram_ext/middlewares/__init__.py
--rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.3/aiogram_ext/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.3/aiogram_ext/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.3/aiogram_ext/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.3/aiogram_ext/middlewares/throttling.py
--rw-r--r--   0        0        0      300 2023-04-12 10:56:59.665565 aiogram-ext-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.3/README.md
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      465 2023-04-12 10:53:39.977438 aiogram-ext-0.0.4/aiogram_ext/__init__.py
+-rw-r--r--   0        0        0     6468 2023-04-12 10:34:24.416929 aiogram-ext-0.0.4/aiogram_ext/_currents.py
+-rw-r--r--   0        0        0     2291 2023-04-12 10:34:24.385343 aiogram-ext-0.0.4/aiogram_ext/_questions.py
+-rw-r--r--   0        0        0     5406 2023-04-11 11:53:07.707408 aiogram-ext-0.0.4/aiogram_ext/_states.py
+-rw-r--r--   0        0        0     1170 2023-04-12 10:10:11.862874 aiogram-ext-0.0.4/aiogram_ext/buttons.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.4/aiogram_ext/context.py
+-rw-r--r--   0        0        0     1132 2023-04-12 11:08:54.370551 aiogram-ext-0.0.4/aiogram_ext/deps.py
+-rw-r--r--   0        0        0     5887 2023-04-12 11:08:56.310732 aiogram-ext-0.0.4/aiogram_ext/dispatcher.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.4/aiogram_ext/filters.py
+-rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.4/aiogram_ext/helpers.py
+-rw-r--r--   0        0        0      700 2023-04-12 10:34:05.006090 aiogram-ext-0.0.4/aiogram_ext/keyboards.py
+-rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.4/aiogram_ext/middlewares/__init__.py
+-rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.4/aiogram_ext/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.4/aiogram_ext/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.4/aiogram_ext/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.4/aiogram_ext/middlewares/throttling.py
+-rw-r--r--   0        0        0      300 2023-04-12 11:09:27.940421 aiogram-ext-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.4/README.md
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.4/PKG-INFO
```

### Comparing `aiogram-ext-0.0.3/aiogram_ext/_currents.py` & `aiogram-ext-0.0.4/aiogram_ext/_currents.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/_questions.py` & `aiogram-ext-0.0.4/aiogram_ext/_questions.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/_states.py` & `aiogram-ext-0.0.4/aiogram_ext/_states.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/buttons.py` & `aiogram-ext-0.0.4/aiogram_ext/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/context.py` & `aiogram-ext-0.0.4/aiogram_ext/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 from typing import TypeVar
+
 from .deps import (
     ContextInstanceMixin,
     FSMContext,
     Dispatcher,
     Update,
     Message,
     Chat,
     User,
-    CallbackQuery,
+    Query,
     InlineQuery,
     ChosenInlineResult,
     ShippingQuery,
     PreCheckoutQuery,
     Poll,
     PollAnswer,
     ChatMemberUpdated,
@@ -45,15 +46,15 @@
         return super().__getattribute__(item)
 
 
 update = make_context_obj(Update)
 message = make_context_obj(Message)
 chat = make_context_obj(Chat)
 user = make_context_obj(User)
-callback_query = make_context_obj(CallbackQuery)
+callback_query = make_context_obj(Query)
 inline_query = make_context_obj(InlineQuery)
 chosen_inline_result = make_context_obj(ChosenInlineResult)
 shipping_query = make_context_obj(ShippingQuery)
 pre_checkout_query = make_context_obj(PreCheckoutQuery)
 poll = make_context_obj(Poll)
 poll_answer = make_context_obj(PollAnswer)
 chat_member_updated = make_context_obj(ChatMemberUpdated)
```

### Comparing `aiogram-ext-0.0.3/aiogram_ext/deps.py` & `aiogram-ext-0.0.4/aiogram_ext/deps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from copy import deepcopy
 
 from aiogram import Bot, Dispatcher
 from aiogram.dispatcher import FSMContext
+from aiogram.dispatcher.filters.state import State
 from aiogram.types import (
     ReplyKeyboardMarkup,
     InlineKeyboardMarkup,
     InlineKeyboardButton,
     KeyboardButton,
     Update,
     Message,
@@ -44,8 +45,9 @@
     "PreCheckoutQuery",
     "Poll",
     "PollAnswer",
     "ChatMemberUpdated",
     "executor",
     "deepcopy",
     "ReplyKeyboardRemove",
+    "State",
 ]
```

### Comparing `aiogram-ext-0.0.3/aiogram_ext/dispatcher.py` & `aiogram-ext-0.0.4/aiogram_ext/dispatcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 from typing import TypeVar
 
-from .deps import Dispatcher as _Dispatcher, executor
+from .buttons import CallbackButton
+from .deps import Dispatcher as _Dispatcher, executor, State
 from .filters import (
     CallbackQueryButton,
     InlineQueryButton,
     MessageButton,
     StorageDataFilter,
 )
 
@@ -52,29 +53,14 @@
                 self.message_handlers,
                 self.edited_message_handlers,
             ],
         )
 
         super()._setup_filters()
 
-    def run_polling(
-        self,
-        *,
-        loop=None,
-        skip_updates=False,
-        reset_webhook=True,
-        on_startup=None,
-        on_shutdown=None,
-        timeout=20,
-        relax=0.1,
-        fast=True,
-    ):
-        payload = self._gen_payload(locals())
-        executor.start_polling(self, **payload)
-
     def run_webhook(
         self,
         webhook_host,
         webhook_path,
         *,
         skip_updates=None,
         on_startup=None,
@@ -191,7 +177,28 @@
         text_contains=None,
         text_endswith=None,
         run_task=None,
         **kwargs,
     ):
         payload = self._gen_payload(locals(), exclude=["custom_filters"])
         return super().inline_handler(*custom_filters, **payload)
+
+    def command(self, command: str, state: str = None):
+        return self.message_handler(commands=command, state=state)
+
+    def button(self, button: CallbackButton):
+        return self.callback_query_handler(button=button)
+
+    def text(self, text: str = None, state: str | State = None):
+        return self.message_handler(button=text, state=state)
+
+    def contact(self, state: str | State = None):
+        return self.message_handler(content_types="contact", state=state)
+
+    def document(self, state: str | State = None):
+        return self.message_handler(content_types="document", state=state)
+
+    def photo(self, state: str | State = None):
+        return self.message_handler(content_types="photo", state=state)
+
+    def run(self):
+        executor.start_polling(self)
```

### Comparing `aiogram-ext-0.0.3/aiogram_ext/filters.py` & `aiogram-ext-0.0.4/aiogram_ext/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/keyboards.py` & `aiogram-ext-0.0.4/aiogram_ext/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/middlewares/_conversation.py` & `aiogram-ext-0.0.4/aiogram_ext/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/middlewares/_membership.py` & `aiogram-ext-0.0.4/aiogram_ext/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/middlewares/misc.py` & `aiogram-ext-0.0.4/aiogram_ext/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.3/aiogram_ext/middlewares/throttling.py` & `aiogram-ext-0.0.4/aiogram_ext/middlewares/throttling.py`

 * *Files identical despite different names*

