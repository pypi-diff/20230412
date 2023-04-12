# Comparing `tmp/nonebot-plugin-chatgpt-0.7.4.tar.gz` & `tmp/nonebot-plugin-chatgpt-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-0.7.4.tar", last modified: Sat Feb 11 17:32:37 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-0.7.5.tar", last modified: Wed Apr 12 08:10:20 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-0.7.4.tar` & `nonebot-plugin-chatgpt-0.7.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/LICENSE
--rw-r--r--   0        0        0     5507 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/README.md
--rw-r--r--   0        0        0     7409 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/__init__.py
--rw-r--r--   0        0        0     9795 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/chatgpt.py
--rw-r--r--   0        0        0      953 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/config.py
--rw-r--r--   0        0        0      815 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/data.py
--rw-r--r--   0        0        0     4084 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/utils.py
--rw-r--r--   0        0        0      685 2023-02-11 17:32:27.811027 nonebot-plugin-chatgpt-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     5885 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/LICENSE
+-rw-r--r--   0        0        0     5507 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/README.md
+-rw-r--r--   0        0        0     7409 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/__init__.py
+-rw-r--r--   0        0        0    10007 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/chatgpt.py
+-rw-r--r--   0        0        0      953 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/config.py
+-rw-r--r--   0        0        0      815 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/data.py
+-rw-r--r--   0        0        0     4084 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/utils.py
+-rw-r--r--   0        0        0      685 2023-04-12 08:10:10.742257 nonebot-plugin-chatgpt-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     5885 1970-01-01 00:00:00.000000 nonebot-plugin-chatgpt-0.7.5/PKG-INFO
```

### Comparing `nonebot-plugin-chatgpt-0.7.4/LICENSE` & `nonebot-plugin-chatgpt-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-0.7.4/README.md` & `nonebot-plugin-chatgpt-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/__init__.py` & `nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/chatgpt.py` & `nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/chatgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,40 +118,38 @@
         await page.goto("https://chat.openai.com/chat")
         yield page
         await page.close()
 
     async def get_chat_response(self, prompt: str) -> str:
         async with self.get_page() as page:
             await page.wait_for_load_state("domcontentloaded")
-            if not await page.locator("text=OpenAI Discord").is_visible():
+            if not await page.locator("text=Updates & FAQ").is_visible():
                 await self.get_cf_cookies(page)
             logger.debug("正在发送请求")
 
             async def change_json(route: Route):
                 await route.continue_(
                     post_data=json.dumps(self.get_payload(prompt)),
                 )
 
             await self.content.route(
                 "https://chat.openai.com/backend-api/conversation", change_json
             )
             await page.wait_for_load_state("domcontentloaded")
-            await page.wait_for_load_state("networkidle")
             session_expired = page.locator("button", has_text="Log in")
             if await session_expired.is_visible():
                 logger.debug("检测到session过期")
                 return "token失效，请重新设置token"
-            next_botton = page.locator(
-                ".btn.flex.justify-center.gap-2.btn-neutral.ml-auto"
-            )
+            next_botton = page.get_by_role("button", name="Next")
+            next_botton2 = page.get_by_role("button", name="Done")
             if await next_botton.is_visible():
                 logger.debug("检测到初次打开弹窗")
                 await next_botton.click()
                 await next_botton.click()
-                await page.click(".btn.flex.justify-center.gap-2.btn-primary.ml-auto")
+                await next_botton2.click()
             async with page.expect_response(
                 "https://chat.openai.com/backend-api/conversation",
                 timeout=self.timeout * 1000,
             ) as response_info:
                 textarea = page.locator("textarea")
                 botton = page.locator('button[class="absolute p-1 rounded-md text-gray-500 bottom-1.5 right-1 md:bottom-2.5 md:right-2 hover:bg-gray-100 dark:hover:text-gray-400 dark:hover:bg-gray-900 disabled:hover:bg-transparent dark:disabled:hover:bg-transparent"]')
                 logger.debug("正在等待回复")
@@ -183,15 +181,15 @@
 
     async def refresh_session(self) -> None:
         logger.debug("正在刷新session")
         if self.auto_auth:
             await self.login()
         else:
             async with self.get_page() as page:
-                if not await page.locator("text=OpenAI Discord").is_visible():
+                if not await page.locator("text=Updates & FAQ").is_visible():
                     await self.get_cf_cookies(page)
                 await page.wait_for_load_state("domcontentloaded")
                 session_expired = page.locator("text=Your session has expired")
                 if await session_expired.count():
                     logger.opt(colors=True).error("刷新会话失败, session token 已过期, 请重新设置")
             cookies = await self.content.cookies()
             for i in cookies:
@@ -231,14 +229,20 @@
         for _ in range(20):
             button = page.get_by_role("button", name="Verify you are human")
             if await button.count():
                 await button.click()
             label = page.locator("label span")
             if await label.count():
                 await label.click()
+            try:
+                label2 = page.frame_locator("iframe[title=\"Widget containing a Cloudflare security challenge\"]").get_by_label("Verify you are human")
+                if await label2.count():
+                    await label2.check()
+            except Exception as _:
+                pass
             await page.wait_for_timeout(1000)
-            cf = page.locator("text=OpenAI Discord")
+            cf = page.locator("text=Updates & FAQ")
             if await cf.is_visible():
                 break
         else:
             logger.error("cf cookies获取失败")
         logger.debug("cf cookies获取成功")
```

### Comparing `nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/config.py` & `nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/data.py` & `nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/data.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-0.7.4/nonebot_plugin_chatgpt/utils.py` & `nonebot-plugin-chatgpt-0.7.5/nonebot_plugin_chatgpt/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-0.7.4/pyproject.toml` & `nonebot-plugin-chatgpt-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-chatgpt"
-version = "0.7.4"
+version = "0.7.5"
 description = "NoneBot2 plugin for AI chat"
 authors = [
     { name = "Akirami", email = "Akiramiaya@outlook.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc2",
     "nonebot-adapter-onebot>=2.1.5",
```

### Comparing `nonebot-plugin-chatgpt-0.7.4/PKG-INFO` & `nonebot-plugin-chatgpt-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt
-Version: 0.7.4
+Version: 0.7.5
 Summary: NoneBot2 plugin for AI chat
 License: MIT
 Author-email: Akirami <Akiramiaya@outlook.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/A-kirami/nonebot-plugin-chatgpt
 Project-URL: Repository, https://github.com/A-kirami/nonebot-plugin-chatgpt
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt Version: 0.7.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-chatgpt Version: 0.7.5 Summary:
 NoneBot2 plugin for AI chat License: MIT Author-email: Akirami
 outlook.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 A-kirami/nonebot-plugin-chatgpt Project-URL: Repository, https://github.com/A-
 kirami/nonebot-plugin-chatgpt Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
 # nonebot-plugin-chatgpt _â¨ ChatGPT AI å¯¹è¯ â¨_ [license] [pypi] [python]
```

