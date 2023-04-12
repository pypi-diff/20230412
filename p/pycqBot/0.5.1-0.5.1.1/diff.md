# Comparing `tmp/pycqBot-0.5.1.tar.gz` & `tmp/pycqBot-0.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycqBot-0.5.1.tar", last modified: Sun Apr  9 17:49:13 2023, max compression
+gzip compressed data, was "pycqBot-0.5.1.1.tar", last modified: Wed Apr 12 17:24:30 2023, max compression
```

## Comparing `pycqBot-0.5.1.tar` & `pycqBot-0.5.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/
--rw-r--r--   0 sakura    (1000) sakura    (1000)     2815 2023-04-09 17:49:13.335149 pycqBot-0.5.1/PKG-INFO
--rwxrwx---   0 sakura    (1000) sakura    (1000)     1785 2023-04-09 10:34:02.000000 pycqBot-0.5.1/README.md
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.331149 pycqBot-0.5.1/pycqBot/
--rwxrwx---   0 sakura    (1000) sakura    (1000)     2484 2023-04-09 17:49:10.000000 pycqBot-0.5.1/pycqBot/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     6178 2023-04-08 10:20:54.000000 pycqBot-0.5.1/pycqBot/asyncHttp.py
--rw-r--r--   0 sakura    (1000) sakura    (1000)    45946 2023-04-09 07:34:10.000000 pycqBot-0.5.1/pycqBot/cqApi.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    17794 2023-04-09 17:47:46.000000 pycqBot-0.5.1/pycqBot/cqCode.py
--rw-r--r--   0 sakura    (1000) sakura    (1000)    11984 2023-04-09 07:33:21.000000 pycqBot-0.5.1/pycqBot/cqEvent.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    33223 2023-04-09 17:48:08.000000 pycqBot-0.5.1/pycqBot/cqHttpApi.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/data/
--rwxrwx---   0 sakura    (1000) sakura    (1000)      226 2023-04-03 10:50:19.000000 pycqBot-0.5.1/pycqBot/data/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4127 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/data/event.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4221 2023-04-09 08:49:03.000000 pycqBot-0.5.1/pycqBot/data/message.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4502 2023-04-04 10:57:32.000000 pycqBot-0.5.1/pycqBot/data/user.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)      378 2023-04-08 11:46:45.000000 pycqBot-0.5.1/pycqBot/object.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/__init__.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/bilibili/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/bilibili/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    23487 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/bilibili/bilibili.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/manage/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/manage/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4818 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/manage/manage.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/pixiv/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/pixiv/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)    15785 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/pixiv/pixiv.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/test/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/test/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)      868 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/test/test.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.335149 pycqBot-0.5.1/pycqBot/plugin/twitter/
--rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1/pycqBot/plugin/twitter/__init__.py
--rwxrwx---   0 sakura    (1000) sakura    (1000)     4603 2023-04-08 09:09:33.000000 pycqBot-0.5.1/pycqBot/plugin/twitter/twitter.py
-drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-09 17:49:13.331149 pycqBot-0.5.1/pycqBot.egg-info/
--rwxrwx---   0 sakura    (1000) sakura    (1000)     2815 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/PKG-INFO
--rwxrwx---   0 sakura    (1000) sakura    (1000)      755 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/SOURCES.txt
--rwxrwx---   0 sakura    (1000) sakura    (1000)        1 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/dependency_links.txt
--rwxrwx---   0 sakura    (1000) sakura    (1000)       57 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/requires.txt
--rwxrwx---   0 sakura    (1000) sakura    (1000)        8 2023-04-09 17:49:13.000000 pycqBot-0.5.1/pycqBot.egg-info/top_level.txt
--rw-r--r--   0 sakura    (1000) sakura    (1000)       38 2023-04-09 17:49:13.335149 pycqBot-0.5.1/setup.cfg
--rwxrwx---   0 sakura    (1000) sakura    (1000)     1012 2023-04-09 10:10:46.000000 pycqBot-0.5.1/setup.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/
+-rw-r--r--   0 sakura    (1000) sakura    (1000)     2817 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/PKG-INFO
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     1785 2023-04-09 10:34:02.000000 pycqBot-0.5.1.1/README.md
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     2486 2023-04-12 17:20:50.000000 pycqBot-0.5.1.1/pycqBot/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     6178 2023-04-08 10:20:54.000000 pycqBot-0.5.1.1/pycqBot/asyncHttp.py
+-rw-r--r--   0 sakura    (1000) sakura    (1000)    45946 2023-04-09 07:34:10.000000 pycqBot-0.5.1.1/pycqBot/cqApi.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    17794 2023-04-09 17:47:46.000000 pycqBot-0.5.1.1/pycqBot/cqCode.py
+-rw-r--r--   0 sakura    (1000) sakura    (1000)    11990 2023-04-12 17:11:51.000000 pycqBot-0.5.1.1/pycqBot/cqEvent.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    33223 2023-04-09 17:48:08.000000 pycqBot-0.5.1.1/pycqBot/cqHttpApi.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/data/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      226 2023-04-03 10:50:19.000000 pycqBot-0.5.1.1/pycqBot/data/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4278 2023-04-12 17:17:25.000000 pycqBot-0.5.1.1/pycqBot/data/event.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4214 2023-04-12 17:24:25.000000 pycqBot-0.5.1.1/pycqBot/data/message.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4502 2023-04-04 10:57:32.000000 pycqBot-0.5.1.1/pycqBot/data/user.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      378 2023-04-08 11:46:45.000000 pycqBot-0.5.1.1/pycqBot/object.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/plugin/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1.1/pycqBot/plugin/__init__.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/plugin/bilibili/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1.1/pycqBot/plugin/bilibili/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    23487 2023-04-08 09:09:33.000000 pycqBot-0.5.1.1/pycqBot/plugin/bilibili/bilibili.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/plugin/manage/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1.1/pycqBot/plugin/manage/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4818 2023-04-08 09:09:33.000000 pycqBot-0.5.1.1/pycqBot/plugin/manage/manage.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/plugin/pixiv/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1.1/pycqBot/plugin/pixiv/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)    15785 2023-04-08 09:09:33.000000 pycqBot-0.5.1.1/pycqBot/plugin/pixiv/pixiv.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/plugin/test/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1.1/pycqBot/plugin/test/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      868 2023-04-08 09:09:33.000000 pycqBot-0.5.1.1/pycqBot/plugin/test/test.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot/plugin/twitter/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        0 2023-04-02 16:34:46.000000 pycqBot-0.5.1.1/pycqBot/plugin/twitter/__init__.py
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     4603 2023-04-08 09:09:33.000000 pycqBot-0.5.1.1/pycqBot/plugin/twitter/twitter.py
+drwxr-xr-x   0 sakura    (1000) sakura    (1000)        0 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/pycqBot.egg-info/
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     2817 2023-04-12 17:24:29.000000 pycqBot-0.5.1.1/pycqBot.egg-info/PKG-INFO
+-rwxrwx---   0 sakura    (1000) sakura    (1000)      755 2023-04-12 17:24:29.000000 pycqBot-0.5.1.1/pycqBot.egg-info/SOURCES.txt
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        1 2023-04-12 17:24:29.000000 pycqBot-0.5.1.1/pycqBot.egg-info/dependency_links.txt
+-rwxrwx---   0 sakura    (1000) sakura    (1000)       57 2023-04-12 17:24:29.000000 pycqBot-0.5.1.1/pycqBot.egg-info/requires.txt
+-rwxrwx---   0 sakura    (1000) sakura    (1000)        8 2023-04-12 17:24:29.000000 pycqBot-0.5.1.1/pycqBot.egg-info/top_level.txt
+-rw-r--r--   0 sakura    (1000) sakura    (1000)       38 2023-04-12 17:24:30.075153 pycqBot-0.5.1.1/setup.cfg
+-rwxrwx---   0 sakura    (1000) sakura    (1000)     1014 2023-04-12 17:19:33.000000 pycqBot-0.5.1.1/setup.py
```

### Comparing `pycqBot-0.5.1/PKG-INFO` & `pycqBot-0.5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycqBot
-Version: 0.5.1
+Version: 0.5.1.1
 Summary: go-cqhttp python 框架，可以用于快速塔建 bot
 Home-page: https://github.com/FengLiuFeseliud/pycqBot
 Author: FengLiuFeseliud
 Author-email: 17351198406@qq.com
 License: AGPL-3.0 License
 Description: # pycqBot
```

### Comparing `pycqBot-0.5.1/README.md` & `pycqBot-0.5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/__init__.py` & `pycqBot-0.5.1.1/pycqBot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pycqBot.cqHttpApi import cqBot, cqHttpApi, cqLog
 from pycqBot.object import Plugin
 
 
-__VERSIONS__ = "v0.5.1"
+__VERSIONS__ = "v0.5.1.1"
 
 
 TIT = """
 #################################################################
 ██████╗ ██╗   ██╗ ██████╗ ██████╗ ██████╗  ██████╗ ████████╗
 ██╔══██╗╚██╗ ██╔╝██╔════╝██╔═══██╗██╔══██╗██╔═══██╗╚══██╔══╝
 ██████╔╝ ╚████╔╝ ██║     ██║   ██║██████╔╝██║   ██║   ██║
```

### Comparing `pycqBot-0.5.1/pycqBot/asyncHttp.py` & `pycqBot-0.5.1.1/pycqBot/asyncHttp.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/cqApi.py` & `pycqBot-0.5.1.1/pycqBot/cqApi.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/cqCode.py` & `pycqBot-0.5.1.1/pycqBot/cqCode.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/cqEvent.py` & `pycqBot-0.5.1.1/pycqBot/cqEvent.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         go-cqhttp 文档:
         https://docs.go-cqhttp.org/event/#%E7%A7%81%E8%81%8A%E6%B6%88%E6%81%AF
         """
         pass
 
     def message_sent_private_friend(self, message: Private_Message):
         """
-        私聊好友消息
+        自身消息私聊上报
 
         go-cqhttp 文档:
         https://docs.go-cqhttp.org/event/#%E7%A7%81%E8%81%8A%E6%B6%88%E6%81%AF
         """
         pass
 
     def message_private_group_self(self, message: Private_Message):
```

### Comparing `pycqBot-0.5.1/pycqBot/cqHttpApi.py` & `pycqBot-0.5.1.1/pycqBot/cqHttpApi.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/data/event.py` & `pycqBot-0.5.1.1/pycqBot/data/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     from pycqBot.cqHttpApi import cqHttpApi
 
 
 class Message:
 
     MESSAGE_POST_TYPE: str = "message"
     """消息事件类型"""
+    MESSAGE_SENT_POST_TYPE: str = "message_sent"
+    """Bot 自身消息事件类型"""
 
     PRIVATE_MESSAGE_TYPE: str = "private"
     """私聊消息类型"""
 
     GROUP_MESSAGE_TYPE: str = "group"
     """群消息类型"""
 
@@ -131,15 +133,15 @@
 
     def get_event_sub_type(self) -> str:
         return self.meta_event_type
     
 
 def _get_event(message: str) -> Event:
     message_data = json.loads(message)
-    if message_data["post_type"] == Message.MESSAGE_POST_TYPE:
+    if message_data["post_type"] == Message.MESSAGE_POST_TYPE or message_data["post_type"] == Message.MESSAGE_SENT_POST_TYPE:
         return Message_Event(message_data)
     
     if message_data["post_type"] == Meta.META_POST_TYPE:
         return Meta_Event(message_data)
     
     if message_data["post_type"] == Notice.NOTICE_POST_TYPE:
         return Notice_Event(message_data)
```

### Comparing `pycqBot-0.5.1/pycqBot/data/message.py` & `pycqBot-0.5.1.1/pycqBot/data/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         self.target_id: int = message_data["target_id"]
         """接收者 QQ 号"""
 
         self.temp_source: Optional[int] = message_data["temp_source"] if "temp_source" in message_data else None
         """临时会话来源"""
 
     def reply(self, message: str, auto_escape: bool = False) -> None:
-        self._cqapi.send_private_msg(self.sender.id, "%s%s" % (reply(msg_id=self.id), message), self.temp_source, auto_escape)
+        self._cqapi.send_private_msg(self.sender.id, "%s%s" % (reply(self.id), message), self.temp_source, auto_escape)
 
     def reply_not_code(self, message: str, auto_escape: bool=False) -> None:
         self._cqapi.send_private_msg(self.sender.id, message, self.temp_source, auto_escape)
 
 class Group_Message(Message):
     """群消息"""
```

### Comparing `pycqBot-0.5.1/pycqBot/data/user.py` & `pycqBot-0.5.1.1/pycqBot/data/user.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/plugin/bilibili/bilibili.py` & `pycqBot-0.5.1.1/pycqBot/plugin/bilibili/bilibili.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/plugin/manage/manage.py` & `pycqBot-0.5.1.1/pycqBot/plugin/manage/manage.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/plugin/pixiv/pixiv.py` & `pycqBot-0.5.1.1/pycqBot/plugin/pixiv/pixiv.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/plugin/test/test.py` & `pycqBot-0.5.1.1/pycqBot/plugin/test/test.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot/plugin/twitter/twitter.py` & `pycqBot-0.5.1.1/pycqBot/plugin/twitter/twitter.py`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/pycqBot.egg-info/PKG-INFO` & `pycqBot-0.5.1.1/pycqBot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycqBot
-Version: 0.5.1
+Version: 0.5.1.1
 Summary: go-cqhttp python 框架，可以用于快速塔建 bot
 Home-page: https://github.com/FengLiuFeseliud/pycqBot
 Author: FengLiuFeseliud
 Author-email: 17351198406@qq.com
 License: AGPL-3.0 License
 Description: # pycqBot
```

### Comparing `pycqBot-0.5.1/pycqBot.egg-info/SOURCES.txt` & `pycqBot-0.5.1.1/pycqBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycqBot-0.5.1/setup.py` & `pycqBot-0.5.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pycqBot",
-    version="0.5.1",
+    version="0.5.1.1",
     description="go-cqhttp python 框架，可以用于快速塔建 bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

