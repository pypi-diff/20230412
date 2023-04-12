# Comparing `tmp/nonebot_plugin_gshisbanner-0.4.6.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.4.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.4.7.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.4.6.tar` & `nonebot_plugin_gshisbanner-0.4.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/LICENSE
--rw-r--r--   0        0        0     4279 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/README.md
--rw-r--r--   0        0        0      241 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      406 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      287 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3668 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1182 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     4486 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2621 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      576 2023-04-09 03:11:36.647067 nonebot_plugin_gshisbanner-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/LICENSE
+-rw-r--r--   0        0        0     4443 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/README.md
+-rw-r--r--   0        0        0      241 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      406 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      292 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3663 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1182 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     4509 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2654 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      576 2023-04-12 11:18:09.723778 nonebot_plugin_gshisbanner-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.4.7/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.4.6/LICENSE` & `nonebot_plugin_gshisbanner-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.6/README.md` & `nonebot_plugin_gshisbanner-0.4.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,18 +48,20 @@
 # 单次合并转发消息长度（int）,默认为10
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
 
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
-·· 1."banners.52v6.com" #默认
-·· 2."genshin-gacha-banners.vercel.app" #vercel代理，国内可能无法直连
-·· 3."genshin-gacha-banners.52v6.com" #cloudfare代理，可能会被墙
-·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/genshin-gacha-banners/master/public" #ghproxy代理的raw文件，大多数情况可用
+·· 1."banners.52v6.com/data" #默认
+·· 2."genshin-gacha-banners.vercel.app/data" #vercel代理，国内可能无法直连
+·· 3."genshin-gacha-banners.52v6.com/data" #cloudfare代理，可能会被墙
+·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
+     ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
+     ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
 ```
 
 ## 🎉 使用
 ### 指令表
 |        指令         |    权限    | 需要@ | 范围 |                             说明                             |
 | :-----------------: | :--------: | :---: | :--: | :----------------------------------------------------------: |
 | [name]历史卡池(num) |    ALL     |  否   | ALL  | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
```

#### html2text {}

```diff
@@ -10,22 +10,25 @@
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"]  ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
 åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
 # ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸²
 gshisbanner_json_url: str # åå²å¡æ± jsonåè¡¨ä¸è½½ä½ç½® # å¯éå¼ Â·Â·
-1."banners.52v6.com" #é»è®¤ Â·Â· 2."genshin-gacha-banners.vercel.app"
-#vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â· 3."genshin-gacha-
-banners.52v6.com" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â· 4."ghproxy.com/https:
-//raw.githubusercontent.com/KeyPJ/genshin-gacha-banners/master/public"
-#ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ ``` ## ð ä½¿ç¨ ###
-æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :-----------------:
-| :--------: | :---: | :--: | :------------------------------------------------
-----------: | | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+1."banners.52v6.com/data" #é»è®¤ Â·Â· 2."genshin-gacha-banners.vercel.app/
+data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â· 3."genshin-gacha-
+banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â· 4."ghproxy.com/
+https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha"
+##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
+##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
+(å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
+(éè¦æ¯æhttps) ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | | :-----------------: | :--------: | :---: | :--: |
+:----------------------------------------------------------: | |
+[name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
```

### Comparing `nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ) -> Union[Dict, List[Dict]]:
     """
     :param cha: 类型
     :param cache_dir: 本地缓存
     :return: Union[dict, list[dict]]
     """
     cache_dir.mkdir(parents=True, exist_ok=True)
-    url = f"https://{config.gshisbanner_json_url}/data/{'character' if cha else 'weapon'}.json"
+    url = f"https://{config.gshisbanner_json_url}/{'character' if cha else 'weapon'}.json"
     cache_path = cache_dir / ("character.json" if cha else "weapon.json")
     return await load_json_from_url(url, path=cache_path)
 
 
 async def deal_info_from_name(
     name: str, choose: str
 ) -> List[Dict[str, Union[str, List[str]]]]:
```

### Comparing `nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
     )
     # 获取角色真实名字
     real_name, real_type = find_name(type_name)
     if real_name is None or real_type not in ["角色", "武器"]:
         await old_gacha.finish("该角色/武器不存在或是从未up过")
     # 获取up信息
     info = await deal_info_from_name(real_name, "cha" if real_type == "角色" else "wep")
-    await word_send_from_name(bot, event, real_name, info, length)
+    if length > 0:
+        await word_send_from_name(bot, event, real_name, info, length)
     await old_gacha.finish()
 
 
 @version_gacha.handle()
 async def _(bot: Bot, event: MessageEvent, regex_dict: dict = RegexDict()):
     # 判断是否为三卡池的版本
     if regex_dict["version"] not in special_version and regex_dict["upordown"] == "3":
```

### Comparing `nonebot_plugin_gshisbanner-0.4.6/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.4.7/nonebot_plugin_gshisbanner/send.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 DRIVER = get_driver()
 NICKNAME: str = (
     list(DRIVER.config.nickname)[0] if list(DRIVER.config.nickname) else "BOT"
 )
 
 
-# 角色历史卡池文字合并转发处理
+# 角色历史卡池文字合并转发预处理
 async def word_send_from_name(bot, event, real_name, info, length):
     end_time = datetime.strptime(info[0]["end"], "%Y-%m-%d %H:%M:%S").date()
     end_t = (datetime.now().date() - end_time).days
     delta_time = f"最近一次up距离现在已有{end_t}天" if end_t > 0 else f"当前正在up中,距离结束还有约{-end_t}天"
     msg_content = f"{real_name}{delta_time}"
     for i in range(0, len(info), length):
         if i == 0:
             msg = msg_content
         else:
             msg = []
         await send_banner_info(bot, event, msg, info[i: i + length])
 
 
-# 版本卡池文字合并转发处理
+# 版本卡池文字合并转发预处理
 async def word_send_from_version(bot, event, version, info):
     msg_content = f"{version}版本卡池"
     await send_banner_info(bot, event, msg_content, info)
 
 
 # 合并转发
 async def send_forward_msg(bot, event, info):
@@ -41,14 +41,15 @@
         await bot.call_api(
             "send_private_forward_msg",
             user_id=event.user_id,
             messages=info,
         )
 
 
+# 合并转发最终处理
 async def send_banner_info(bot, event, msg_content, banner_info):
     msg = [
         {
             "type": "node",
             "data": {
                 "name": NICKNAME,
                 "uin": event.self_id,
```

### Comparing `nonebot_plugin_gshisbanner-0.4.6/pyproject.toml` & `nonebot_plugin_gshisbanner-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "0.4.6"
+version = "0.4.7"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
 
 [[tool.poetry.source]]
```

### Comparing `nonebot_plugin_gshisbanner-0.4.6/PKG-INFO` & `nonebot_plugin_gshisbanner-0.4.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.4.6
+Version: 0.4.7
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -66,18 +66,20 @@
 # 单次合并转发消息长度（int）,默认为10
 # 越大单次转发内容更多，合并转发的次数更少，越小单单次转发内容更少，但合并转发的次数更多
 # 不要设置为>99或者<0的数字或者任意字符串
 
 gshisbanner_json_url: str
 # 历史卡池json列表下载位置
 # 可选值
-·· 1."banners.52v6.com" #默认
-·· 2."genshin-gacha-banners.vercel.app" #vercel代理，国内可能无法直连
-·· 3."genshin-gacha-banners.52v6.com" #cloudfare代理，可能会被墙
-·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/genshin-gacha-banners/master/public" #ghproxy代理的raw文件，大多数情况可用
+·· 1."banners.52v6.com/data" #默认
+·· 2."genshin-gacha-banners.vercel.app/data" #vercel代理，国内可能无法直连
+·· 3."genshin-gacha-banners.52v6.com/data" #cloudfare代理，可能会被墙
+·· 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha" 
+     ##ghproxy代理的raw文件，大多数情况可用，不过不稳定
+     ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
 ```
 
 ## 🎉 使用
 ### 指令表
 |        指令         |    权限    | 需要@ | 范围 |                             说明                             |
 | :-----------------: | :--------: | :---: | :--: | :----------------------------------------------------------: |
 | [name]历史卡池(num) |    ALL     |  否   | ALL  | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.4.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.4.7 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.1,<3.0) Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0)
@@ -19,22 +19,25 @@
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"]  ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
 åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
 # ä¸è¦è®¾ç½®ä¸º>99æè<0çæ°å­æèä»»æå­ç¬¦ä¸²
 gshisbanner_json_url: str # åå²å¡æ± jsonåè¡¨ä¸è½½ä½ç½® # å¯éå¼ Â·Â·
-1."banners.52v6.com" #é»è®¤ Â·Â· 2."genshin-gacha-banners.vercel.app"
-#vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â· 3."genshin-gacha-
-banners.52v6.com" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â· 4."ghproxy.com/https:
-//raw.githubusercontent.com/KeyPJ/genshin-gacha-banners/master/public"
-#ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ ``` ## ð ä½¿ç¨ ###
-æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :-----------------:
-| :--------: | :---: | :--: | :------------------------------------------------
-----------: | | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+1."banners.52v6.com/data" #é»è®¤ Â·Â· 2."genshin-gacha-banners.vercel.app/
+data" #vercelä»£çï¼å½åå¯è½æ æ³ç´è¿ Â·Â· 3."genshin-gacha-
+banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â· 4."ghproxy.com/
+https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/gacha"
+##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
+##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
+(å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
+(éè¦æ¯æhttps) ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé |
+éè¦@ | èå´ | è¯´æ | | :-----------------: | :--------: | :---: | :--: |
+:----------------------------------------------------------: | |
+[name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
 | | å·æ°åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
```

