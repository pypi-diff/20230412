# Comparing `tmp/nonebot-plugin-clock-0.7.1.tar.gz` & `tmp/nonebot-plugin-clock-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.7.1.tar", last modified: Sat Apr  8 12:20:33 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.8.tar", last modified: Wed Apr 12 10:42:00 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.7.1.tar` & `nonebot-plugin-clock-0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-03-27 08:36:41.000000 nonebot-plugin-clock-0.7.1/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-03-29 09:01:49.000000 nonebot-plugin-clock-0.7.1/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1019 2023-04-08 12:05:30.000000 nonebot-plugin-clock-0.7.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-03-27 08:40:54.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     5274 2023-04-08 12:18:29.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1821 2023-03-30 03:48:52.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-08 11:51:35.000000 nonebot-plugin-clock-0.7.1/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-08 12:20:33.000000 nonebot-plugin-clock-0.7.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-08 12:20:25.000000 nonebot-plugin-clock-0.7.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      301 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1284 2023-04-12 10:23:52.000000 nonebot-plugin-clock-0.8/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     5674 2023-04-12 10:39:38.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1820 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      301 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-12 10:42:00.000000 nonebot-plugin-clock-0.8/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      550 2023-04-12 10:41:57.000000 nonebot-plugin-clock-0.8/setup.py
```

### Comparing `nonebot-plugin-clock-0.7.1/LICENSE` & `nonebot-plugin-clock-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.8/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.8/nonebot_plugin_clock/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 import re
 
 from datetime import datetime, timedelta
-
+from nonebot.permission import SUPERUSER
 from nonebot import on_command, get_bot, get_driver
 from nonebot.adapters.onebot.v11.bot import Bot
 from nonebot.adapters.onebot.v11.event import Event
 from nonebot.adapters.onebot.v11.message import Message, MessageSegment
 from nonebot.params import CommandArg
 from nonebot.typing import T_State
 from nonebot import require
 
 from .database import db
 from .Clock import Clock
 
 scheduler = require('nonebot_plugin_apscheduler').scheduler
 
-"""
-
-"""
-
-white_list = getattr(get_driver().config, 'clock_white_list', [])
-black_list = getattr(get_driver().config, 'clock_black_list', [])
+WHITELIST = getattr(get_driver().config, 'CLOCK_WHITE_LIST', [])
+BLACKLIST = getattr(get_driver().config, 'CLOCK_BLACK_LIST', [])
+CLOCK_DATA = {}
 
+async def CLOCK_RULE(event: Event) -> bool:
+    
+    # 黑名单优先判定
+    if BLACKLIST:
+        return event.user_id not in BLACKLIST
+    
+    if WHITELIST:
+        if event.sender.role == "member" and event.user_id not in WHITELIST:
+            return False
+        
+    return True
 
-CLOCK_DATA = {}
 
 
 def create_clock_scheduler(clock):
     '''
     创建闹钟任务
     '''
     CLOCK_DATA[clock.id] = clock
@@ -85,32 +92,43 @@
 # 创建闹钟
 add_clock_qq = on_command('添加闹钟', aliases={'设置闹钟',})
 @add_clock_qq.handle()
 async def _(bot: Bot, event: Event, state: T_State, messages: Message = CommandArg()):
 
     messages = str(messages).split(' ', 1)
     content = ''
-    ones = 1
 
     if len(messages) < 2:
         await add_clock_qq.finish(message="添加格式为: “添加闹钟 时间 内容”")
 
     time_ = get_time(messages[0])
     if not time_:
         await add_clock_qq.finish(message="时间格式错误")
 
     for msg in Message(messages[1]):
         if url:=msg.data.get("url"):
             content += str(MessageSegment(msg.type, {"file":url}))
         else:
             content += str(msg)
 
-    
-    state['content'] = content if content else '⏰'
+
     state['time'] = time_
+    state['type'] = 'private'
+    state['user'] = event.user_id
+    state['content'] = content if content else '⏰'
+
+    if 'group' in event.get_event_name():
+        res1 = await SUPERUSER(bot, event)
+        res2 = await CLOCK_RULE(event)
+        if not (res1 or res2):
+            await add_clock_qq.finish(message="你没有该权限哦～")
+        state['type'] = 'group'
+        state['user'] = event.group_id
+
+    
 
 
 @add_clock_qq.got('ones', prompt="⏰不重复, 设置为每日输入[Y/y]\n设置周几 如周一周三输入[13]\n设置某天，如圣诞输入 [12.25]")
 async def _(bot: Bot, event: Event, state: T_State):
 
     state['ones'] = str(state['ones'])
     ones = 0 if state['ones'] in ['Y', 'y'] else 1
@@ -121,60 +139,55 @@
         week = state['ones']
         ones = 0
 
     elif ret:=re.match(r'([0-9]{0,2})[./]([0-9]{1,2})$', state['ones']):
         month, day = ret.groups()
 
     data = {
-        'user' : event.user_id,
+        'user' : state['user'],
         'content' : state['content'],
         'time' : state['time'],
-        'type' : 'private',
+        'type' : state['type'],
         'ones' : ones,
         'week' : week,
         'day' : day,
         'month' : month
     }
        
-    if 'group' in event.get_event_name():
-
-        if white_list and event.user_id not in white_list:
-            await add_clock_qq.finish(message="你没有该权限哦～")
-        if black_list and event.user_id in black_list:
-            await add_clock_qq.finish(message="你没有该权限哦～")
-
-        # info = await bot.get_group_member_info(group_id = event.group_id, user_id=event.user_id)
-        # if info['role'] == level:
-            # ...
-
-
-        data['type'] = 'group'
-        data['user'] = event.group_id
-
-
     add_clock(**data)
     ones_ = {1:'不重复', 0:'重复'}
     await add_clock_qq.finish(message=f"[{ones_[ones]}]添加成功～")
 
 
+
+
 # # 查看闹钟
 check = on_command('查看闹钟',  aliases={'提醒事项', '闹钟','⏰'}, block=True)
 @check.handle()
 async def add_handle(bot: Bot, event: Event):
-    try:
-        uid = event.group_id
-    except:
-        uid = event.user_id
+
+    uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
+
+
+    def check_(msg: str) -> str:
+
+        message = ""
+        for m in Message(msg):
+            if m.type == 'at':
+                message += f"@{m.data['qq']}"
+            else:
+                message += str(m)
+        return message
     
     clock_msg = []
-
     for id in CLOCK_DATA:
         clock = CLOCK_DATA[id]
         if clock.user == uid:
-            clock_msg.append(clock.get_info())
+            clock_msg.append(check_(clock.get_info()))
+
     if clock_msg:
         await bot.send(event, message= Message('\n'.join(clock_msg)))
     else:
         await bot.send(event, message='目前没有闹钟')
```

### Comparing `nonebot-plugin-clock-0.7.1/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.8/nonebot_plugin_clock/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import os
 import sqlite3
-from .Clock import Clock
+from Clock import Clock
 
 TABLE = "CLOCKS"
 db_ = os.path.dirname(__file__) + '/data.sqlite'
 
 
 if not os.path.exists(db_):
```

