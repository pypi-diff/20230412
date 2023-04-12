# Comparing `tmp/nonebot-plugin-chatgpt-plus-0.8.3.tar.gz` & `tmp/nonebot-plugin-chatgpt-plus-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.3.tar", last modified: Wed Apr  5 15:51:34 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-plus-0.8.4.tar", last modified: Wed Apr 12 09:14:49 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-plus-0.8.3.tar` & `nonebot-plugin-chatgpt-plus-0.8.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/LICENSE
--rw-r--r--   0        0        0     6841 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/README.md
--rw-r--r--   0        0        0    12750 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/__init__.py
--rw-r--r--   0        0        0    13419 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/chatgpt.py
--rw-r--r--   0        0        0     1032 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/config.py
--rw-r--r--   0        0        0      892 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/data.py
--rw-r--r--   0        0        0     5678 2023-04-05 15:51:27.736403 nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/utils.py
--rw-r--r--   0        0        0      725 2023-04-05 15:51:27.740403 nonebot-plugin-chatgpt-plus-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     7238 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/LICENSE
+-rw-r--r--   0        0        0     6921 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/README.md
+-rw-r--r--   0        0        0    13268 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/__init__.py
+-rw-r--r--   0        0        0    14117 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/chatgpt.py
+-rw-r--r--   0        0        0     1032 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/config.py
+-rw-r--r--   0        0        0      892 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/data.py
+-rw-r--r--   0        0        0     5678 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/utils.py
+-rw-r--r--   0        0        0      725 2023-04-12 09:14:37.807643 nonebot-plugin-chatgpt-plus-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     7318 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-plus-0.8.4/PKG-INFO
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/LICENSE` & `nonebot-plugin-chatgpt-plus-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/README.md` & `nonebot-plugin-chatgpt-plus-0.8.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 | CHATGPT_SESSION_TOKEN | 否 | 空字符串 | ChatGPT 的 session_token，如配置则优先使用 |
 | CHATGPT_PUID | 否 | 空字符串 | ChatGPT PLUS账号的puid，使用官方API必填 |
 | CHATGPT_MODEL | 否 | 空字符串 | 模型，免费账号只有一个，PLUS账号可使用`gpt-4` |
 | CHATGPT_ACCOUNT | 否 | 空字符串 | ChatGPT 登陆邮箱，未配置则使用 session_token |
 | CHATGPT_PASSWORD | 否 | 空字符串 | ChatGPT 登陆密码，未配置则使用 session_token |
 | CHATGPT_CD_TIME | 否 | 60 | 冷却时间，单位：秒|
 | CHATGPT_NOTICE | 否 | True | 收到请求时进行回复提醒 |
+| CHATGPT_AUTO_REFRESH | 否 | True | 会话不存在时，自动刷新会话 |
 | CHATGPT_PROXIES | 否 | None | 代理地址，格式为： `http://ip:port` |
 | CHATGPT_REFRESH_INTERVAL | 否 | 30 | session_token 自动刷新间隔，单位：分钟 |
 | CHATGPT_COMMAND | 否 | 空字符串 | 触发聊天的命令，可以是 `字符串` 或者 `字符串列表`。<br>如果为空字符串或者空列表，则默认响应全部消息  |
 | CHATGPT_TO_ME | 否 | True | 是否需要@机器人 |
 | CHATGPT_TIMEOUT | 否 | 30 | 请求服务器的超时时间，单位：秒 |
 | CHATGPT_API | 否 | https://chat.loli.vet/ | API 地址，可配置反代，默认值可绕CF盾 |
 | CHATGPT_IMAGE | 否 | False | 是否以图片形式发送。<br>如果无法显示文字，请[点击此处](https://github.com/kexue-z/nonebot-plugin-htmlrender#%E5%B8%B8%E8%A7%81%E7%96%91%E9%9A%BE%E6%9D%82%E7%97%87)查看解决办法 |
```

#### html2text {}

```diff
@@ -25,15 +25,16 @@
 session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_PUID | å¦ | ç©ºå­ç¬¦ä¸²
 | ChatGPT PLUSè´¦å·çpuidï¼ä½¿ç¨å®æ¹APIå¿å¡« | | CHATGPT_MODEL | å¦ |
 ç©ºå­ç¬¦ä¸² | æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` |
 | CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
 ç»éé®ç®±ï¼æªéç½®åä½¿ç¨ session_token | | CHATGPT_PASSWORD | å¦ |
 ç©ºå­ç¬¦ä¸² | ChatGPT ç»éå¯ç ï¼æªéç½®åä½¿ç¨ session_token | |
 CHATGPT_CD_TIME | å¦ | 60 | å·å´æ¶é´ï¼åä½ï¼ç§| | CHATGPT_NOTICE |
-å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_PROXIES | å¦ | None
+å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_AUTO_REFRESH | å¦ |
+True | ä¼è¯ä¸å­å¨æ¶ï¼èªå¨å·æ°ä¼è¯ | | CHATGPT_PROXIES | å¦ | None
 | ä»£çå°åï¼æ ¼å¼ä¸ºï¼ `http://ip:port` | | CHATGPT_REFRESH_INTERVAL |
 å¦ | 30 | session_token èªå¨å·æ°é´éï¼åä½ï¼åé | |
 CHATGPT_COMMAND | å¦ | ç©ºå­ç¬¦ä¸² | è§¦åèå¤©çå½ä»¤ï¼å¯ä»¥æ¯
 `å­ç¬¦ä¸²` æè `å­ç¬¦ä¸²åè¡¨`ã
 å¦æä¸ºç©ºå­ç¬¦ä¸²æèç©ºåè¡¨ï¼åé»è®¤ååºå¨é¨æ¶æ¯ | |
 CHATGPT_TO_ME | å¦ | True | æ¯å¦éè¦@æºå¨äºº | | CHATGPT_TIMEOUT | å¦ |
 30 | è¯·æ±æå¡å¨çè¶æ¶æ¶é´ï¼åä½ï¼ç§ | | CHATGPT_API | å¦ |
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/__init__.py` & `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,14 +125,25 @@
         msg = await chat_bot(**cvst, played_name=played_name).get_chat_response(text)
         if (
             msg == "token失效，请重新设置token"
             and chat_bot.session_token != config.chatgpt_session_token
         ):
             chat_bot.session_token = config.chatgpt_session_token
             msg = await chat_bot(**cvst, played_name=played_name).get_chat_response(text)
+        elif (
+            msg == "会话不存在"
+        ):
+            if config.chatgpt_auto_refresh:
+                has_title = False
+                cvst['conversation_id'].append(None)
+                cvst['parent_id'].append(chat_bot.id)
+                await matcher.send("会话不存在，已自动刷新对话，等待响应...", reply_message=True)
+                msg = await chat_bot(**cvst, played_name=played_name).get_chat_response(text)
+            else:
+                msg += ",请刷新会话"
     except Exception as e:
         lockers[event.user_id] = False
         error = f"{type(e).__name__}: {e}"
         logger.opt(exception=e).error(f"ChatGPT request failed: {error}")
         await matcher.finish(
             f"请求 ChatGPT 服务器时出现问题，请稍后再试\n错误信息: {error}", reply_message=True
         )
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/chatgpt.py` & `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/chatgpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import uuid
+import httpx
+
 from typing import Any, Dict, Optional
+from typing_extensions import Self
 from urllib.parse import urljoin
-
-import httpx
 from nonebot.log import logger
-from nonebot.utils import escape_tag, run_sync
-from typing_extensions import Self
+from nonebot.utils import escape_tag
 
 from .utils import convert_seconds
 
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
@@ -48,14 +48,16 @@
 
         if self.session_token:
             self.auto_auth = False
         elif self.account and self.password:
             self.auto_auth = True
         else:
             raise ValueError("至少需要配置 session_token 或者 account 和 password")
+        if self.api_url.startswith('https://chat.openai.com') and not self.plus_puid:
+            raise ValueError("使用官方API请配置puid")
 
     def __call__(
         self, conversation_id: Optional[str] = None, parent_id: Optional[str] = None, played_name: Optional[str] = None
     ) -> Self:
         self.conversation_id = conversation_id[-1] if conversation_id else None
         self.parent_id = parent_id[-1] if parent_id else self.id
         self.played_name = played_name
@@ -78,15 +80,15 @@
             "Referer": "https://chat.openai.com/chat",
         }
     
     def get_played_info(self, name: str) -> Dict[str, Any]:
         return {
             "id": self.id,
             "author": {
-                "role": "system",
+                "role": "tool",
                 "name": name,
                 "metadata": {}
             },
             "content": {
                 "content_type": "text",
                 "parts": [
                     "You must follow the user's instructions to play the specified role in the first person and give the response information according to the changed role. If necessary, you can generate a reply in the specified format to call the extension function.",
@@ -137,28 +139,39 @@
                 headers=self.headers,
                 json=self.get_payload(prompt),
                 cookies=cookies,
                 timeout=self.timeout,
             ) as response:
                 if response.status_code == 429:
                     msg = ""
-                    resp: dict = response.json()
+                    _buffer = bytearray()
+                    async for chunk in response.aiter_bytes():
+                        _buffer.extend(chunk)
+                    resp: dict = json.loads(_buffer.decode())
                     if detail := resp.get('detail'):
                         if isinstance(detail, str):
                             msg += "\n" + detail
                         elif seconds := detail.get('clears_in'):
                             msg = f"\n请在 {convert_seconds(seconds)} 后重试"
                     return "请求过多，请放慢速度" + msg
                 if response.status_code == 401:
                     return "token失效，请重新设置token"
+                if response.status_code == 403:
+                    return "API错误，请联系开发者修复"
+                if response.status_code == 404:
+                    return "会话不存在"
                 if response.is_error:
+                    _buffer = bytearray()
+                    async for chunk in response.aiter_bytes():
+                        _buffer.extend(chunk)
+                    resp_text = _buffer.decode()
                     logger.opt(colors=True).error(
-                        f"非预期的响应内容: <r>HTTP{response.status_code}</r> {escape_tag(response.text)}"
+                        f"非预期的响应内容: <r>HTTP{response.status_code}</r> {escape_tag(resp_text)}"
                     )
-                    return f"ChatGPT 服务器返回了非预期的内容: HTTP{response.status_code}\n{escape_tag(response.text)}"
+                    return f"ChatGPT 服务器返回了非预期的内容: HTTP{response.status_code}\n{escape_tag(resp_text)}"
                 data_list = []
                 async for line in response.aiter_lines():
                     if line.startswith("data:"):
                         data = line[6:]
                         if data.startswith("{"):
                             try:
                                 data_list.append(json.loads(data))
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/config.py` & `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/data.py` & `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/data.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/nonebot_plugin_chatgpt_plus/utils.py` & `nonebot-plugin-chatgpt-plus-0.8.4/nonebot_plugin_chatgpt_plus/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from collections import defaultdict, deque
 import json
+
+from collections import defaultdict, deque
 from pathlib import Path
 from typing import (
     Any,
     AsyncGenerator,
     Dict,
     List,
     Literal,
@@ -56,15 +57,15 @@
 def single_run_locker() -> Any:
     async def check_running(
         matcher: Matcher, event: MessageEvent
     ) -> AsyncGenerator[None, None]:
         lockers[event.user_id] = lockers[event.user_id]
         if lockers[event.user_id]:
             await matcher.finish(
-                f"我知道你很急，但你先别急", reply_message=True
+                "我知道你很急，但你先别急", reply_message=True
             )
         yield
 
     return Depends(check_running)
 
 def create_matcher(
     command: Union[str, List[str]],
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/pyproject.toml` & `nonebot-plugin-chatgpt-plus-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-chatgpt-plus"
-version = "0.8.3"
+version = "0.8.4"
 description = "NoneBot2 plugin for AI chat"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-chatgpt-plus-0.8.3/PKG-INFO` & `nonebot-plugin-chatgpt-plus-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-plus
-Version: 0.8.3
+Version: 0.8.4
 Summary: NoneBot2 plugin for AI chat
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Project-URL: Repository, https://github.com/AkashiCoin/nonebot-plugin-chatgpt-plus
 Description-Content-Type: text/markdown
@@ -93,14 +93,15 @@
 | CHATGPT_SESSION_TOKEN | 否 | 空字符串 | ChatGPT 的 session_token，如配置则优先使用 |
 | CHATGPT_PUID | 否 | 空字符串 | ChatGPT PLUS账号的puid，使用官方API必填 |
 | CHATGPT_MODEL | 否 | 空字符串 | 模型，免费账号只有一个，PLUS账号可使用`gpt-4` |
 | CHATGPT_ACCOUNT | 否 | 空字符串 | ChatGPT 登陆邮箱，未配置则使用 session_token |
 | CHATGPT_PASSWORD | 否 | 空字符串 | ChatGPT 登陆密码，未配置则使用 session_token |
 | CHATGPT_CD_TIME | 否 | 60 | 冷却时间，单位：秒|
 | CHATGPT_NOTICE | 否 | True | 收到请求时进行回复提醒 |
+| CHATGPT_AUTO_REFRESH | 否 | True | 会话不存在时，自动刷新会话 |
 | CHATGPT_PROXIES | 否 | None | 代理地址，格式为： `http://ip:port` |
 | CHATGPT_REFRESH_INTERVAL | 否 | 30 | session_token 自动刷新间隔，单位：分钟 |
 | CHATGPT_COMMAND | 否 | 空字符串 | 触发聊天的命令，可以是 `字符串` 或者 `字符串列表`。<br>如果为空字符串或者空列表，则默认响应全部消息  |
 | CHATGPT_TO_ME | 否 | True | 是否需要@机器人 |
 | CHATGPT_TIMEOUT | 否 | 30 | 请求服务器的超时时间，单位：秒 |
 | CHATGPT_API | 否 | https://chat.loli.vet/ | API 地址，可配置反代，默认值可绕CF盾 |
 | CHATGPT_IMAGE | 否 | False | 是否以图片形式发送。<br>如果无法显示文字，请[点击此处](https://github.com/kexue-z/nonebot-plugin-htmlrender#%E5%B8%B8%E8%A7%81%E7%96%91%E9%9A%BE%E6%9D%82%E7%97%87)查看解决办法 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt-plus Version: 0.8.4 Summary:
 NoneBot2 plugin for AI chat License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 AkashiCoin/nonebot-plugin-chatgpt-plus Project-URL: Repository, https://
 github.com/AkashiCoin/nonebot-plugin-chatgpt-plus Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -31,15 +31,16 @@
 session_tokenï¼å¦éç½®åä¼åä½¿ç¨ | | CHATGPT_PUID | å¦ | ç©ºå­ç¬¦ä¸²
 | ChatGPT PLUSè´¦å·çpuidï¼ä½¿ç¨å®æ¹APIå¿å¡« | | CHATGPT_MODEL | å¦ |
 ç©ºå­ç¬¦ä¸² | æ¨¡åï¼åè´¹è´¦å·åªæä¸ä¸ªï¼PLUSè´¦å·å¯ä½¿ç¨`gpt-4` |
 | CHATGPT_ACCOUNT | å¦ | ç©ºå­ç¬¦ä¸² | ChatGPT
 ç»éé®ç®±ï¼æªéç½®åä½¿ç¨ session_token | | CHATGPT_PASSWORD | å¦ |
 ç©ºå­ç¬¦ä¸² | ChatGPT ç»éå¯ç ï¼æªéç½®åä½¿ç¨ session_token | |
 CHATGPT_CD_TIME | å¦ | 60 | å·å´æ¶é´ï¼åä½ï¼ç§| | CHATGPT_NOTICE |
-å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_PROXIES | å¦ | None
+å¦ | True | æ¶å°è¯·æ±æ¶è¿è¡åå¤æé | | CHATGPT_AUTO_REFRESH | å¦ |
+True | ä¼è¯ä¸å­å¨æ¶ï¼èªå¨å·æ°ä¼è¯ | | CHATGPT_PROXIES | å¦ | None
 | ä»£çå°åï¼æ ¼å¼ä¸ºï¼ `http://ip:port` | | CHATGPT_REFRESH_INTERVAL |
 å¦ | 30 | session_token èªå¨å·æ°é´éï¼åä½ï¼åé | |
 CHATGPT_COMMAND | å¦ | ç©ºå­ç¬¦ä¸² | è§¦åèå¤©çå½ä»¤ï¼å¯ä»¥æ¯
 `å­ç¬¦ä¸²` æè `å­ç¬¦ä¸²åè¡¨`ã
 å¦æä¸ºç©ºå­ç¬¦ä¸²æèç©ºåè¡¨ï¼åé»è®¤ååºå¨é¨æ¶æ¯ | |
 CHATGPT_TO_ME | å¦ | True | æ¯å¦éè¦@æºå¨äºº | | CHATGPT_TIMEOUT | å¦ |
 30 | è¯·æ±æå¡å¨çè¶æ¶æ¶é´ï¼åä½ï¼ç§ | | CHATGPT_API | å¦ |
```

