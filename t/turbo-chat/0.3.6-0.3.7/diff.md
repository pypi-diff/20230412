# Comparing `tmp/turbo_chat-0.3.6.tar.gz` & `tmp/turbo_chat-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_chat-0.3.6.tar", max compression
+gzip compressed data, was "turbo_chat-0.3.7.tar", max compression
```

## Comparing `turbo_chat-0.3.6.tar` & `turbo_chat-0.3.7.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0     1075 2023-03-27 06:50:49.642216 turbo_chat-0.3.6/LICENSE
--rw-r--r--   0        0        0     9573 2023-04-05 05:13:21.205711 turbo_chat-0.3.6/README.md
--rw-r--r--   0        0        0     1124 2023-04-05 05:14:30.918587 turbo_chat-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      898 2023-04-05 05:13:21.209711 turbo_chat-0.3.6/turbo_chat/__init__.py
--rw-r--r--   0        0        0      237 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/__init__.py
--rw-r--r--   0        0        0      520 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/qa.py
--rw-r--r--   0        0        0     1377 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/self_ask.py
--rw-r--r--   0        0        0       72 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/subqueries/__init__.py
--rw-r--r--   0        0        0     1887 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/bots/subqueries/bot.py
--rw-r--r--   0        0        0      636 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/subqueries/scratchpad.py
--rw-r--r--   0        0        0     1747 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/subqueries/template.py
--rw-r--r--   0        0        0      422 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/bots/summarize.py
--rw-r--r--   0        0        0       66 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/bots/tool/__init__.py
--rw-r--r--   0        0        0     4270 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/bots/tool/bot.py
--rw-r--r--   0        0        0      426 2023-03-29 09:31:03.306136 turbo_chat-0.3.6/turbo_chat/bots/tool/scratchpad.py
--rw-r--r--   0        0        0     2940 2023-04-03 13:40:06.231883 turbo_chat-0.3.6/turbo_chat/bots/tool/template.py
--rw-r--r--   0        0        0      154 2023-04-05 05:13:21.209711 turbo_chat-0.3.6/turbo_chat/cache/__init__.py
--rw-r--r--   0        0        0     1324 2023-04-05 05:13:21.209711 turbo_chat-0.3.6/turbo_chat/cache/redis.py
--rw-r--r--   0        0        0      638 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/cache/simple.py
--rw-r--r--   0        0        0     1111 2023-03-27 07:04:17.075676 turbo_chat-0.3.6/turbo_chat/chat.py
--rw-r--r--   0        0        0     1277 2023-04-03 13:40:06.231883 turbo_chat-0.3.6/turbo_chat/completion.py
--rw-r--r--   0        0        0      446 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/config.py
--rw-r--r--   0        0        0      488 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/errors.py
--rw-r--r--   0        0        0      239 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/memory/__init__.py
--rw-r--r--   0        0        0      788 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/memory/local_memory.py
--rw-r--r--   0        0        0     1358 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/memory/summary_memory.py
--rw-r--r--   0        0        0     1604 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/memory/truncated_memory.py
--rw-r--r--   0        0        0      796 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/runner.py
--rw-r--r--   0        0        0      356 2023-03-27 09:35:21.119756 turbo_chat-0.3.6/turbo_chat/structs/__init__.py
--rw-r--r--   0        0        0     1198 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/structs/messages.py
--rw-r--r--   0        0        0      968 2023-03-28 17:49:03.767496 turbo_chat-0.3.6/turbo_chat/structs/proxies.py
--rw-r--r--   0        0        0      795 2023-03-29 09:31:03.306136 turbo_chat-0.3.6/turbo_chat/structs/result.py
--rw-r--r--   0        0        0     1567 2023-04-05 05:13:21.209711 turbo_chat-0.3.6/turbo_chat/structs/scratchpad.py
--rw-r--r--   0        0        0      495 2023-03-29 07:56:38.680320 turbo_chat-0.3.6/turbo_chat/structs/signals.py
--rw-r--r--   0        0        0     5832 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/turbo.py
--rw-r--r--   0        0        0      360 2023-03-29 09:31:03.310136 turbo_chat-0.3.6/turbo_chat/types/__init__.py
--rw-r--r--   0        0        0      770 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/types/cache.py
--rw-r--r--   0        0        0      841 2023-03-28 17:49:03.767496 turbo_chat-0.3.6/turbo_chat/types/generators.py
--rw-r--r--   0        0        0     3387 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/types/memory.py
--rw-r--r--   0        0        0     3029 2023-03-30 10:03:00.267473 turbo_chat-0.3.6/turbo_chat/types/messages.py
--rw-r--r--   0        0        0       74 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/types/misc.py
--rw-r--r--   0        0        0      218 2023-03-29 09:31:03.314136 turbo_chat-0.3.6/turbo_chat/types/tools.py
--rw-r--r--   0        0        0      300 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/utils/__init__.py
--rw-r--r--   0        0        0     1111 2023-04-03 13:40:06.231883 turbo_chat-0.3.6/turbo_chat/utils/args.py
--rw-r--r--   0        0        0      425 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/utils/fn.py
--rw-r--r--   0        0        0      137 2023-03-27 09:38:54.782616 turbo_chat-0.3.6/turbo_chat/utils/lang.py
--rw-r--r--   0        0        0      355 2023-03-29 12:12:23.477099 turbo_chat-0.3.6/turbo_chat/utils/pprint.py
--rw-r--r--   0        0        0     1110 2023-03-27 06:50:49.646216 turbo_chat-0.3.6/turbo_chat/utils/retries.py
--rw-r--r--   0        0        0     1029 2023-04-03 13:40:06.231883 turbo_chat-0.3.6/turbo_chat/utils/template.py
--rw-r--r--   0        0        0     2050 2023-03-27 09:39:01.086701 turbo_chat-0.3.6/turbo_chat/utils/tokens.py
--rw-r--r--   0        0        0    10680 1970-01-01 00:00:00.000000 turbo_chat-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-27 06:50:49.642216 turbo_chat-0.3.7/LICENSE
+-rw-r--r--   0        0        0    10839 2023-04-12 08:40:24.985314 turbo_chat-0.3.7/README.md
+-rw-r--r--   0        0        0     1276 2023-04-12 08:40:24.989314 turbo_chat-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      898 2023-04-05 05:13:21.209711 turbo_chat-0.3.7/turbo_chat/__init__.py
+-rw-r--r--   0        0        0      237 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/__init__.py
+-rw-r--r--   0        0        0      520 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/qa.py
+-rw-r--r--   0        0        0     1377 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/self_ask.py
+-rw-r--r--   0        0        0       72 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/subqueries/__init__.py
+-rw-r--r--   0        0        0     1887 2023-03-30 10:03:00.267473 turbo_chat-0.3.7/turbo_chat/bots/subqueries/bot.py
+-rw-r--r--   0        0        0      636 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/subqueries/scratchpad.py
+-rw-r--r--   0        0        0     1747 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/subqueries/template.py
+-rw-r--r--   0        0        0      422 2023-03-30 10:03:00.267473 turbo_chat-0.3.7/turbo_chat/bots/summarize.py
+-rw-r--r--   0        0        0       66 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/bots/tool/__init__.py
+-rw-r--r--   0        0        0     4270 2023-03-30 10:03:00.267473 turbo_chat-0.3.7/turbo_chat/bots/tool/bot.py
+-rw-r--r--   0        0        0      426 2023-03-29 09:31:03.306136 turbo_chat-0.3.7/turbo_chat/bots/tool/scratchpad.py
+-rw-r--r--   0        0        0     2940 2023-04-03 13:40:06.231883 turbo_chat-0.3.7/turbo_chat/bots/tool/template.py
+-rw-r--r--   0        0        0      154 2023-04-05 05:13:21.209711 turbo_chat-0.3.7/turbo_chat/cache/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-12 03:09:32.852539 turbo_chat-0.3.7/turbo_chat/cache/redis.py
+-rw-r--r--   0        0        0      638 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/cache/simple.py
+-rw-r--r--   0        0        0     1303 2023-04-12 08:29:36.369017 turbo_chat-0.3.7/turbo_chat/chat.py
+-rw-r--r--   0        0        0     1343 2023-04-12 06:52:00.686614 turbo_chat-0.3.7/turbo_chat/completion.py
+-rw-r--r--   0        0        0      446 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/config.py
+-rw-r--r--   0        0        0      488 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/errors.py
+-rw-r--r--   0        0        0      239 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/memory/__init__.py
+-rw-r--r--   0        0        0      788 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/memory/local_memory.py
+-rw-r--r--   0        0        0     1358 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/memory/summary_memory.py
+-rw-r--r--   0        0        0     1604 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/memory/truncated_memory.py
+-rw-r--r--   0        0        0      796 2023-04-11 16:57:02.142061 turbo_chat-0.3.7/turbo_chat/runner.py
+-rw-r--r--   0        0        0      356 2023-03-27 09:35:21.119756 turbo_chat-0.3.7/turbo_chat/structs/__init__.py
+-rw-r--r--   0        0        0     1198 2023-03-30 10:03:00.267473 turbo_chat-0.3.7/turbo_chat/structs/messages.py
+-rw-r--r--   0        0        0      968 2023-03-28 17:49:03.767496 turbo_chat-0.3.7/turbo_chat/structs/proxies.py
+-rw-r--r--   0        0        0      795 2023-03-29 09:31:03.306136 turbo_chat-0.3.7/turbo_chat/structs/result.py
+-rw-r--r--   0        0        0     1567 2023-04-05 05:13:21.209711 turbo_chat-0.3.7/turbo_chat/structs/scratchpad.py
+-rw-r--r--   0        0        0      495 2023-03-29 07:56:38.680320 turbo_chat-0.3.7/turbo_chat/structs/signals.py
+-rw-r--r--   0        0        0     6262 2023-04-12 08:29:36.369017 turbo_chat-0.3.7/turbo_chat/turbo.py
+-rw-r--r--   0        0        0      360 2023-03-29 09:31:03.310136 turbo_chat-0.3.7/turbo_chat/types/__init__.py
+-rw-r--r--   0        0        0      770 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/types/cache.py
+-rw-r--r--   0        0        0      855 2023-04-12 06:52:00.686614 turbo_chat-0.3.7/turbo_chat/types/generators.py
+-rw-r--r--   0        0        0     3387 2023-03-30 10:03:00.267473 turbo_chat-0.3.7/turbo_chat/types/memory.py
+-rw-r--r--   0        0        0     3029 2023-03-30 10:03:00.267473 turbo_chat-0.3.7/turbo_chat/types/messages.py
+-rw-r--r--   0        0        0       74 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/types/misc.py
+-rw-r--r--   0        0        0      218 2023-03-29 09:31:03.314136 turbo_chat-0.3.7/turbo_chat/types/tools.py
+-rw-r--r--   0        0        0      300 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/utils/__init__.py
+-rw-r--r--   0        0        0     1111 2023-04-03 13:40:06.231883 turbo_chat-0.3.7/turbo_chat/utils/args.py
+-rw-r--r--   0        0        0  1681126 2023-04-12 06:17:06.606268 turbo_chat-0.3.7/turbo_chat/utils/cl100k_base.tiktoken
+-rw-r--r--   0        0        0     2589 2023-04-12 08:29:36.373017 turbo_chat-0.3.7/turbo_chat/utils/debug.py
+-rw-r--r--   0        0        0      425 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/utils/fn.py
+-rw-r--r--   0        0        0      137 2023-03-27 09:38:54.782616 turbo_chat-0.3.7/turbo_chat/utils/lang.py
+-rw-r--r--   0        0        0      343 2023-04-12 08:29:36.373017 turbo_chat-0.3.7/turbo_chat/utils/pprint.py
+-rw-r--r--   0        0        0     1110 2023-03-27 06:50:49.646216 turbo_chat-0.3.7/turbo_chat/utils/retries.py
+-rw-r--r--   0        0        0     1029 2023-04-03 13:40:06.231883 turbo_chat-0.3.7/turbo_chat/utils/template.py
+-rw-r--r--   0        0        0     3711 2023-04-12 06:17:06.610268 turbo_chat-0.3.7/turbo_chat/utils/tokens.py
+-rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 turbo_chat-0.3.7/PKG-INFO
```

### Comparing `turbo_chat-0.3.6/LICENSE` & `turbo_chat-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/README.md` & `turbo_chat-0.3.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -179,14 +179,23 @@
 
 ```
 
 ---
 
 ### Latest Changes
 
+* version: 0.3.7. PR [#57](https://github.com/creatorrr/turbo-chat/pull/57) by [@creatorrr](https://github.com/creatorrr).
+* f/support multi choice. PR [#56](https://github.com/creatorrr/turbo-chat/pull/56) by [@creatorrr](https://github.com/creatorrr).
+* feat: Support multiple choices selector; n > 1. PR [#55](https://github.com/creatorrr/turbo-chat/pull/55) by [@creatorrr](https://github.com/creatorrr).
+* feat: Support positional arguments for running apps. PR [#54](https://github.com/creatorrr/turbo-chat/pull/54) by [@creatorrr](https://github.com/creatorrr).
+* feat: Make get_encoding faster. PR [#53](https://github.com/creatorrr/turbo-chat/pull/53) by [@creatorrr](https://github.com/creatorrr).
+* feat: Add ttl support to redis_cache. PR [#52](https://github.com/creatorrr/turbo-chat/pull/52) by [@creatorrr](https://github.com/creatorrr).
+* feat: Support for parsing completions. PR [#51](https://github.com/creatorrr/turbo-chat/pull/51) by [@creatorrr](https://github.com/creatorrr).
+* version: 0.3.6. PR [#50](https://github.com/creatorrr/turbo-chat/pull/50) by [@creatorrr](https://github.com/creatorrr).
+* feat: Add RedisCache implementation. PR [#49](https://github.com/creatorrr/turbo-chat/pull/49) by [@creatorrr](https://github.com/creatorrr).
 * fix: Fix json array. PR [#48](https://github.com/creatorrr/turbo-chat/pull/48) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.5. PR [#47](https://github.com/creatorrr/turbo-chat/pull/47) by [@creatorrr](https://github.com/creatorrr).
 * fix: Fix how function signature and docstring was being parsed. PR [#46](https://github.com/creatorrr/turbo-chat/pull/46) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.4. PR [#45](https://github.com/creatorrr/turbo-chat/pull/45) by [@creatorrr](https://github.com/creatorrr).
 * feat: Add @completion decorator. PR [#44](https://github.com/creatorrr/turbo-chat/pull/44) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.3. PR [#43](https://github.com/creatorrr/turbo-chat/pull/43) by [@creatorrr](https://github.com/creatorrr).
 * feat: Memory expects memory_args, Assistant no longer yields automatically. PR [#42](https://github.com/creatorrr/turbo-chat/pull/42) by [@creatorrr](https://github.com/creatorrr).
```

### Comparing `turbo_chat-0.3.6/pyproject.toml` & `turbo_chat-0.3.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turbo-chat"
-version = "0.3.6"
+version = "0.3.7"
 description = "Idiomatic way to build chatgpt apps using async generators in python"
 authors = ["Diwank Singh Tomer <singh@diwank.name>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "turbo_chat"}]
 
 [tool.poetry.dependencies]
@@ -18,26 +18,30 @@
 jinja2 = "^3.1.2"
 jinja2schema = "^0.1.4"
 jsonschema = "^4.17.3"
 lemminflect = "^0.2.3"
 proxytypes = "^0.10.0"
 dirtyjson = "^1.0.8"
 redis = {version = ">=4.5.0,<5.0.0", optional = true}
+pygments = {version = "^2.15.0", optional = true}
+colorama = {version = "^0.4.6", optional = true}
+blobfile = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ruff = "^0.0.254"
 pytype = "^2023.3.2"
 poethepoet = "^0.18.1"
 ward = "^0.67.2b0"
 ipython = "^8.11.0"
 nest-asyncio = "^1.5.6"
 
 [tool.poetry.extras]
 redis = ["redis"]
+debug = ["colorama", "pygments"]
 
 [tool.poe.tasks]
 _ruff = "ruff --fix **/*.py"
 _black = "black ."
 _pytype = "pytype --config=pytype.toml"
 lint = ["_ruff", "_black"]
 check = ["lint", "_pytype"]
```

### Comparing `turbo_chat-0.3.6/turbo_chat/__init__.py` & `turbo_chat-0.3.7/turbo_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/qa.py` & `turbo_chat-0.3.7/turbo_chat/bots/qa.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/self_ask.py` & `turbo_chat-0.3.7/turbo_chat/bots/self_ask.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/subqueries/bot.py` & `turbo_chat-0.3.7/turbo_chat/bots/subqueries/bot.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/subqueries/scratchpad.py` & `turbo_chat-0.3.7/turbo_chat/bots/subqueries/scratchpad.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/subqueries/template.py` & `turbo_chat-0.3.7/turbo_chat/bots/subqueries/template.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/tool/bot.py` & `turbo_chat-0.3.7/turbo_chat/bots/tool/bot.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/bots/tool/template.py` & `turbo_chat-0.3.7/turbo_chat/bots/tool/template.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/cache/redis.py` & `turbo_chat-0.3.7/turbo_chat/cache/redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 class RedisCache(BaseCache):
     """Redis cache"""
 
     client: redis.Redis
     prefix: str
+    ttl: int = 0
 
     async def setup(
         self,
         client: redis.Redis,
         prefix: str = "turbo_cache",
     ):
         self.client = client
@@ -38,15 +39,22 @@
         result: int = await self.client.exists(self.to_key(key))
         return bool(result)
 
     async def set(self, key, value) -> None:
         _key = self.to_key(key)
         _value = self.serialize(value)
 
-        await self.client.set(_key, _value)
+        # Set ttl
+        ttl = self.ttl
+        opts = {}
+        if ttl:
+            opts["px"] = ttl
+            opts["keepttl"] = True
+
+        await self.client.set(_key, _value, **opts)
 
     async def get(self, key) -> Any:
         _key = self.to_key(key)
         result = await self.client.get(_key)
 
         assert result, "key not found"
```

### Comparing `turbo_chat-0.3.6/turbo_chat/cache/simple.py` & `turbo_chat-0.3.7/turbo_chat/cache/simple.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/completion.py` & `turbo_chat-0.3.7/turbo_chat/completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from functools import wraps
 import inspect
 from typing import (
     Awaitable,
     Callable,
     Protocol,
-    Union,
+    TypeVar,
 )
 
 
 from .structs import (
     Generate,
     User,
 )
@@ -17,49 +18,52 @@
 from .utils.args import ensure_args
 
 
 __all__ = [
     "completion",
 ]
 
+T = TypeVar("T")
 
-class CompletionFnWithResult(Protocol):
-    def __call__(self, result: str, **kwargs) -> Awaitable[str]:
+
+class CompletionFn(Protocol):
+    def __call__(self, *args, **kwargs) -> Awaitable[None]:
         ...
 
 
-class CompletionFnWithoutResult(Protocol):
-    def __call__(self, **kwargs) -> Awaitable[None]:
+class Completion(Protocol[T]):
+    def __call__(self, *args, **kwargs) -> Awaitable[T]:
         ...
 
 
-CompletionFn = Union[CompletionFnWithResult, CompletionFnWithoutResult]
-
-
-class Completion(Protocol):
-    def __call__(self, **kwargs) -> Awaitable[str]:
-        ...
+ParseFn = Callable[[str], T]
 
 
 # Decorator
-def completion(**opts) -> Callable[[CompletionFn], Completion]:
+def completion(
+    parse: ParseFn[T] = lambda s: str(s),
+    **opts,
+) -> Callable[[CompletionFn], Completion[T]]:
     """Parameterized decorator for creating a simple generate function"""
 
     def wrapper(fn: CompletionFn):
-        @turbo(**opts)
+        @turbo(original_fn=fn, **opts)
         async def generate(**kwargs):
             yield User(template=inspect.getdoc(fn), variables=kwargs)
             yield Generate()
 
-        # @wraps(fn)
-        async def wrapped(**kwargs) -> str:
+        @wraps(fn)
+        async def wrapped(*args, **kwargs) -> str:
+            params = inspect.signature(fn).bind(*args, **kwargs)
+            opts = params.arguments
+
             # Ensure args
-            assert ensure_args(fn, kwargs)
+            assert ensure_args(fn, opts)
 
             # Get result
-            result = await generate(**kwargs).run()
+            result = await generate(**opts).run()
 
-            return result.content
+            return parse(result.content)
 
         return wrapped
 
     return wrapper
```

### Comparing `turbo_chat-0.3.6/turbo_chat/memory/local_memory.py` & `turbo_chat-0.3.7/turbo_chat/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/memory/summary_memory.py` & `turbo_chat-0.3.7/turbo_chat/memory/summary_memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/memory/truncated_memory.py` & `turbo_chat-0.3.7/turbo_chat/memory/truncated_memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/runner.py` & `turbo_chat-0.3.7/turbo_chat/runner.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/structs/messages.py` & `turbo_chat-0.3.7/turbo_chat/structs/messages.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/structs/proxies.py` & `turbo_chat-0.3.7/turbo_chat/structs/proxies.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/structs/result.py` & `turbo_chat-0.3.7/turbo_chat/structs/result.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/structs/scratchpad.py` & `turbo_chat-0.3.7/turbo_chat/structs/scratchpad.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/turbo.py` & `turbo_chat-0.3.7/turbo_chat/turbo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from datetime import datetime
 from functools import wraps
 import inspect
 from typing import (
     Any,
     Callable,
+    List,
     Optional,
     Type,
 )
 
+from openai.openai_object import OpenAIObject
+
 from .chat import run_chat
 from .config import TurboModel
 from .errors import InvalidValueYieldedError
 from .memory import LocalMemory
 
 from .structs import (
     Assistant,
@@ -47,14 +50,19 @@
 # Decorator
 def turbo(
     memory_class: Type[BaseMemory] = LocalMemory,
     model: TurboModel = "gpt-3.5-turbo-0301",
     stream: bool = False,
     cache_class: Optional[Type[BaseCache]] = None,
     debug: Optional[Callable[[dict], None]] = None,
+    original_fn: Optional[Callable] = None,
+    select_choice: Callable[[List[OpenAIObject]], OpenAIObject] = (
+        lambda choices: choices[0]
+    ),
+    n: int = 1,
     **kwargs,
 ) -> Callable[[TurboGenTemplateFn], TurboGenFn]:
     """Parameterized decorator for creating a chatml app from an async generator"""
 
     # Streaming not supported yet
     if stream:
         raise NotImplementedError("Streaming not supported yet")
@@ -69,24 +77,28 @@
     )
 
     # Prepare openai args
     chat_completion_args = {
         **kwargs,
         "model": model,
         "stream": stream,
+        "n": n,
     }
 
     # Parameterized decorator fn
     def wrap_turbo_gen_fn(gen_fn: TurboGenTemplateFn) -> TurboGenFn:
         """Wrapper for chatml app async generator"""
 
         @wraps(gen_fn)
-        async def turbo_gen_fn(**context) -> TurboGenWrapper:
+        async def turbo_gen_fn(*args, **kwargs) -> TurboGenWrapper:
             """Wrapped chatml app from an async generator"""
 
+            params = inspect.signature(original_fn or gen_fn).bind(*args, **kwargs)
+            context = params.arguments
+
             memory_args = context.pop("memory_args", {})
             cache_args = context.pop("cache_args", {})
 
             # Init memory
             memory = memory_class(model=model)
             assert ensure_args(memory.setup, memory_args)
             await memory.setup(**memory_args)
@@ -164,14 +176,15 @@
                     elif isinstance(output, Generate):
                         output_dict = output.dict()
                         forward = output_dict.pop("forward")
 
                         payload = await run_chat(
                             memory,
                             cache,
+                            select_choice=select_choice,
                             **{
                                 **chat_completion_args,
                                 **output_dict,
                             },
                         )
 
                         # Yield generated result if needed
```

### Comparing `turbo_chat-0.3.6/turbo_chat/types/cache.py` & `turbo_chat-0.3.7/turbo_chat/types/cache.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/types/generators.py` & `turbo_chat-0.3.7/turbo_chat/types/generators.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,10 +40,11 @@
     settings: dict
 
     def configure(self, new_settings: dict) -> "TurboGenFn":
         ...
 
     def __call__(
         self,
-        **context,
+        *args,
+        **kwargs,
     ) -> TurboGenWrapper:
         ...
```

### Comparing `turbo_chat-0.3.6/turbo_chat/types/memory.py` & `turbo_chat-0.3.7/turbo_chat/types/memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/types/messages.py` & `turbo_chat-0.3.7/turbo_chat/types/messages.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/utils/args.py` & `turbo_chat-0.3.7/turbo_chat/utils/args.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/utils/retries.py` & `turbo_chat-0.3.7/turbo_chat/utils/retries.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/turbo_chat/utils/template.py` & `turbo_chat-0.3.7/turbo_chat/utils/template.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.6/PKG-INFO` & `turbo_chat-0.3.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: turbo-chat
-Version: 0.3.6
+Version: 0.3.7
 Summary: Idiomatic way to build chatgpt apps using async generators in python
 License: MIT
 Author: Diwank Singh Tomer
 Author-email: singh@diwank.name
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: debug
 Provides-Extra: redis
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: blobfile (>=2.0.1,<3.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0) ; extra == "debug"
 Requires-Dist: dirtyjson (>=1.0.8,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jinja2schema (>=0.1.4,<0.2.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: lemminflect (>=0.2.3,<0.3.0)
 Requires-Dist: openai (>=0.27.0,<0.28.0)
 Requires-Dist: parse (>=1.19.0,<2.0.0)
 Requires-Dist: proxytypes (>=0.10.0,<0.11.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pygments (>=2.15.0,<3.0.0) ; extra == "debug"
 Requires-Dist: redis (>=4.5.0,<5.0.0) ; extra == "redis"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tiktoken (>=0.3.1,<0.4.0)
 Description-Content-Type: text/markdown
 
 # turbo-chat
 
@@ -208,14 +212,23 @@
 
 ```
 
 ---
 
 ### Latest Changes
 
+* version: 0.3.7. PR [#57](https://github.com/creatorrr/turbo-chat/pull/57) by [@creatorrr](https://github.com/creatorrr).
+* f/support multi choice. PR [#56](https://github.com/creatorrr/turbo-chat/pull/56) by [@creatorrr](https://github.com/creatorrr).
+* feat: Support multiple choices selector; n > 1. PR [#55](https://github.com/creatorrr/turbo-chat/pull/55) by [@creatorrr](https://github.com/creatorrr).
+* feat: Support positional arguments for running apps. PR [#54](https://github.com/creatorrr/turbo-chat/pull/54) by [@creatorrr](https://github.com/creatorrr).
+* feat: Make get_encoding faster. PR [#53](https://github.com/creatorrr/turbo-chat/pull/53) by [@creatorrr](https://github.com/creatorrr).
+* feat: Add ttl support to redis_cache. PR [#52](https://github.com/creatorrr/turbo-chat/pull/52) by [@creatorrr](https://github.com/creatorrr).
+* feat: Support for parsing completions. PR [#51](https://github.com/creatorrr/turbo-chat/pull/51) by [@creatorrr](https://github.com/creatorrr).
+* version: 0.3.6. PR [#50](https://github.com/creatorrr/turbo-chat/pull/50) by [@creatorrr](https://github.com/creatorrr).
+* feat: Add RedisCache implementation. PR [#49](https://github.com/creatorrr/turbo-chat/pull/49) by [@creatorrr](https://github.com/creatorrr).
 * fix: Fix json array. PR [#48](https://github.com/creatorrr/turbo-chat/pull/48) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.5. PR [#47](https://github.com/creatorrr/turbo-chat/pull/47) by [@creatorrr](https://github.com/creatorrr).
 * fix: Fix how function signature and docstring was being parsed. PR [#46](https://github.com/creatorrr/turbo-chat/pull/46) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.4. PR [#45](https://github.com/creatorrr/turbo-chat/pull/45) by [@creatorrr](https://github.com/creatorrr).
 * feat: Add @completion decorator. PR [#44](https://github.com/creatorrr/turbo-chat/pull/44) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.3. PR [#43](https://github.com/creatorrr/turbo-chat/pull/43) by [@creatorrr](https://github.com/creatorrr).
 * feat: Memory expects memory_args, Assistant no longer yields automatically. PR [#42](https://github.com/creatorrr/turbo-chat/pull/42) by [@creatorrr](https://github.com/creatorrr).
```

