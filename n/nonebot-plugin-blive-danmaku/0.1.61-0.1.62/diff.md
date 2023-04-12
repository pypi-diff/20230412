# Comparing `tmp/nonebot_plugin_blive_danmaku-0.1.61.tar.gz` & `tmp/nonebot_plugin_blive_danmaku-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.61.tar", max compression
+gzip compressed data, was "nonebot_plugin_blive_danmaku-0.1.62.tar", max compression
```

## Comparing `nonebot_plugin_blive_danmaku-0.1.61.tar` & `nonebot_plugin_blive_danmaku-0.1.62.tar`

### file list

```diff
@@ -1,34 +1,31 @@
--rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.61/LICENSE
--rw-r--r--   0        0        0      127 2023-04-11 12:02:27.067229 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/__init__.py
--rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.git
--rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
--rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.gitignore
--rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
--rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
--rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
--rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
--rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/LICENSE
--rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/README.md
--rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
--rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/sample.py
--rw-r--r--   0        0        0       99 2023-04-11 12:02:27.068736 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 17:28:27.970418 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/__init__.py
--rw-r--r--   0        0        0      848 2023-04-09 17:33:40.134826 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_off.py
--rw-r--r--   0        0        0      847 2023-04-09 17:32:58.298393 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_on.py
--rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/__init__.py
--rw-r--r--   0        0        0     1409 2023-04-11 12:03:03.764913 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
--rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
--rw-r--r--   0        0        0      980 2023-04-11 12:02:27.070244 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
--rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
--rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
--rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
--rw-r--r--   0        0        0     3671 2023-04-10 09:03:17.352805 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
--rw-r--r--   0        0        0     2838 2023-04-11 12:14:08.615605 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/live.py
--rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/config.py
--rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/__init__.py
--rw-r--r--   0        0        0     2813 2023-04-11 12:07:23.972087 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/db.py
--rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/model.py
--rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/utils/__init__.py
--rw-r--r--   0        0        0      951 2023-04-11 12:14:24.249514 nonebot_plugin_blive_danmaku-0.1.61/pyproject.toml
--rw-r--r--   0        0        0     2745 2023-04-11 12:02:27.048184 nonebot_plugin_blive_danmaku-0.1.61/README.md
--rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.61/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-07 16:32:26.658635 nonebot_plugin_blive_danmaku-0.1.62/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-12 02:09:23.365107 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-04 00:23:10.472267 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/.git
+-rw-r--r--   0        0        0       68 2023-04-04 00:23:14.371312 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/.gitattributes
+-rw-r--r--   0        0        0     1260 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/.gitignore
+-rw-r--r--   0        0        0       96 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/__init__.py
+-rw-r--r--   0        0        0    21920 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py
+-rw-r--r--   0        0        0     5365 2023-04-04 00:23:14.374439 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py
+-rw-r--r--   0        0        0    12447 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py
+-rw-r--r--   0        0        0     1084 2023-04-04 00:23:14.372334 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/LICENSE
+-rw-r--r--   0        0        0      457 2023-04-04 00:23:14.373344 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/README.md
+-rw-r--r--   0        0        0       31 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/requirements.txt
+-rw-r--r--   0        0        0     2928 2023-04-04 00:23:14.375451 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/sample.py
+-rw-r--r--   0        0        0       99 2023-04-12 02:09:23.365107 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:26:16.349686 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/__init__.py
+-rw-r--r--   0        0        0     1409 2023-04-12 02:09:23.366107 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_add.py
+-rw-r--r--   0        0        0     1398 2023-04-09 17:27:28.520785 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py
+-rw-r--r--   0        0        0      980 2023-04-12 02:09:23.366107 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_list.py
+-rw-r--r--   0        0        0      831 2023-04-09 17:27:43.407410 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_off.py
+-rw-r--r--   0        0        0      822 2023-04-09 17:27:52.919328 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_on.py
+-rw-r--r--   0        0        0        0 2023-04-10 07:19:16.340181 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/subscribe/__init__.py
+-rw-r--r--   0        0        0     4588 2023-04-12 02:12:34.778723 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py
+-rw-r--r--   0        0        0     2131 2023-04-12 02:12:04.648097 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/subscribe/live.py
+-rw-r--r--   0        0        0      261 2023-04-10 15:15:41.674275 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/config.py
+-rw-r--r--   0        0        0       18 2023-04-07 06:14:41.544558 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/database/__init__.py
+-rw-r--r--   0        0        0     2896 2023-04-12 02:11:02.538862 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/database/db.py
+-rw-r--r--   0        0        0     1984 2023-04-10 14:49:04.632614 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/database/model.py
+-rw-r--r--   0        0        0     3870 2023-04-10 13:46:27.863711 nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/utils/__init__.py
+-rw-r--r--   0        0        0      951 2023-04-12 02:09:48.929528 nonebot_plugin_blive_danmaku-0.1.62/pyproject.toml
+-rw-r--r--   0        0        0     2745 2023-04-12 02:09:23.364107 nonebot_plugin_blive_danmaku-0.1.62/README.md
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 nonebot_plugin_blive_danmaku-0.1.62/PKG-INFO
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.62/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/.gitignore` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/client.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/handlers.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/blivedm/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/LICENSE` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/blivedm/sample.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/blivedm/sample.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_off.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_on.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.params import ArgPlainText
 from nonebot import on_command
 from ...utils import get_type_id,handle_uid,permission_check,uid_check
 from ...database import Db as db
 
-live_on = on_command("关闭直播推送", priority=5)
-live_on.__doc__ = """关闭直播推送 UID"""
-live_on.handle()(permission_check)
-live_on.handle()(handle_uid)
-live_on.got("uid", prompt="请输入一个UID")(uid_check)
+sub_on = on_command("开启路灯", priority=5)
+sub_on.__doc__ = """开启路灯 UID"""
+sub_on.handle()(permission_check)
+sub_on.handle()(handle_uid)
+sub_on.got("uid", prompt="请输入一个UID")(uid_check)
 
-@live_on.handle()
+@sub_on.handle()
 async def _(event: MessageEvent, uid: str = ArgPlainText("uid")):
-    """关闭开播提醒"""
+    """开启路灯"""
     type_id = await get_type_id(event)
-    res = await db.update_sub("live", False, uid=uid, type_id=type_id, type=event.message_type)
+    res = await db.update_sub("street_lamp", True, uid=uid, type_id=type_id, type=event.message_type)
     if res:
-        await live_on.finish(f'已关闭 {uid} 开播提醒')
-    await live_on.finish(f'未订阅 {uid}')
+        await sub_on.finish(f'已开启 {uid} 路灯')
+    await sub_on.finish(f'未订阅 {uid}')
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/live/live_on.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_off.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.params import ArgPlainText
 from nonebot import on_command
 from ...utils import get_type_id,handle_uid,permission_check,uid_check
 from ...database import Db as db
 
-live_on = on_command("开启直播推送", priority=5)
-live_on.__doc__ = """开启直播推送 UID"""
-live_on.handle()(permission_check)
-live_on.handle()(handle_uid)
-live_on.got("uid", prompt="请输入一个UID")(uid_check)
+sub_off = on_command("关闭路灯", priority=5)
+sub_off.__doc__ = """关闭路灯 UID"""
+sub_off.handle()(permission_check)
+sub_off.handle()(handle_uid)
+sub_off.got("uid", prompt="请输入一个UID")(uid_check)
 
-@live_on.handle()
+@sub_off.handle()
 async def _(event: MessageEvent, uid: str = ArgPlainText("uid")):
-    """开启开播提醒"""
+    """关闭路灯"""
     type_id = await get_type_id(event)
-    res = await db.update_sub("live", True, uid=uid, type_id=type_id, type=event.message_type)
+    res = await db.update_sub("street_lamp", False, uid=uid, type_id=type_id, type=event.message_type)
     if res:
-        await live_on.finish(f'已开启 {uid} 开播提醒')
-    await live_on.finish(f'未订阅 {uid}')
+        await sub_off.finish(f'已开启 {uid} 路灯')
+    await sub_off.finish(f'未订阅 {uid}')
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_add.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_add.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_delete.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/sub/sub_list.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/sub/sub_list.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/subscribe/danmaku.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,24 +44,39 @@
                 model = ClientModel(room_id)
                 model.client.add_handler(handler)
                 model.client.start()
                 model.uid=uid
                 model.name=info["uname"]
                 model.live_time=get_timespan(room_info["live_time"])
                 clients.append(model)
+
+                start_timespan = get_timespan(room_info["live_time"])
+                cover = (
+                    info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
+                )
+                room = db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
+                if not room:
+                    await db.add_room(room_id=room_id, cover=cover, title=info["title"], name=info["uname"], start_time=start_timespan, end_time=0)
         else:
             if new_status == 0:
                 model = index[0]
                 client = model.client
                 try:
                     asyncio.gather(client.join())
                 finally:
                     await asyncio.gather(client.stop_and_close())
                     clients.remove(model)
                     logger.info(f'{info["uname"]}下播了，断开直播间连接')
+                
+                now = int(time.time())
+                room_id = info["short_id"] if info["short_id"] else info["room_id"]
+                room_list = await db.get_rooms(room_id=room_id, uid=uid)
+                room_list.sort(key=lambda x:x.start_time, reverse=True)
+                room = room_list[0]
+                await db.update_room("end_time", now, room_id=room_id, uid=uid, start_time=room.start_time)
 
     
 
 class MsgHandler(blivedm.BaseHandler):
     async def _on_danmaku(self, client: blivedm.BLiveClient, message: blivedm.DanmakuMessage):
         if(message.msg.startswith("#路灯")):
             logger.info(f'{client.room_owner_uid}的直播间收到路灯：{message.uname} -> {message.msg}')
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/command/subscribe/live.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/command/subscribe/live.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,15 @@
     "interval", seconds=12, id="live_sched"
 )
 async def live():
     """开播提醒"""
     plugin_config = Config.parse_obj(get_driver().config)
     if plugin_config.danmaku_group_notice is False:
         return
-    sub_list = await db.get_subs()
-    uids = []
-    for x in sub_list:
-        uids.append(x.uid)
+    uids = db.get_sub_list("live")
 
     if not uids:
         return
     
     res = await get_rooms_info_by_uids(uids, reqtype="web", proxies=None)
     if not res:
         return
@@ -47,28 +44,17 @@
             logger.info(f"{name} 开播了")
             url = f"https://live.bilibili.com/{room_id}"
             cover = (
                 info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
             )
             title = info["title"]
             msg = f"{name} 正在直播：\n{title}\n{MessageSegment.image(cover)}\n{url}"
-
-            start_timespan = get_timespan(room_info["live_time"])
-            room = db.get_room(room_id=room_id, uid=uid, start_time=start_timespan)
-            if not room:
-                await db.add_room(room_id=room_id, cover=cover, title=info["title"], name=info["uname"], start_time=start_timespan, end_time=0)
         else:
             logger.info(f"{name} 下播了")
             cover = (
                 info["cover_from_user"] if info["cover_from_user"] else info["keyframe"]
             )
             msg = f"{name} 下播了\n{MessageSegment.image(cover)}"
-
-            now = int(time.time())
-            room_list = await db.get_rooms(room_id=room_id, uid=uid)
-            room_list.sort(key=lambda x:x.start_time, reverse=True)
-            room = room_list[0]
-            await db.update_room("end_time", now, room_id=room_id, uid=uid, start_time=room.start_time)
         sub_list = await db.get_subs(uid=uid)
         for sub in sub_list:
             await send_msg(bot_id=sub.bot_id, send_type=sub.type, type_id=sub.type_id, message=msg)
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/db.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/database/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot import get_driver
 from tortoise import Tortoise
 from tortoise.connection import connections
 
 from ..utils import get_path
 from .model import Sub, LiveRoom, Danmaku
 
-sub_dict = {"street_lamp": []}
+sub_dict = {"street_lamp": [], "live": []}
 
 class Db:
     @classmethod
     async def init(cls):
         config={
             "connections":{"danmaku_bot":f"sqlite://{get_path('danmakuBot.sqlite3')}"},
             "apps":{
@@ -58,14 +58,15 @@
     def get_sub_list(cls, key):
         return sub_dict[key]
  
     @classmethod
     async def update_sub_list(cls):
         subs = Sub.all()
         sub_dict["street_lamp"] = list(set([sub.uid async for sub in subs if sub.street_lamp]))
+        sub_dict["live"] = list(set([sub.uid async for sub in subs]))
     
     @classmethod
     async def get_rooms(cls, **kwargs):
         res = await LiveRoom.get(**kwargs)
         return res
     
     @classmethod
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/database/model.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/database/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/nonebot_plugin_blive_danmaku/utils/__init__.py` & `nonebot_plugin_blive_danmaku-0.1.62/nonebot_plugin_blive_danmaku/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/pyproject.toml` & `nonebot_plugin_blive_danmaku-0.1.62/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-blive-danmaku"
-version = "0.1.61"
+version = "0.1.62"
 description = "A danmaku plugin for Nonebot2"
 authors = ["ricardo <thespirit@vip.qq.com>"]
 documentation = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku#readme"
 license = "MIT"
 homepage = "https://github.com/zangxx66/nonebot_plugin_blive_danmaku"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "bilibili", "danmaku"]
```

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/README.md` & `nonebot_plugin_blive_danmaku-0.1.62/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blive_danmaku-0.1.61/PKG-INFO` & `nonebot_plugin_blive_danmaku-0.1.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blive-danmaku
-Version: 0.1.61
+Version: 0.1.62
 Summary: A danmaku plugin for Nonebot2
 Home-page: https://github.com/zangxx66/nonebot_plugin_blive_danmaku
 License: MIT
 Keywords: nonebot,nonebot2,bilibili,danmaku
 Author: ricardo
 Author-email: thespirit@vip.qq.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.61
+Metadata-Version: 2.1 Name: nonebot-plugin-blive-danmaku Version: 0.1.62
 Summary: A danmaku plugin for Nonebot2 Home-page: https://github.com/zangxx66/
 nonebot_plugin_blive_danmaku License: MIT Keywords:
 nonebot,nonebot2,bilibili,danmaku Author: ricardo Author-email:
 thespirit@vip.qq.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

