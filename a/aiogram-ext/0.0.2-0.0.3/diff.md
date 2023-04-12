# Comparing `tmp/aiogram-ext-0.0.2.tar.gz` & `tmp/aiogram-ext-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.0.2.tar", last modified: Wed Apr 12 10:34:49 2023, max compression
+gzip compressed data, was "aiogram-ext-0.0.3.tar", last modified: Wed Apr 12 10:57:04 2023, max compression
```

## Comparing `aiogram-ext-0.0.2.tar` & `aiogram-ext-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      392 2023-04-12 10:10:11.929473 aiogram-ext-0.0.2/aiogram_ext/__init__.py
--rw-r--r--   0        0        0     3007 2023-04-11 11:53:07.691383 aiogram-ext-0.0.2/aiogram_ext/_bot.py
--rw-r--r--   0        0        0     6468 2023-04-12 10:34:24.416929 aiogram-ext-0.0.2/aiogram_ext/_currents.py
--rw-r--r--   0        0        0     2099 2023-04-11 11:53:07.649026 aiogram-ext-0.0.2/aiogram_ext/_models.py
--rw-r--r--   0        0        0     2291 2023-04-12 10:34:24.385343 aiogram-ext-0.0.2/aiogram_ext/_questions.py
--rw-r--r--   0        0        0     5406 2023-04-11 11:53:07.707408 aiogram-ext-0.0.2/aiogram_ext/_states.py
--rw-r--r--   0        0        0     1170 2023-04-12 10:10:11.862874 aiogram-ext-0.0.2/aiogram_ext/buttons.py
--rw-r--r--   0        0        0     1665 2023-04-11 12:03:57.675683 aiogram-ext-0.0.2/aiogram_ext/context.py
--rw-r--r--   0        0        0     1009 2023-04-12 10:10:11.908271 aiogram-ext-0.0.2/aiogram_ext/deps.py
--rw-r--r--   0        0        0     5382 2023-04-11 12:09:03.428321 aiogram-ext-0.0.2/aiogram_ext/dispatcher.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.2/aiogram_ext/filters.py
--rw-r--r--   0        0        0      700 2023-04-12 10:34:05.006090 aiogram-ext-0.0.2/aiogram_ext/keyboards.py
--rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.2/aiogram_ext/middlewares/__init__.py
--rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.2/aiogram_ext/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.2/aiogram_ext/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.2/aiogram_ext/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.2/aiogram_ext/middlewares/throttling.py
--rw-r--r--   0        0        0      300 2023-04-12 10:34:42.485684 aiogram-ext-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.2/README.md
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      465 2023-04-12 10:53:39.977438 aiogram-ext-0.0.3/aiogram_ext/__init__.py
+-rw-r--r--   0        0        0     6468 2023-04-12 10:34:24.416929 aiogram-ext-0.0.3/aiogram_ext/_currents.py
+-rw-r--r--   0        0        0     2291 2023-04-12 10:34:24.385343 aiogram-ext-0.0.3/aiogram_ext/_questions.py
+-rw-r--r--   0        0        0     5406 2023-04-11 11:53:07.707408 aiogram-ext-0.0.3/aiogram_ext/_states.py
+-rw-r--r--   0        0        0     1170 2023-04-12 10:10:11.862874 aiogram-ext-0.0.3/aiogram_ext/buttons.py
+-rw-r--r--   0        0        0     1665 2023-04-11 12:03:57.675683 aiogram-ext-0.0.3/aiogram_ext/context.py
+-rw-r--r--   0        0        0     1066 2023-04-12 10:53:39.961747 aiogram-ext-0.0.3/aiogram_ext/deps.py
+-rw-r--r--   0        0        0     5382 2023-04-11 12:09:03.428321 aiogram-ext-0.0.3/aiogram_ext/dispatcher.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.3/aiogram_ext/filters.py
+-rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.3/aiogram_ext/helpers.py
+-rw-r--r--   0        0        0      700 2023-04-12 10:34:05.006090 aiogram-ext-0.0.3/aiogram_ext/keyboards.py
+-rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.3/aiogram_ext/middlewares/__init__.py
+-rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.3/aiogram_ext/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.3/aiogram_ext/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.3/aiogram_ext/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.3/aiogram_ext/middlewares/throttling.py
+-rw-r--r--   0        0        0      300 2023-04-12 10:56:59.665565 aiogram-ext-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.3/README.md
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.3/PKG-INFO
```

### Comparing `aiogram-ext-0.0.2/aiogram_ext/_currents.py` & `aiogram-ext-0.0.3/aiogram_ext/_currents.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/_questions.py` & `aiogram-ext-0.0.3/aiogram_ext/_questions.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/_states.py` & `aiogram-ext-0.0.3/aiogram_ext/_states.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/buttons.py` & `aiogram-ext-0.0.3/aiogram_ext/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/context.py` & `aiogram-ext-0.0.3/aiogram_ext/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/deps.py` & `aiogram-ext-0.0.3/aiogram_ext/deps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,51 @@
+from copy import deepcopy
+
 from aiogram import Bot, Dispatcher
 from aiogram.dispatcher import FSMContext
 from aiogram.types import (
     ReplyKeyboardMarkup,
     InlineKeyboardMarkup,
     InlineKeyboardButton,
     KeyboardButton,
     Update,
     Message,
     Chat,
     User,
-    CallbackQuery,
+    CallbackQuery as Query,
     InlineQuery,
     ChosenInlineResult,
     ShippingQuery,
     PreCheckoutQuery,
     Poll,
     PollAnswer,
     ChatMemberUpdated,
+    ReplyKeyboardRemove,
 )
-from aiogram.utils.mixins import ContextInstanceMixin
 from aiogram.utils import executor
-from copy import deepcopy
+from aiogram.utils.mixins import ContextInstanceMixin
 
 __all__ = [
     "ReplyKeyboardMarkup",
     "InlineKeyboardMarkup",
     "InlineKeyboardButton",
     "KeyboardButton",
     "Bot",
     "Dispatcher",
     "FSMContext",
     "ContextInstanceMixin",
     "Update",
     "Message",
     "Chat",
     "User",
-    "CallbackQuery",
+    "Query",
     "InlineQuery",
     "ChosenInlineResult",
     "ShippingQuery",
     "PreCheckoutQuery",
     "Poll",
     "PollAnswer",
     "ChatMemberUpdated",
     "executor",
     "deepcopy",
+    "ReplyKeyboardRemove",
 ]
```

### Comparing `aiogram-ext-0.0.2/aiogram_ext/dispatcher.py` & `aiogram-ext-0.0.3/aiogram_ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/filters.py` & `aiogram-ext-0.0.3/aiogram_ext/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/keyboards.py` & `aiogram-ext-0.0.3/aiogram_ext/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/middlewares/_conversation.py` & `aiogram-ext-0.0.3/aiogram_ext/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/middlewares/_membership.py` & `aiogram-ext-0.0.3/aiogram_ext/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/middlewares/misc.py` & `aiogram-ext-0.0.3/aiogram_ext/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.2/aiogram_ext/middlewares/throttling.py` & `aiogram-ext-0.0.3/aiogram_ext/middlewares/throttling.py`

 * *Files identical despite different names*

