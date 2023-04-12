# Comparing `tmp/nonebot-plugin-sky-2.2.5.post1.tar.gz` & `tmp/nonebot-plugin-sky-2.2.5.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sky-2.2.5.post1.tar", last modified: Tue Apr  4 07:29:01 2023, max compression
+gzip compressed data, was "nonebot-plugin-sky-2.2.5.post2.tar", last modified: Wed Apr 12 10:11:53 2023, max compression
```

## Comparing `nonebot-plugin-sky-2.2.5.post1.tar` & `nonebot-plugin-sky-2.2.5.post2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.682736 nonebot-plugin-sky-2.2.5.post1/
--rw-rw-rw-   0        0        0    35823 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/LICENSE
--rw-rw-rw-   0        0        0    15702 2023-04-04 07:29:01.681739 nonebot-plugin-sky-2.2.5.post1/PKG-INFO
--rw-rw-rw-   0        0        0    15172 2023-04-04 07:28:06.000000 nonebot-plugin-sky-2.2.5.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.634864 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/
--rw-rw-rw-   0        0        0     6153 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.645835 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-03-02 08:15:25.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/command.py
--rw-rw-rw-   0        0        0     1810 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/helper_at_all.py
--rw-rw-rw-   0        0        0     1261 2023-02-24 05:45:59.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/load_config.py
--rw-rw-rw-   0        0        0     1747 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/msg_forward.py
--rw-rw-rw-   0        0        0     1560 2023-02-24 02:36:59.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/travelling_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.648827 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/guild/
--rw-rw-rw-   0        0        0     1160 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/guild/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/guild/light_beauty.py
--rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/guild/light_cute.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.652816 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.655808 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/daily_tasks/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/daily_tasks/__init__.py
--rw-rw-rw-   0        0        0     2547 2023-04-04 06:39:21.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/daily_tasks/international.py
--rw-rw-rw-   0        0        0     3077 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/daily_tasks/national.py
--rw-rw-rw-   0        0        0      637 2023-03-02 07:17:23.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/public_notice.py
--rw-rw-rw-   0        0        0    13738 2023-03-02 03:54:13.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/query_tools.py
--rw-rw-rw-   0        0        0     1080 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/queue.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.658800 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/travelling_spirit/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/travelling_spirit/international.py
--rw-rw-rw-   0        0        0     2998 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/travelling_spirit/national.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.662789 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/
--rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.670768 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/
--rw-rw-rw-   0        0        0    16051 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/eating.jpg
--rw-rw-rw-   0        0        0    89789 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_braid.gif
--rw-rw-rw-   0        0        0    79644 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_bun.gif
--rw-rw-rw-   0        0        0    72146 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_cat.gif
--rw-rw-rw-   0        0        0    87935 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_fox.gif
--rw-rw-rw-   0        0        0    80542 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
--rw-rw-rw-   0        0        0    95522 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/go.jpg
--rw-rw-rw-   0        0        0      274 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/menu.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.671765 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/menu_image/
--rw-rw-rw-   0        0        0   824527 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/menu_image/menu.png
--rw-rw-rw-   0        0        0       95 2023-02-20 02:53:16.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/pusher.py
--rw-rw-rw-   0        0        0     3791 2023-03-02 09:17:27.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.680742 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/
--rw-rw-rw-   0        0        0     2280 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/__init__.py
--rw-rw-rw-   0        0        0      405 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/bot_loader.py
--rw-rw-rw-   0        0        0      607 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/chain_reply.py
--rw-rw-rw-   0        0        0     5068 2023-04-04 07:28:06.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/check_update.py
--rw-rw-rw-   0        0        0     6369 2023-03-23 08:02:10.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/data_pack.py
--rw-rw-rw-   0        0        0      391 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/date_util.py
--rw-rw-rw-   0        0        0      746 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/json_cards.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 07:28:06.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/notice_board.py
-drwxrwxrwx   0        0        0        0 2023-04-04 07:29:01.639877 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/
--rw-rw-rw-   0        0        0    15702 2023-04-04 07:29:01.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1950 2023-04-04 07:29:01.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 07:29:01.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-04-04 07:29:01.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-04 07:29:01.000000 nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 07:29:01.682736 nonebot-plugin-sky-2.2.5.post1/setup.cfg
--rw-rw-rw-   0        0        0     1397 2023-04-04 07:28:06.000000 nonebot-plugin-sky-2.2.5.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.237843 nonebot-plugin-sky-2.2.5.post2/
+-rw-rw-rw-   0        0        0    35823 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/LICENSE
+-rw-rw-rw-   0        0        0    15750 2023-04-12 10:11:53.237843 nonebot-plugin-sky-2.2.5.post2/PKG-INFO
+-rw-rw-rw-   0        0        0    15220 2023-04-12 09:44:24.000000 nonebot-plugin-sky-2.2.5.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.159032 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/
+-rw-rw-rw-   0        0        0     6153 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.172999 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-03-02 08:15:25.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/command.py
+-rw-rw-rw-   0        0        0     1810 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/helper_at_all.py
+-rw-rw-rw-   0        0        0     1261 2023-02-24 05:45:59.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/load_config.py
+-rw-rw-rw-   0        0        0     1747 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/msg_forward.py
+-rw-rw-rw-   0        0        0     1560 2023-02-24 02:36:59.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/travelling_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.176989 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/
+-rw-rw-rw-   0        0        0     1160 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/light_beauty.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/light_cute.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.182975 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.187963 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-04-04 06:39:21.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/international.py
+-rw-rw-rw-   0        0        0     3077 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/national.py
+-rw-rw-rw-   0        0        0      637 2023-03-02 07:17:23.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/public_notice.py
+-rw-rw-rw-   0        0        0    13738 2023-03-02 03:54:13.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/query_tools.py
+-rw-rw-rw-   0        0        0     1080 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/queue.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.191953 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-04-04 06:46:44.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/international.py
+-rw-rw-rw-   0        0        0     2996 2023-04-12 10:08:03.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/national.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.196951 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/
+-rw-rw-rw-   0        0        0        0 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.217891 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/
+-rw-rw-rw-   0        0        0    16051 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/eating.jpg
+-rw-rw-rw-   0        0        0    89789 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_braid.gif
+-rw-rw-rw-   0        0        0    79644 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_bun.gif
+-rw-rw-rw-   0        0        0    72146 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_cat.gif
+-rw-rw-rw-   0        0        0    87935 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_fox.gif
+-rw-rw-rw-   0        0        0    80542 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
+-rw-rw-rw-   0        0        0    95522 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/go.jpg
+-rw-rw-rw-   0        0        0      274 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.219886 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu_image/
+-rw-rw-rw-   0        0        0   824527 2023-01-27 06:30:50.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu_image/menu.png
+-rw-rw-rw-   0        0        0       95 2023-02-20 02:53:16.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/pusher.py
+-rw-rw-rw-   0        0        0     3791 2023-03-02 09:17:27.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.236845 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/
+-rw-rw-rw-   0        0        0     2280 2023-04-04 06:34:38.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/bot_loader.py
+-rw-rw-rw-   0        0        0      607 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/chain_reply.py
+-rw-rw-rw-   0        0        0     5067 2023-04-12 09:51:04.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/check_update.py
+-rw-rw-rw-   0        0        0     6369 2023-03-23 08:02:10.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/data_pack.py
+-rw-rw-rw-   0        0        0      391 2023-02-20 03:43:12.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/date_util.py
+-rw-rw-rw-   0        0        0      746 2023-03-02 03:18:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/json_cards.py
+-rw-rw-rw-   0        0        0     1264 2023-04-04 07:30:19.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/notice_board.py
+drwxrwxrwx   0        0        0        0 2023-04-12 10:11:53.165019 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/
+-rw-rw-rw-   0        0        0    15750 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1950 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-12 10:11:53.000000 nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 10:11:53.238840 nonebot-plugin-sky-2.2.5.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1397 2023-04-12 09:44:24.000000 nonebot-plugin-sky-2.2.5.post2/setup.py
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/LICENSE` & `nonebot-plugin-sky-2.2.5.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/PKG-INFO` & `nonebot-plugin-sky-2.2.5.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.5.post1
+Version: 2.2.5.post2
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -286,14 +286,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.12 v2.2.5.post2
+
+修复已知问题
+
 2023.4.4 v2.2.5.post1
 
 修复插件公告镜像源地址
 
 2023.4.4 v2.2.5
 
 1.修复国际服任务获取不到的问题
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.5.post1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.5.post2 Summary:
 nonebot2 plugin sky Home-page: https://github.com/Kaguya233qwq/
 nonebot_plugin_sky Author: Kaguya233qwq Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Classifier: Natural Language :: Chinese
 (Simplified) Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -111,19 +111,20 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.4 v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å
-2023.4.4 v2.2.5 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢
-2.ä¿®å¤å¤å»ç¸å³é®é¢ 3.ç°å¨å¾çåéä¸åågo-
-cqhttpçæ¬çå½±å 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23
-v2.2.4 ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
+â¨æ´æ°æ¥å¿â¨ 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4
+v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
+1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
+3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
+4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
+ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
 ä¿®å¤å·²ç¥çé®é¢ 2023.3.7 v2.2.2
 åéééå å·¥ä½å¿æ²¡ææ¶é´æ´æ°ï¼
 æ´æ¢å¤å»æ°æ®æºä¸ºå¾®å@åéåå1å· 2023.3.2 v2.2.1
 1.ä¿®å¤åéå®æ¹å¬åä¸æä»¶å¬åå²çªé®é¢
 2.ä¿®å¤æ·»å æä»¤å½ä»¤æ­»å¾ªç¯é®é¢ 3.ä¿®å¤lxmlè­¦åé®é¢
 4.è¡çæ¥è¯¢å¢å å¯¹åºå¼å¸¸æè·å¤ç
 æ´æ©çè®°å½ï¼2023.3.1ä¹åï¼ 2023.3.1 v2.2
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/README.md` & `nonebot-plugin-sky-2.2.5.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.12 v2.2.5.post2
+
+修复已知问题
+
 2023.4.4 v2.2.5.post1
 
 修复插件公告镜像源地址
 
 2023.4.4 v2.2.5
 
 1.修复国际服任务获取不到的问题
```

#### html2text {}

```diff
@@ -104,19 +104,20 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.4 v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å
-2023.4.4 v2.2.5 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢
-2.ä¿®å¤å¤å»ç¸å³é®é¢ 3.ç°å¨å¾çåéä¸åågo-
-cqhttpçæ¬çå½±å 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23
-v2.2.4 ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
+â¨æ´æ°æ¥å¿â¨ 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4
+v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
+1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
+3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
+4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
+ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
 ä¿®å¤å·²ç¥çé®é¢ 2023.3.7 v2.2.2
 åéééå å·¥ä½å¿æ²¡ææ¶é´æ´æ°ï¼
 æ´æ¢å¤å»æ°æ®æºä¸ºå¾®å@åéåå1å· 2023.3.2 v2.2.1
 1.ä¿®å¤åéå®æ¹å¬åä¸æä»¶å¬åå²çªé®é¢
 2.ä¿®å¤æ·»å æä»¤å½ä»¤æ­»å¾ªç¯é®é¢ 3.ä¿®å¤lxmlè­¦åé®é¢
 4.è¡çæ¥è¯¢å¢å å¯¹åºå¼å¸¸æè·å¤ç
 æ´æ©çè®°å½ï¼2023.3.1ä¹åï¼ 2023.3.1 v2.2
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/__init__.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/command.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/helper_at_all.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/helper_at_all.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/load_config.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/msg_forward.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/msg_forward.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/config/travelling_cache.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/config/travelling_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/guild/__init__.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/daily_tasks/international.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/daily_tasks/national.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/daily_tasks/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/public_notice.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/public_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/query_tools.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/query_tools.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/queue.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/queue.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/travelling_spirit/international.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/sky/travelling_spirit/national.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/sky/travelling_spirit/national.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,17 +40,17 @@
                 )
                 content = response.json()
                 overhead = content['data']['list']
                 for log in overhead:
                     if (
                             log.get('pic_infos') and
                             re.findall(
-                                r'#(光遇)*?([\u4e00-\u9fa5])*?(先祖)*?(复刻)*?([\u4e00-\u9fa5])*?#',
+                                r'#(光遇复刻)*([\u4e00-\u9fa5])*(先祖复刻)*([\u4e00-\u9fa5])*#',
                                 log['text_raw']
-                            ) and time_no_more(log.get('created_at'), 12, 50)
+                            ) and time_no_more(log.get('created_at'), 12, 30)
                             # 为了包包我已经放弃了优雅。
                     ):
                         return log
         return None
 
     async def get_data(self):
         """获取复刻数据"""
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/eating.jpg` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/eating.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_braid.gif` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_braid.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_bun.gif` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_bun.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_cat.gif` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_fox.gif` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_fox.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/helper_image/go.jpg` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/helper_image/go.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/menu_image/menu.png` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/menu_image/menu.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/tools/scheduler.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/__init__.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/chain_reply.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/chain_reply.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/check_update.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/check_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from nonebot import on_command, logger
 from ..config.command import get_cmd_alias
 
 logging.captureWarnings(True)  # 去掉建议使用SSL验证的显示
 
-Version = 'v2.2.5.post1'  # 全局插件版本信息  （不用加v！）
+Version = '2.2.5.post2'  # 全局插件版本信息  （不用加v！）
 
 
 async def get_datapack_ver():
     """
     检查本地数据包版本
     """
     try:
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/data_pack.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/data_pack.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/json_cards.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/json_cards.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky/utils_/notice_board.py` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky/utils_/notice_board.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,14 @@
             headers=headers
         )
         bs = BeautifulSoup(res.text, 'lxml')
         results_ = ''
         notice_list = bs.find_all(class_='line')
         for notice in notice_list:
             results_ += notice.text
-        print(results_)
         return results_
 
 
 Notice = on_command("noticeboard", aliases=get_cmd_alias('noticeboard'))
 
 
 @Notice.handle()
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/PKG-INFO` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.5.post1
+Version: 2.2.5.post2
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -286,14 +286,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.4.12 v2.2.5.post2
+
+修复已知问题
+
 2023.4.4 v2.2.5.post1
 
 修复插件公告镜像源地址
 
 2023.4.4 v2.2.5
 
 1.修复国际服任务获取不到的问题
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.5.post1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.5.post2 Summary:
 nonebot2 plugin sky Home-page: https://github.com/Kaguya233qwq/
 nonebot_plugin_sky Author: Kaguya233qwq Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Classifier: Natural Language :: Chinese
 (Simplified) Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -111,19 +111,20 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.4.4 v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å
-2023.4.4 v2.2.5 1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢
-2.ä¿®å¤å¤å»ç¸å³é®é¢ 3.ç°å¨å¾çåéä¸åågo-
-cqhttpçæ¬çå½±å 4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23
-v2.2.4 ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
+â¨æ´æ°æ¥å¿â¨ 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4
+v2.2.5.post1 ä¿®å¤æä»¶å¬åéåæºå°å 2023.4.4 v2.2.5
+1.ä¿®å¤å½éæä»»å¡è·åä¸å°çé®é¢ 2.ä¿®å¤å¤å»ç¸å³é®é¢
+3.ç°å¨å¾çåéä¸åågo-cqhttpçæ¬çå½±å
+4.å¤å»åæ¢å¾ä¸åä½¿ç¨è½¬åæ¶æ¯æ¨¡å¼ 2023.3.23 v2.2.4
+ä¿®å¤å·²ç¥é®é¢ï¼æ´æ¢é¡¹ç®çgiteeéåä»åº 2023.3.21 v2.2.3
 ä¿®å¤å·²ç¥çé®é¢ 2023.3.7 v2.2.2
 åéééå å·¥ä½å¿æ²¡ææ¶é´æ´æ°ï¼
 æ´æ¢å¤å»æ°æ®æºä¸ºå¾®å@åéåå1å· 2023.3.2 v2.2.1
 1.ä¿®å¤åéå®æ¹å¬åä¸æä»¶å¬åå²çªé®é¢
 2.ä¿®å¤æ·»å æä»¤å½ä»¤æ­»å¾ªç¯é®é¢ 3.ä¿®å¤lxmlè­¦åé®é¢
 4.è¡çæ¥è¯¢å¢å å¯¹åºå¼å¸¸æè·å¤ç
 æ´æ©çè®°å½ï¼2023.3.1ä¹åï¼ 2023.3.1 v2.2
```

### Comparing `nonebot-plugin-sky-2.2.5.post1/nonebot_plugin_sky.egg-info/SOURCES.txt` & `nonebot-plugin-sky-2.2.5.post2/nonebot_plugin_sky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.5.post1/setup.py` & `nonebot-plugin-sky-2.2.5.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Files = get_files(r'nonebot_plugin_sky/tools/helper_image')
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
 setuptools.setup(
     name='nonebot-plugin-sky',
-    version='v2.2.5.post1',
+    version='v2.2.5.post2',
     author='Kaguya233qwq',
     author_email='1435608435@qq.com',
     keywords=["pip", "nonebot2", "nonebot", "sky光遇", "光遇"],
     url='https://github.com/Kaguya233qwq/nonebot_plugin_sky',
     description='''nonebot2 plugin sky''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

