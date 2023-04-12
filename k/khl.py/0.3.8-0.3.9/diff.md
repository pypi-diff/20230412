# Comparing `tmp/khl.py-0.3.8.tar.gz` & `tmp/khl.py-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/khl.py/khl.py/dist/tmpqfc6zny4/khl.py-0.3.8.tar", last modified: Sun Oct 30 03:06:14 2022, max compression
+gzip compressed data, was "/home/runner/work/khl.py/khl.py/dist/tmphwvax4kt/khl.py-0.3.9.tar", last modified: Mon Nov 21 05:14:26 2022, max compression
```

## Comparing `khl.py-0.3.8.tar` & `khl.py-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-30 03:06:02.000000 khl.py-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-10-30 03:06:14.000000 khl.py-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-10-30 03:06:02.000000 khl.py-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl/bot/
--rw-r--r--   0 runner    (1001) docker     (121)    19572 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/bot/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15169 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/guild.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl/command/
--rw-r--r--   0 runner    (1001) docker     (121)     7139 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/lexer.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/cert.py
--rw-r--r--   0 runner    (1001) docker     (121)    11541 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5827 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/receiver.py
--rw-r--r--   0 runner    (1001) docker     (121)    10528 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/user.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/permission.py
--rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7893 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl/task/
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/task/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/game.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     3736 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/requester.py
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl/card/
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     8760 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/module.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/card_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/element.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/struct.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-10-30 03:06:02.000000 khl.py-0.3.8/khl/card/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-10-30 03:06:14.000000 khl.py-0.3.8/khl.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-30 03:06:02.000000 khl.py-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-10-30 03:06:14.000000 khl.py-0.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-21 05:14:09.000000 khl.py-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-11-21 05:14:26.000000 khl.py-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1878 2022-11-21 05:14:09.000000 khl.py-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl/bot/
+-rw-r--r--   0 runner    (1001) docker     (121)    19572 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/bot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16189 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/guild.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl/command/
+-rw-r--r--   0 runner    (1001) docker     (121)     7139 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4130 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/cert.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12316 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5827 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10686 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1887 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9767 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7893 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3046 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl/task/
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/task/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/game.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3736 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/requester.py
+-rw-r--r--   0 runner    (1001) docker     (121)      763 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl/card/
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8760 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/card_message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3191 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/element.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/card.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/struct.py
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-11-21 05:14:09.000000 khl.py-0.3.9/khl/card/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-11-21 05:14:26.000000 khl.py-0.3.9/khl.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-11-21 05:14:09.000000 khl.py-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-11-21 05:14:26.000000 khl.py-0.3.9/PKG-INFO
```

### Comparing `khl.py-0.3.8/LICENSE` & `khl.py-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/setup.cfg` & `khl.py-0.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = khl.py
-version = 0.3.8
+version = 0.3.9
 author = TWT233
 author_email = TWT2333@outlook.com
 description = Python SDK for kaiheila.cn API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TWT233/khl.py
 project_urls =
```

### Comparing `khl.py-0.3.8/README.md` & `khl.py-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/bot/bot.py` & `khl.py-0.3.9/khl/bot/bot.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/guild.py` & `khl.py-0.3.9/khl/guild.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """guild related stuffs: Guild, ChannelCategory"""
 import logging
+import time
 import warnings
 from typing import List, Union, Dict, IO
 
 from . import api
 from .channel import Channel, public_channel_factory, PublicChannel, PublicVoiceChannel
 from .gateway import Requestable, Gateway
 from .interface import LazyLoadable
@@ -44,14 +45,30 @@
         rt: List[Role] = []
         for role in guild_roles:
             if role['role_id'] in self.roles:
                 rt.append(Role(**role))
         return rt
 
 
+class GuildBoost:
+    """Guild boost"""
+    user_id: str
+    guild_id: str
+    start_time: int
+    end_time: int
+    user: User
+
+    def __init__(self, **kwargs) -> None:
+        self.user_id = kwargs.get('user_id')
+        self.guild_id = kwargs.get('guild_id')
+        self.start_time = kwargs.get('start_time')
+        self.end_time = kwargs.get('end_time')
+        self.user = User(**kwargs.get('user'), _gate_=kwargs.get('_gate_', None))
+
+
 class ChannelCategory(Requestable):
     """represent a channel set"""
     id: str
     name: str
     master_id: str
     guild_id: str
     level: int
@@ -361,7 +378,20 @@
         if name is not None:
             params['name'] = name
         return await self.gate.exec_req(api.GuildEmoji.update(**params))
 
     async def delete_emoji(self, id: str):
         """delete a custom emoji"""
         return await self.gate.exec_req(api.GuildEmoji.delete(id))
+
+    async def fetch_boost(self, start_time: int = 0, end_time: int = int(time.time()), **kwargs) -> List[GuildBoost]:
+        """
+        list the boost in guild.
+
+        :param start_time: start_time time stamp (Sec).
+        :param end_time: end_time time stamp (Sec). Default to now time.
+        """
+        boost_list = await self.gate.exec_paged_req(
+            api.GuildBoost.history(guild_id=self.id, start_time=start_time, end_time=end_time),
+            **kwargs
+        )
+        return [GuildBoost(**item, _gate_=self.gate) for item in boost_list]
```

### Comparing `khl.py-0.3.8/khl/gateway.py` & `khl.py-0.3.9/khl/gateway.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/command/command.py` & `khl.py-0.3.9/khl/command/command.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/command/parser.py` & `khl.py-0.3.9/khl/command/parser.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/command/manager.py` & `khl.py-0.3.9/khl/command/manager.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/command/exception.py` & `khl.py-0.3.9/khl/command/exception.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/command/rule.py` & `khl.py-0.3.9/khl/command/rule.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/command/lexer.py` & `khl.py-0.3.9/khl/command/lexer.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/cert.py` & `khl.py-0.3.9/khl/cert.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/client.py` & `khl.py-0.3.9/khl/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """abstraction of khl client: handle to communicate with khl"""
 import asyncio
 import inspect
 import logging
+import time
 from pathlib import Path
 from typing import Dict, List, Callable, Coroutine, Union, IO
 
 from . import api
 from .channel import public_channel_factory, PublicChannel, Channel, PublicTextChannel
 from .game import Game
 from .gateway import Gateway, Requestable
-from .guild import Guild
+from .guild import Guild, GuildBoost
 from .interface import AsyncRunnable
 from .message import RawMessage, Message, Event, PublicMessage, PrivateMessage
 from ._types import SoftwareTypes, MessageTypes, SlowModeTypes
 from .user import User
 from .util import unpack_id, unpack_value
 
 log = logging.getLogger(__name__)
@@ -293,9 +294,26 @@
                              topic: str = None,
                              slow_mode: Union[int, SlowModeTypes] = None) -> PublicChannel:
         """update channel's settings"""
         channel = channel if isinstance(channel, PublicChannel) else await self.fetch_public_channel(channel)
         channel_data = await channel.update(name, topic, slow_mode)
         return public_channel_factory(_gate_=self.gate, **channel_data)
 
+    async def fetch_guild_boost(self,
+                                guild: Union[str, Guild],
+                                start_time: int = 0,
+                                end_time: int = int(time.time()),
+                                **kwargs):
+        """
+        list the boost in guild.
+
+        :param guild: guild_id or Guild object.
+        :param start_time: start_time time stamp (Sec).
+        :param end_time: end_time time stamp (Sec). Default to now time.
+        """
+        boost_list = await self.gate.exec_paged_req(
+            api.GuildBoost.history(guild_id=unpack_id(guild), start_time=start_time, end_time=end_time),
+            **kwargs)
+        return [GuildBoost(**item, _gate_=self.gate) for item in boost_list]
+
     async def start(self):
         await asyncio.gather(self.handle_pkg(), self.gate.run(self._pkg_queue))
```

### Comparing `khl.py-0.3.8/khl/receiver.py` & `khl.py-0.3.9/khl/receiver.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/api.py` & `khl.py-0.3.9/khl/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,26 @@
         guild_id,
         user_id,
         type,
     ):
         ...
 
 
+class GuildBoost:
+
+    @staticmethod
+    @req('GET')
+    def history(
+            guild_id,
+            start_time,
+            end_time
+    ):
+        ...
+
+
 class Blacklist:
 
     @staticmethod
     @req('GET')
     def list(
             guild_id
     ):
```

### Comparing `khl.py-0.3.8/khl/user.py` & `khl.py-0.3.9/khl/user.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/permission.py` & `khl.py-0.3.9/khl/permission.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/channel.py` & `khl.py-0.3.9/khl/channel.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/message.py` & `khl.py-0.3.9/khl/message.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/_types.py` & `khl.py-0.3.9/khl/_types.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/interface.py` & `khl.py-0.3.9/khl/interface.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/task/manager.py` & `khl.py-0.3.9/khl/task/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,7 +74,12 @@
         return lambda func: self._scheduler.add_job(func, trigger)
 
     async def start(self):
         self._scheduler.configure({'event_loop': self.loop}, '')
         self._scheduler.add_listener(lambda e: log.exception('error raised during task', exc_info=e.exception),
                                      EVENT_JOB_ERROR)
         self._scheduler.start()  # reminder: this is not blocking
+
+    @property
+    def scheduler(self):
+        """getter, get the scheduler"""
+        return self._scheduler
```

### Comparing `khl.py-0.3.8/khl/game.py` & `khl.py-0.3.9/khl/game.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/role.py` & `khl.py-0.3.9/khl/role.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/requester.py` & `khl.py-0.3.9/khl/requester.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/__init__.py` & `khl.py-0.3.9/khl/__init__.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/card/color.py` & `khl.py-0.3.9/khl/card/color.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/card/module.py` & `khl.py-0.3.9/khl/card/module.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/card/interface.py` & `khl.py-0.3.9/khl/card/interface.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/card/element.py` & `khl.py-0.3.9/khl/card/element.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/card/card.py` & `khl.py-0.3.9/khl/card/card.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl/card/struct.py` & `khl.py-0.3.9/khl/card/struct.py`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl.py.egg-info/SOURCES.txt` & `khl.py-0.3.9/khl.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khl.py-0.3.8/khl.py.egg-info/PKG-INFO` & `khl.py-0.3.9/khl.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khl.py
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python SDK for kaiheila.cn API
 Home-page: https://github.com/TWT233/khl.py
 Author: TWT233
 Author-email: TWT2333@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/TWT233/khl.py/issues
 Project-URL: Tutorial, https://github.com/TWT233/khl.py/tree/main/example
```

### Comparing `khl.py-0.3.8/PKG-INFO` & `khl.py-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khl.py
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python SDK for kaiheila.cn API
 Home-page: https://github.com/TWT233/khl.py
 Author: TWT233
 Author-email: TWT2333@outlook.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/TWT233/khl.py/issues
 Project-URL: Tutorial, https://github.com/TWT233/khl.py/tree/main/example
```

