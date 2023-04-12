# Comparing `tmp/aiogram-ext-0.0.5.tar.gz` & `tmp/aiogram-ext-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.0.5.tar", last modified: Wed Apr 12 11:18:15 2023, max compression
+gzip compressed data, was "aiogram-ext-0.0.6.tar", last modified: Wed Apr 12 14:38:37 2023, max compression
```

## Comparing `aiogram-ext-0.0.5.tar` & `aiogram-ext-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,16 @@
--rw-r--r--   0        0        0      465 2023-04-12 10:53:39.977438 aiogram-ext-0.0.5/aiogram_ext/__init__.py
--rw-r--r--   0        0        0     6468 2023-04-12 10:34:24.416929 aiogram-ext-0.0.5/aiogram_ext/_currents.py
--rw-r--r--   0        0        0     2291 2023-04-12 10:34:24.385343 aiogram-ext-0.0.5/aiogram_ext/_questions.py
--rw-r--r--   0        0        0     5406 2023-04-11 11:53:07.707408 aiogram-ext-0.0.5/aiogram_ext/_states.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.5/aiogram_ext/buttons.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.5/aiogram_ext/context.py
--rw-r--r--   0        0        0     1132 2023-04-12 11:08:54.370551 aiogram-ext-0.0.5/aiogram_ext/deps.py
--rw-r--r--   0        0        0     5887 2023-04-12 11:08:56.310732 aiogram-ext-0.0.5/aiogram_ext/dispatcher.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.5/aiogram_ext/filters.py
--rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.5/aiogram_ext/helpers.py
--rw-r--r--   0        0        0      700 2023-04-12 10:34:05.006090 aiogram-ext-0.0.5/aiogram_ext/keyboards.py
--rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.5/aiogram_ext/middlewares/__init__.py
--rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.5/aiogram_ext/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.5/aiogram_ext/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.5/aiogram_ext/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.5/aiogram_ext/middlewares/throttling.py
--rw-r--r--   0        0        0      300 2023-04-12 11:18:11.705125 aiogram-ext-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.5/README.md
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      465 2023-04-12 10:53:39.977438 aiogram-ext-0.0.6/aiogram_ext/__init__.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.0.6/aiogram_ext/buttons.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.0.6/aiogram_ext/context.py
+-rw-r--r--   0        0        0     1132 2023-04-12 11:08:54.370551 aiogram-ext-0.0.6/aiogram_ext/deps.py
+-rw-r--r--   0        0        0     5887 2023-04-12 11:08:56.310732 aiogram-ext-0.0.6/aiogram_ext/dispatcher.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.0.6/aiogram_ext/filters.py
+-rw-r--r--   0        0        0      459 2023-04-12 10:56:42.149572 aiogram-ext-0.0.6/aiogram_ext/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.0.6/aiogram_ext/keyboards.py
+-rw-r--r--   0        0        0      154 2023-04-12 10:34:24.400978 aiogram-ext-0.0.6/aiogram_ext/middlewares/__init__.py
+-rw-r--r--   0        0        0     6983 2023-04-12 10:34:24.432621 aiogram-ext-0.0.6/aiogram_ext/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.0.6/aiogram_ext/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.0.6/aiogram_ext/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.0.6/aiogram_ext/middlewares/throttling.py
+-rw-r--r--   0        0        0      300 2023-04-12 14:38:14.534221 aiogram-ext-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.0.6/README.md
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.0.6/PKG-INFO
```

### Comparing `aiogram-ext-0.0.5/aiogram_ext/buttons.py` & `aiogram-ext-0.0.6/aiogram_ext/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/context.py` & `aiogram-ext-0.0.6/aiogram_ext/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/deps.py` & `aiogram-ext-0.0.6/aiogram_ext/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/dispatcher.py` & `aiogram-ext-0.0.6/aiogram_ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/filters.py` & `aiogram-ext-0.0.6/aiogram_ext/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/keyboards.py` & `aiogram-ext-0.0.6/aiogram_ext/keyboards.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 )
 
 ReplyButton = str | KeyboardButton
 
 
 class ReplyKeyboard(ReplyKeyboardMarkup):
     buttons: list[ReplyButton] = None
+    row_width = 1
 
-    def __init__(self, *buttons: str | KeyboardButton, row_width=1):
-        super().__init__(row_width=row_width, resize_keyboard=True)
+    def __init__(self, *buttons: str | KeyboardButton):
+        super().__init__(row_width=self.row_width, resize_keyboard=True)
         self.add(*(self.buttons or []), *buttons)
 
 
 class InlineKeyboard(InlineKeyboardMarkup):
     buttons: list[InlineButton] = None
+    row_width = 1
 
-    def __init__(self, *buttons: InlineButton, row_width=1):
-        super().__init__(row_width=row_width)
+    def __init__(self, *buttons: InlineButton):
+        super().__init__(row_width=self.row_width)
         self.add(*(self.buttons or []), *buttons)
```

### Comparing `aiogram-ext-0.0.5/aiogram_ext/middlewares/_conversation.py` & `aiogram-ext-0.0.6/aiogram_ext/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/middlewares/_membership.py` & `aiogram-ext-0.0.6/aiogram_ext/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/middlewares/misc.py` & `aiogram-ext-0.0.6/aiogram_ext/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.0.5/aiogram_ext/middlewares/throttling.py` & `aiogram-ext-0.0.6/aiogram_ext/middlewares/throttling.py`

 * *Files identical despite different names*

