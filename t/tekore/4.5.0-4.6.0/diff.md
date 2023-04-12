# Comparing `tmp/tekore-4.5.0.tar.gz` & `tmp/tekore-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tekore-4.5.0.tar", last modified: Sun Nov  6 13:32:42 2022, max compression
+gzip compressed data, was "tekore-4.6.0.tar", last modified: Wed Apr 12 18:05:49 2023, max compression
```

## Comparing `tekore-4.5.0.tar` & `tekore-4.6.0.tar`

### file list

```diff
@@ -1,111 +1,200 @@
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.534644 tekore-4.5.0/
--rw-r--r--   0 felix      (502) staff       (20)     1075 2022-10-08 08:41:53.000000 tekore-4.5.0/LICENSE
--rw-r--r--   0 felix      (502) staff       (20)       47 2022-10-08 08:41:53.000000 tekore-4.5.0/MANIFEST.in
--rw-r--r--   0 felix      (502) staff       (20)     4019 2022-11-06 13:32:42.534521 tekore-4.5.0/PKG-INFO
--rw-r--r--   0 felix      (502) staff       (20)     2818 2022-10-08 08:41:53.000000 tekore-4.5.0/readme_pypi.rst
--rw-r--r--   0 felix      (502) staff       (20)       38 2022-11-06 13:32:42.534679 tekore-4.5.0/setup.cfg
--rw-r--r--   0 felix      (502) staff       (20)     2817 2022-11-06 12:05:15.000000 tekore-4.5.0/setup.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.525859 tekore-4.5.0/tekore/
--rw-r--r--   0 felix      (502) staff       (20)        6 2022-11-06 13:30:25.000000 tekore-4.5.0/tekore/VERSION
--rw-r--r--   0 felix      (502) staff       (20)     2662 2022-11-06 12:31:36.000000 tekore-4.5.0/tekore/__init__.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.526790 tekore-4.5.0/tekore/_auth/
--rw-r--r--   0 felix      (502) staff       (20)      379 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/__init__.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.527214 tekore-4.5.0/tekore/_auth/expiring/
--rw-r--r--   0 felix      (502) staff       (20)       70 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/expiring/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     9403 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/expiring/client.py
--rw-r--r--   0 felix      (502) staff       (20)     1564 2022-11-06 12:30:09.000000 tekore-4.5.0/tekore/_auth/expiring/decor.py
--rw-r--r--   0 felix      (502) staff       (20)     2766 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/expiring/token.py
--rw-r--r--   0 felix      (502) staff       (20)     8872 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/refreshing.py
--rw-r--r--   0 felix      (502) staff       (20)     5636 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/scope.py
--rw-r--r--   0 felix      (502) staff       (20)     8349 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_auth/util.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.527804 tekore-4.5.0/tekore/_client/
--rw-r--r--   0 felix      (502) staff       (20)       26 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/__init__.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.529184 tekore-4.5.0/tekore/_client/api/
--rw-r--r--   0 felix      (502) staff       (20)      568 2022-10-17 20:54:54.000000 tekore-4.5.0/tekore/_client/api/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     2061 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/album.py
--rw-r--r--   0 felix      (502) staff       (20)     3167 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/artist.py
--rw-r--r--   0 felix      (502) staff       (20)     2904 2022-10-18 18:57:48.000000 tekore-4.5.0/tekore/_client/api/audiobook.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.529389 tekore-4.5.0/tekore/_client/api/browse/
--rw-r--r--   0 felix      (502) staff       (20)     7142 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/browse/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)      636 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/browse/validate.py
--rw-r--r--   0 felix      (502) staff       (20)     1795 2022-10-18 19:07:33.000000 tekore-4.5.0/tekore/_client/api/chapter.py
--rw-r--r--   0 felix      (502) staff       (20)     1796 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/episode.py
--rw-r--r--   0 felix      (502) staff       (20)     5541 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/follow.py
--rw-r--r--   0 felix      (502) staff       (20)     8938 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/library.py
--rw-r--r--   0 felix      (502) staff       (20)      481 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/markets.py
--rw-r--r--   0 felix      (502) staff       (20)     1948 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/personalisation.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.529721 tekore-4.5.0/tekore/_client/api/player/
--rw-r--r--   0 felix      (502) staff       (20)      175 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/player/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     7275 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/player/modify.py
--rw-r--r--   0 felix      (502) staff       (20)     4141 2022-10-17 20:16:45.000000 tekore-4.5.0/tekore/_client/api/player/view.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.530148 tekore-4.5.0/tekore/_client/api/playlist/
--rw-r--r--   0 felix      (502) staff       (20)      264 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/playlist/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     6363 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/playlist/items.py
--rw-r--r--   0 felix      (502) staff       (20)     2742 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/playlist/modify.py
--rw-r--r--   0 felix      (502) staff       (20)     7589 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/playlist/view.py
--rw-r--r--   0 felix      (502) staff       (20)     3497 2022-11-06 10:49:48.000000 tekore-4.5.0/tekore/_client/api/search.py
--rw-r--r--   0 felix      (502) staff       (20)     3072 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/show.py
--rw-r--r--   0 felix      (502) staff       (20)     2478 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/track.py
--rw-r--r--   0 felix      (502) staff       (20)      916 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/api/user.py
--rw-r--r--   0 felix      (502) staff       (20)     4338 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/base.py
--rw-r--r--   0 felix      (502) staff       (20)     4188 2022-11-06 10:22:48.000000 tekore-4.5.0/tekore/_client/chunked.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.530352 tekore-4.5.0/tekore/_client/decor/
--rw-r--r--   0 felix      (502) staff       (20)     2726 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/decor/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     1034 2022-11-06 12:30:09.000000 tekore-4.5.0/tekore/_client/decor/handle.py
--rw-r--r--   0 felix      (502) staff       (20)     3964 2022-10-17 20:55:08.000000 tekore-4.5.0/tekore/_client/full.py
--rw-r--r--   0 felix      (502) staff       (20)     4174 2022-11-06 12:32:19.000000 tekore-4.5.0/tekore/_client/paging.py
--rw-r--r--   0 felix      (502) staff       (20)     1257 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_client/process.py
--rw-r--r--   0 felix      (502) staff       (20)     5820 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_config.py
--rw-r--r--   0 felix      (502) staff       (20)     3862 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_convert.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.532364 tekore-4.5.0/tekore/_model/
--rw-r--r--   0 felix      (502) staff       (20)     2391 2022-10-18 19:38:25.000000 tekore-4.5.0/tekore/_model/__init__.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.532654 tekore-4.5.0/tekore/_model/album/
--rw-r--r--   0 felix      (502) staff       (20)     1393 2022-11-06 10:37:16.000000 tekore-4.5.0/tekore/_model/album/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)      977 2022-11-06 10:37:56.000000 tekore-4.5.0/tekore/_model/album/base.py
--rw-r--r--   0 felix      (502) staff       (20)     1661 2022-11-06 10:39:34.000000 tekore-4.5.0/tekore/_model/album/full.py
--rw-r--r--   0 felix      (502) staff       (20)     1312 2022-11-06 10:43:16.000000 tekore-4.5.0/tekore/_model/artist.py
--rw-r--r--   0 felix      (502) staff       (20)     2246 2022-11-06 10:43:37.000000 tekore-4.5.0/tekore/_model/audio_analysis.py
--rw-r--r--   0 felix      (502) staff       (20)      491 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_model/audio_features.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.532957 tekore-4.5.0/tekore/_model/audiobook/
--rw-r--r--   0 felix      (502) staff       (20)      584 2022-11-06 10:39:50.000000 tekore-4.5.0/tekore/_model/audiobook/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     1094 2022-11-06 10:40:17.000000 tekore-4.5.0/tekore/_model/audiobook/base.py
--rw-r--r--   0 felix      (502) staff       (20)      451 2022-11-06 10:40:38.000000 tekore-4.5.0/tekore/_model/audiobook/full.py
--rw-r--r--   0 felix      (502) staff       (20)      315 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_model/base.py
--rw-r--r--   0 felix      (502) staff       (20)      650 2022-11-06 10:44:13.000000 tekore-4.5.0/tekore/_model/category.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.533377 tekore-4.5.0/tekore/_model/chapter/
--rw-r--r--   0 felix      (502) staff       (20)      825 2022-11-06 10:40:56.000000 tekore-4.5.0/tekore/_model/chapter/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)      892 2022-11-06 10:41:18.000000 tekore-4.5.0/tekore/_model/chapter/base.py
--rw-r--r--   0 felix      (502) staff       (20)      602 2022-11-06 10:41:41.000000 tekore-4.5.0/tekore/_model/chapter/full.py
--rw-r--r--   0 felix      (502) staff       (20)      495 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_model/context.py
--rw-r--r--   0 felix      (502) staff       (20)     2988 2022-11-06 10:50:06.000000 tekore-4.5.0/tekore/_model/currently_playing.py
--rw-r--r--   0 felix      (502) staff       (20)      807 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_model/device.py
--rw-r--r--   0 felix      (502) staff       (20)     2504 2022-11-06 10:45:32.000000 tekore-4.5.0/tekore/_model/episode.py
--rw-r--r--   0 felix      (502) staff       (20)     1818 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_model/error.py
--rw-r--r--   0 felix      (502) staff       (20)     1299 2022-11-06 10:45:51.000000 tekore-4.5.0/tekore/_model/local.py
--rw-r--r--   0 felix      (502) staff       (20)     1047 2022-11-06 10:22:44.000000 tekore-4.5.0/tekore/_model/member.py
--rw-r--r--   0 felix      (502) staff       (20)      786 2022-11-06 10:46:07.000000 tekore-4.5.0/tekore/_model/paging.py
--rw-r--r--   0 felix      (502) staff       (20)     1240 2022-11-06 10:46:26.000000 tekore-4.5.0/tekore/_model/play_history.py
--rw-r--r--   0 felix      (502) staff       (20)     3654 2022-11-06 10:47:12.000000 tekore-4.5.0/tekore/_model/playlist.py
--rw-r--r--   0 felix      (502) staff       (20)     1211 2022-11-06 10:47:25.000000 tekore-4.5.0/tekore/_model/recommendations.py
--rw-r--r--   0 felix      (502) staff       (20)     6556 2022-10-08 10:12:49.000000 tekore-4.5.0/tekore/_model/serialise.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.533725 tekore-4.5.0/tekore/_model/show/
--rw-r--r--   0 felix      (502) staff       (20)     1128 2022-11-06 10:42:10.000000 tekore-4.5.0/tekore/_model/show/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)      876 2022-11-06 10:42:37.000000 tekore-4.5.0/tekore/_model/show/base.py
--rw-r--r--   0 felix      (502) staff       (20)      560 2022-11-06 10:42:49.000000 tekore-4.5.0/tekore/_model/show/full.py
--rw-r--r--   0 felix      (502) staff       (20)     3871 2022-11-06 10:50:31.000000 tekore-4.5.0/tekore/_model/track.py
--rw-r--r--   0 felix      (502) staff       (20)     1744 2022-11-06 10:48:41.000000 tekore-4.5.0/tekore/_model/user.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.534342 tekore-4.5.0/tekore/_sender/
--rw-r--r--   0 felix      (502) staff       (20)      449 2022-11-06 12:31:24.000000 tekore-4.5.0/tekore/_sender/__init__.py
--rw-r--r--   0 felix      (502) staff       (20)     1259 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_sender/base.py
--rw-r--r--   0 felix      (502) staff       (20)     3189 2022-11-06 12:44:51.000000 tekore-4.5.0/tekore/_sender/client.py
--rw-r--r--   0 felix      (502) staff       (20)     3004 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_sender/concrete.py
--rw-r--r--   0 felix      (502) staff       (20)     2753 2022-11-06 12:53:00.000000 tekore-4.5.0/tekore/_sender/error.py
--rw-r--r--   0 felix      (502) staff       (20)     9867 2022-10-08 10:07:26.000000 tekore-4.5.0/tekore/_sender/extending.py
--rw-r--r--   0 felix      (502) staff       (20)     1212 2022-10-08 08:41:53.000000 tekore-4.5.0/tekore/_start.py
--rw-r--r--   0 felix      (502) staff       (20)     3982 2022-10-18 19:21:54.000000 tekore-4.5.0/tekore/model.py
-drwxr-xr-x   0 felix      (502) staff       (20)        0 2022-11-06 13:32:42.526386 tekore-4.5.0/tekore.egg-info/
--rw-r--r--   0 felix      (502) staff       (20)     4019 2022-11-06 13:32:42.000000 tekore-4.5.0/tekore.egg-info/PKG-INFO
--rw-r--r--   0 felix      (502) staff       (20)     2534 2022-11-06 13:32:42.000000 tekore-4.5.0/tekore.egg-info/SOURCES.txt
--rw-r--r--   0 felix      (502) staff       (20)        1 2022-11-06 13:32:42.000000 tekore-4.5.0/tekore.egg-info/dependency_links.txt
--rw-r--r--   0 felix      (502) staff       (20)      386 2022-11-06 13:32:42.000000 tekore-4.5.0/tekore.egg-info/requires.txt
--rw-r--r--   0 felix      (502) staff       (20)        7 2022-11-06 13:32:42.000000 tekore-4.5.0/tekore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.319480 tekore-4.6.0/
+-rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-4.6.0/LICENSE
+-rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-4.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5362 2023-04-12 18:05:49.319480 tekore-4.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4184 2023-01-05 23:44:39.000000 tekore-4.6.0/contributing.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.220962 tekore-4.6.0/docs/
+-rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.227964 tekore-4.6.0/docs/src/
+-rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/404.rst
+-rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/advanced_usage.rst
+-rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/auth_guide.rst
+-rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-4.6.0/docs/src/conf.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.230964 tekore-4.6.0/docs/src/examples/
+-rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-4.6.0/docs/src/examples/artist_follower.rst
+-rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-4.6.0/docs/src/examples/async_server.rst
+-rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-4.6.0/docs/src/examples/auth_server.rst
+-rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-4.6.0/docs/src/examples/creating_scripts.rst
+-rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-4.6.0/docs/src/examples/discord_bot.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.236465 tekore-4.6.0/docs/src/examples/scripts/
+-rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/albums_top_artist.rst
+-rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/analyse_from_playlist.rst
+-rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/follow_by_search.rst
+-rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/follow_category_playlist.rst
+-rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/play_saved_album.rst
+-rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/recommended_playlist.rst
+-rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/related_artists_top_artist.rst
+-rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-4.6.0/docs/src/examples/scripts/scrape_playlists.rst
+-rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-4.6.0/docs/src/examples/scripts/tracks_new_release.rst
+-rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/examples/scripts.rst
+-rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/examples.rst
+-rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-4.6.0/docs/src/getting_started.rst
+-rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-4.6.0/docs/src/index.rst
+-rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-4.6.0/docs/src/logo.png
+-rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-4.6.0/docs/src/logo_small.png
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.240966 tekore-4.6.0/docs/src/reference/
+-rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-4.6.0/docs/src/reference/auth.rst
+-rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference/client.rst
+-rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-4.6.0/docs/src/reference/config.rst
+-rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-4.6.0/docs/src/reference/conversions.rst
+-rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference/errors.rst
+-rw-rw-rw-   0        0        0     7784 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference/models.rst
+-rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-4.6.0/docs/src/reference/senders.rst
+-rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-4.6.0/docs/src/reference.rst
+-rw-rw-rw-   0        0        0    19676 2023-04-12 17:55:05.000000 tekore-4.6.0/docs/src/release_notes.rst
+-rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-4.6.0/docs/src/resources.rst
+-rw-rw-rw-   0        0        0     2069 2023-04-12 17:36:57.000000 tekore-4.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-4.6.0/readme_pypi.rst
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.243466 tekore-4.6.0/requirements/
+-rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/build
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/checks
+-rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/dev
+-rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/docs
+-rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-4.6.0/requirements/tests
+-rw-rw-rw-   0        0        0       42 2023-04-12 18:05:49.319480 tekore-4.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.212961 tekore-4.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.245467 tekore-4.6.0/src/tekore/
+-rw-rw-rw-   0        0        0     2610 2023-04-12 17:55:05.000000 tekore-4.6.0/src/tekore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.250968 tekore-4.6.0/src/tekore/_auth/
+-rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.252968 tekore-4.6.0/src/tekore/_auth/expiring/
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/__init__.py
+-rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/client.py
+-rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/decor.py
+-rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/expiring/token.py
+-rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/refreshing.py
+-rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/scope.py
+-rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_auth/util.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.256969 tekore-4.6.0/src/tekore/_client/
+-rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.266470 tekore-4.6.0/src/tekore/_client/api/
+-rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/album.py
+-rw-rw-rw-   0        0        0     3186 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/artist.py
+-rw-rw-rw-   0        0        0     2866 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/audiobook.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.267971 tekore-4.6.0/src/tekore/_client/api/browse/
+-rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/browse/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/browse/validate.py
+-rw-rw-rw-   0        0        0     1761 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/chapter.py
+-rw-rw-rw-   0        0        0     1762 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/episode.py
+-rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/follow.py
+-rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/library.py
+-rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/markets.py
+-rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/personalisation.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.269971 tekore-4.6.0/src/tekore/_client/api/player/
+-rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/player/__init__.py
+-rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/player/modify.py
+-rw-rw-rw-   0        0        0     4091 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/player/view.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.272471 tekore-4.6.0/src/tekore/_client/api/playlist/
+-rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/__init__.py
+-rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/items.py
+-rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/modify.py
+-rw-rw-rw-   0        0        0     7617 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/playlist/view.py
+-rw-rw-rw-   0        0        0     3578 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/search.py
+-rw-rw-rw-   0        0        0     2985 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/show.py
+-rw-rw-rw-   0        0        0     2469 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/track.py
+-rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/api/user.py
+-rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/base.py
+-rw-rw-rw-   0        0        0     4194 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/chunked.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.273471 tekore-4.6.0/src/tekore/_client/decor/
+-rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/decor/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/decor/handle.py
+-rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/full.py
+-rw-rw-rw-   0        0        0     4299 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/paging.py
+-rw-rw-rw-   0        0        0     1316 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_client/process.py
+-rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_config.py
+-rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-4.6.0/src/tekore/_convert.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.287474 tekore-4.6.0/src/tekore/_model/
+-rw-rw-rw-   0        0        0     2394 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.288974 tekore-4.6.0/src/tekore/_model/album/
+-rw-rw-rw-   0        0        0     1442 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/album/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/album/base.py
+-rw-rw-rw-   0        0        0     1788 2023-03-26 08:36:33.000000 tekore-4.6.0/src/tekore/_model/album/full.py
+-rw-rw-rw-   0        0        0     1369 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/artist.py
+-rw-rw-rw-   0        0        0     2336 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audio_analysis.py
+-rw-rw-rw-   0        0        0      518 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audio_features.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.290475 tekore-4.6.0/src/tekore/_model/audiobook/
+-rw-rw-rw-   0        0        0      607 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audiobook/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audiobook/base.py
+-rw-rw-rw-   0        0        0      468 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/audiobook/full.py
+-rw-rw-rw-   0        0        0      335 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/base.py
+-rw-rw-rw-   0        0        0      679 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/category.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.291975 tekore-4.6.0/src/tekore/_model/chapter/
+-rw-rw-rw-   0        0        0      860 2023-03-26 09:38:45.000000 tekore-4.6.0/src/tekore/_model/chapter/__init__.py
+-rw-rw-rw-   0        0        0      900 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/chapter/base.py
+-rw-rw-rw-   0        0        0      627 2023-03-26 09:38:45.000000 tekore-4.6.0/src/tekore/_model/chapter/full.py
+-rw-rw-rw-   0        0        0      522 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/context.py
+-rw-rw-rw-   0        0        0     3070 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/currently_playing.py
+-rw-rw-rw-   0        0        0      845 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/device.py
+-rw-rw-rw-   0        0        0     2563 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/episode.py
+-rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/error.py
+-rw-rw-rw-   0        0        0     1362 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/local.py
+-rw-rw-rw-   0        0        0     1110 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/member.py
+-rw-rw-rw-   0        0        0      834 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/paging.py
+-rw-rw-rw-   0        0        0     1291 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/play_history.py
+-rw-rw-rw-   0        0        0     3789 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/playlist.py
+-rw-rw-rw-   0        0        0     1259 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/recommendations.py
+-rw-rw-rw-   0        0        0     7555 2023-04-12 17:42:29.000000 tekore-4.6.0/src/tekore/_model/serialise.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.293475 tekore-4.6.0/src/tekore/_model/show/
+-rw-rw-rw-   0        0        0     1176 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/show/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/show/base.py
+-rw-rw-rw-   0        0        0      582 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/show/full.py
+-rw-rw-rw-   0        0        0     4011 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/track.py
+-rw-rw-rw-   0        0        0     1808 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_model/user.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.297475 tekore-4.6.0/src/tekore/_sender/
+-rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/base.py
+-rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/client.py
+-rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/concrete.py
+-rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/error.py
+-rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/_sender/extending.py
+-rw-rw-rw-   0        0        0     4202 2023-01-05 23:44:39.000000 tekore-4.6.0/src/tekore/model.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.248467 tekore-4.6.0/src/tekore.egg-info/
+-rw-rw-rw-   0        0        0     5362 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4979 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-12 18:05:49.000000 tekore-4.6.0/src/tekore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.301476 tekore-4.6.0/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/_util.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.303977 tekore-4.6.0/tests/auth/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.0/tests/auth/__init__.py
+-rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/expiring.py
+-rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/refreshing.py
+-rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/scope.py
+-rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/auth/util.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.315979 tekore-4.6.0/tests/client/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-4.6.0/tests/client/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/_resources.py
+-rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/album.py
+-rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/artist.py
+-rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-4.6.0/tests/client/audiobook.py
+-rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/base.py
+-rw-rw-rw-   0        0        0     3444 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/browse.py
+-rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-4.6.0/tests/client/chapter.py
+-rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/episode.py
+-rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/follow.py
+-rw-rw-rw-   0        0        0    13417 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/full.py
+-rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/library.py
+-rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-4.6.0/tests/client/markets.py
+-rw-rw-rw-   0        0        0     3652 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/paging.py
+-rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-4.6.0/tests/client/personalisation.py
+-rw-rw-rw-   0        0        0     6147 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/player.py
+-rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/playlist.py
+-rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/search.py
+-rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/show.py
+-rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/client/track.py
+-rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-4.6.0/tests/client/user.py
+-rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/config.py
+-rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/convert.py
+-rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/error.py
+-rw-rw-rw-   0        0        0     6902 2023-04-12 17:33:26.000000 tekore-4.6.0/tests/model.py
+drwxrwxrwx   0        0        0        0 2023-04-12 18:05:49.318479 tekore-4.6.0/tests/sender/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-4.6.0/tests/sender/__init__.py
+-rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/base.py
+-rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/caching.py
+-rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/client.py
+-rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-4.6.0/tests/sender/retrying.py
+-rw-rw-rw-   0        0        0     2404 2023-04-12 18:04:45.000000 tekore-4.6.0/tox.ini
```

### Comparing `tekore-4.5.0/LICENSE` & `tekore-4.6.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019-2021 Felix Hildén
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019-2023 Felix Hildén
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tekore-4.5.0/PKG-INFO` & `tekore-4.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,132 @@
-Metadata-Version: 2.1
-Name: tekore
-Version: 4.5.0
-Summary: Client for the Spotify Web API
-Home-page: https://tekore.readthedocs.io
-Download-URL: https://pypi.org/project/tekore
-Author: Felix Hildén
-Author-email: felix.hilden@gmail.com
-Maintainer: Felix Hildén
-Maintainer-email: felix.hilden@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/felix-hilden/tekore
-Project-URL: Issues, https://github.com/felix-hilden/tekore/issues
-Project-URL: Documentation, https://tekore.readthedocs.io
-Keywords: spotify web api client
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Multimedia :: Sound/Audio
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: checks
-Provides-Extra: dev
-License-File: LICENSE
-
-|logo|
-
-|python| |downloads|
-
-Welcome to the Python Package Index page of Tekore!
-We provide a client for the Spotify Web API for Python,
-complete with all available endpoints and authentication methods,
-async support and loads of additional features.
-Tekore allows you to interact with the API effortlessly.
-Here's five lines to get you full access and start playing your top songs.
-
-.. code:: python
-
-    import tekore as tk
-
-    conf = (client_id, client_secret, redirect_uri)
-    token = tk.prompt_for_user_token(*conf, scope=tk.scope.every)
-
-    spotify = tk.Spotify(token)
-    tracks = spotify.current_user_top_tracks(limit=10)
-    spotify.playback_start_tracks([t.id for t in tracks.items])
-
-See our online documentation on `Read The Docs`_ for tutorials,
-examples, package reference and a detailed description of features.
-If you've found a bug or would like to propose a feature,
-please submit an issue on `GitHub`_.
-Join our `Discord <https://discord.gg/wcRXgJu>`_ community
-to ask for help or discuss just about anything related to Tekore.
-You can also ask a question on
-`Stack Overflow <https://stackoverflow.com/questions/tagged/tekore>`_.
-
-Installation
-============
-Tekore can be installed from the Package Index via ``pip``.
-
-.. code:: sh
-
-    $ pip install tekore
-
-Changelog
-=========
-A detailed changelog can be found on our RTD documentation's
-`Release notes <https://tekore.readthedocs.io/page/release_notes.html>`_.
-
-Versioning
-==========
-When requiring Tekore in projects or other packages,
-please pin the version down to at least a specific major release
-to avoid compatibility issues.
-For example:
-
-.. code:: python
-
-    setup(
-        install_requires=[
-            'tekore~=4.0'
-        ]
-    )
-
-Tekore provides both stable and beta endpoints of the Web API.
-However, beta endpoints may be changed by Spotify without prior notice,
-so older versions of the library may have unintended issues.
-Because of this, Tekore follows a modified form of
-`Semantic Versioning <https://semver.org/>`_.
-Incompatible changes in the library are still introduced in major versions,
-and new features and endpoints are added in minor versions.
-But endpoints removed by Spotify are removed in minor versions and changes
-to endpoints are implemented as bugfixes.
-See the Web API `documentation <web api_>`_ for further information on beta endpoints.
-
-
-.. |logo| image:: https://raw.githubusercontent.com/felix-hilden/tekore/master/docs/src/logo_small.png
-   :alt: logo
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/tekore
-   :alt: python version
-
-.. |downloads| image:: https://pepy.tech/badge/tekore/month
-   :alt: monthly downloads
-
-.. _github: https://github.com/felix-hilden/tekore
-.. _read the docs: https://tekore.readthedocs.io
-.. _web api: https://developer.spotify.com/documentation/web-api
+Metadata-Version: 2.1
+Name: tekore
+Version: 4.6.0
+Summary: Client for the Spotify Web API
+Author-email: Felix Hildén <felix.hilden@gmail.com>
+Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2019-2023 Felix Hildén
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://pypi.org/project/tekore
+Project-URL: Download, https://pypi.org/project/tekore
+Project-URL: Source, https://github.com/felix-hilden/tekore
+Project-URL: Issues, https://github.com/felix-hilden/tekore/issues
+Project-URL: Documentation, https://tekore.rtfd.org
+Keywords: spotify,web,api,client
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+|logo|
+
+|python| |downloads|
+
+Welcome to the Python Package Index page of Tekore!
+We provide a client for the Spotify Web API for Python,
+complete with all available endpoints and authentication methods,
+async support and loads of additional features.
+Tekore allows you to interact with the API effortlessly.
+Here's five lines to get you full access and start playing your top songs.
+
+.. code:: python
+
+    import tekore as tk
+
+    conf = (client_id, client_secret, redirect_uri)
+    token = tk.prompt_for_user_token(*conf, scope=tk.scope.every)
+
+    spotify = tk.Spotify(token)
+    tracks = spotify.current_user_top_tracks(limit=10)
+    spotify.playback_start_tracks([t.id for t in tracks.items])
+
+See our online documentation on `Read The Docs`_ for tutorials,
+examples, package reference and a detailed description of features.
+If you've found a bug or would like to propose a feature,
+please submit an issue on `GitHub`_.
+Join our `Discord <https://discord.gg/wcRXgJu>`_ community
+to ask for help or discuss just about anything related to Tekore.
+You can also ask a question on
+`Stack Overflow <https://stackoverflow.com/questions/tagged/tekore>`_.
+
+Installation
+============
+Tekore can be installed from the Package Index via ``pip``.
+
+.. code:: sh
+
+    $ pip install tekore
+
+Changelog
+=========
+A detailed changelog can be found on our RTD documentation's
+`Release notes <https://tekore.readthedocs.io/page/release_notes.html>`_.
+
+Versioning
+==========
+When requiring Tekore in projects or other packages,
+please pin the version down to at least a specific major release
+to avoid compatibility issues.
+For example:
+
+.. code:: python
+
+    setup(
+        install_requires=[
+            'tekore~=4.0'
+        ]
+    )
+
+Tekore provides both stable and beta endpoints of the Web API.
+However, beta endpoints may be changed by Spotify without prior notice,
+so older versions of the library may have unintended issues.
+Because of this, Tekore follows a modified form of
+`Semantic Versioning <https://semver.org/>`_.
+Incompatible changes in the library are still introduced in major versions,
+and new features and endpoints are added in minor versions.
+But endpoints removed by Spotify are removed in minor versions and changes
+to endpoints are implemented as bugfixes.
+See the Web API `documentation <web api_>`_ for further information on beta endpoints.
+
+
+.. |logo| image:: https://raw.githubusercontent.com/felix-hilden/tekore/master/docs/src/logo_small.png
+   :alt: logo
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/tekore
+   :alt: python version
+
+.. |downloads| image:: https://pepy.tech/badge/tekore/month
+   :alt: monthly downloads
+
+.. _github: https://github.com/felix-hilden/tekore
+.. _read the docs: https://tekore.readthedocs.io
+.. _web api: https://developer.spotify.com/documentation/web-api
```

### Comparing `tekore-4.5.0/readme_pypi.rst` & `tekore-4.6.0/readme_pypi.rst`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-|logo|
-
-|python| |downloads|
-
-Welcome to the Python Package Index page of Tekore!
-We provide a client for the Spotify Web API for Python,
-complete with all available endpoints and authentication methods,
-async support and loads of additional features.
-Tekore allows you to interact with the API effortlessly.
-Here's five lines to get you full access and start playing your top songs.
-
-.. code:: python
-
-    import tekore as tk
-
-    conf = (client_id, client_secret, redirect_uri)
-    token = tk.prompt_for_user_token(*conf, scope=tk.scope.every)
-
-    spotify = tk.Spotify(token)
-    tracks = spotify.current_user_top_tracks(limit=10)
-    spotify.playback_start_tracks([t.id for t in tracks.items])
-
-See our online documentation on `Read The Docs`_ for tutorials,
-examples, package reference and a detailed description of features.
-If you've found a bug or would like to propose a feature,
-please submit an issue on `GitHub`_.
-Join our `Discord <https://discord.gg/wcRXgJu>`_ community
-to ask for help or discuss just about anything related to Tekore.
-You can also ask a question on
-`Stack Overflow <https://stackoverflow.com/questions/tagged/tekore>`_.
-
-Installation
-============
-Tekore can be installed from the Package Index via ``pip``.
-
-.. code:: sh
-
-    $ pip install tekore
-
-Changelog
-=========
-A detailed changelog can be found on our RTD documentation's
-`Release notes <https://tekore.readthedocs.io/page/release_notes.html>`_.
-
-Versioning
-==========
-When requiring Tekore in projects or other packages,
-please pin the version down to at least a specific major release
-to avoid compatibility issues.
-For example:
-
-.. code:: python
-
-    setup(
-        install_requires=[
-            'tekore~=4.0'
-        ]
-    )
-
-Tekore provides both stable and beta endpoints of the Web API.
-However, beta endpoints may be changed by Spotify without prior notice,
-so older versions of the library may have unintended issues.
-Because of this, Tekore follows a modified form of
-`Semantic Versioning <https://semver.org/>`_.
-Incompatible changes in the library are still introduced in major versions,
-and new features and endpoints are added in minor versions.
-But endpoints removed by Spotify are removed in minor versions and changes
-to endpoints are implemented as bugfixes.
-See the Web API `documentation <web api_>`_ for further information on beta endpoints.
-
-
-.. |logo| image:: https://raw.githubusercontent.com/felix-hilden/tekore/master/docs/src/logo_small.png
-   :alt: logo
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/tekore
-   :alt: python version
-
-.. |downloads| image:: https://pepy.tech/badge/tekore/month
-   :alt: monthly downloads
-
-.. _github: https://github.com/felix-hilden/tekore
-.. _read the docs: https://tekore.readthedocs.io
-.. _web api: https://developer.spotify.com/documentation/web-api
+|logo|
+
+|python| |downloads|
+
+Welcome to the Python Package Index page of Tekore!
+We provide a client for the Spotify Web API for Python,
+complete with all available endpoints and authentication methods,
+async support and loads of additional features.
+Tekore allows you to interact with the API effortlessly.
+Here's five lines to get you full access and start playing your top songs.
+
+.. code:: python
+
+    import tekore as tk
+
+    conf = (client_id, client_secret, redirect_uri)
+    token = tk.prompt_for_user_token(*conf, scope=tk.scope.every)
+
+    spotify = tk.Spotify(token)
+    tracks = spotify.current_user_top_tracks(limit=10)
+    spotify.playback_start_tracks([t.id for t in tracks.items])
+
+See our online documentation on `Read The Docs`_ for tutorials,
+examples, package reference and a detailed description of features.
+If you've found a bug or would like to propose a feature,
+please submit an issue on `GitHub`_.
+Join our `Discord <https://discord.gg/wcRXgJu>`_ community
+to ask for help or discuss just about anything related to Tekore.
+You can also ask a question on
+`Stack Overflow <https://stackoverflow.com/questions/tagged/tekore>`_.
+
+Installation
+============
+Tekore can be installed from the Package Index via ``pip``.
+
+.. code:: sh
+
+    $ pip install tekore
+
+Changelog
+=========
+A detailed changelog can be found on our RTD documentation's
+`Release notes <https://tekore.readthedocs.io/page/release_notes.html>`_.
+
+Versioning
+==========
+When requiring Tekore in projects or other packages,
+please pin the version down to at least a specific major release
+to avoid compatibility issues.
+For example:
+
+.. code:: python
+
+    setup(
+        install_requires=[
+            'tekore~=4.0'
+        ]
+    )
+
+Tekore provides both stable and beta endpoints of the Web API.
+However, beta endpoints may be changed by Spotify without prior notice,
+so older versions of the library may have unintended issues.
+Because of this, Tekore follows a modified form of
+`Semantic Versioning <https://semver.org/>`_.
+Incompatible changes in the library are still introduced in major versions,
+and new features and endpoints are added in minor versions.
+But endpoints removed by Spotify are removed in minor versions and changes
+to endpoints are implemented as bugfixes.
+See the Web API `documentation <web api_>`_ for further information on beta endpoints.
+
+
+.. |logo| image:: https://raw.githubusercontent.com/felix-hilden/tekore/master/docs/src/logo_small.png
+   :alt: logo
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/tekore
+   :alt: python version
+
+.. |downloads| image:: https://pepy.tech/badge/tekore/month
+   :alt: monthly downloads
+
+.. _github: https://github.com/felix-hilden/tekore
+.. _read the docs: https://tekore.readthedocs.io
+.. _web api: https://developer.spotify.com/documentation/web-api
```

### Comparing `tekore-4.5.0/tekore/_auth/expiring/client.py` & `tekore-4.6.0/src/tekore/_auth/expiring/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,309 +1,299 @@
-from base64 import b64encode as _b64encode
-from typing import Tuple
-from hashlib import sha256
-from secrets import token_urlsafe
-
-from urllib.parse import urlencode
-
-from .decor import parse_token, parse_refreshed_token
-from .token import Token
-from ..scope import Scope
-from ..._sender import Sender, Client, send_and_process, Request
-
-OAUTH_AUTHORIZE_URL = 'https://accounts.spotify.com/authorize'
-OAUTH_TOKEN_URL = 'https://accounts.spotify.com/api/token'
-
-
-def b64encode(msg: str) -> str:
-    """Encode a unicode string in base-64."""
-    return _b64encode(msg.encode()).decode()
-
-
-def b64urlencode(msg: bytes) -> str:
-    """Encode bytes in url-safe base-64 alphabet."""
-    encoded = _b64encode(msg).decode()
-    stripped = encoded.split("=")[0]
-    return stripped.replace("+", "-").replace("/", "_")
-
-
-class Credentials(Client):
-    """
-    Client for retrieving access tokens.
-
-    Parameters
-    ----------
-    client_id
-        client id
-    client_secret
-        client secret, not required for PKCE user authorisation
-    redirect_uri
-        whitelisted redirect URI, required for user authorisation
-    sender
-        request sender
-    asynchronous
-        synchronicity requirement
-    """
-
-    def __init__(
-        self,
-        client_id: str,
-        client_secret: str = None,
-        redirect_uri: str = None,
-        sender: Sender = None,
-        asynchronous: bool = None,
-    ):
-        super().__init__(sender, asynchronous)
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.redirect_uri = redirect_uri
-
-    def __repr__(self):
-        options = [
-            f'client_id={self.client_id!r}',
-            f'client_secret={self.client_secret!r}',
-            f'redirect_uri={self.redirect_uri!r}',
-            f'sender={self.sender!r}',
-        ]
-        return type(self).__name__ + '(' + ', '.join(options) + ')'
-
-    def _token_request(self, payload: dict, auth: bool) -> Request:
-        if auth:
-            if self.client_secret is None:
-                raise ValueError(
-                    f'A client secret is required! Got `{self.client_secret}`.'
-                )
-            token = b64encode(self.client_id + ':' + self.client_secret)
-            headers = {'Authorization': f'Basic {token}'}
-        else:
-            headers = None
-
-        return Request('POST', OAUTH_TOKEN_URL, data=payload, headers=headers)
-
-    @send_and_process(parse_token(uses_pkce=False))
-    def request_client_token(self) -> Token:
-        """
-        Request a client token.
-
-        Returns
-        -------
-        Token
-            client access token
-        """
-        payload = {'grant_type': 'client_credentials'}
-        return self._token_request(payload, auth=True), ()
-
-    def _user_auth_payload(self, scope, state):
-        payload = {
-            'client_id': self.client_id,
-            'redirect_uri': self.redirect_uri,
-            'response_type': 'code',
-        }
-        if isinstance(scope, list):
-            scope = Scope(*scope)
-        if scope is not None:
-            payload['scope'] = str(scope)
-        if state is not None:
-            payload['state'] = state
-        return payload
-
-    def user_authorisation_url(
-        self,
-        scope=None,
-        state: str = None,
-        show_dialog: bool = False
-    ) -> str:
-        """
-        Construct an authorisation URL.
-
-        Step 1/2 in authorisation code flow.
-        User should be redirected to the resulting URL for authorisation.
-        Step 2/2: :meth:`request_user_token`.
-
-        Parameters
-        ----------
-        scope
-            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-            or a space-separated list of scopes as a string
-        state
-            additional state
-        show_dialog
-            force login dialog even if previously authorised
-
-        Returns
-        -------
-        str
-            login URL
-        """
-        payload = self._user_auth_payload(scope, state)
-        payload['show_dialog'] = str(show_dialog).lower()
-        return OAUTH_AUTHORIZE_URL + '?' + urlencode(payload)
-
-    @send_and_process(parse_token(uses_pkce=False))
-    def request_user_token(self, code: str) -> Token:
-        """
-        Request a new user token.
-
-        Step 2/2 in authorisation code flow.
-        Code is provided as a URL parameter in the redirect URI
-        after login in step 1: :meth:`user_authorisation_url`.
-
-        Parameters
-        ----------
-        code
-            code from redirect parameters
-
-        Returns
-        -------
-        Token
-            user access token
-        """
-        payload = {
-            'code': code,
-            'redirect_uri': self.redirect_uri,
-            'grant_type': 'authorization_code'
-        }
-        return self._token_request(payload, auth=True), ()
-
-    @send_and_process(parse_refreshed_token(uses_pkce=False))
-    def refresh_user_token(self, refresh_token: str) -> Token:
-        """
-        Request a refreshed user token.
-
-        Parameters
-        ----------
-        refresh_token
-            refresh token
-
-        Returns
-        -------
-        Token
-            refreshed user access token
-        """
-        payload = {
-            'refresh_token': refresh_token,
-            'grant_type': 'refresh_token'
-        }
-        return self._token_request(payload, auth=True), (refresh_token,)
-
-    def pkce_user_authorisation(
-        self,
-        scope=None,
-        state: str = None,
-        verifier_bytes: int = 32,
-    ) -> Tuple[str, str]:
-        """
-        Construct authorisation URL and verifier.
-
-        Step 1/2 in authorisation code flow with proof key for code exchange.
-        The user should be redirected to the resulting URL for authorisation.
-        The verifier is passed to :meth:`request_pkce_token` in step 2.
-
-        Parameters
-        ----------
-        scope
-            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-            or a space-separated list of scopes as a string
-        state
-            additional state
-        verifier_bytes
-            number of bytes to generate PKCE verifier with, ``32 <= bytes <= 96``.
-            The specified range of bytes generates the appropriate number of
-            characters (43 - 128) after base-64 encoding, as required in RFC 7636.
-
-        Returns
-        -------
-        Tuple[str, str]
-            authorisation URL and PKCE code verifier
-        """
-        assert 32 <= verifier_bytes <= 96, 'Invalid number of verifier bytes!'
-        verifier = token_urlsafe(verifier_bytes)
-
-        sha = sha256(verifier.encode())
-        challenge = b64urlencode(sha.digest())
-
-        payload = self._user_auth_payload(scope, state)
-        payload['code_challenge'] = challenge
-        payload['code_challenge_method'] = 'S256'
-
-        auth_url = OAUTH_AUTHORIZE_URL + '?' + urlencode(payload)
-        return auth_url, verifier
-
-    @send_and_process(parse_token(uses_pkce=True))
-    def request_pkce_token(self, code: str, verifier: str) -> Token:
-        """
-        Request a new PKCE user token.
-
-        Step 2/2 in authorisation code flow with proof key for code exchange.
-        Code is provided as a URL parameter in the redirect URI
-        after login in step 1: :meth:`pkce_user_authorisation`.
-
-        Parameters
-        ----------
-        code
-            code from redirect parameters
-        verifier
-            PKCE code verifier generated for authorisation URL
-
-        Returns
-        -------
-        Token
-            user access token
-        """
-        payload = {
-            'client_id': self.client_id,
-            'code': code,
-            'code_verifier': verifier,
-            'grant_type': 'authorization_code',
-            'redirect_uri': self.redirect_uri,
-        }
-        return self._token_request(payload, auth=False), ()
-
-    @send_and_process(parse_refreshed_token(uses_pkce=True))
-    def refresh_pkce_token(self, refresh_token: str) -> Token:
-        """
-        Request a refreshed PKCE user token.
-
-        Parameters
-        ----------
-        refresh_token
-            refresh token
-
-        Returns
-        -------
-        Token
-            refreshed user access token
-        """
-        payload = {
-            'client_id': self.client_id,
-            'grant_type': 'refresh_token',
-            'refresh_token': refresh_token,
-        }
-        return self._token_request(payload, auth=False), (refresh_token,)
-
-    def refresh(self, token: Token) -> Token:
-        """
-        Refresh an access token.
-
-        Both client and user tokens are accepted and refreshed.
-        The correct refreshing method is applied regardless if PKCE was used or not.
-        For client tokens, a new token is returned.
-        For user tokens, a refreshed token is returned.
-
-        Parameters
-        ----------
-        token
-            token to be refreshed
-
-        Returns
-        -------
-        Token
-            refreshed access token
-        """
-        if token.refresh_token is None:
-            return self.request_client_token()
-        elif token.uses_pkce:
-            return self.refresh_pkce_token(token.refresh_token)
-        else:
-            return self.refresh_user_token(token.refresh_token)
+from base64 import b64encode as _b64encode
+from hashlib import sha256
+from secrets import token_urlsafe
+from typing import Tuple
+from urllib.parse import urlencode
+
+from ..._sender import Client, Request, Sender, send_and_process
+from ..scope import Scope
+from .decor import parse_refreshed_token, parse_token
+from .token import Token
+
+OAUTH_AUTHORIZE_URL = "https://accounts.spotify.com/authorize"
+OAUTH_TOKEN_URL = "https://accounts.spotify.com/api/token"
+
+
+def b64encode(msg: str) -> str:
+    """Encode a unicode string in base-64."""
+    return _b64encode(msg.encode()).decode()
+
+
+def b64urlencode(msg: bytes) -> str:
+    """Encode bytes in url-safe base-64 alphabet."""
+    encoded = _b64encode(msg).decode()
+    stripped = encoded.split("=")[0]
+    return stripped.replace("+", "-").replace("/", "_")
+
+
+class Credentials(Client):
+    """
+    Client for retrieving access tokens.
+
+    Parameters
+    ----------
+    client_id
+        client id
+    client_secret
+        client secret, not required for PKCE user authorisation
+    redirect_uri
+        whitelisted redirect URI, required for user authorisation
+    sender
+        request sender
+    asynchronous
+        synchronicity requirement
+    """
+
+    def __init__(
+        self,
+        client_id: str,
+        client_secret: str = None,
+        redirect_uri: str = None,
+        sender: Sender = None,
+        asynchronous: bool = None,
+    ):
+        super().__init__(sender, asynchronous)
+        self.client_id = client_id
+        self.client_secret = client_secret
+        self.redirect_uri = redirect_uri
+
+    def __repr__(self):
+        options = [
+            f"client_id={self.client_id!r}",
+            f"client_secret={self.client_secret!r}",
+            f"redirect_uri={self.redirect_uri!r}",
+            f"sender={self.sender!r}",
+        ]
+        return type(self).__name__ + "(" + ", ".join(options) + ")"
+
+    def _token_request(self, payload: dict, auth: bool) -> Request:
+        if auth:
+            if self.client_secret is None:
+                raise ValueError(
+                    f"A client secret is required! Got `{self.client_secret}`."
+                )
+            token = b64encode(self.client_id + ":" + self.client_secret)
+            headers = {"Authorization": f"Basic {token}"}
+        else:
+            headers = None
+
+        return Request("POST", OAUTH_TOKEN_URL, data=payload, headers=headers)
+
+    @send_and_process(parse_token(uses_pkce=False))
+    def request_client_token(self) -> Token:
+        """
+        Request a client token.
+
+        Returns
+        -------
+        Token
+            client access token
+        """
+        payload = {"grant_type": "client_credentials"}
+        return self._token_request(payload, auth=True), ()
+
+    def _user_auth_payload(self, scope, state):
+        payload = {
+            "client_id": self.client_id,
+            "redirect_uri": self.redirect_uri,
+            "response_type": "code",
+        }
+        if isinstance(scope, list):
+            scope = Scope(*scope)
+        if scope is not None:
+            payload["scope"] = str(scope)
+        if state is not None:
+            payload["state"] = state
+        return payload
+
+    def user_authorisation_url(
+        self, scope=None, state: str = None, show_dialog: bool = False
+    ) -> str:
+        """
+        Construct an authorisation URL.
+
+        Step 1/2 in authorisation code flow.
+        User should be redirected to the resulting URL for authorisation.
+        Step 2/2: :meth:`request_user_token`.
+
+        Parameters
+        ----------
+        scope
+            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+            or a space-separated list of scopes as a string
+        state
+            additional state
+        show_dialog
+            force login dialog even if previously authorised
+
+        Returns
+        -------
+        str
+            login URL
+        """
+        payload = self._user_auth_payload(scope, state)
+        payload["show_dialog"] = str(show_dialog).lower()
+        return OAUTH_AUTHORIZE_URL + "?" + urlencode(payload)
+
+    @send_and_process(parse_token(uses_pkce=False))
+    def request_user_token(self, code: str) -> Token:
+        """
+        Request a new user token.
+
+        Step 2/2 in authorisation code flow.
+        Code is provided as a URL parameter in the redirect URI
+        after login in step 1: :meth:`user_authorisation_url`.
+
+        Parameters
+        ----------
+        code
+            code from redirect parameters
+
+        Returns
+        -------
+        Token
+            user access token
+        """
+        payload = {
+            "code": code,
+            "redirect_uri": self.redirect_uri,
+            "grant_type": "authorization_code",
+        }
+        return self._token_request(payload, auth=True), ()
+
+    @send_and_process(parse_refreshed_token(uses_pkce=False))
+    def refresh_user_token(self, refresh_token: str) -> Token:
+        """
+        Request a refreshed user token.
+
+        Parameters
+        ----------
+        refresh_token
+            refresh token
+
+        Returns
+        -------
+        Token
+            refreshed user access token
+        """
+        payload = {"refresh_token": refresh_token, "grant_type": "refresh_token"}
+        return self._token_request(payload, auth=True), (refresh_token,)
+
+    def pkce_user_authorisation(
+        self, scope=None, state: str = None, verifier_bytes: int = 32
+    ) -> Tuple[str, str]:
+        """
+        Construct authorisation URL and verifier.
+
+        Step 1/2 in authorisation code flow with proof key for code exchange.
+        The user should be redirected to the resulting URL for authorisation.
+        The verifier is passed to :meth:`request_pkce_token` in step 2.
+
+        Parameters
+        ----------
+        scope
+            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+            or a space-separated list of scopes as a string
+        state
+            additional state
+        verifier_bytes
+            number of bytes to generate PKCE verifier with, ``32 <= bytes <= 96``.
+            The specified range of bytes generates the appropriate number of
+            characters (43 - 128) after base-64 encoding, as required in RFC 7636.
+
+        Returns
+        -------
+        Tuple[str, str]
+            authorisation URL and PKCE code verifier
+        """
+        assert 32 <= verifier_bytes <= 96, "Invalid number of verifier bytes!"
+        verifier = token_urlsafe(verifier_bytes)
+
+        sha = sha256(verifier.encode())
+        challenge = b64urlencode(sha.digest())
+
+        payload = self._user_auth_payload(scope, state)
+        payload["code_challenge"] = challenge
+        payload["code_challenge_method"] = "S256"
+
+        auth_url = OAUTH_AUTHORIZE_URL + "?" + urlencode(payload)
+        return auth_url, verifier
+
+    @send_and_process(parse_token(uses_pkce=True))
+    def request_pkce_token(self, code: str, verifier: str) -> Token:
+        """
+        Request a new PKCE user token.
+
+        Step 2/2 in authorisation code flow with proof key for code exchange.
+        Code is provided as a URL parameter in the redirect URI
+        after login in step 1: :meth:`pkce_user_authorisation`.
+
+        Parameters
+        ----------
+        code
+            code from redirect parameters
+        verifier
+            PKCE code verifier generated for authorisation URL
+
+        Returns
+        -------
+        Token
+            user access token
+        """
+        payload = {
+            "client_id": self.client_id,
+            "code": code,
+            "code_verifier": verifier,
+            "grant_type": "authorization_code",
+            "redirect_uri": self.redirect_uri,
+        }
+        return self._token_request(payload, auth=False), ()
+
+    @send_and_process(parse_refreshed_token(uses_pkce=True))
+    def refresh_pkce_token(self, refresh_token: str) -> Token:
+        """
+        Request a refreshed PKCE user token.
+
+        Parameters
+        ----------
+        refresh_token
+            refresh token
+
+        Returns
+        -------
+        Token
+            refreshed user access token
+        """
+        payload = {
+            "client_id": self.client_id,
+            "grant_type": "refresh_token",
+            "refresh_token": refresh_token,
+        }
+        return self._token_request(payload, auth=False), (refresh_token,)
+
+    def refresh(self, token: Token) -> Token:
+        """
+        Refresh an access token.
+
+        Both client and user tokens are accepted and refreshed.
+        The correct refreshing method is applied regardless if PKCE was used or not.
+        For client tokens, a new token is returned.
+        For user tokens, a refreshed token is returned.
+
+        Parameters
+        ----------
+        token
+            token to be refreshed
+
+        Returns
+        -------
+        Token
+            refreshed access token
+        """
+        if token.refresh_token is None:
+            return self.request_client_token()
+        elif token.uses_pkce:
+            return self.refresh_pkce_token(token.refresh_token)
+        else:
+            return self.refresh_user_token(token.refresh_token)
```

### Comparing `tekore-4.5.0/tekore/_auth/expiring/decor.py` & `tekore-4.6.0/src/tekore/_auth/expiring/decor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-from typing import Callable
-
-from .token import Token
-from ..._sender.error import get_error
-from ..._sender import Request, Response
-
-
-def handle_errors(request: Request, response: Response) -> None:
-    """Examine response and raise errors accordingly."""
-    if response.status_code < 400:
-        return
-
-    if response.status_code < 500:
-        error_str = f"{response.status_code} {response.content['error']}"
-        description = response.content.get('error_description', None)
-        if description is not None:
-            error_str += ': ' + description
-    else:
-        error_str = 'Unexpected error!'
-
-    error_cls = get_error(response.status_code)
-    raise error_cls(error_str, request=request, response=response)
-
-
-def parse_token(uses_pkce: bool) -> Callable:
-    """Wrap token parsing conditional to PKCE usage."""
-    def func(request: Request, response: Response) -> Token:
-        """Parse token object from response."""
-        handle_errors(request, response)
-        return Token(response.content, uses_pkce)
-    return func
-
-
-def parse_refreshed_token(uses_pkce: bool) -> Callable:
-    """Wrap token parsing conditional to PKCE usage."""
-    def func(
-        request: Request, response: Response, refresh_token: str
-    ) -> Token:
-        """Replace new refresh token with old value if empty."""
-        handle_errors(request, response)
-        refreshed = Token(response.content, uses_pkce)
-
-        if refreshed.refresh_token is None:
-            refreshed._refresh_token = refresh_token
-
-        return refreshed
-    return func
+from typing import Callable
+
+from ..._sender import Request, Response
+from ..._sender.error import get_error
+from .token import Token
+
+
+def handle_errors(request: Request, response: Response) -> None:
+    """Examine response and raise errors accordingly."""
+    if response.status_code < 400:
+        return
+
+    if response.status_code < 500:
+        error_str = f"{response.status_code} {response.content['error']}"
+        description = response.content.get("error_description", None)
+        if description is not None:
+            error_str += ": " + description
+    else:
+        error_str = "Unexpected error!"
+
+    error_cls = get_error(response.status_code)
+    raise error_cls(error_str, request=request, response=response)
+
+
+def parse_token(uses_pkce: bool) -> Callable:
+    """Wrap token parsing conditional to PKCE usage."""
+
+    def func(request: Request, response: Response) -> Token:
+        """Parse token object from response."""
+        handle_errors(request, response)
+        return Token(response.content, uses_pkce)
+
+    return func
+
+
+def parse_refreshed_token(uses_pkce: bool) -> Callable:
+    """Wrap token parsing conditional to PKCE usage."""
+
+    def func(request: Request, response: Response, refresh_token: str) -> Token:
+        """Replace new refresh token with old value if empty."""
+        handle_errors(request, response)
+        refreshed = Token(response.content, uses_pkce)
+
+        if refreshed.refresh_token is None:
+            refreshed._refresh_token = refresh_token
+
+        return refreshed
+
+    return func
```

### Comparing `tekore-4.5.0/tekore/_auth/refreshing.py` & `tekore-4.6.0/src/tekore/_auth/refreshing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,301 +1,291 @@
-from typing import Union, Tuple
-
-from .expiring import Credentials, AccessToken, Token
-from .scope import Scope
-from .._sender import Sender
-
-
-class RefreshingToken(AccessToken):
-    """
-    Automatically refreshing access token.
-
-    Returned from utility functions and :class:`RefreshingCredentials`.
-    It shouldn't have to be instantiated outside of the functions,
-    unless you are sure that you want to.
-
-    Uses an instance of :class:`Credentials` to automatically request
-    a new access token when the old one is about to expire.
-    This occurs when the :attr:`access_token` property is read.
-
-    Both :attr:`expires_in` and :attr:`expires_at` are always ``None``,
-    and :attr:`is_expiring` is always ``False``.
-
-    Parameters
-    ----------
-    token
-        access token object
-    credentials
-        credentials manager for token refreshing
-
-    Attributes
-    ----------
-    credentials
-        credentials manager for token refreshing
-    """
-
-    def __init__(self, token: Token, credentials: Credentials):
-        self._token = token
-        self.credentials = credentials
-
-    def __repr__(self):
-        options = [
-            f'access_token={self.access_token!r}',
-            f'refresh_token={self.refresh_token!r}',
-            f'scope={self.scope!r}',
-        ]
-        return type(self).__name__ + '(' + ', '.join(options) + ')'
-
-    @property
-    def access_token(self) -> str:
-        """Bearer token value."""
-        if self._token.is_expiring:
-            self._token = self.credentials.refresh(self._token)
-
-        return self._token.access_token
-
-    @property
-    def refresh_token(self) -> Union[str, None]:
-        """
-        Refresh token for generating new access tokens.
-
-        ``None`` if the token is an application token.
-        """
-        return self._token.refresh_token
-
-    @property
-    def token_type(self) -> str:
-        """How the token may be used, always 'Bearer'."""
-        return self._token.token_type
-
-    @property
-    def scope(self) -> Scope:
-        """
-        Privileges granted to the token.
-
-        Empty :class:`Scope` if the token is an application token
-        or a user token without any scopes.
-        """
-        return self._token.scope
-
-    @property
-    def expires_in(self) -> None:
-        """Seconds until token expiration, always ``None``."""
-        return None
-
-    @property
-    def expires_at(self) -> None:
-        """When the token expires, always ``None``."""
-        return None
-
-    @property
-    def is_expiring(self) -> bool:
-        """Determine whether token is about to expire, always ``False``."""
-        return False
-
-    @property
-    def uses_pkce(self) -> bool:
-        """Proof key for code exchange used in authorisation."""
-        return self._token.uses_pkce
-
-
-class RefreshingCredentials:
-    """
-    Synchronous client for self-refreshing tokens.
-
-    Delegates to an underlying :class:`Credentials` manager
-    and parses tokens it returns into :class:`RefreshingToken`.
-
-    Parameters
-    ----------
-    client_id
-        client id
-    client_secret
-        client secret, not required for PKCE user authorisation
-    redirect_uri
-        whitelisted redirect URI, required for user authorisation
-    sender
-        synchronous request sender
-
-    Attributes
-    ----------
-    credentials
-        underlying credentials manager for token refreshing
-    """
-
-    def __init__(
-        self,
-        client_id: str,
-        client_secret: str = None,
-        redirect_uri: str = None,
-        sender: Sender = None
-    ):
-        self.credentials = Credentials(
-            client_id,
-            client_secret,
-            redirect_uri,
-            sender,
-            asynchronous=False
-        )
-
-    def __repr__(self):
-        options = [
-            f'client_id={self.credentials.client_id!r}',
-            f'client_secret={self.credentials.client_secret!r}',
-            f'redirect_uri={self.credentials.redirect_uri!r}',
-            f'sender={self.credentials.sender!r}',
-        ]
-        return type(self).__name__ + '(' + ', '.join(options) + ')'
-
-    def request_client_token(self) -> RefreshingToken:
-        """
-        Request a refreshing client token.
-
-        Returns
-        -------
-        RefreshingToken
-            automatically refreshing client token
-        """
-        token = self.credentials.request_client_token()
-        return RefreshingToken(token, self.credentials)
-
-    def user_authorisation_url(
-        self,
-        scope=None,
-        state: str = None,
-        show_dialog: bool = False
-    ) -> str:
-        """
-        Construct an authorisation URL.
-
-        Step 1/2 in authorisation code flow.
-        User should be redirected to the resulting URL for authorisation.
-        Step 2/2: :meth:`request_user_token`.
-
-        Parameters
-        ----------
-        scope
-            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-            or a space-separated list of scopes as a string
-        state
-            additional state
-        show_dialog
-            force login dialog even if previously authorised
-
-        Returns
-        -------
-        str
-            login URL
-        """
-        return self.credentials.user_authorisation_url(scope, state, show_dialog)
-
-    def request_user_token(self, code: str) -> RefreshingToken:
-        """
-        Request a new refreshing user token.
-
-        Step 2/2 in authorisation code flow.
-        Code is provided as a URL parameter in the redirect URI
-        after login in step 1: :meth:`user_authorisation_url`.
-
-        Parameters
-        ----------
-        code
-            code from redirect parameters
-
-        Returns
-        -------
-        RefreshingToken
-            automatically refreshing user token
-        """
-        token = self.credentials.request_user_token(code)
-        return RefreshingToken(token, self.credentials)
-
-    def refresh_user_token(self, refresh_token: str) -> RefreshingToken:
-        """
-        Request an automatically refreshing user token with a refresh token.
-
-        Parameters
-        ----------
-        refresh_token
-            refresh token
-
-        Returns
-        -------
-        RefreshingToken
-            automatically refreshing user token
-        """
-        token = self.credentials.refresh_user_token(refresh_token)
-        return RefreshingToken(token, self.credentials)
-
-    def pkce_user_authorisation(
-        self,
-        scope=None,
-        state: str = None,
-        verifier_bytes: int = 32,
-    ) -> Tuple[str, str]:
-        """
-        Construct authorisation URL and verifier.
-
-        Step 1/2 in authorisation code flow with proof key for code exchange.
-        The user should be redirected to the resulting URL for authorisation.
-        The verifier is passed to :meth:`request_pkce_token` in step 2.
-
-        Parameters
-        ----------
-        scope
-            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-            or a space-separated list of scopes as a string
-        state
-            additional state
-        verifier_bytes
-            number of bytes to generate PKCE verifier with, ``32 <= bytes <= 96``.
-            The specified range of bytes generates the appropriate number of
-            characters (43 - 128) after base-64 encoding, as required in RFC 7636.
-
-        Returns
-        -------
-        Tuple[str, str]
-            authorisation URL and PKCE code verifier
-        """
-        return self.credentials.pkce_user_authorisation(scope, state, verifier_bytes)
-
-    def request_pkce_token(self, code: str, verifier: str) -> RefreshingToken:
-        """
-        Request a new PKCE user token.
-
-        Step 2/2 in authorisation code flow with proof key for code exchange.
-        Code is provided as a URL parameter in the redirect URI
-        after login in step 1: :meth:`pkce_user_authorisation`.
-
-        Parameters
-        ----------
-        code
-            code from redirect parameters
-        verifier
-            PKCE code verifier generated for authorisation URL
-
-        Returns
-        -------
-        RefreshingToken
-            user access token
-        """
-        token = self.credentials.request_pkce_token(code, verifier)
-        return RefreshingToken(token, self.credentials)
-
-    def refresh_pkce_token(self, refresh_token: str) -> RefreshingToken:
-        """
-        Request a refreshed PKCE user token.
-
-        Parameters
-        ----------
-        refresh_token
-            refresh token
-
-        Returns
-        -------
-        RefreshingToken
-            refreshed user access token
-        """
-        token = self.credentials.refresh_pkce_token(refresh_token)
-        return RefreshingToken(token, self.credentials)
+from typing import Tuple, Union
+
+from .._sender import Sender
+from .expiring import AccessToken, Credentials, Token
+from .scope import Scope
+
+
+class RefreshingToken(AccessToken):
+    """
+    Automatically refreshing access token.
+
+    Returned from utility functions and :class:`RefreshingCredentials`.
+    It shouldn't have to be instantiated outside of the functions,
+    unless you are sure that you want to.
+
+    Uses an instance of :class:`Credentials` to automatically request
+    a new access token when the old one is about to expire.
+    This occurs when the :attr:`access_token` property is read.
+
+    Both :attr:`expires_in` and :attr:`expires_at` are always ``None``,
+    and :attr:`is_expiring` is always ``False``.
+
+    Parameters
+    ----------
+    token
+        access token object
+    credentials
+        credentials manager for token refreshing
+
+    Attributes
+    ----------
+    credentials
+        credentials manager for token refreshing
+    """
+
+    def __init__(self, token: Token, credentials: Credentials):
+        self._token = token
+        self.credentials = credentials
+
+    def __repr__(self):
+        options = [
+            f"access_token={self.access_token!r}",
+            f"refresh_token={self.refresh_token!r}",
+            f"scope={self.scope!r}",
+        ]
+        return type(self).__name__ + "(" + ", ".join(options) + ")"
+
+    @property
+    def access_token(self) -> str:
+        """Bearer token value."""
+        if self._token.is_expiring:
+            self._token = self.credentials.refresh(self._token)
+
+        return self._token.access_token
+
+    @property
+    def refresh_token(self) -> Union[str, None]:
+        """
+        Refresh token for generating new access tokens.
+
+        ``None`` if the token is an application token.
+        """
+        return self._token.refresh_token
+
+    @property
+    def token_type(self) -> str:
+        """How the token may be used, always 'Bearer'."""
+        return self._token.token_type
+
+    @property
+    def scope(self) -> Scope:
+        """
+        Privileges granted to the token.
+
+        Empty :class:`Scope` if the token is an application token
+        or a user token without any scopes.
+        """
+        return self._token.scope
+
+    @property
+    def expires_in(self) -> None:
+        """Seconds until token expiration, always ``None``."""
+        return None
+
+    @property
+    def expires_at(self) -> None:
+        """When the token expires, always ``None``."""
+        return None
+
+    @property
+    def is_expiring(self) -> bool:
+        """Determine whether token is about to expire, always ``False``."""
+        return False
+
+    @property
+    def uses_pkce(self) -> bool:
+        """Proof key for code exchange used in authorisation."""
+        return self._token.uses_pkce
+
+
+class RefreshingCredentials:
+    """
+    Synchronous client for self-refreshing tokens.
+
+    Delegates to an underlying :class:`Credentials` manager
+    and parses tokens it returns into :class:`RefreshingToken`.
+
+    Parameters
+    ----------
+    client_id
+        client id
+    client_secret
+        client secret, not required for PKCE user authorisation
+    redirect_uri
+        whitelisted redirect URI, required for user authorisation
+    sender
+        synchronous request sender
+
+    Attributes
+    ----------
+    credentials
+        underlying credentials manager for token refreshing
+    """
+
+    def __init__(
+        self,
+        client_id: str,
+        client_secret: str = None,
+        redirect_uri: str = None,
+        sender: Sender = None,
+    ):
+        self.credentials = Credentials(
+            client_id, client_secret, redirect_uri, sender, asynchronous=False
+        )
+
+    def __repr__(self):
+        options = [
+            f"client_id={self.credentials.client_id!r}",
+            f"client_secret={self.credentials.client_secret!r}",
+            f"redirect_uri={self.credentials.redirect_uri!r}",
+            f"sender={self.credentials.sender!r}",
+        ]
+        return type(self).__name__ + "(" + ", ".join(options) + ")"
+
+    def request_client_token(self) -> RefreshingToken:
+        """
+        Request a refreshing client token.
+
+        Returns
+        -------
+        RefreshingToken
+            automatically refreshing client token
+        """
+        token = self.credentials.request_client_token()
+        return RefreshingToken(token, self.credentials)
+
+    def user_authorisation_url(
+        self, scope=None, state: str = None, show_dialog: bool = False
+    ) -> str:
+        """
+        Construct an authorisation URL.
+
+        Step 1/2 in authorisation code flow.
+        User should be redirected to the resulting URL for authorisation.
+        Step 2/2: :meth:`request_user_token`.
+
+        Parameters
+        ----------
+        scope
+            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+            or a space-separated list of scopes as a string
+        state
+            additional state
+        show_dialog
+            force login dialog even if previously authorised
+
+        Returns
+        -------
+        str
+            login URL
+        """
+        return self.credentials.user_authorisation_url(scope, state, show_dialog)
+
+    def request_user_token(self, code: str) -> RefreshingToken:
+        """
+        Request a new refreshing user token.
+
+        Step 2/2 in authorisation code flow.
+        Code is provided as a URL parameter in the redirect URI
+        after login in step 1: :meth:`user_authorisation_url`.
+
+        Parameters
+        ----------
+        code
+            code from redirect parameters
+
+        Returns
+        -------
+        RefreshingToken
+            automatically refreshing user token
+        """
+        token = self.credentials.request_user_token(code)
+        return RefreshingToken(token, self.credentials)
+
+    def refresh_user_token(self, refresh_token: str) -> RefreshingToken:
+        """
+        Request an automatically refreshing user token with a refresh token.
+
+        Parameters
+        ----------
+        refresh_token
+            refresh token
+
+        Returns
+        -------
+        RefreshingToken
+            automatically refreshing user token
+        """
+        token = self.credentials.refresh_user_token(refresh_token)
+        return RefreshingToken(token, self.credentials)
+
+    def pkce_user_authorisation(
+        self, scope=None, state: str = None, verifier_bytes: int = 32
+    ) -> Tuple[str, str]:
+        """
+        Construct authorisation URL and verifier.
+
+        Step 1/2 in authorisation code flow with proof key for code exchange.
+        The user should be redirected to the resulting URL for authorisation.
+        The verifier is passed to :meth:`request_pkce_token` in step 2.
+
+        Parameters
+        ----------
+        scope
+            token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+            a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+            or a space-separated list of scopes as a string
+        state
+            additional state
+        verifier_bytes
+            number of bytes to generate PKCE verifier with, ``32 <= bytes <= 96``.
+            The specified range of bytes generates the appropriate number of
+            characters (43 - 128) after base-64 encoding, as required in RFC 7636.
+
+        Returns
+        -------
+        Tuple[str, str]
+            authorisation URL and PKCE code verifier
+        """
+        return self.credentials.pkce_user_authorisation(scope, state, verifier_bytes)
+
+    def request_pkce_token(self, code: str, verifier: str) -> RefreshingToken:
+        """
+        Request a new PKCE user token.
+
+        Step 2/2 in authorisation code flow with proof key for code exchange.
+        Code is provided as a URL parameter in the redirect URI
+        after login in step 1: :meth:`pkce_user_authorisation`.
+
+        Parameters
+        ----------
+        code
+            code from redirect parameters
+        verifier
+            PKCE code verifier generated for authorisation URL
+
+        Returns
+        -------
+        RefreshingToken
+            user access token
+        """
+        token = self.credentials.request_pkce_token(code, verifier)
+        return RefreshingToken(token, self.credentials)
+
+    def refresh_pkce_token(self, refresh_token: str) -> RefreshingToken:
+        """
+        Request a refreshed PKCE user token.
+
+        Parameters
+        ----------
+        refresh_token
+            refresh token
+
+        Returns
+        -------
+        RefreshingToken
+            refreshed user access token
+        """
+        token = self.credentials.refresh_pkce_token(refresh_token)
+        return RefreshingToken(token, self.credentials)
```

### Comparing `tekore-4.5.0/tekore/_auth/scope.py` & `tekore-4.6.0/src/tekore/_auth/scope.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-from enum import Enum
-
-
-class scope(Enum):
-    """
-    User access token privileges.
-
-    The string representation of a member is its enum value.
-
-    .. code:: python
-
-       s = tk.scope.user_read_email
-       print(s)  # -> 'user-read-email'
-
-    Also provides three scopes that are a combination of others.
-
-    .. code:: python
-
-        tk.scope.read: Scope = ...            # All read scopes
-        tk.scope.write: Scope = ...           # All write scopes
-        tk.scope.every: Scope = read + write  # All available scopes
-
-    .. note::
-
-        :attr:`app_remote_control` and :attr:`streaming` are only used outside
-        of the Web API, and are not included in the premade scope combinations.
-
-    Addition and subtraction from both sides is supported
-    but delegated to :class:`Scope` and always returns a :class:`Scope`.
-    """
-
-    user_read_email = 'user-read-email'
-    user_read_private = 'user-read-private'
-    user_top_read = 'user-top-read'
-    user_read_recently_played = 'user-read-recently-played'
-
-    user_follow_read = 'user-follow-read'
-    user_follow_modify = 'user-follow-modify'
-    user_library_read = 'user-library-read'
-    user_library_modify = 'user-library-modify'
-
-    user_read_currently_playing = 'user-read-currently-playing'
-    user_read_playback_state = 'user-read-playback-state'
-    user_read_playback_position = 'user-read-playback-position'
-    user_modify_playback_state = 'user-modify-playback-state'
-
-    playlist_modify_public = 'playlist-modify-public'
-    playlist_read_collaborative = 'playlist-read-collaborative'
-    playlist_read_private = 'playlist-read-private'
-    playlist_modify_private = 'playlist-modify-private'
-
-    ugc_image_upload = 'ugc-image-upload'
-
-    app_remote_control = 'app-remote-control'
-    streaming = 'streaming'
-
-    def __str__(self):
-        """Enum value."""
-        return self.value
-
-    def __add__(self, other) -> 'Scope':
-        """Combine to a set of scopes."""
-        return Scope(self) + other
-
-    def __radd__(self, other) -> 'Scope':
-        """Combine to a set of scopes."""
-        return other + Scope(self)
-
-    def __sub__(self, other) -> 'Scope':
-        """Remove scope from another."""
-        return Scope(self) - other
-
-    def __rsub__(self, other) -> 'Scope':
-        """Remove scope from another."""
-        return other - Scope(self)
-
-
-class Scope(frozenset):
-    """
-    Set of :class:`scopes <scope>` for a token.
-
-    Instantiated with an unpacked list of strings or :class:`scopes <scope>`.
-
-    .. code:: python
-
-        bruce = tk.Scope(*tk.scope)
-        sally = tk.Scope(tk.scope.user_read_email, 'ugc-image-upload')
-        elise = tk.Scope(*sally, *timmy, tk.scope.user_follow_modify)
-
-    Also supports flexible addition and subtraction from both sides
-    with strings, :class:`scopes <scope>` and other :class:`Scope` objects.
-    Addition is a set-like union, subtraction is a set-like relative complement.
-    If any operation is unsuccessful, :class:`NotImplementedError` is raised.
-
-    .. code:: python
-
-        waldo = tk.scopes.user_follow_read + sally + elise - 'user-read-email'
-
-    The string representation of a :class:`Scope` is a sorted,
-    space-separated concatenation of its members.
-
-    .. code:: python
-
-       s = tk.Scope('b', 'c', 'a')
-       print(s)  # -> 'a b c'
-    """
-
-    def __new__(cls, *members):
-        """
-        Construct a new set of scopes.
-
-        Parameters
-        ----------
-        members
-            unpacked list of members of the new scope
-        """
-        return super().__new__(cls, [str(m) for m in members])
-
-    def __repr__(self):
-        """Readable representation."""
-        members = "'" + "', '".join(sorted(self)) + "'"
-        return f'Scope({members})'
-
-    def __str__(self):
-        """Join members with spaces."""
-        return ' '.join(sorted(self))
-
-    def __add__(self, other) -> 'Scope':
-        """Combine two sets of scopes."""
-        if isinstance(other, (str, scope)):
-            other = {str(other)}
-        elif not isinstance(other, Scope):
-            e = f'Addition not defined for {type(self)} and {type(other)}!'
-            raise NotImplementedError(e)
-        return type(self)(*self.union(other))
-
-    def __radd__(self, other) -> 'Scope':
-        """Combine two sets of scopes."""
-        return self + other
-
-    def __sub__(self, other) -> 'Scope':
-        """Remove scopes from a set."""
-        if isinstance(other, (str, scope)):
-            other = {str(other)}
-        elif not isinstance(other, Scope):
-            e = f'Difference not defined for {type(self)} and {type(other)}!'
-            raise NotImplementedError(e)
-        return type(self)(*self.difference(other))
-
-    def __rsub__(self, other) -> 'Scope':
-        """Remove scopes from a set."""
-        if not isinstance(other, (str, scope)):
-            e = f'Difference not defined for {type(other)} and {type(self)}!'
-            raise NotImplementedError(e)
-        return Scope(other) - self
-
-
-scope.read = Scope(
-    scope.user_read_email,
-    scope.user_read_private,
-    scope.user_top_read,
-    scope.user_read_recently_played,
-    scope.user_follow_read,
-    scope.user_library_read,
-    scope.user_read_currently_playing,
-    scope.user_read_playback_state,
-    scope.user_read_playback_position,
-    scope.playlist_read_collaborative,
-    scope.playlist_read_private
-)
-scope.write = Scope(
-    scope.user_follow_modify,
-    scope.user_library_modify,
-    scope.user_modify_playback_state,
-    scope.playlist_modify_public,
-    scope.playlist_modify_private,
-    scope.ugc_image_upload
-)
-scope.every = scope.read + scope.write
+from enum import Enum
+
+
+class scope(Enum):
+    """
+    User access token privileges.
+
+    The string representation of a member is its enum value.
+
+    .. code:: python
+
+       s = tk.scope.user_read_email
+       print(s)  # -> 'user-read-email'
+
+    Also provides three scopes that are a combination of others.
+
+    .. code:: python
+
+        tk.scope.read: Scope = ...            # All read scopes
+        tk.scope.write: Scope = ...           # All write scopes
+        tk.scope.every: Scope = read + write  # All available scopes
+
+    .. note::
+
+        :attr:`app_remote_control` and :attr:`streaming` are only used outside
+        of the Web API, and are not included in the premade scope combinations.
+
+    Addition and subtraction from both sides is supported
+    but delegated to :class:`Scope` and always returns a :class:`Scope`.
+    """
+
+    user_read_email = "user-read-email"
+    user_read_private = "user-read-private"
+    user_top_read = "user-top-read"
+    user_read_recently_played = "user-read-recently-played"
+
+    user_follow_read = "user-follow-read"
+    user_follow_modify = "user-follow-modify"
+    user_library_read = "user-library-read"
+    user_library_modify = "user-library-modify"
+
+    user_read_currently_playing = "user-read-currently-playing"
+    user_read_playback_state = "user-read-playback-state"
+    user_read_playback_position = "user-read-playback-position"
+    user_modify_playback_state = "user-modify-playback-state"
+
+    playlist_modify_public = "playlist-modify-public"
+    playlist_read_collaborative = "playlist-read-collaborative"
+    playlist_read_private = "playlist-read-private"
+    playlist_modify_private = "playlist-modify-private"
+
+    ugc_image_upload = "ugc-image-upload"
+
+    app_remote_control = "app-remote-control"
+    streaming = "streaming"
+
+    def __str__(self):
+        """Enum value."""
+        return self.value
+
+    def __add__(self, other) -> "Scope":
+        """Combine to a set of scopes."""
+        return Scope(self) + other
+
+    def __radd__(self, other) -> "Scope":
+        """Combine to a set of scopes."""
+        return other + Scope(self)
+
+    def __sub__(self, other) -> "Scope":
+        """Remove scope from another."""
+        return Scope(self) - other
+
+    def __rsub__(self, other) -> "Scope":
+        """Remove scope from another."""
+        return other - Scope(self)
+
+
+class Scope(frozenset):
+    """
+    Set of :class:`scopes <scope>` for a token.
+
+    Instantiated with an unpacked list of strings or :class:`scopes <scope>`.
+
+    .. code:: python
+
+        bruce = tk.Scope(*tk.scope)
+        sally = tk.Scope(tk.scope.user_read_email, 'ugc-image-upload')
+        elise = tk.Scope(*sally, *timmy, tk.scope.user_follow_modify)
+
+    Also supports flexible addition and subtraction from both sides
+    with strings, :class:`scopes <scope>` and other :class:`Scope` objects.
+    Addition is a set-like union, subtraction is a set-like relative complement.
+    If any operation is unsuccessful, :class:`NotImplementedError` is raised.
+
+    .. code:: python
+
+        waldo = tk.scopes.user_follow_read + sally + elise - 'user-read-email'
+
+    The string representation of a :class:`Scope` is a sorted,
+    space-separated concatenation of its members.
+
+    .. code:: python
+
+       s = tk.Scope('b', 'c', 'a')
+       print(s)  # -> 'a b c'
+    """
+
+    def __new__(cls, *members):
+        """
+        Construct a new set of scopes.
+
+        Parameters
+        ----------
+        members
+            unpacked list of members of the new scope
+        """
+        return super().__new__(cls, [str(m) for m in members])
+
+    def __repr__(self):
+        """Readable representation."""
+        members = "'" + "', '".join(sorted(self)) + "'"
+        return f"Scope({members})"
+
+    def __str__(self):
+        """Join members with spaces."""
+        return " ".join(sorted(self))
+
+    def __add__(self, other) -> "Scope":
+        """Combine two sets of scopes."""
+        if isinstance(other, (str, scope)):
+            other = {str(other)}
+        elif not isinstance(other, Scope):
+            e = f"Addition not defined for {type(self)} and {type(other)}!"
+            raise NotImplementedError(e)
+        return type(self)(*self.union(other))
+
+    def __radd__(self, other) -> "Scope":
+        """Combine two sets of scopes."""
+        return self + other
+
+    def __sub__(self, other) -> "Scope":
+        """Remove scopes from a set."""
+        if isinstance(other, (str, scope)):
+            other = {str(other)}
+        elif not isinstance(other, Scope):
+            e = f"Difference not defined for {type(self)} and {type(other)}!"
+            raise NotImplementedError(e)
+        return type(self)(*self.difference(other))
+
+    def __rsub__(self, other) -> "Scope":
+        """Remove scopes from a set."""
+        if not isinstance(other, (str, scope)):
+            e = f"Difference not defined for {type(other)} and {type(self)}!"
+            raise NotImplementedError(e)
+        return Scope(other) - self
+
+
+scope.read = Scope(
+    scope.user_read_email,
+    scope.user_read_private,
+    scope.user_top_read,
+    scope.user_read_recently_played,
+    scope.user_follow_read,
+    scope.user_library_read,
+    scope.user_read_currently_playing,
+    scope.user_read_playback_state,
+    scope.user_read_playback_position,
+    scope.playlist_read_collaborative,
+    scope.playlist_read_private,
+)
+scope.write = Scope(
+    scope.user_follow_modify,
+    scope.user_library_modify,
+    scope.user_modify_playback_state,
+    scope.playlist_modify_public,
+    scope.playlist_modify_private,
+    scope.ugc_image_upload,
+)
+scope.every = scope.read + scope.write
```

### Comparing `tekore-4.5.0/tekore/_auth/util.py` & `tekore-4.6.0/src/tekore/_auth/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,338 +1,321 @@
-import webbrowser
-
-from typing import Union
-from secrets import token_urlsafe
-from urllib.parse import urlparse, parse_qs
-
-from .expiring import Token, Credentials
-from .refreshing import RefreshingToken, RefreshingCredentials
-
-
-def gen_state(n_bytes: int = 32) -> str:
-    """
-    Generate state to use in user authorisation.
-
-    The generated state is random and URL-safe.
-    It is generated using :func:`secrets.token_urlsafe`.
-    """
-    return token_urlsafe(n_bytes)
-
-
-def _parse_url_param(url: str, param: str) -> str:
-    query = urlparse(url).query
-    code = parse_qs(query).get(param, None)
-
-    if code is None:
-        raise KeyError(f'Passed URL contains no parameter `{param}`!')
-    elif len(code) > 1:
-        raise KeyError(f'Passed URL contains multiple values for `{param}`!')
-
-    return code[0]
-
-
-def parse_code_from_url(url: str) -> str:
-    """
-    Parse an URL for parameter 'code'.
-
-    Returns
-    -------
-    str
-        value of 'code'
-
-    Raises
-    ------
-    KeyError
-        if 'code' is not available or has multiple values
-    """
-    return _parse_url_param(url, 'code')
-
-
-def parse_state_from_url(url: str) -> str:
-    """
-    Parse an URL for parameter 'state'.
-
-    Returns
-    -------
-    str
-        value of 'state'
-
-    Raises
-    ------
-    KeyError
-        if 'state' is not available or has multiple values
-    """
-    return _parse_url_param(url, 'state')
-
-
-class UserAuth:
-    """
-    Implement user authorisation flow.
-
-    Implements all steps and security checks for user authorisation.
-    The responsibility of the caller is to redirect a user to the given URL
-    and provide the resulting redirect URI or its parameters.
-    Can be used with an asynchronous credentials client.
-
-    Parameters
-    ----------
-    cred
-        credentials client
-    scope
-        token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-        a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-        or a space-separated list of scopes as a string
-    pkce
-        use proof key for code exchange
-
-    Attributes
-    ----------
-    url: str
-        address to redirect a user to for authorisation
-    state: str
-        generated additional state
-    verifier: str
-        PKCE code verifier, :class:`None` if PKCE is not used
-
-    Examples
-    --------
-    .. code:: python
-
-        auth = tk.UserAuth(cred, scope)
-
-        # Redirect user to auth.url and parse parameters
-        code, state = ...
-        token = auth.request_token(code, state)
-
-        # Or leave parsing to UserAuth
-        redirected = ...
-        token = auth.request_token(url=redirected)
-
-        # With an asynchronous client
-        token = await auth.request_token(url=redirected)
-    """
-
-    def __init__(
-        self,
-        cred: Union[Credentials, RefreshingCredentials],
-        scope=None,
-        pkce: bool = False,
-    ):
-        self._cred = cred
-        self.state = gen_state()
-        self.verifier = None
-        if pkce:
-            self.url, self.verifier = self._cred.pkce_user_authorisation(
-                scope, self.state
-            )
-        else:
-            self.url = self._cred.user_authorisation_url(
-                scope, self.state, show_dialog=True
-            )
-
-    def __repr__(self):
-        options = [
-            f'cred={self._cred!r}',
-            f'url={self.url!r}',
-            f'state={self.state!r}',
-            f'verifier={self.verifier}',
-        ]
-        return type(self).__name__ + '(' + ', '.join(options) + ')'
-
-    def request_token(
-        self,
-        code: str = None,
-        state: str = None,
-        url: str = None,
-    ) -> Union[Token, RefreshingToken]:
-        """
-        Verify state consistency and request token.
-
-        Parameters
-        ----------
-        code
-            code from redirect parameters, required if url was not specified
-        state
-            state from redirect parameters, required if url was not specified
-        url
-            if specified, code and state are parsed from this URL instead
-
-        Returns
-        -------
-        Union[Token, RefreshingToken]
-            access token
-
-        Raises
-        ------
-        AssertionError
-            if state is inconsistent
-        """
-        if url is not None:
-            code = parse_code_from_url(url)
-            state = parse_state_from_url(url)
-
-        if self.state != state:
-            raise AssertionError(
-                f'Inconsistent state! Expected `{self.state}`, got `{state}`.'
-            )
-
-        if self.verifier is not None:
-            return self._cred.request_pkce_token(code, self.verifier)
-        else:
-            return self._cred.request_user_token(code)
-
-
-def request_client_token(
-    client_id: str,
-    client_secret: str
-) -> RefreshingToken:
-    """
-    Request for client credentials.
-
-    Parameters
-    ----------
-    client_id
-        client ID
-    client_secret
-        client secret
-
-    Returns
-    -------
-    RefreshingToken
-        automatically refreshing client token
-    """
-    cred = RefreshingCredentials(client_id, client_secret)
-    return cred.request_client_token()
-
-
-def prompt_for_user_token(
-    client_id: str,
-    client_secret: str,
-    redirect_uri: str,
-    scope=None
-) -> RefreshingToken:
-    """
-    Prompt for manual authorisation.
-
-    Open a web browser for the user to log in with Spotify.
-    Prompt to paste the URL after logging in to complete authorisation.
-
-    Parameters
-    ----------
-    client_id
-        client ID
-    client_secret
-        client secret
-    redirect_uri
-        whitelisted redirect URI
-    scope
-        token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-        a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-        or a space-separated list of scopes as a string
-
-    Returns
-    -------
-    RefreshingToken
-        automatically refreshing user token
-
-    Raises
-    ------
-    AssertionError
-        if state is inconsistent
-    """
-    cred = RefreshingCredentials(client_id, client_secret, redirect_uri)
-    auth = UserAuth(cred, scope=scope)
-
-    print('Opening browser for Spotify login...')
-    webbrowser.open(auth.url)
-    redirected = input('Please paste redirect URL: ').strip()
-    return auth.request_token(url=redirected)
-
-
-def refresh_user_token(
-    client_id: str,
-    client_secret: str,
-    refresh_token: str
-) -> RefreshingToken:
-    """
-    Request a refreshed user token.
-
-    Parameters
-    ----------
-    client_id
-        client ID
-    client_secret
-        client secret
-    refresh_token
-        refresh token
-
-    Returns
-    -------
-    RefreshingToken
-        automatically refreshing user token
-    """
-    cred = RefreshingCredentials(client_id, client_secret)
-    return cred.refresh_user_token(refresh_token)
-
-
-def prompt_for_pkce_token(
-    client_id: str,
-    redirect_uri: str,
-    scope=None
-) -> RefreshingToken:
-    """
-    Prompt for manual authorisation with PKCE.
-
-    Open a web browser for the user to log in with Spotify.
-    Prompt to paste the URL after logging in to complete authorisation.
-
-    Parameters
-    ----------
-    client_id
-        client ID
-    redirect_uri
-        whitelisted redirect URI
-    scope
-        token privileges, accepts a :class:`Scope`, a single :class:`scope`,
-        a list of :class:`scopes <scope>` and strings for :class:`Scope`,
-        or a space-separated list of scopes as a string
-
-    Returns
-    -------
-    RefreshingToken
-        automatically refreshing PKCE user token
-
-    Raises
-    ------
-    AssertionError
-        if state is inconsistent
-    """
-    cred = RefreshingCredentials(client_id, redirect_uri=redirect_uri)
-    auth = UserAuth(cred, scope=scope, pkce=True)
-
-    print('Opening browser for Spotify login...')
-    webbrowser.open(auth.url)
-    redirected = input('Please paste redirect URL: ').strip()
-    return auth.request_token(url=redirected)
-
-
-def refresh_pkce_token(
-    client_id: str,
-    refresh_token: str
-) -> RefreshingToken:
-    """
-    Request a refreshed PKCE user token.
-
-    Parameters
-    ----------
-    client_id
-        client ID
-    refresh_token
-        refresh token
-
-    Returns
-    -------
-    RefreshingToken
-        automatically refreshing user token
-    """
-    cred = RefreshingCredentials(client_id)
-    return cred.refresh_pkce_token(refresh_token)
+import webbrowser
+from secrets import token_urlsafe
+from typing import Union
+from urllib.parse import parse_qs, urlparse
+
+from .expiring import Credentials, Token
+from .refreshing import RefreshingCredentials, RefreshingToken
+
+
+def gen_state(n_bytes: int = 32) -> str:
+    """
+    Generate state to use in user authorisation.
+
+    The generated state is random and URL-safe.
+    It is generated using :func:`secrets.token_urlsafe`.
+    """
+    return token_urlsafe(n_bytes)
+
+
+def _parse_url_param(url: str, param: str) -> str:
+    query = urlparse(url).query
+    code = parse_qs(query).get(param, None)
+
+    if code is None:
+        raise KeyError(f"Passed URL contains no parameter `{param}`!")
+    elif len(code) > 1:
+        raise KeyError(f"Passed URL contains multiple values for `{param}`!")
+
+    return code[0]
+
+
+def parse_code_from_url(url: str) -> str:
+    """
+    Parse an URL for parameter 'code'.
+
+    Returns
+    -------
+    str
+        value of 'code'
+
+    Raises
+    ------
+    KeyError
+        if 'code' is not available or has multiple values
+    """
+    return _parse_url_param(url, "code")
+
+
+def parse_state_from_url(url: str) -> str:
+    """
+    Parse an URL for parameter 'state'.
+
+    Returns
+    -------
+    str
+        value of 'state'
+
+    Raises
+    ------
+    KeyError
+        if 'state' is not available or has multiple values
+    """
+    return _parse_url_param(url, "state")
+
+
+class UserAuth:
+    """
+    Implement user authorisation flow.
+
+    Implements all steps and security checks for user authorisation.
+    The responsibility of the caller is to redirect a user to the given URL
+    and provide the resulting redirect URI or its parameters.
+    Can be used with an asynchronous credentials client.
+
+    Parameters
+    ----------
+    cred
+        credentials client
+    scope
+        token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+        a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+        or a space-separated list of scopes as a string
+    pkce
+        use proof key for code exchange
+
+    Attributes
+    ----------
+    url: str
+        address to redirect a user to for authorisation
+    state: str
+        generated additional state
+    verifier: str
+        PKCE code verifier, :class:`None` if PKCE is not used
+
+    Examples
+    --------
+    .. code:: python
+
+        auth = tk.UserAuth(cred, scope)
+
+        # Redirect user to auth.url and parse parameters
+        code, state = ...
+        token = auth.request_token(code, state)
+
+        # Or leave parsing to UserAuth
+        redirected = ...
+        token = auth.request_token(url=redirected)
+
+        # With an asynchronous client
+        token = await auth.request_token(url=redirected)
+    """
+
+    def __init__(
+        self,
+        cred: Union[Credentials, RefreshingCredentials],
+        scope=None,
+        pkce: bool = False,
+    ):
+        self._cred = cred
+        self.state = gen_state()
+        self.verifier = None
+        if pkce:
+            self.url, self.verifier = self._cred.pkce_user_authorisation(
+                scope, self.state
+            )
+        else:
+            self.url = self._cred.user_authorisation_url(
+                scope, self.state, show_dialog=True
+            )
+
+    def __repr__(self):
+        options = [
+            f"cred={self._cred!r}",
+            f"url={self.url!r}",
+            f"state={self.state!r}",
+            f"verifier={self.verifier}",
+        ]
+        return type(self).__name__ + "(" + ", ".join(options) + ")"
+
+    def request_token(
+        self, code: str = None, state: str = None, url: str = None
+    ) -> Union[Token, RefreshingToken]:
+        """
+        Verify state consistency and request token.
+
+        Parameters
+        ----------
+        code
+            code from redirect parameters, required if url was not specified
+        state
+            state from redirect parameters, required if url was not specified
+        url
+            if specified, code and state are parsed from this URL instead
+
+        Returns
+        -------
+        Union[Token, RefreshingToken]
+            access token
+
+        Raises
+        ------
+        AssertionError
+            if state is inconsistent
+        """
+        if url is not None:
+            code = parse_code_from_url(url)
+            state = parse_state_from_url(url)
+
+        if self.state != state:
+            raise AssertionError(
+                f"Inconsistent state! Expected `{self.state}`, got `{state}`."
+            )
+
+        if self.verifier is not None:
+            return self._cred.request_pkce_token(code, self.verifier)
+        else:
+            return self._cred.request_user_token(code)
+
+
+def request_client_token(client_id: str, client_secret: str) -> RefreshingToken:
+    """
+    Request for client credentials.
+
+    Parameters
+    ----------
+    client_id
+        client ID
+    client_secret
+        client secret
+
+    Returns
+    -------
+    RefreshingToken
+        automatically refreshing client token
+    """
+    cred = RefreshingCredentials(client_id, client_secret)
+    return cred.request_client_token()
+
+
+def prompt_for_user_token(
+    client_id: str, client_secret: str, redirect_uri: str, scope=None
+) -> RefreshingToken:
+    """
+    Prompt for manual authorisation.
+
+    Open a web browser for the user to log in with Spotify.
+    Prompt to paste the URL after logging in to complete authorisation.
+
+    Parameters
+    ----------
+    client_id
+        client ID
+    client_secret
+        client secret
+    redirect_uri
+        whitelisted redirect URI
+    scope
+        token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+        a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+        or a space-separated list of scopes as a string
+
+    Returns
+    -------
+    RefreshingToken
+        automatically refreshing user token
+
+    Raises
+    ------
+    AssertionError
+        if state is inconsistent
+    """
+    cred = RefreshingCredentials(client_id, client_secret, redirect_uri)
+    auth = UserAuth(cred, scope=scope)
+
+    print("Opening browser for Spotify login...")
+    webbrowser.open(auth.url)
+    redirected = input("Please paste redirect URL: ").strip()
+    return auth.request_token(url=redirected)
+
+
+def refresh_user_token(
+    client_id: str, client_secret: str, refresh_token: str
+) -> RefreshingToken:
+    """
+    Request a refreshed user token.
+
+    Parameters
+    ----------
+    client_id
+        client ID
+    client_secret
+        client secret
+    refresh_token
+        refresh token
+
+    Returns
+    -------
+    RefreshingToken
+        automatically refreshing user token
+    """
+    cred = RefreshingCredentials(client_id, client_secret)
+    return cred.refresh_user_token(refresh_token)
+
+
+def prompt_for_pkce_token(
+    client_id: str, redirect_uri: str, scope=None
+) -> RefreshingToken:
+    """
+    Prompt for manual authorisation with PKCE.
+
+    Open a web browser for the user to log in with Spotify.
+    Prompt to paste the URL after logging in to complete authorisation.
+
+    Parameters
+    ----------
+    client_id
+        client ID
+    redirect_uri
+        whitelisted redirect URI
+    scope
+        token privileges, accepts a :class:`Scope`, a single :class:`scope`,
+        a list of :class:`scopes <scope>` and strings for :class:`Scope`,
+        or a space-separated list of scopes as a string
+
+    Returns
+    -------
+    RefreshingToken
+        automatically refreshing PKCE user token
+
+    Raises
+    ------
+    AssertionError
+        if state is inconsistent
+    """
+    cred = RefreshingCredentials(client_id, redirect_uri=redirect_uri)
+    auth = UserAuth(cred, scope=scope, pkce=True)
+
+    print("Opening browser for Spotify login...")
+    webbrowser.open(auth.url)
+    redirected = input("Please paste redirect URL: ").strip()
+    return auth.request_token(url=redirected)
+
+
+def refresh_pkce_token(client_id: str, refresh_token: str) -> RefreshingToken:
+    """
+    Request a refreshed PKCE user token.
+
+    Parameters
+    ----------
+    client_id
+        client ID
+    refresh_token
+        refresh token
+
+    Returns
+    -------
+    RefreshingToken
+        automatically refreshing user token
+    """
+    cred = RefreshingCredentials(client_id)
+    return cred.refresh_pkce_token(refresh_token)
```

### Comparing `tekore-4.5.0/tekore/_client/api/album.py` & `tekore-4.6.0/src/tekore/_client/api/album.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore.model import FullAlbum, SimpleTrackPaging, ModelList
-
-
-class SpotifyAlbum(SpotifyBase):
-    """Album API endpoints."""
-
-    @scopes()
-    @send_and_process(single(FullAlbum))
-    def album(
-            self,
-            album_id: str,
-            market: str = None
-    ) -> FullAlbum:
-        """
-        Get an album.
-
-        Parameters
-        ----------
-        album_id
-            album ID
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        """
-        return self._get('albums/' + album_id, market=market)
-
-    @scopes()
-    @send_and_process(single(SimpleTrackPaging))
-    @maximise_limit(50)
-    def album_tracks(
-            self,
-            album_id: str,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SimpleTrackPaging:
-        """
-        Get tracks on album.
-
-        Parameters
-        ----------
-        album_id
-            album ID
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get(
-            f'albums/{album_id}/tracks',
-            market=market,
-            limit=limit,
-            offset=offset
-        )
-
-    @scopes()
-    @chunked('album_ids', 1, 20, join_lists)
-    @send_and_process(model_list(FullAlbum, 'albums'))
-    def albums(
-            self,
-            album_ids: list,
-            market: str = None
-    ) -> ModelList[FullAlbum]:
-        """
-        Get multiple albums.
-
-        Parameters
-        ----------
-        album_ids
-            list of album IDs, max 20 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        """
-        return self._get('albums/?ids=' + ','.join(album_ids), market=market)
+from tekore.model import FullAlbum, ModelList, SimpleTrackPaging
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyAlbum(SpotifyBase):
+    """Album API endpoints."""
+
+    @scopes()
+    @send_and_process(single(FullAlbum))
+    def album(self, album_id: str, market: str = None) -> FullAlbum:
+        """
+        Get an album.
+
+        Parameters
+        ----------
+        album_id
+            album ID
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        """
+        return self._get("albums/" + album_id, market=market)
+
+    @scopes()
+    @send_and_process(single(SimpleTrackPaging))
+    @maximise_limit(50)
+    def album_tracks(
+        self, album_id: str, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SimpleTrackPaging:
+        """
+        Get tracks on album.
+
+        Parameters
+        ----------
+        album_id
+            album ID
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get(
+            f"albums/{album_id}/tracks", market=market, limit=limit, offset=offset
+        )
+
+    @scopes()
+    @chunked("album_ids", 1, 20, join_lists)
+    @send_and_process(model_list(FullAlbum, "albums"))
+    def albums(self, album_ids: list, market: str = None) -> ModelList[FullAlbum]:
+        """
+        Get multiple albums.
+
+        Parameters
+        ----------
+        album_ids
+            list of album IDs, max 20 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        """
+        return self._get("albums/?ids=" + ",".join(album_ids), market=market)
```

### Comparing `tekore-4.5.0/tekore/_client/api/artist.py` & `tekore-4.6.0/src/tekore/_client/api/artist.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,107 @@
-from typing import List, Union
-
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore.model import (
-    FullArtist,
-    SimpleAlbumPaging,
-    FullTrack,
-    AlbumGroup,
-    ModelList,
-)
-
-
-class SpotifyArtist(SpotifyBase):
-    """Artist API endpoints."""
-
-    @scopes()
-    @send_and_process(single(FullArtist))
-    def artist(self, artist_id: str) -> FullArtist:
-        """
-        Get information for an artist.
-
-        Parameters
-        ----------
-        artist_id
-            artist ID
-        """
-        return self._get('artists/' + artist_id)
-
-    @scopes()
-    @chunked('artist_ids', 1, 50, join_lists)
-    @send_and_process(model_list(FullArtist, 'artists'))
-    def artists(self, artist_ids: list) -> ModelList[FullArtist]:
-        """
-        Get information for multiple artists.
-
-        Parameters
-        ----------
-        artist_ids
-            list of artist IDs, max 50 without chunking
-        """
-        return self._get('artists/?ids=' + ','.join(artist_ids))
-
-    @scopes()
-    @send_and_process(single(SimpleAlbumPaging))
-    @maximise_limit(50)
-    def artist_albums(
-            self,
-            artist_id: str,
-            include_groups: List[Union[str, AlbumGroup]] = None,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SimpleAlbumPaging:
-        """
-        Get an artist's albums.
-
-        Parameters
-        ----------
-        artist_id
-            the artist ID
-        include_groups
-            album groups to include in the response
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        if include_groups is not None:
-            include_groups = ','.join(str(g) for g in include_groups)
-        return self._get(
-            f'artists/{artist_id}/albums',
-            include_groups=include_groups,
-            market=market,
-            limit=limit,
-            offset=offset
-        )
-
-    @scopes()
-    @send_and_process(model_list(FullTrack, 'tracks'))
-    def artist_top_tracks(
-            self,
-            artist_id: str,
-            market: str
-    ) -> ModelList[FullTrack]:
-        """
-        Get an artist's top 10 tracks by country.
-
-        Parameters
-        ----------
-        artist_id
-            the artist ID
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        """
-        return self._get(f'artists/{artist_id}/top-tracks', country=market)
-
-    @scopes()
-    @send_and_process(model_list(FullArtist, 'artists'))
-    def artist_related_artists(self, artist_id: str) -> ModelList[FullArtist]:
-        """
-        Get artists similar to an identified artist.
-
-        Similarity is based on analysis of
-        the Spotify community's listening history.
-
-        Parameters
-        ----------
-        artist_id
-            artist ID
-        """
-        return self._get(f'artists/{artist_id}/related-artists')
+from typing import List, Union
+
+from tekore.model import AlbumGroup, FullArtist, FullTrack, ModelList, SimpleAlbumPaging
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyArtist(SpotifyBase):
+    """Artist API endpoints."""
+
+    @scopes()
+    @send_and_process(single(FullArtist))
+    def artist(self, artist_id: str) -> FullArtist:
+        """
+        Get information for an artist.
+
+        Parameters
+        ----------
+        artist_id
+            artist ID
+        """
+        return self._get("artists/" + artist_id)
+
+    @scopes()
+    @chunked("artist_ids", 1, 50, join_lists)
+    @send_and_process(model_list(FullArtist, "artists"))
+    def artists(self, artist_ids: list) -> ModelList[FullArtist]:
+        """
+        Get information for multiple artists.
+
+        Parameters
+        ----------
+        artist_ids
+            list of artist IDs, max 50 without chunking
+        """
+        return self._get("artists/?ids=" + ",".join(artist_ids))
+
+    @scopes()
+    @send_and_process(single(SimpleAlbumPaging))
+    @maximise_limit(50)
+    def artist_albums(
+        self,
+        artist_id: str,
+        include_groups: List[Union[str, AlbumGroup]] = None,
+        market: str = None,
+        limit: int = 20,
+        offset: int = 0,
+    ) -> SimpleAlbumPaging:
+        """
+        Get an artist's albums.
+
+        Parameters
+        ----------
+        artist_id
+            the artist ID
+        include_groups
+            album groups to include in the response
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        if include_groups is not None:
+            include_groups = ",".join(str(g) for g in include_groups)
+        return self._get(
+            f"artists/{artist_id}/albums",
+            include_groups=include_groups,
+            market=market,
+            limit=limit,
+            offset=offset,
+        )
+
+    @scopes()
+    @send_and_process(model_list(FullTrack, "tracks"))
+    def artist_top_tracks(self, artist_id: str, market: str) -> ModelList[FullTrack]:
+        """
+        Get an artist's top 10 tracks by country.
+
+        Parameters
+        ----------
+        artist_id
+            the artist ID
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        """
+        return self._get(f"artists/{artist_id}/top-tracks", country=market)
+
+    @scopes()
+    @send_and_process(model_list(FullArtist, "artists"))
+    def artist_related_artists(self, artist_id: str) -> ModelList[FullArtist]:
+        """
+        Get artists similar to an identified artist.
+
+        Similarity is based on analysis of
+        the Spotify community's listening history.
+
+        Parameters
+        ----------
+        artist_id
+            artist ID
+        """
+        return self._get(f"artists/{artist_id}/related-artists")
```

### Comparing `tekore-4.5.0/tekore/_client/api/audiobook.py` & `tekore-4.6.0/src/tekore/_client/api/audiobook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,91 +1,82 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore.model import FullAudiobook, SimpleChapterPaging, ModelList
-
-
-class SpotifyAudiobook(SpotifyBase):
-    """Audiobook API endpoints."""
-
-    @scopes()
-    @send_and_process(single(FullAudiobook))
-    def audiobook(
-            self,
-            audiobook_id: str,
-            market: str = None
-    ) -> FullAudiobook:
-        """
-        Get information for an audiobook.
-
-        Parameters
-        ----------
-        audiobook_id
-            audiobook ID
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the show is considered unavailable.
-        """
-        return self._get('audiobooks/' + audiobook_id, market=market)
-
-    @scopes()
-    @chunked('audiobook_ids', 1, 50, join_lists)
-    @send_and_process(model_list(FullAudiobook, 'audiobooks'))
-    def audiobooks(
-            self,
-            audiobook_ids: list,
-            market: str = None
-    ) -> ModelList[FullAudiobook]:
-        """
-        Get information for multiple audiobooks.
-
-        Parameters
-        ----------
-        audiobook_ids
-            the audiobook IDs, max 50 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the show is considered unavailable.
-        """
-        return self._get('audiobook/?ids=' + ','.join(audiobook_ids), market=market)
-
-    @scopes()
-    @send_and_process(single(SimpleChapterPaging))
-    @maximise_limit(50)
-    def audiobook_chapters(
-            self,
-            audiobook_id: str,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SimpleChapterPaging:
-        """
-        Get chapters of an audiobook.
-
-        Parameters
-        ----------
-        audiobook_id
-            audiobook ID
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the show is considered unavailable.
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get(
-            f'audiobooks/{audiobook_id}/chapters',
-            market=market,
-            limit=limit,
-            offset=offset
-        )
+from tekore.model import FullAudiobook, ModelList, SimpleChapterPaging
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyAudiobook(SpotifyBase):
+    """Audiobook API endpoints."""
+
+    @scopes()
+    @send_and_process(single(FullAudiobook))
+    def audiobook(self, audiobook_id: str, market: str = None) -> FullAudiobook:
+        """
+        Get information for an audiobook.
+
+        Parameters
+        ----------
+        audiobook_id
+            audiobook ID
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the show is considered unavailable.
+        """
+        return self._get("audiobooks/" + audiobook_id, market=market)
+
+    @scopes()
+    @chunked("audiobook_ids", 1, 50, join_lists)
+    @send_and_process(model_list(FullAudiobook, "audiobooks"))
+    def audiobooks(
+        self, audiobook_ids: list, market: str = None
+    ) -> ModelList[FullAudiobook]:
+        """
+        Get information for multiple audiobooks.
+
+        Parameters
+        ----------
+        audiobook_ids
+            the audiobook IDs, max 50 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the show is considered unavailable.
+        """
+        return self._get("audiobook/?ids=" + ",".join(audiobook_ids), market=market)
+
+    @scopes()
+    @send_and_process(single(SimpleChapterPaging))
+    @maximise_limit(50)
+    def audiobook_chapters(
+        self, audiobook_id: str, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SimpleChapterPaging:
+        """
+        Get chapters of an audiobook.
+
+        Parameters
+        ----------
+        audiobook_id
+            audiobook ID
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the show is considered unavailable.
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get(
+            f"audiobooks/{audiobook_id}/chapters",
+            market=market,
+            limit=limit,
+            offset=offset,
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/browse/validate.py` & `tekore-4.6.0/src/tekore/_client/api/browse/validate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from itertools import product
-from tekore.model import RecommendationAttribute
-
-prefixes = {'min', 'max', 'target'}
-attributes = set(str(a) for a in RecommendationAttribute)
-valid = set('_'.join(i) for i in product(prefixes, attributes))
-
-
-def validate_attributes(candidates: dict) -> None:
-    """
-    Validate recommendation attributes.
-
-    Parameters
-    ----------
-    candidates
-        recommendation attributes to validate
-
-    Raises
-    ------
-    ValueError
-        if any attribute is not allowed
-    """
-    for name in candidates:
-        if name not in valid:
-            raise ValueError(f'Invalid attribute `{name}`!')
+from itertools import product
+
+from tekore.model import RecommendationAttribute
+
+prefixes = {"min", "max", "target"}
+attributes = set(str(a) for a in RecommendationAttribute)
+valid = set("_".join(i) for i in product(prefixes, attributes))
+
+
+def validate_attributes(candidates: dict) -> None:
+    """
+    Validate recommendation attributes.
+
+    Parameters
+    ----------
+    candidates
+        recommendation attributes to validate
+
+    Raises
+    ------
+    ValueError
+        if any attribute is not allowed
+    """
+    for name in candidates:
+        if name not in valid:
+            raise ValueError(f"Invalid attribute `{name}`!")
```

### Comparing `tekore-4.5.0/tekore/_client/api/chapter.py` & `tekore-4.6.0/src/tekore/_client/api/chapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,49 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore.model import FullChapter, ModelList
-
-
-class SpotifyChapter(SpotifyBase):
-    """Chapter API endpoints."""
-
-    @scopes()
-    @send_and_process(single(FullChapter))
-    def chapter(
-            self,
-            chapter_id: str,
-            market: str = None
-    ) -> FullChapter:
-        """
-        Get information for a chapter.
-
-        Parameters
-        ----------
-        chapter_id
-            chapter ID
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the episode is considered unavailable.
-        """
-        return self._get('chapters/' + chapter_id, market=market)
-
-    @scopes()
-    @chunked('chapter_ids', 1, 50, join_lists)
-    @send_and_process(model_list(FullChapter, 'chapters'))
-    def chapters(
-            self,
-            chapter_ids: list,
-            market: str = None
-    ) -> ModelList[FullChapter]:
-        """
-        Get information for multiple chapters.
-
-        Parameters
-        ----------
-        chapter_ids
-            the chapter IDs, max 50 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the episode is considered unavailable.
-        """
-        return self._get('chapters/?ids=' + ','.join(chapter_ids), market=market)
+from tekore.model import FullChapter, ModelList
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyChapter(SpotifyBase):
+    """Chapter API endpoints."""
+
+    @scopes()
+    @send_and_process(single(FullChapter))
+    def chapter(self, chapter_id: str, market: str = None) -> FullChapter:
+        """
+        Get information for a chapter.
+
+        Parameters
+        ----------
+        chapter_id
+            chapter ID
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the episode is considered unavailable.
+        """
+        return self._get("chapters/" + chapter_id, market=market)
+
+    @scopes()
+    @chunked("chapter_ids", 1, 50, join_lists)
+    @send_and_process(model_list(FullChapter, "chapters"))
+    def chapters(self, chapter_ids: list, market: str = None) -> ModelList[FullChapter]:
+        """
+        Get information for multiple chapters.
+
+        Parameters
+        ----------
+        chapter_ids
+            the chapter IDs, max 50 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the episode is considered unavailable.
+        """
+        return self._get("chapters/?ids=" + ",".join(chapter_ids), market=market)
```

### Comparing `tekore-4.5.0/tekore/_client/api/episode.py` & `tekore-4.6.0/src/tekore/_client/api/episode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,49 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore.model import FullEpisode, ModelList
-
-
-class SpotifyEpisode(SpotifyBase):
-    """Episode API endpoints."""
-
-    @scopes()
-    @send_and_process(single(FullEpisode))
-    def episode(
-            self,
-            episode_id: str,
-            market: str = None
-    ) -> FullEpisode:
-        """
-        Get information for an episode.
-
-        Parameters
-        ----------
-        episode_id
-            episode ID
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the episode is considered unavailable.
-        """
-        return self._get('episodes/' + episode_id, market=market)
-
-    @scopes()
-    @chunked('episode_ids', 1, 50, join_lists)
-    @send_and_process(model_list(FullEpisode, 'episodes'))
-    def episodes(
-            self,
-            episode_ids: list,
-            market: str = None
-    ) -> ModelList[FullEpisode]:
-        """
-        Get information for multiple episodes.
-
-        Parameters
-        ----------
-        episode_ids
-            the episode IDs, max 50 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the episode is considered unavailable.
-        """
-        return self._get('episodes/?ids=' + ','.join(episode_ids), market=market)
+from tekore.model import FullEpisode, ModelList
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyEpisode(SpotifyBase):
+    """Episode API endpoints."""
+
+    @scopes()
+    @send_and_process(single(FullEpisode))
+    def episode(self, episode_id: str, market: str = None) -> FullEpisode:
+        """
+        Get information for an episode.
+
+        Parameters
+        ----------
+        episode_id
+            episode ID
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the episode is considered unavailable.
+        """
+        return self._get("episodes/" + episode_id, market=market)
+
+    @scopes()
+    @chunked("episode_ids", 1, 50, join_lists)
+    @send_and_process(model_list(FullEpisode, "episodes"))
+    def episodes(self, episode_ids: list, market: str = None) -> ModelList[FullEpisode]:
+        """
+        Get information for multiple episodes.
+
+        Parameters
+        ----------
+        episode_ids
+            the episode IDs, max 50 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the episode is considered unavailable.
+        """
+        return self._get("episodes/?ids=" + ",".join(episode_ids), market=market)
```

### Comparing `tekore-4.5.0/tekore/_client/api/follow.py` & `tekore-4.6.0/src/tekore/_client/api/follow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,179 @@
-from typing import List
-
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from ..process import single, nothing
-from ..chunked import chunked, join_lists, return_none
-from tekore._auth import scope
-from tekore.model import FullArtistCursorPaging
-
-
-class SpotifyFollow(SpotifyBase):
-    """Follow API endpoints."""
-
-    @scopes(optional=[scope.playlist_read_private])
-    @chunked('user_ids', 2, 5, join_lists)
-    @send_and_process(nothing)
-    def playlist_is_following(self, playlist_id: str, user_ids: list) -> List[bool]:
-        """
-        Check if users are following a playlist.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        user_ids
-            list of user IDs, max 5 without chunking
-
-        Returns
-        -------
-        List[bool]
-            follow statuses in the same order that the user IDs were given
-        """
-        return self._get(
-            f'playlists/{playlist_id}/followers/contains',
-            ids=','.join(user_ids)
-        )
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(nothing)
-    def playlist_follow(
-            self,
-            playlist_id: str,
-            public: bool = True
-    ) -> None:
-        """
-        Follow a playlist as current user.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        public
-            follow publicly
-        """
-        payload = {'public': public}
-        return self._put(f'playlists/{playlist_id}/followers', payload=payload)
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(nothing)
-    def playlist_unfollow(self, playlist_id: str) -> None:
-        """
-        Unfollow a playlist as current user.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        """
-        return self._delete(f'playlists/{playlist_id}/followers')
-
-    @scopes([scope.user_follow_read])
-    @send_and_process(single(FullArtistCursorPaging, from_item='artists'))
-    @maximise_limit(50)
-    def followed_artists(
-            self,
-            limit: int = 20,
-            after: str = None
-    ) -> FullArtistCursorPaging:
-        """
-        Get artists followed by the current user.
-
-        Parameters
-        ----------
-        limit
-            the number of items to return (1..50)
-        after
-            the last artist ID retrieved from the previous request
-        """
-        return self._get('me/following', type='artist', limit=limit, after=after)
-
-    @scopes([scope.user_follow_read])
-    @chunked('artist_ids', 1, 50, join_lists)
-    @send_and_process(nothing)
-    def artists_is_following(self, artist_ids: list) -> List[bool]:
-        """
-        Check if current user follows artists.
-
-        Parameters
-        ----------
-        artist_ids
-            list of artist IDs, max 50 without chunking
-
-        Returns
-        -------
-        List[bool]
-            follow statuses in the same order that the artist IDs were given
-        """
-        return self._get(
-            'me/following/contains',
-            type='artist',
-            ids=','.join(artist_ids)
-        )
-
-    @scopes([scope.user_follow_modify])
-    @chunked('artist_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def artists_follow(self, artist_ids: list) -> None:
-        """
-        Follow artists as current user.
-
-        Parameters
-        ----------
-        artist_ids
-            list of artist IDs, max 50 without chunking
-        """
-        return self._put('me/following', type='artist', ids=','.join(artist_ids))
-
-    @scopes([scope.user_follow_modify])
-    @chunked('artist_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def artists_unfollow(self, artist_ids: list) -> None:
-        """
-        Unfollow artists as current user.
-
-        Parameters
-        ----------
-        artist_ids
-            list of artist IDs, max 50 without chunking
-        """
-        return self._delete('me/following', type='artist', ids=','.join(artist_ids))
-
-    @scopes([scope.user_follow_read])
-    @chunked('user_ids', 1, 50, join_lists)
-    @send_and_process(nothing)
-    def users_is_following(self, user_ids: list) -> List[bool]:
-        """
-        Check if current user follows users.
-
-        Parameters
-        ----------
-        user_ids
-            list of user IDs, max 50 without chunking
-
-        Returns
-        -------
-        List[bool]
-            follow statuses in the same order that the user IDs were given
-        """
-        return self._get(
-            'me/following/contains', type='user', ids=','.join(user_ids)
-        )
-
-    @scopes([scope.user_follow_modify])
-    @chunked('user_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def users_follow(self, user_ids: list) -> None:
-        """
-        Follow users as current user.
-
-        Parameters
-        ----------
-        user_ids
-            list of user IDs, max 50 without chunking
-        """
-        return self._put('me/following', type='user', ids=','.join(user_ids))
-
-    @scopes([scope.user_follow_modify])
-    @chunked('user_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def users_unfollow(self, user_ids: list) -> None:
-        """
-        Unfollow users as current user.
-
-        Parameters
-        ----------
-        user_ids
-            list of user IDs, max 50 without chunking
-        """
-        return self._delete('me/following', type='user', ids=','.join(user_ids))
+from typing import List
+
+from tekore._auth import scope
+from tekore.model import FullArtistCursorPaging
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists, return_none
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import nothing, single
+
+
+class SpotifyFollow(SpotifyBase):
+    """Follow API endpoints."""
+
+    @scopes(optional=[scope.playlist_read_private])
+    @chunked("user_ids", 2, 5, join_lists)
+    @send_and_process(nothing)
+    def playlist_is_following(self, playlist_id: str, user_ids: list) -> List[bool]:
+        """
+        Check if users are following a playlist.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        user_ids
+            list of user IDs, max 5 without chunking
+
+        Returns
+        -------
+        List[bool]
+            follow statuses in the same order that the user IDs were given
+        """
+        return self._get(
+            f"playlists/{playlist_id}/followers/contains", ids=",".join(user_ids)
+        )
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(nothing)
+    def playlist_follow(self, playlist_id: str, public: bool = True) -> None:
+        """
+        Follow a playlist as current user.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        public
+            follow publicly
+        """
+        payload = {"public": public}
+        return self._put(f"playlists/{playlist_id}/followers", payload=payload)
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(nothing)
+    def playlist_unfollow(self, playlist_id: str) -> None:
+        """
+        Unfollow a playlist as current user.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        """
+        return self._delete(f"playlists/{playlist_id}/followers")
+
+    @scopes([scope.user_follow_read])
+    @send_and_process(single(FullArtistCursorPaging, from_item="artists"))
+    @maximise_limit(50)
+    def followed_artists(
+        self, limit: int = 20, after: str = None
+    ) -> FullArtistCursorPaging:
+        """
+        Get artists followed by the current user.
+
+        Parameters
+        ----------
+        limit
+            the number of items to return (1..50)
+        after
+            the last artist ID retrieved from the previous request
+        """
+        return self._get("me/following", type="artist", limit=limit, after=after)
+
+    @scopes([scope.user_follow_read])
+    @chunked("artist_ids", 1, 50, join_lists)
+    @send_and_process(nothing)
+    def artists_is_following(self, artist_ids: list) -> List[bool]:
+        """
+        Check if current user follows artists.
+
+        Parameters
+        ----------
+        artist_ids
+            list of artist IDs, max 50 without chunking
+
+        Returns
+        -------
+        List[bool]
+            follow statuses in the same order that the artist IDs were given
+        """
+        return self._get(
+            "me/following/contains", type="artist", ids=",".join(artist_ids)
+        )
+
+    @scopes([scope.user_follow_modify])
+    @chunked("artist_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def artists_follow(self, artist_ids: list) -> None:
+        """
+        Follow artists as current user.
+
+        Parameters
+        ----------
+        artist_ids
+            list of artist IDs, max 50 without chunking
+        """
+        return self._put("me/following", type="artist", ids=",".join(artist_ids))
+
+    @scopes([scope.user_follow_modify])
+    @chunked("artist_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def artists_unfollow(self, artist_ids: list) -> None:
+        """
+        Unfollow artists as current user.
+
+        Parameters
+        ----------
+        artist_ids
+            list of artist IDs, max 50 without chunking
+        """
+        return self._delete("me/following", type="artist", ids=",".join(artist_ids))
+
+    @scopes([scope.user_follow_read])
+    @chunked("user_ids", 1, 50, join_lists)
+    @send_and_process(nothing)
+    def users_is_following(self, user_ids: list) -> List[bool]:
+        """
+        Check if current user follows users.
+
+        Parameters
+        ----------
+        user_ids
+            list of user IDs, max 50 without chunking
+
+        Returns
+        -------
+        List[bool]
+            follow statuses in the same order that the user IDs were given
+        """
+        return self._get("me/following/contains", type="user", ids=",".join(user_ids))
+
+    @scopes([scope.user_follow_modify])
+    @chunked("user_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def users_follow(self, user_ids: list) -> None:
+        """
+        Follow users as current user.
+
+        Parameters
+        ----------
+        user_ids
+            list of user IDs, max 50 without chunking
+        """
+        return self._put("me/following", type="user", ids=",".join(user_ids))
+
+    @scopes([scope.user_follow_modify])
+    @chunked("user_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def users_unfollow(self, user_ids: list) -> None:
+        """
+        Unfollow users as current user.
+
+        Parameters
+        ----------
+        user_ids
+            list of user IDs, max 50 without chunking
+        """
+        return self._delete("me/following", type="user", ids=",".join(user_ids))
```

### Comparing `tekore-4.5.0/tekore/_client/api/library.py` & `tekore-4.6.0/src/tekore/_client/api/library.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,297 +1,289 @@
-from typing import List
-
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from ..process import single, nothing
-from ..chunked import chunked, join_lists, return_none
-from tekore._auth import scope
-from tekore.model import (
-    SavedAlbumPaging, SavedEpisodePaging, SavedTrackPaging, SavedShowPaging
-)
-
-
-class SpotifyLibrary(SpotifyBase):
-    """Library API endpoints."""
-
-    @scopes([scope.user_library_read])
-    @send_and_process(single(SavedAlbumPaging))
-    @maximise_limit(50)
-    def saved_albums(
-            self,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SavedAlbumPaging:
-        """
-        Get the albums saved in the current user's library.
-
-        Parameters
-        ----------
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get('me/albums', market=market, limit=limit, offset=offset)
-
-    @scopes([scope.user_library_read])
-    @chunked('album_ids', 1, 50, join_lists)
-    @send_and_process(nothing)
-    def saved_albums_contains(self, album_ids: list) -> List[bool]:
-        """
-        Check if user has saved albums.
-
-        Parameters
-        ----------
-        album_ids
-            list of album IDs, max 50 without chunking
-
-        Returns
-        -------
-        List[bool]
-            save statuses in the same order the album IDs were given
-        """
-        return self._get('me/albums/contains?ids=' + ','.join(album_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('album_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_albums_add(self, album_ids: list) -> None:
-        """
-        Save albums for current user.
-
-        Parameters
-        ----------
-        album_ids
-            list of album IDs, max 50 without chunking
-        """
-        return self._put('me/albums?ids=' + ','.join(album_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('album_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_albums_delete(self, album_ids: list) -> None:
-        """
-        Remove albums for current user.
-
-        Parameters
-        ----------
-        album_ids
-            list of album IDs, max 50 without chunking
-        """
-        return self._delete('me/albums?ids=' + ','.join(album_ids))
-
-    @scopes([scope.user_library_read])
-    @send_and_process(single(SavedEpisodePaging))
-    @maximise_limit(50)
-    def saved_episodes(
-            self,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SavedEpisodePaging:
-        """
-        Get the episodes saved in the current user's library.
-
-        Parameters
-        ----------
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get('me/episodes', market=market, limit=limit, offset=offset)
-
-    @scopes([scope.user_library_read])
-    @chunked('episode_ids', 1, 50, join_lists)
-    @send_and_process(nothing)
-    def saved_episodes_contains(self, episode_ids: list) -> List[bool]:
-        """
-        Check if user has saved episodes.
-
-        Parameters
-        ----------
-        episode_ids
-            list of episode IDs, max 50 without chunking
-
-        Returns
-        -------
-        List[bool]
-            save statuses in the same order the episode IDs were given
-        """
-        return self._get('me/episodes/contains?ids=' + ','.join(episode_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('episode_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_episodes_add(self, episode_ids: list) -> None:
-        """
-        Save episodes for current user.
-
-        Parameters
-        ----------
-        episode_ids
-            list of episode IDs, max 50 without chunking
-        """
-        return self._put('me/episodes?ids=' + ','.join(episode_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('episode_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_episodes_delete(self, episode_ids: list) -> None:
-        """
-        Remove episodes for current user.
-
-        Parameters
-        ----------
-        episode_ids
-            list of episode IDs, max 50 without chunking
-        """
-        return self._delete('me/episodes?ids=' + ','.join(episode_ids))
-
-    @scopes([scope.user_library_read])
-    @send_and_process(single(SavedTrackPaging))
-    @maximise_limit(50)
-    def saved_tracks(
-            self,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SavedTrackPaging:
-        """
-        Get the songs saved in the current user's library.
-
-        Parameters
-        ----------
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get('me/tracks', market=market, limit=limit, offset=offset)
-
-    @scopes([scope.user_library_read])
-    @chunked('track_ids', 1, 50, join_lists)
-    @send_and_process(nothing)
-    def saved_tracks_contains(self, track_ids: list) -> List[bool]:
-        """
-        Check if user has saved tracks.
-
-        Parameters
-        ----------
-        track_ids
-            list of track IDs, max 50 without chunking
-
-        Returns
-        -------
-        List[bool]
-            save statuses in the same order the track IDs were given
-        """
-        return self._get('me/tracks/contains?ids=' + ','.join(track_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('track_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_tracks_add(self, track_ids: list) -> None:
-        """
-        Save tracks for current user.
-
-        Parameters
-        ----------
-        track_ids
-            list of track IDs, max 50 without chunking
-        """
-        return self._put('me/tracks/?ids=' + ','.join(track_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('track_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_tracks_delete(self, track_ids: list) -> None:
-        """
-        Remove tracks for current user.
-
-        Parameters
-        ----------
-        track_ids
-            list of track IDs, max 50 without chunking
-        """
-        return self._delete('me/tracks/?ids=' + ','.join(track_ids))
-
-    @scopes([scope.user_library_read])
-    @send_and_process(single(SavedShowPaging))
-    @maximise_limit(50)
-    def saved_shows(
-            self,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SavedShowPaging:
-        """
-        Get the shows saved in the current user's library.
-
-        Parameters
-        ----------
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get('me/shows', market=market, limit=limit, offset=offset)
-
-    @scopes([scope.user_library_read])
-    @chunked('show_ids', 1, 50, join_lists)
-    @send_and_process(nothing)
-    def saved_shows_contains(self, show_ids: list) -> List[bool]:
-        """
-        Check if user has saved shows.
-
-        Parameters
-        ----------
-        show_ids
-            list of show IDs, max 50 without chunking
-
-        Returns
-        -------
-        List[bool]
-            save statuses in the same order the show IDs were given
-        """
-        return self._get('me/shows/contains?ids=' + ','.join(show_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('show_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_shows_add(self, show_ids: list) -> None:
-        """
-        Save shows for current user.
-
-        Parameters
-        ----------
-        show_ids
-            list of show IDs, max 50 without chunking
-        """
-        return self._put('me/shows/?ids=' + ','.join(show_ids))
-
-    @scopes([scope.user_library_modify])
-    @chunked('show_ids', 1, 50, return_none)
-    @send_and_process(nothing)
-    def saved_shows_delete(self, show_ids: list, market: str = None) -> None:
-        """
-        Remove shows for current user.
-
-        Parameters
-        ----------
-        show_ids
-            list of show IDs, max 50 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code, only remove shows that are
-            available in the specified market, overrided by token's country
-        """
-        return self._delete('me/shows/?ids=' + ','.join(show_ids), market=market)
+from typing import List
+
+from tekore._auth import scope
+from tekore.model import (
+    SavedAlbumPaging,
+    SavedEpisodePaging,
+    SavedShowPaging,
+    SavedTrackPaging,
+)
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists, return_none
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import nothing, single
+
+
+class SpotifyLibrary(SpotifyBase):
+    """Library API endpoints."""
+
+    @scopes([scope.user_library_read])
+    @send_and_process(single(SavedAlbumPaging))
+    @maximise_limit(50)
+    def saved_albums(
+        self, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SavedAlbumPaging:
+        """
+        Get the albums saved in the current user's library.
+
+        Parameters
+        ----------
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get("me/albums", market=market, limit=limit, offset=offset)
+
+    @scopes([scope.user_library_read])
+    @chunked("album_ids", 1, 50, join_lists)
+    @send_and_process(nothing)
+    def saved_albums_contains(self, album_ids: list) -> List[bool]:
+        """
+        Check if user has saved albums.
+
+        Parameters
+        ----------
+        album_ids
+            list of album IDs, max 50 without chunking
+
+        Returns
+        -------
+        List[bool]
+            save statuses in the same order the album IDs were given
+        """
+        return self._get("me/albums/contains?ids=" + ",".join(album_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("album_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_albums_add(self, album_ids: list) -> None:
+        """
+        Save albums for current user.
+
+        Parameters
+        ----------
+        album_ids
+            list of album IDs, max 50 without chunking
+        """
+        return self._put("me/albums?ids=" + ",".join(album_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("album_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_albums_delete(self, album_ids: list) -> None:
+        """
+        Remove albums for current user.
+
+        Parameters
+        ----------
+        album_ids
+            list of album IDs, max 50 without chunking
+        """
+        return self._delete("me/albums?ids=" + ",".join(album_ids))
+
+    @scopes([scope.user_library_read])
+    @send_and_process(single(SavedEpisodePaging))
+    @maximise_limit(50)
+    def saved_episodes(
+        self, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SavedEpisodePaging:
+        """
+        Get the episodes saved in the current user's library.
+
+        Parameters
+        ----------
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get("me/episodes", market=market, limit=limit, offset=offset)
+
+    @scopes([scope.user_library_read])
+    @chunked("episode_ids", 1, 50, join_lists)
+    @send_and_process(nothing)
+    def saved_episodes_contains(self, episode_ids: list) -> List[bool]:
+        """
+        Check if user has saved episodes.
+
+        Parameters
+        ----------
+        episode_ids
+            list of episode IDs, max 50 without chunking
+
+        Returns
+        -------
+        List[bool]
+            save statuses in the same order the episode IDs were given
+        """
+        return self._get("me/episodes/contains?ids=" + ",".join(episode_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("episode_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_episodes_add(self, episode_ids: list) -> None:
+        """
+        Save episodes for current user.
+
+        Parameters
+        ----------
+        episode_ids
+            list of episode IDs, max 50 without chunking
+        """
+        return self._put("me/episodes?ids=" + ",".join(episode_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("episode_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_episodes_delete(self, episode_ids: list) -> None:
+        """
+        Remove episodes for current user.
+
+        Parameters
+        ----------
+        episode_ids
+            list of episode IDs, max 50 without chunking
+        """
+        return self._delete("me/episodes?ids=" + ",".join(episode_ids))
+
+    @scopes([scope.user_library_read])
+    @send_and_process(single(SavedTrackPaging))
+    @maximise_limit(50)
+    def saved_tracks(
+        self, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SavedTrackPaging:
+        """
+        Get the songs saved in the current user's library.
+
+        Parameters
+        ----------
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get("me/tracks", market=market, limit=limit, offset=offset)
+
+    @scopes([scope.user_library_read])
+    @chunked("track_ids", 1, 50, join_lists)
+    @send_and_process(nothing)
+    def saved_tracks_contains(self, track_ids: list) -> List[bool]:
+        """
+        Check if user has saved tracks.
+
+        Parameters
+        ----------
+        track_ids
+            list of track IDs, max 50 without chunking
+
+        Returns
+        -------
+        List[bool]
+            save statuses in the same order the track IDs were given
+        """
+        return self._get("me/tracks/contains?ids=" + ",".join(track_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("track_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_tracks_add(self, track_ids: list) -> None:
+        """
+        Save tracks for current user.
+
+        Parameters
+        ----------
+        track_ids
+            list of track IDs, max 50 without chunking
+        """
+        return self._put("me/tracks/?ids=" + ",".join(track_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("track_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_tracks_delete(self, track_ids: list) -> None:
+        """
+        Remove tracks for current user.
+
+        Parameters
+        ----------
+        track_ids
+            list of track IDs, max 50 without chunking
+        """
+        return self._delete("me/tracks/?ids=" + ",".join(track_ids))
+
+    @scopes([scope.user_library_read])
+    @send_and_process(single(SavedShowPaging))
+    @maximise_limit(50)
+    def saved_shows(
+        self, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SavedShowPaging:
+        """
+        Get the shows saved in the current user's library.
+
+        Parameters
+        ----------
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get("me/shows", market=market, limit=limit, offset=offset)
+
+    @scopes([scope.user_library_read])
+    @chunked("show_ids", 1, 50, join_lists)
+    @send_and_process(nothing)
+    def saved_shows_contains(self, show_ids: list) -> List[bool]:
+        """
+        Check if user has saved shows.
+
+        Parameters
+        ----------
+        show_ids
+            list of show IDs, max 50 without chunking
+
+        Returns
+        -------
+        List[bool]
+            save statuses in the same order the show IDs were given
+        """
+        return self._get("me/shows/contains?ids=" + ",".join(show_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("show_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_shows_add(self, show_ids: list) -> None:
+        """
+        Save shows for current user.
+
+        Parameters
+        ----------
+        show_ids
+            list of show IDs, max 50 without chunking
+        """
+        return self._put("me/shows/?ids=" + ",".join(show_ids))
+
+    @scopes([scope.user_library_modify])
+    @chunked("show_ids", 1, 50, return_none)
+    @send_and_process(nothing)
+    def saved_shows_delete(self, show_ids: list, market: str = None) -> None:
+        """
+        Remove shows for current user.
+
+        Parameters
+        ----------
+        show_ids
+            list of show IDs, max 50 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code, only remove shows that are
+            available in the specified market, overrided by token's country
+        """
+        return self._delete("me/shows/?ids=" + ",".join(show_ids), market=market)
```

### Comparing `tekore-4.5.0/tekore/_client/api/personalisation.py` & `tekore-4.6.0/src/tekore/_client/api/personalisation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,56 @@
-from ..process import single
-from ..decor import send_and_process, maximise_limit, scopes
-from ..base import SpotifyBase
-from tekore._auth import scope
-from tekore.model import FullArtistOffsetPaging, FullTrackPaging
-
-
-class SpotifyPersonalisation(SpotifyBase):
-    """Personalisation API endpoints."""
-
-    @scopes([scope.user_top_read])
-    @send_and_process(single(FullArtistOffsetPaging))
-    @maximise_limit(50)
-    def current_user_top_artists(
-            self,
-            time_range: str = 'medium_term',
-            limit: int = 20,
-            offset: int = 0
-    ) -> FullArtistOffsetPaging:
-        """
-        Get the current user's top artists.
-
-        Parameters
-        ----------
-        time_range
-            Over what time frame are the affinities computed.
-            Valid-values: short_term, medium_term, long_term
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get(
-            'me/top/artists',
-            time_range=time_range,
-            limit=limit,
-            offset=offset
-        )
-
-    @scopes([scope.user_top_read])
-    @send_and_process(single(FullTrackPaging))
-    @maximise_limit(50)
-    def current_user_top_tracks(
-            self,
-            time_range: str = 'medium_term',
-            limit: int = 20,
-            offset: int = 0
-    ) -> FullTrackPaging:
-        """
-        Get the current user's top tracks.
-
-        Parameters
-        ----------
-        time_range
-            Over what time frame are the affinities computed.
-            Valid-values: short_term, medium_term, long_term
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get(
-            'me/top/tracks',
-            time_range=time_range,
-            limit=limit,
-            offset=offset
-        )
+from tekore._auth import scope
+from tekore.model import FullArtistOffsetPaging, FullTrackPaging
+
+from ..base import SpotifyBase
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import single
+
+
+class SpotifyPersonalisation(SpotifyBase):
+    """Personalisation API endpoints."""
+
+    @scopes([scope.user_top_read])
+    @send_and_process(single(FullArtistOffsetPaging))
+    @maximise_limit(50)
+    def current_user_top_artists(
+        self, time_range: str = "medium_term", limit: int = 20, offset: int = 0
+    ) -> FullArtistOffsetPaging:
+        """
+        Get the current user's top artists.
+
+        Parameters
+        ----------
+        time_range
+            Over what time frame are the affinities computed.
+            Valid-values: short_term, medium_term, long_term
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get(
+            "me/top/artists", time_range=time_range, limit=limit, offset=offset
+        )
+
+    @scopes([scope.user_top_read])
+    @send_and_process(single(FullTrackPaging))
+    @maximise_limit(50)
+    def current_user_top_tracks(
+        self, time_range: str = "medium_term", limit: int = 20, offset: int = 0
+    ) -> FullTrackPaging:
+        """
+        Get the current user's top tracks.
+
+        Parameters
+        ----------
+        time_range
+            Over what time frame are the affinities computed.
+            Valid-values: short_term, medium_term, long_term
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get(
+            "me/top/tracks", time_range=time_range, limit=limit, offset=offset
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/player/modify.py` & `tekore-4.6.0/src/tekore/_client/api/player/modify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,247 +1,237 @@
-from typing import Union
-
-from tekore._auth import scope
-from tekore.model import RepeatState
-from tekore._convert import to_uri
-from ...base import SpotifyBase
-from ...decor import send_and_process, scopes
-from ...process import nothing
-
-
-def offset_to_dict(offset: Union[int, str]):
-    """
-    Parse playback start offset to an appropriate payload member.
-
-    If offset is an integer, it is an index to a track position.
-    If it is a string, it is a URI of a specific track.
-    """
-    if isinstance(offset, int):
-        return {'position': offset}
-    elif isinstance(offset, str):
-        return {'uri': to_uri('track', offset)}
-
-
-class SpotifyPlayerModify(SpotifyBase):
-    """Player API endpoints that modify state."""
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_transfer(self, device_id: str, force_play: bool = False) -> None:
-        """
-        Transfer playback to another device.
-
-        Parameters
-        ----------
-        device_id
-            device to transfer playback to
-        force_play
-            true: play after transfer, false: keep current state
-        """
-        payload = {
-            'device_ids': [device_id],
-            'play': force_play
-        }
-        return self._put('me/player', payload=payload)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_resume(self, device_id: str = None) -> None:
-        """
-        Resume user's playback.
-
-        Parameters
-        ----------
-        device_id
-            device to start playback on
-        """
-        return self._put('me/player/play', device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_start_tracks(
-            self,
-            track_ids: list,
-            offset: Union[int, str] = None,
-            position_ms: int = None,
-            device_id: str = None
-    ) -> None:
-        """
-        Start playback of one or more tracks.
-
-        Parameters
-        ----------
-        track_ids
-            track IDs to start playing
-        offset
-            offset into tracks by index or track ID
-        position_ms
-            initial position of first played track
-        device_id
-            device to start playback on
-        """
-        payload = {
-            'uris': [to_uri('track', t) for t in track_ids],
-            'offset': offset_to_dict(offset),
-            'position_ms': position_ms,
-        }
-        payload = {k: v for k, v in payload.items() if v is not None}
-        return self._put('me/player/play', payload=payload, device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_start_context(
-            self,
-            context_uri: str,
-            offset: Union[int, str] = None,
-            position_ms: int = None,
-            device_id: str = None
-    ) -> None:
-        """
-        Start playback of a context: an album, artist or playlist.
-
-        Parameters
-        ----------
-        context_uri
-            context to start playing
-        offset
-            offset into context by index or track ID,
-            only available when context is an album or playlist
-        position_ms
-            initial position of first played track
-        device_id
-            device to start playback on
-        """
-        payload = {
-            'context_uri': context_uri,
-            'offset': offset_to_dict(offset),
-            'position_ms': position_ms,
-        }
-        payload = {k: v for k, v in payload.items() if v is not None}
-        return self._put('me/player/play', payload=payload, device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_queue_add(self, uri: str, device_id: str = None) -> None:
-        """
-        Add a track or an episode to a user's queue.
-
-        Parameters
-        ----------
-        uri
-            resource to add, track or episode
-        device_id
-            devide to extend the queue on
-        """
-        return self._post('me/player/queue', uri=uri, device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_pause(self, device_id: str = None) -> None:
-        """
-        Pause a user's playback.
-
-        Parameters
-        ----------
-        device_id
-            device to pause playback on
-        """
-        return self._put('me/player/pause', device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_next(self, device_id: str = None) -> None:
-        """
-        Skip user's playback to next track.
-
-        Parameters
-        ----------
-        device_id
-            device to skip track on
-        """
-        return self._post('me/player/next', device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_previous(self, device_id: str = None) -> None:
-        """
-        Skip user's playback to previous track.
-
-        Parameters
-        ----------
-        device_id
-            device to skip track on
-        """
-        return self._post('me/player/previous', device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_seek(self, position_ms: int, device_id: str = None) -> None:
-        """
-        Seek to position in current playing track.
-
-        Parameters
-        ----------
-        position_ms
-            position on track
-        device_id
-            device to seek on
-        """
-        return self._put(
-            'me/player/seek',
-            position_ms=position_ms,
-            device_id=device_id
-        )
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_repeat(
-            self,
-            state: Union[str, RepeatState],
-            device_id: str = None
-    ) -> None:
-        """
-        Set repeat mode for playback.
-
-        Parameters
-        ----------
-        state
-            `track`, `context`, or `off`
-        device_id
-            device to set repeat on
-        """
-        return self._put('me/player/repeat', state=str(state), device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_shuffle(self, state: bool, device_id: str = None) -> None:
-        """
-        Toggle shuffle for user's playback.
-
-        Parameters
-        ----------
-        state
-            shuffle state
-        device_id
-            device to toggle shuffle on
-        """
-        state = 'true' if state else 'false'
-        return self._put('me/player/shuffle', state=state, device_id=device_id)
-
-    @scopes([scope.user_modify_playback_state])
-    @send_and_process(nothing)
-    def playback_volume(self, volume_percent: int, device_id: str = None) -> None:
-        """
-        Set volume for user's playback.
-
-        Parameters
-        ----------
-        volume_percent
-            volume to set (0..100)
-        device_id
-            device to set volume on
-        """
-        return self._put(
-            'me/player/volume',
-            volume_percent=volume_percent,
-            device_id=device_id
-        )
+from typing import Union
+
+from tekore._auth import scope
+from tekore._convert import to_uri
+from tekore.model import RepeatState
+
+from ...base import SpotifyBase
+from ...decor import scopes, send_and_process
+from ...process import nothing
+
+
+def offset_to_dict(offset: Union[int, str]):
+    """
+    Parse playback start offset to an appropriate payload member.
+
+    If offset is an integer, it is an index to a track position.
+    If it is a string, it is a URI of a specific track.
+    """
+    if isinstance(offset, int):
+        return {"position": offset}
+    elif isinstance(offset, str):
+        return {"uri": to_uri("track", offset)}
+
+
+class SpotifyPlayerModify(SpotifyBase):
+    """Player API endpoints that modify state."""
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_transfer(self, device_id: str, force_play: bool = False) -> None:
+        """
+        Transfer playback to another device.
+
+        Parameters
+        ----------
+        device_id
+            device to transfer playback to
+        force_play
+            true: play after transfer, false: keep current state
+        """
+        payload = {"device_ids": [device_id], "play": force_play}
+        return self._put("me/player", payload=payload)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_resume(self, device_id: str = None) -> None:
+        """
+        Resume user's playback.
+
+        Parameters
+        ----------
+        device_id
+            device to start playback on
+        """
+        return self._put("me/player/play", device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_start_tracks(
+        self,
+        track_ids: list,
+        offset: Union[int, str] = None,
+        position_ms: int = None,
+        device_id: str = None,
+    ) -> None:
+        """
+        Start playback of one or more tracks.
+
+        Parameters
+        ----------
+        track_ids
+            track IDs to start playing
+        offset
+            offset into tracks by index or track ID
+        position_ms
+            initial position of first played track
+        device_id
+            device to start playback on
+        """
+        payload = {
+            "uris": [to_uri("track", t) for t in track_ids],
+            "offset": offset_to_dict(offset),
+            "position_ms": position_ms,
+        }
+        payload = {k: v for k, v in payload.items() if v is not None}
+        return self._put("me/player/play", payload=payload, device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_start_context(
+        self,
+        context_uri: str,
+        offset: Union[int, str] = None,
+        position_ms: int = None,
+        device_id: str = None,
+    ) -> None:
+        """
+        Start playback of a context: an album, artist or playlist.
+
+        Parameters
+        ----------
+        context_uri
+            context to start playing
+        offset
+            offset into context by index or track ID,
+            only available when context is an album or playlist
+        position_ms
+            initial position of first played track
+        device_id
+            device to start playback on
+        """
+        payload = {
+            "context_uri": context_uri,
+            "offset": offset_to_dict(offset),
+            "position_ms": position_ms,
+        }
+        payload = {k: v for k, v in payload.items() if v is not None}
+        return self._put("me/player/play", payload=payload, device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_queue_add(self, uri: str, device_id: str = None) -> None:
+        """
+        Add a track or an episode to a user's queue.
+
+        Parameters
+        ----------
+        uri
+            resource to add, track or episode
+        device_id
+            devide to extend the queue on
+        """
+        return self._post("me/player/queue", uri=uri, device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_pause(self, device_id: str = None) -> None:
+        """
+        Pause a user's playback.
+
+        Parameters
+        ----------
+        device_id
+            device to pause playback on
+        """
+        return self._put("me/player/pause", device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_next(self, device_id: str = None) -> None:
+        """
+        Skip user's playback to next track.
+
+        Parameters
+        ----------
+        device_id
+            device to skip track on
+        """
+        return self._post("me/player/next", device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_previous(self, device_id: str = None) -> None:
+        """
+        Skip user's playback to previous track.
+
+        Parameters
+        ----------
+        device_id
+            device to skip track on
+        """
+        return self._post("me/player/previous", device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_seek(self, position_ms: int, device_id: str = None) -> None:
+        """
+        Seek to position in current playing track.
+
+        Parameters
+        ----------
+        position_ms
+            position on track
+        device_id
+            device to seek on
+        """
+        return self._put("me/player/seek", position_ms=position_ms, device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_repeat(
+        self, state: Union[str, RepeatState], device_id: str = None
+    ) -> None:
+        """
+        Set repeat mode for playback.
+
+        Parameters
+        ----------
+        state
+            `track`, `context`, or `off`
+        device_id
+            device to set repeat on
+        """
+        return self._put("me/player/repeat", state=str(state), device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_shuffle(self, state: bool, device_id: str = None) -> None:
+        """
+        Toggle shuffle for user's playback.
+
+        Parameters
+        ----------
+        state
+            shuffle state
+        device_id
+            device to toggle shuffle on
+        """
+        state = "true" if state else "false"
+        return self._put("me/player/shuffle", state=state, device_id=device_id)
+
+    @scopes([scope.user_modify_playback_state])
+    @send_and_process(nothing)
+    def playback_volume(self, volume_percent: int, device_id: str = None) -> None:
+        """
+        Set volume for user's playback.
+
+        Parameters
+        ----------
+        volume_percent
+            volume to set (0..100)
+        device_id
+            device to set volume on
+        """
+        return self._put(
+            "me/player/volume", volume_percent=volume_percent, device_id=device_id
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/player/view.py` & `tekore-4.6.0/src/tekore/_client/api/player/view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,138 +1,125 @@
-from ...process import single, model_list
-from ...decor import send_and_process, maximise_limit, scopes
-from ...base import SpotifyBase
-from tekore._auth import scope
-from tekore.model import (
-    ModelList,
-    CurrentlyPlayingContext,
-    CurrentlyPlaying,
-    PlayHistoryPaging,
-    Device,
-    Queue,
-)
-
-
-class SpotifyPlayerView(SpotifyBase):
-    """Player API endpoints that view state."""
-
-    @scopes([scope.user_read_playback_state])
-    @send_and_process(single(CurrentlyPlayingContext))
-    def playback(
-            self,
-            market: str = None,
-            tracks_only: bool = False
-    ) -> CurrentlyPlayingContext:
-        """
-        Get information about user's current playback.
-
-        Parameters
-        ----------
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        tracks_only
-            return only tracks in the currently playing item,
-            if True, episodes have None as the currently playing item
-
-        Returns
-        -------
-        CurrentlyPlayingContext
-            information about current playback
-        """
-        if tracks_only is True:
-            additional_types = None
-        else:
-            additional_types = 'episode'
-
-        return self._get(
-            'me/player',
-            market=market,
-            additional_types=additional_types
-        )
-
-    @scopes(
-        [scope.user_read_playback_state, scope.user_read_currently_playing],
-        [scope.user_read_playback_state, scope.user_read_currently_playing]
-    )
-    @send_and_process(single(CurrentlyPlaying))
-    def playback_currently_playing(
-            self,
-            market: str = None,
-            tracks_only: bool = False
-    ) -> CurrentlyPlaying:
-        """
-        Get user's currently playing track.
-
-        Only one of the scopes above is required.
-
-        Parameters
-        ----------
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        tracks_only
-            return only tracks in the currently playing item,
-            if True, episodes have None as the currently playing item
-
-        Returns
-        -------
-        CurrentlyPlaying
-            information about the current track playing
-        """
-        if tracks_only is True:
-            additional_types = None
-        else:
-            additional_types = 'episode'
-
-        return self._get(
-            'me/player/currently-playing',
-            market=market,
-            additional_types=additional_types
-        )
-
-    @scopes([scope.user_read_recently_played])
-    @send_and_process(single(PlayHistoryPaging))
-    @maximise_limit(50)
-    def playback_recently_played(
-            self,
-            limit: int = 20,
-            after: int = None,
-            before: int = None
-    ) -> PlayHistoryPaging:
-        """
-        Get tracks from the current user's recently played tracks.
-
-        Only ``after`` or ``before`` should be specified at one time.
-
-        Parameters
-        ----------
-        limit
-            the number of items to return (1..50)
-        after
-            a unix timestamp in milliseconds, must not be specified with 'before'
-        before
-            a unix timestamp in milliseconds, must not be specified with 'after'
-        """
-        return self._get(
-            'me/player/recently-played',
-            limit=limit,
-            after=after,
-            before=before
-        )
-
-    @scopes([scope.user_read_playback_state])
-    @send_and_process(model_list(Device, 'devices'))
-    def playback_devices(self) -> ModelList[Device]:
-        """Get a user's available devices."""
-        return self._get('me/player/devices')
-
-    @scopes([scope.user_read_playback_state])
-    @send_and_process(single(Queue))
-    def playback_queue(self) -> Queue:
-        """
-        Get items in a user's queue.
-
-        The result also include items in the current playback context
-        even though they are not explicitly in the queue.
-        The number of items in the queue is inconsistent,
-        but from manual experimentation at least two items are returned.
-        """
-        return self._get('me/player/queue')
+from tekore._auth import scope
+from tekore.model import (
+    CurrentlyPlaying,
+    CurrentlyPlayingContext,
+    Device,
+    ModelList,
+    PlayHistoryPaging,
+    Queue,
+)
+
+from ...base import SpotifyBase
+from ...decor import maximise_limit, scopes, send_and_process
+from ...process import model_list, single
+
+
+class SpotifyPlayerView(SpotifyBase):
+    """Player API endpoints that view state."""
+
+    @scopes([scope.user_read_playback_state])
+    @send_and_process(single(CurrentlyPlayingContext))
+    def playback(
+        self, market: str = None, tracks_only: bool = False
+    ) -> CurrentlyPlayingContext:
+        """
+        Get information about user's current playback.
+
+        Parameters
+        ----------
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        tracks_only
+            return only tracks in the currently playing item,
+            if True, episodes have None as the currently playing item
+
+        Returns
+        -------
+        CurrentlyPlayingContext
+            information about current playback
+        """
+        if tracks_only is True:
+            additional_types = None
+        else:
+            additional_types = "episode"
+
+        return self._get("me/player", market=market, additional_types=additional_types)
+
+    @scopes(
+        [scope.user_read_playback_state, scope.user_read_currently_playing],
+        [scope.user_read_playback_state, scope.user_read_currently_playing],
+    )
+    @send_and_process(single(CurrentlyPlaying))
+    def playback_currently_playing(
+        self, market: str = None, tracks_only: bool = False
+    ) -> CurrentlyPlaying:
+        """
+        Get user's currently playing track.
+
+        Only one of the scopes above is required.
+
+        Parameters
+        ----------
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        tracks_only
+            return only tracks in the currently playing item,
+            if True, episodes have None as the currently playing item
+
+        Returns
+        -------
+        CurrentlyPlaying
+            information about the current track playing
+        """
+        if tracks_only is True:
+            additional_types = None
+        else:
+            additional_types = "episode"
+
+        return self._get(
+            "me/player/currently-playing",
+            market=market,
+            additional_types=additional_types,
+        )
+
+    @scopes([scope.user_read_recently_played])
+    @send_and_process(single(PlayHistoryPaging))
+    @maximise_limit(50)
+    def playback_recently_played(
+        self, limit: int = 20, after: int = None, before: int = None
+    ) -> PlayHistoryPaging:
+        """
+        Get tracks from the current user's recently played tracks.
+
+        Only ``after`` or ``before`` should be specified at one time.
+
+        Parameters
+        ----------
+        limit
+            the number of items to return (1..50)
+        after
+            a unix timestamp in milliseconds, must not be specified with 'before'
+        before
+            a unix timestamp in milliseconds, must not be specified with 'after'
+        """
+        return self._get(
+            "me/player/recently-played", limit=limit, after=after, before=before
+        )
+
+    @scopes([scope.user_read_playback_state])
+    @send_and_process(model_list(Device, "devices"))
+    def playback_devices(self) -> ModelList[Device]:
+        """Get a user's available devices."""
+        return self._get("me/player/devices")
+
+    @scopes([scope.user_read_playback_state])
+    @send_and_process(single(Queue))
+    def playback_queue(self) -> Queue:
+        """
+        Get items in a user's queue.
+
+        The result also include items in the current playback context
+        even though they are not explicitly in the queue.
+        The number of items in the queue is inconsistent,
+        but from manual experimentation at least two items are returned.
+        """
+        return self._get("me/player/queue")
```

### Comparing `tekore-4.5.0/tekore/_client/api/playlist/items.py` & `tekore-4.6.0/src/tekore/_client/api/playlist/items.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,233 +1,202 @@
-from typing import List, Tuple
-
-from tekore._auth import scope
-from ...base import SpotifyBase
-from ...decor import send_and_process, scopes
-from ...process import top_item, nothing
-from ...chunked import chunked, return_last
-
-
-class SpotifyPlaylistItems(SpotifyBase):
-    """Playlist API endpoints for manipulating playlist items."""
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @chunked('uris', 2, 100, return_last, reverse='position', reverse_pos=3)
-    @send_and_process(top_item('snapshot_id'))
-    def playlist_add(
-            self,
-            playlist_id: str,
-            uris: list,
-            position: int = None
-    ) -> str:
-        """
-        Add items.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        uris
-            list of URIs, max 100 without chunking
-        position
-            index to insert the items in
-
-        Returns
-        -------
-        str
-            snapshot ID for the playlist
-        """
-        return self._post(
-            f'playlists/{playlist_id}/tracks',
-            payload={'uris': uris},
-            position=position
-        )
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(nothing)
-    def playlist_clear(self, playlist_id: str) -> None:
-        """
-        Remove all items.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        """
-        return self._put(f'playlists/{playlist_id}/tracks', payload={'uris': []})
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(nothing)
-    def playlist_replace(self, playlist_id: str, uris: list) -> None:
-        """
-        Replace all items.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        uris
-            list of URIs, max 100
-        """
-        return self._put(
-            f'playlists/{playlist_id}/tracks',
-            payload={'uris': uris}
-        )
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(top_item('snapshot_id'))
-    def playlist_reorder(
-            self,
-            playlist_id: str,
-            range_start: int,
-            insert_before: int,
-            range_length: int = 1,
-            snapshot_id: str = None
-    ) -> str:
-        """
-        Reorder items.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        range_start
-            position of the first item to be reordered
-        range_length
-            number of items to be reordered
-        insert_before
-            position where the items should be inserted
-        snapshot_id
-            snapshot ID for the playlist
-
-        Returns
-        -------
-        str
-            snapshot ID for the playlist
-        """
-        payload = {
-            'range_start': range_start,
-            'range_length': range_length,
-            'insert_before': insert_before
-        }
-        if snapshot_id:
-            payload['snapshot_id'] = snapshot_id
-        return self._put(f'playlists/{playlist_id}/tracks', payload=payload)
-
-    def _generic_playlist_remove(
-            self,
-            playlist_id: str,
-            payload: dict,
-            snapshot_id: str = None
-    ) -> str:
-        if snapshot_id:
-            payload['snapshot_id'] = snapshot_id
-        return self._delete(f'playlists/{playlist_id}/tracks', payload=payload)
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @chunked('uris', 2, 100, return_last, chain='snapshot_id', chain_pos=3)
-    @send_and_process(top_item('snapshot_id'))
-    def playlist_remove(
-            self,
-            playlist_id: str,
-            uris: list,
-            snapshot_id: str = None
-    ) -> str:
-        """
-        Remove items by URI.
-
-        Removes all occurrences of the specified items.
-        Note that when chunked, ``snapshot_id`` is not updated between requests.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        uris
-            list of URIs, max 100 without chunking
-        snapshot_id
-            snapshot ID for the playlist
-
-        Returns
-        -------
-        str
-            snapshot ID for the playlist
-        """
-        items = [{'uri': uri} for uri in uris]
-        return self._generic_playlist_remove(
-            playlist_id,
-            {'tracks': items},
-            snapshot_id
-        )
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(top_item('snapshot_id'))
-    def playlist_remove_occurrences(
-            self,
-            playlist_id: str,
-            refs: List[Tuple[str, int]],
-            snapshot_id: str = None
-    ) -> str:
-        """
-        Remove items by URI and position.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        refs
-            a list of tuples containing the URI and index of items to remove
-        snapshot_id
-            snapshot ID for the playlist
-
-        Returns
-        -------
-        str
-            snapshot ID for the playlist
-        """
-        gathered = {}
-        for uri, ix in refs:
-            gathered.setdefault(uri, []).append(ix)
-
-        items = [
-            {
-                'uri': uri,
-                'positions': ix_list
-            }
-            for uri, ix_list in gathered.items()
-        ]
-        return self._generic_playlist_remove(
-            playlist_id,
-            {'tracks': items},
-            snapshot_id
-        )
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(top_item('snapshot_id'))
-    def playlist_remove_indices(
-            self,
-            playlist_id: str,
-            indices: list,
-            snapshot_id: str
-    ) -> str:
-        """
-        Remove items by position.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        indices
-            a list of indices of tracks to remove
-        snapshot_id
-            snapshot ID for the playlist
-
-        Returns
-        -------
-        str
-            snapshot ID for the playlist
-        """
-        return self._generic_playlist_remove(
-            playlist_id,
-            {'positions': indices},
-            snapshot_id
-        )
+from typing import List, Tuple
+
+from tekore._auth import scope
+
+from ...base import SpotifyBase
+from ...chunked import chunked, return_last
+from ...decor import scopes, send_and_process
+from ...process import nothing, top_item
+
+
+class SpotifyPlaylistItems(SpotifyBase):
+    """Playlist API endpoints for manipulating playlist items."""
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @chunked("uris", 2, 100, return_last, reverse="position", reverse_pos=3)
+    @send_and_process(top_item("snapshot_id"))
+    def playlist_add(self, playlist_id: str, uris: list, position: int = None) -> str:
+        """
+        Add items.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        uris
+            list of URIs, max 100 without chunking
+        position
+            index to insert the items in
+
+        Returns
+        -------
+        str
+            snapshot ID for the playlist
+        """
+        return self._post(
+            f"playlists/{playlist_id}/tracks", payload={"uris": uris}, position=position
+        )
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(nothing)
+    def playlist_clear(self, playlist_id: str) -> None:
+        """
+        Remove all items.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        """
+        return self._put(f"playlists/{playlist_id}/tracks", payload={"uris": []})
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(nothing)
+    def playlist_replace(self, playlist_id: str, uris: list) -> None:
+        """
+        Replace all items.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        uris
+            list of URIs, max 100
+        """
+        return self._put(f"playlists/{playlist_id}/tracks", payload={"uris": uris})
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(top_item("snapshot_id"))
+    def playlist_reorder(
+        self,
+        playlist_id: str,
+        range_start: int,
+        insert_before: int,
+        range_length: int = 1,
+        snapshot_id: str = None,
+    ) -> str:
+        """
+        Reorder items.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        range_start
+            position of the first item to be reordered
+        range_length
+            number of items to be reordered
+        insert_before
+            position where the items should be inserted
+        snapshot_id
+            snapshot ID for the playlist
+
+        Returns
+        -------
+        str
+            snapshot ID for the playlist
+        """
+        payload = {
+            "range_start": range_start,
+            "range_length": range_length,
+            "insert_before": insert_before,
+        }
+        if snapshot_id:
+            payload["snapshot_id"] = snapshot_id
+        return self._put(f"playlists/{playlist_id}/tracks", payload=payload)
+
+    def _generic_playlist_remove(
+        self, playlist_id: str, payload: dict, snapshot_id: str = None
+    ) -> str:
+        if snapshot_id:
+            payload["snapshot_id"] = snapshot_id
+        return self._delete(f"playlists/{playlist_id}/tracks", payload=payload)
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @chunked("uris", 2, 100, return_last, chain="snapshot_id", chain_pos=3)
+    @send_and_process(top_item("snapshot_id"))
+    def playlist_remove(
+        self, playlist_id: str, uris: list, snapshot_id: str = None
+    ) -> str:
+        """
+        Remove items by URI.
+
+        Removes all occurrences of the specified items.
+        Note that when chunked, ``snapshot_id`` is not updated between requests.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        uris
+            list of URIs, max 100 without chunking
+        snapshot_id
+            snapshot ID for the playlist
+
+        Returns
+        -------
+        str
+            snapshot ID for the playlist
+        """
+        items = [{"uri": uri} for uri in uris]
+        return self._generic_playlist_remove(
+            playlist_id, {"tracks": items}, snapshot_id
+        )
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(top_item("snapshot_id"))
+    def playlist_remove_occurrences(
+        self, playlist_id: str, refs: List[Tuple[str, int]], snapshot_id: str = None
+    ) -> str:
+        """
+        Remove items by URI and position.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        refs
+            a list of tuples containing the URI and index of items to remove
+        snapshot_id
+            snapshot ID for the playlist
+
+        Returns
+        -------
+        str
+            snapshot ID for the playlist
+        """
+        gathered = {}
+        for uri, ix in refs:
+            gathered.setdefault(uri, []).append(ix)
+
+        items = [
+            {"uri": uri, "positions": ix_list} for uri, ix_list in gathered.items()
+        ]
+        return self._generic_playlist_remove(
+            playlist_id, {"tracks": items}, snapshot_id
+        )
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(top_item("snapshot_id"))
+    def playlist_remove_indices(
+        self, playlist_id: str, indices: list, snapshot_id: str
+    ) -> str:
+        """
+        Remove items by position.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        indices
+            a list of indices of tracks to remove
+        snapshot_id
+            snapshot ID for the playlist
+
+        Returns
+        -------
+        str
+            snapshot ID for the playlist
+        """
+        return self._generic_playlist_remove(
+            playlist_id, {"positions": indices}, snapshot_id
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/playlist/modify.py` & `tekore-4.6.0/src/tekore/_client/api/playlist/modify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,91 @@
-from ...base import SpotifyBase
-from ...decor import send_and_process, scopes
-from ...process import single, nothing
-from tekore._auth import scope
-from tekore._sender import Request
-from tekore.model import FullPlaylist
-
-
-class SpotifyPlaylistModify(SpotifyBase):
-    """Playlist API endpoints for modifying playlists."""
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(nothing)
-    def playlist_cover_image_upload(self, playlist_id: str, image: str) -> None:
-        """
-        Upload a custom playlist cover image.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        image
-            image data as a base64-encoded string
-        """
-        return Request(
-            method='PUT',
-            url=f'playlists/{playlist_id}/images',
-            headers={'Content-Type': 'image/jpeg'},
-            content=image,
-        ), ()
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(single(FullPlaylist))
-    def playlist_create(
-            self,
-            user_id: str,
-            name: str,
-            public: bool = True,
-            description: str = ''
-    ) -> FullPlaylist:
-        """
-        Create a playlist.
-
-        Parameters
-        ----------
-        user_id
-            user ID
-        name
-            the name of the playlist
-        public
-            is the created playlist public
-        description
-            the description of the playlist
-        """
-        payload = {
-            'name': name,
-            'public': public,
-            'description': description
-        }
-        return self._post(f'users/{user_id}/playlists', payload=payload)
-
-    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
-    @send_and_process(nothing)
-    def playlist_change_details(
-            self,
-            playlist_id: str,
-            name: str = None,
-            public: bool = None,
-            collaborative: bool = None,
-            description: str = None
-    ) -> None:
-        """
-        Change a playlist's details.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        name
-            name of the playlist
-        public
-            is the playlist public
-        collaborative
-            is the playlist collaborative
-        description
-            description of the playlist
-        """
-        payload = {
-            'name': name,
-            'public': public,
-            'collaborative': collaborative,
-            'description': description,
-        }
-        payload = {k: v for k, v in payload.items() if v is not None}
-        return self._put('playlists/' + playlist_id, payload=payload)
+from tekore._auth import scope
+from tekore._sender import Request
+from tekore.model import FullPlaylist
+
+from ...base import SpotifyBase
+from ...decor import scopes, send_and_process
+from ...process import nothing, single
+
+
+class SpotifyPlaylistModify(SpotifyBase):
+    """Playlist API endpoints for modifying playlists."""
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(nothing)
+    def playlist_cover_image_upload(self, playlist_id: str, image: str) -> None:
+        """
+        Upload a custom playlist cover image.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        image
+            image data as a base64-encoded string
+        """
+        return (
+            Request(
+                method="PUT",
+                url=f"playlists/{playlist_id}/images",
+                headers={"Content-Type": "image/jpeg"},
+                content=image,
+            ),
+            (),
+        )
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(single(FullPlaylist))
+    def playlist_create(
+        self, user_id: str, name: str, public: bool = True, description: str = ""
+    ) -> FullPlaylist:
+        """
+        Create a playlist.
+
+        Parameters
+        ----------
+        user_id
+            user ID
+        name
+            the name of the playlist
+        public
+            is the created playlist public
+        description
+            the description of the playlist
+        """
+        payload = {"name": name, "public": public, "description": description}
+        return self._post(f"users/{user_id}/playlists", payload=payload)
+
+    @scopes([scope.playlist_modify_public], [scope.playlist_modify_private])
+    @send_and_process(nothing)
+    def playlist_change_details(
+        self,
+        playlist_id: str,
+        name: str = None,
+        public: bool = None,
+        collaborative: bool = None,
+        description: str = None,
+    ) -> None:
+        """
+        Change a playlist's details.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        name
+            name of the playlist
+        public
+            is the playlist public
+        collaborative
+            is the playlist collaborative
+        description
+            description of the playlist
+        """
+        payload = {
+            "name": name,
+            "public": public,
+            "collaborative": collaborative,
+            "description": description,
+        }
+        payload = {k: v for k, v in payload.items() if v is not None}
+        return self._put("playlists/" + playlist_id, payload=payload)
```

### Comparing `tekore-4.5.0/tekore/_client/api/playlist/view.py` & `tekore-4.6.0/src/tekore/_client/api/playlist/view.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,241 +1,230 @@
-from typing import Union, Callable, Iterable
-from functools import wraps
-
-from ...base import SpotifyBase
-from ...decor import send_and_process, maximise_limit, scopes
-from ...chunked import _get_arg
-from ...process import single, model_list, nothing
-from tekore._auth import scope
-from tekore.model import (
-    ModelList,
-    SimplePlaylistPaging,
-    FullPlaylist,
-    Image,
-    PlaylistTrackPaging
-)
-
-
-def process_if_not_specified(post_func: Callable, *arguments) -> Callable:
-    """
-    Decorate a function to process only if any of arguments is falsy.
-
-    Parameters
-    ----------
-    post_func
-        function to call with response JSON content
-    arguments
-        arguments to check, tuples of (name, position in argument list)
-    """
-    def decorator(function: Callable) -> Callable:
-        async def async_wrapper(self, *args, **kwargs):
-            json = await function(self, *args, **kwargs)
-            return post_func(json)
-
-        @wraps(function)
-        def wrapper(self, *args, **kwargs):
-            falsies = [
-                bool(_get_arg(arg_pos - 1, arg_name, args, kwargs))
-                for arg_name, arg_pos in arguments
-            ]
-            if any(falsies):
-                return function(self, *args, **kwargs)
-
-            if self.is_async:
-                return async_wrapper(self, *args, **kwargs)
-
-            json = function(self, *args, **kwargs)
-            return post_func(json)
-        return wrapper
-    return decorator
-
-
-def parse_additional_types(as_tracks):
-    """Determine `additional_types` argument content."""
-    types = {'track', 'episode'}
-    if as_tracks is True:
-        types = set()
-    elif as_tracks is False:
-        pass
-    else:
-        types = types.difference(as_tracks)
-
-    return ','.join(types) if types else None
-
-
-class SpotifyPlaylistView(SpotifyBase):
-    """Playlist API endpoints for viewing playlists."""
-
-    @scopes(optional=[scope.playlist_read_private, scope.playlist_read_collaborative])
-    @send_and_process(single(SimplePlaylistPaging))
-    @maximise_limit(50)
-    def followed_playlists(
-            self,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SimplePlaylistPaging:
-        """
-        Get a list of the playlists owned or followed by the current user.
-
-        Parameters
-        ----------
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get('me/playlists', limit=limit, offset=offset)
-
-    @scopes(optional=[scope.playlist_read_private, scope.playlist_read_collaborative])
-    @send_and_process(single(SimplePlaylistPaging))
-    @maximise_limit(50)
-    def playlists(
-            self,
-            user_id: str,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SimplePlaylistPaging:
-        """
-        Get a list of the playlists owned or followed by a user.
-
-        Collaborative playlists are only returned for the current user.
-
-        Parameters
-        ----------
-        user_id
-            user ID
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get(
-            f'users/{user_id}/playlists',
-            limit=limit,
-            offset=offset
-        )
-
-    @scopes()
-    @process_if_not_specified(
-        single(FullPlaylist),
-        ('fields', 2),
-        ('as_tracks', 4)
-    )
-    @send_and_process(nothing)
-    def playlist(
-            self,
-            playlist_id: str,
-            fields: str = None,
-            market: str = None,
-            as_tracks: Union[bool, Iterable[str]] = False,
-    ) -> Union[FullPlaylist, dict]:
-        """
-        Get playlist of a user.
-
-        .. note:: Returns a dictionary if ``fields`` or ``as_tracks`` is specified.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        fields
-            which fields to return, see the Web API documentation for details
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-            when using a user token to authenticate.
-            For episodes in the playlist, if a user token is used,
-            the country associated with it overrides this parameter.
-            If an application token is used and no market is specified,
-            episodes are considered unavailable and returned as None.
-        as_tracks
-            return types of items with track-like fields.
-            If :class:`True`, return all other types as tracks.
-            If an iterable is passed, types contained are returned as tracks.
-            Currently the only extra type is ``episode``.
-
-        Returns
-        -------
-        Union[FullPlaylist, dict]
-            playlist object, or raw dictionary if ``fields``
-            or ``as_tracks`` was specified
-        """
-        additional_types = parse_additional_types(as_tracks)
-        return self._get(
-            'playlists/' + playlist_id,
-            fields=fields,
-            market=market,
-            additional_types=additional_types,
-        )
-
-    @scopes()
-    @send_and_process(model_list(Image))
-    def playlist_cover_image(self, playlist_id: str) -> ModelList[Image]:
-        """
-        Get cover image of a playlist.
-
-        .. note:: Returns a list of images.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        """
-        return self._get(f'playlists/{playlist_id}/images')
-
-    @scopes()
-    @process_if_not_specified(
-        single(PlaylistTrackPaging),
-        ('fields', 2),
-        ('as_tracks', 4)
-    )
-    @send_and_process(nothing)
-    def playlist_items(
-            self,
-            playlist_id: str,
-            fields: str = None,
-            market: str = None,
-            as_tracks: Union[bool, Iterable[str]] = False,
-            limit: int = 100,
-            offset: int = 0
-    ) -> Union[PlaylistTrackPaging, dict]:
-        """
-        Full details of items on a playlist.
-
-        .. note:: Returns a dictionary if ``fields`` or ``as_tracks`` is specified.
-
-        Parameters
-        ----------
-        playlist_id
-            playlist ID
-        fields
-            which fields to return, see the Web API documentation for details
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-            when using a user token to authenticate.
-            For episodes in the playlist, if a user token is used,
-            the country associated with it overrides this parameter.
-            If an application token is used and no market is specified,
-            episodes are considered unavailable and returned as None.
-        as_tracks
-            return types of items with track-like fields.
-            If :class:`True`, return all other types as tracks.
-            If an iterable is passed, types contained are returned as tracks.
-            Currently the only extra type is ``episode``.
-        limit
-            the number of items to return (1..100)
-        offset
-            the index of the first item to return
-
-        Returns
-        -------
-        Union[PlaylistTrackPaging, dict]
-            paging object containing playlist items, or raw dictionary
-            if ``fields`` or ``as_tracks`` was specified
-        """
-        return self._get(
-            f'playlists/{playlist_id}/tracks',
-            limit=limit,
-            offset=offset,
-            fields=fields,
-            market=market,
-            additional_types=parse_additional_types(as_tracks),
-        )
+from functools import wraps
+from typing import Callable, Iterable, Union
+
+from tekore._auth import scope
+from tekore.model import (
+    FullPlaylist,
+    Image,
+    ModelList,
+    PlaylistTrackPaging,
+    SimplePlaylistPaging,
+)
+
+from ...base import SpotifyBase
+from ...chunked import _get_arg
+from ...decor import maximise_limit, scopes, send_and_process
+from ...process import model_list, nothing, single
+
+
+def process_if_not_specified(post_func: Callable, *arguments) -> Callable:
+    """
+    Decorate a function to process only if any of arguments is falsy.
+
+    Parameters
+    ----------
+    post_func
+        function to call with response JSON content
+    arguments
+        arguments to check, tuples of (name, position in argument list)
+    """
+
+    def decorator(function: Callable) -> Callable:
+        async def async_wrapper(self, *args, **kwargs):
+            json = await function(self, *args, **kwargs)
+            return post_func(json)
+
+        @wraps(function)
+        def wrapper(self, *args, **kwargs):
+            falsies = [
+                bool(_get_arg(arg_pos - 1, arg_name, args, kwargs))
+                for arg_name, arg_pos in arguments
+            ]
+            if any(falsies):
+                return function(self, *args, **kwargs)
+
+            if self.is_async:
+                return async_wrapper(self, *args, **kwargs)
+
+            json = function(self, *args, **kwargs)
+            return post_func(json)
+
+        return wrapper
+
+    return decorator
+
+
+def parse_additional_types(as_tracks):
+    """Determine `additional_types` argument content."""
+    types = {"track", "episode"}
+    if as_tracks is True:
+        types = set()
+    elif as_tracks is False:
+        pass
+    else:
+        types = types.difference(as_tracks)
+
+    return ",".join(types) if types else None
+
+
+class SpotifyPlaylistView(SpotifyBase):
+    """Playlist API endpoints for viewing playlists."""
+
+    @scopes(optional=[scope.playlist_read_private, scope.playlist_read_collaborative])
+    @send_and_process(single(SimplePlaylistPaging))
+    @maximise_limit(50)
+    def followed_playlists(
+        self, limit: int = 20, offset: int = 0
+    ) -> SimplePlaylistPaging:
+        """
+        Get a list of the playlists owned or followed by the current user.
+
+        Parameters
+        ----------
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get("me/playlists", limit=limit, offset=offset)
+
+    @scopes(optional=[scope.playlist_read_private, scope.playlist_read_collaborative])
+    @send_and_process(single(SimplePlaylistPaging))
+    @maximise_limit(50)
+    def playlists(
+        self, user_id: str, limit: int = 20, offset: int = 0
+    ) -> SimplePlaylistPaging:
+        """
+        Get a list of the playlists owned or followed by a user.
+
+        Collaborative playlists are only returned for the current user.
+
+        Parameters
+        ----------
+        user_id
+            user ID
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get(f"users/{user_id}/playlists", limit=limit, offset=offset)
+
+    @scopes()
+    @process_if_not_specified(single(FullPlaylist), ("fields", 2), ("as_tracks", 4))
+    @send_and_process(nothing)
+    def playlist(
+        self,
+        playlist_id: str,
+        fields: str = None,
+        market: str = None,
+        as_tracks: Union[bool, Iterable[str]] = False,
+    ) -> Union[FullPlaylist, dict]:
+        """
+        Get playlist of a user.
+
+        .. note:: Returns a dictionary if ``fields`` or ``as_tracks`` is specified.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        fields
+            which fields to return, see the Web API documentation for details
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+            when using a user token to authenticate.
+            For episodes in the playlist, if a user token is used,
+            the country associated with it overrides this parameter.
+            If an application token is used and no market is specified,
+            episodes are considered unavailable and returned as None.
+        as_tracks
+            return types of items with track-like fields.
+            If :class:`True`, return all other types as tracks.
+            If an iterable is passed, types contained are returned as tracks.
+            Currently the only extra type is ``episode``.
+
+        Returns
+        -------
+        Union[FullPlaylist, dict]
+            playlist object, or raw dictionary if ``fields``
+            or ``as_tracks`` was specified
+        """
+        additional_types = parse_additional_types(as_tracks)
+        return self._get(
+            "playlists/" + playlist_id,
+            fields=fields,
+            market=market,
+            additional_types=additional_types,
+        )
+
+    @scopes()
+    @send_and_process(model_list(Image))
+    def playlist_cover_image(self, playlist_id: str) -> ModelList[Image]:
+        """
+        Get cover image of a playlist.
+
+        .. note:: Returns a list of images.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        """
+        return self._get(f"playlists/{playlist_id}/images")
+
+    @scopes()
+    @process_if_not_specified(
+        single(PlaylistTrackPaging), ("fields", 2), ("as_tracks", 4)
+    )
+    @send_and_process(nothing)
+    def playlist_items(
+        self,
+        playlist_id: str,
+        fields: str = None,
+        market: str = None,
+        as_tracks: Union[bool, Iterable[str]] = False,
+        limit: int = 100,
+        offset: int = 0,
+    ) -> Union[PlaylistTrackPaging, dict]:
+        """
+        Full details of items on a playlist.
+
+        .. note:: Returns a dictionary if ``fields`` or ``as_tracks`` is specified.
+
+        Parameters
+        ----------
+        playlist_id
+            playlist ID
+        fields
+            which fields to return, see the Web API documentation for details
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+            when using a user token to authenticate.
+            For episodes in the playlist, if a user token is used,
+            the country associated with it overrides this parameter.
+            If an application token is used and no market is specified,
+            episodes are considered unavailable and returned as None.
+        as_tracks
+            return types of items with track-like fields.
+            If :class:`True`, return all other types as tracks.
+            If an iterable is passed, types contained are returned as tracks.
+            Currently the only extra type is ``episode``.
+        limit
+            the number of items to return (1..100)
+        offset
+            the index of the first item to return
+
+        Returns
+        -------
+        Union[PlaylistTrackPaging, dict]
+            paging object containing playlist items, or raw dictionary
+            if ``fields`` or ``as_tracks`` was specified
+        """
+        return self._get(
+            f"playlists/{playlist_id}/tracks",
+            limit=limit,
+            offset=offset,
+            fields=fields,
+            market=market,
+            additional_types=parse_additional_types(as_tracks),
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/search.py` & `tekore-4.6.0/src/tekore/_client/api/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,106 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from tekore.model import (
-    FullArtistOffsetPaging,
-    FullTrackPaging,
-    SimpleAlbumPaging,
-    SimpleAudiobookPaging,
-    SimplePlaylistPaging,
-    SimpleEpisodePaging,
-    SimpleShowPaging,
-)
-
-paging_type = {
-    'artists': FullArtistOffsetPaging,
-    'albums': SimpleAlbumPaging,
-    'audiobooks': SimpleAudiobookPaging,
-    'episodes': SimpleEpisodePaging,
-    'playlists': SimplePlaylistPaging,
-    'shows': SimpleShowPaging,
-    'tracks': FullTrackPaging,
-}
-
-
-def search_result(json: dict):
-    """Unpack search result dicts into respective paging type constructors."""
-    return tuple(paging_type[key].from_kwargs(json[key]) for key in json.keys())
-
-
-class SpotifySearch(SpotifyBase):
-    """Search API endpoints."""
-
-    @scopes()
-    @send_and_process(search_result)
-    @maximise_limit(50)
-    def search(
-            self,
-            query: str,
-            types: tuple = ('track',),
-            market: str = None,
-            include_external: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> tuple:
-        """
-        Search for an item.
-
-        Returns :class:`NotFound` if limit+offset would be above 1000.
-
-        Parameters
-        ----------
-        query
-            search query
-        types
-            resources to search for, tuple of strings containing
-            artist, album, audiobook, track, playlist, show and/or episode
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        include_external
-            if 'audio', response will include any externally hosted audio
-
-        Returns
-        -------
-        tuple
-            Paging objects containing the types of items searched for
-            in the order that they were specified in 'types'.
-
-            * artist: :class:`FullArtistOffsetPaging <model.FullArtistOffsetPaging>`
-            * album: :class:`SimpleAlbumPaging <model.SimpleAlbumPaging>`
-            * audiobook: :class:`SimpleAudiobookPaging <model.SimpleAudiobookPaging>`
-            * episode: :class:`SimpleEpisodePaging <model.SimpleEpisodePaging>`
-            * playlist: :class:`SimplePlaylistPaging <model.SimplePlaylistPaging>`
-            * show: :class:`SimpleShowPaging <model.SimpleShowPaging>`
-            * track: :class:`FullTrackPaging <model.FullTrackPaging>`
-
-        Examples
-        --------
-        .. code:: python
-
-            tracks, = spotify.search('monty python')
-            artists, = spotify.search('sheeran', types=('artist',))
-            albums, tracks = spotify.search('piano', types=('album', 'track'))
-            spotify.search('gold album:boba artist:abba', types=('track',))
-            spotify.search('bob year:1980-2020', types=('show',))
-
-        .. note::
-            You can narrow down search results by specifying field filters
-            (e.g. year range, genre).
-            See the `Search for an Item
-            <https://developer.spotify.com/documentation/web-api/reference/>`_
-            page of the official documentation for more information.
-
-        """
-        return self._get(
-            'search',
-            q=query,
-            type=','.join(types),
-            market=market,
-            include_external=include_external,
-            limit=limit,
-            offset=offset
-        )
+from tekore.model import (
+    FullArtistOffsetPaging,
+    FullTrackPaging,
+    SimpleAlbumPaging,
+    SimpleAudiobookPaging,
+    SimpleEpisodePaging,
+    SimplePlaylistPaging,
+    SimpleShowPaging,
+)
+
+from ..base import SpotifyBase
+from ..decor import maximise_limit, scopes, send_and_process
+
+paging_type = {
+    "artists": FullArtistOffsetPaging,
+    "albums": SimpleAlbumPaging,
+    "audiobooks": SimpleAudiobookPaging,
+    "episodes": SimpleEpisodePaging,
+    "playlists": SimplePlaylistPaging,
+    "shows": SimpleShowPaging,
+    "tracks": FullTrackPaging,
+}
+
+
+def search_result(json: dict):
+    """Unpack search result dicts into respective paging type constructors."""
+    return tuple(paging_type[key].from_kwargs(json[key]) for key in json.keys())
+
+
+class SpotifySearch(SpotifyBase):
+    """Search API endpoints."""
+
+    @scopes()
+    @send_and_process(search_result)
+    @maximise_limit(50)
+    def search(
+        self,
+        query: str,
+        types: tuple = ("track",),
+        market: str = None,
+        include_external: str = None,
+        limit: int = 20,
+        offset: int = 0,
+    ) -> tuple:
+        """
+        Search for an item.
+
+        Returns :class:`NotFound` if limit+offset would be above 1000.
+
+        Parameters
+        ----------
+        query
+            search query
+        types
+            resources to search for, tuple of strings containing
+            artist, album, audiobook, track, playlist, show and/or episode
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        include_external
+            if 'audio', response will include any externally hosted audio
+
+        Returns
+        -------
+        tuple
+            Paging objects containing the types of items searched for
+            in the order that they were specified in 'types'.
+
+            * artist: :class:`FullArtistOffsetPaging <model.FullArtistOffsetPaging>`
+            * album: :class:`SimpleAlbumPaging <model.SimpleAlbumPaging>`
+            * audiobook: :class:`SimpleAudiobookPaging <model.SimpleAudiobookPaging>`
+            * episode: :class:`SimpleEpisodePaging <model.SimpleEpisodePaging>`
+            * playlist: :class:`SimplePlaylistPaging <model.SimplePlaylistPaging>`
+            * show: :class:`SimpleShowPaging <model.SimpleShowPaging>`
+            * track: :class:`FullTrackPaging <model.FullTrackPaging>`
+
+        Examples
+        --------
+        .. code:: python
+
+            tracks, = spotify.search('monty python')
+            artists, = spotify.search('sheeran', types=('artist',))
+            albums, tracks = spotify.search('piano', types=('album', 'track'))
+            spotify.search('gold album:boba artist:abba', types=('track',))
+            spotify.search('bob year:1980-2020', types=('show',))
+
+        .. note::
+            You can narrow down search results by specifying field filters
+            (e.g. year range, genre).
+            See the `Search for an Item
+            <https://developer.spotify.com/documentation/web-api/reference/>`_
+            page of the official documentation for more information.
+
+        """
+        return self._get(
+            "search",
+            q=query,
+            type=",".join(types),
+            market=market,
+            include_external=include_external,
+            limit=limit,
+            offset=offset,
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/show.py` & `tekore-4.6.0/src/tekore/_client/api/show.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,84 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, maximise_limit, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore._auth import scope
-from tekore.model import FullShow, SimpleEpisodePaging, ModelList
-
-
-class SpotifyShow(SpotifyBase):
-    """Show API endpoints."""
-
-    @scopes(optional=[scope.user_read_playback_position])
-    @send_and_process(single(FullShow))
-    def show(
-            self,
-            show_id: str,
-            market: str = None
-    ) -> FullShow:
-        """
-        Get information for a show.
-
-        The user-read-playback-position scope allows
-        episode resume points to be returned.
-
-        Parameters
-        ----------
-        show_id
-            show ID
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the show is considered unavailable.
-        """
-        return self._get('shows/' + show_id, market=market)
-
-    @scopes(optional=[scope.user_read_playback_position])
-    @chunked('show_ids', 1, 50, join_lists)
-    @send_and_process(model_list(FullShow, 'shows'))
-    def shows(
-            self,
-            show_ids: list,
-            market: str = None
-    ) -> ModelList[FullShow]:
-        """
-        Get information for multiple shows.
-
-        The user-read-playback-position scope allows
-        episode resume points to be returned.
-
-        Parameters
-        ----------
-        show_ids
-            the show IDs, max 50 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the show is considered unavailable.
-        """
-        return self._get('shows/?ids=' + ','.join(show_ids), market=market)
-
-    @scopes()
-    @send_and_process(single(SimpleEpisodePaging))
-    @maximise_limit(50)
-    def show_episodes(
-            self,
-            show_id: str,
-            market: str = None,
-            limit: int = 20,
-            offset: int = 0
-    ) -> SimpleEpisodePaging:
-        """
-        Get episodes of a show.
-
-        Parameters
-        ----------
-        show_id
-            show ID
-        market
-            an ISO 3166-1 alpha-2 country code.
-            If a user token is used to authenticate, the country associated
-            with it overrides this parameter.
-            If an application token is used and no market is specified,
-            the show is considered unavailable.
-        limit
-            the number of items to return (1..50)
-        offset
-            the index of the first item to return
-        """
-        return self._get(
-            f'shows/{show_id}/episodes',
-            market=market,
-            limit=limit,
-            offset=offset
-        )
+from tekore._auth import scope
+from tekore.model import FullShow, ModelList, SimpleEpisodePaging
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import maximise_limit, scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyShow(SpotifyBase):
+    """Show API endpoints."""
+
+    @scopes(optional=[scope.user_read_playback_position])
+    @send_and_process(single(FullShow))
+    def show(self, show_id: str, market: str = None) -> FullShow:
+        """
+        Get information for a show.
+
+        The user-read-playback-position scope allows
+        episode resume points to be returned.
+
+        Parameters
+        ----------
+        show_id
+            show ID
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the show is considered unavailable.
+        """
+        return self._get("shows/" + show_id, market=market)
+
+    @scopes(optional=[scope.user_read_playback_position])
+    @chunked("show_ids", 1, 50, join_lists)
+    @send_and_process(model_list(FullShow, "shows"))
+    def shows(self, show_ids: list, market: str = None) -> ModelList[FullShow]:
+        """
+        Get information for multiple shows.
+
+        The user-read-playback-position scope allows
+        episode resume points to be returned.
+
+        Parameters
+        ----------
+        show_ids
+            the show IDs, max 50 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the show is considered unavailable.
+        """
+        return self._get("shows/?ids=" + ",".join(show_ids), market=market)
+
+    @scopes()
+    @send_and_process(single(SimpleEpisodePaging))
+    @maximise_limit(50)
+    def show_episodes(
+        self, show_id: str, market: str = None, limit: int = 20, offset: int = 0
+    ) -> SimpleEpisodePaging:
+        """
+        Get episodes of a show.
+
+        Parameters
+        ----------
+        show_id
+            show ID
+        market
+            an ISO 3166-1 alpha-2 country code.
+            If a user token is used to authenticate, the country associated
+            with it overrides this parameter.
+            If an application token is used and no market is specified,
+            the show is considered unavailable.
+        limit
+            the number of items to return (1..50)
+        offset
+            the index of the first item to return
+        """
+        return self._get(
+            f"shows/{show_id}/episodes", market=market, limit=limit, offset=offset
+        )
```

### Comparing `tekore-4.5.0/tekore/_client/api/track.py` & `tekore-4.6.0/src/tekore/_client/api/track.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,74 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, scopes
-from ..process import single, model_list
-from ..chunked import chunked, join_lists
-from tekore.model import FullTrack, AudioFeatures, AudioAnalysis, ModelList
-
-
-class SpotifyTrack(SpotifyBase):
-    """Track API endpoints."""
-
-    @scopes()
-    @send_and_process(single(FullTrack))
-    def track(
-            self,
-            track_id: str,
-            market: str = None
-    ) -> FullTrack:
-        """
-        Get information for a track.
-
-        Parameters
-        ----------
-        track_id
-            track ID
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        """
-        return self._get('tracks/' + track_id, market=market)
-
-    @scopes()
-    @chunked('track_ids', 1, 50, join_lists)
-    @send_and_process(model_list(FullTrack, 'tracks'))
-    def tracks(
-            self,
-            track_ids: list,
-            market: str = None
-    ) -> ModelList[FullTrack]:
-        """
-        Get information for multiple tracks.
-
-        Parameters
-        ----------
-        track_ids
-            the track IDs, max 50 without chunking
-        market
-            an ISO 3166-1 alpha-2 country code or 'from_token'
-        """
-        return self._get('tracks/?ids=' + ','.join(track_ids), market=market)
-
-    @scopes()
-    @send_and_process(single(AudioAnalysis))
-    def track_audio_analysis(self, track_id: str) -> AudioAnalysis:
-        """
-        Get a detailed audio analysis for a track.
-
-        The analysis describes the track's structure and musical content,
-        including rythm, pitch and timbre.
-        """
-        return self._get('audio-analysis/' + track_id)
-
-    @scopes()
-    @send_and_process(single(AudioFeatures))
-    def track_audio_features(self, track_id: str) -> AudioFeatures:
-        """Get audio feature information for a track."""
-        return self._get('audio-features/' + track_id)
-
-    @scopes()
-    @chunked('track_ids', 1, 100, join_lists)
-    @send_and_process(model_list(AudioFeatures, 'audio_features'))
-    def tracks_audio_features(self, track_ids: list) -> ModelList[AudioFeatures]:
-        """
-        Get audio feature information for multiple tracks.
-
-        Feature information for a track may be ``None`` if not available.
-
-        Parameters
-        ----------
-        track_ids
-            track IDs, max 100 without chunking
-        """
-        return self._get('audio-features?ids=' + ','.join(track_ids))
+from tekore.model import AudioAnalysis, AudioFeatures, FullTrack, ModelList
+
+from ..base import SpotifyBase
+from ..chunked import chunked, join_lists
+from ..decor import scopes, send_and_process
+from ..process import model_list, single
+
+
+class SpotifyTrack(SpotifyBase):
+    """Track API endpoints."""
+
+    @scopes()
+    @send_and_process(single(FullTrack))
+    def track(self, track_id: str, market: str = None) -> FullTrack:
+        """
+        Get information for a track.
+
+        Parameters
+        ----------
+        track_id
+            track ID
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        """
+        return self._get("tracks/" + track_id, market=market)
+
+    @scopes()
+    @chunked("track_ids", 1, 50, join_lists)
+    @send_and_process(model_list(FullTrack, "tracks"))
+    def tracks(self, track_ids: list, market: str = None) -> ModelList[FullTrack]:
+        """
+        Get information for multiple tracks.
+
+        Parameters
+        ----------
+        track_ids
+            the track IDs, max 50 without chunking
+        market
+            an ISO 3166-1 alpha-2 country code or 'from_token'
+        """
+        return self._get("tracks/?ids=" + ",".join(track_ids), market=market)
+
+    @scopes()
+    @send_and_process(single(AudioAnalysis))
+    def track_audio_analysis(self, track_id: str) -> AudioAnalysis:
+        """
+        Get a detailed audio analysis for a track.
+
+        The analysis describes the track's structure and musical content,
+        including rythm, pitch and timbre.
+        """
+        return self._get("audio-analysis/" + track_id)
+
+    @scopes()
+    @send_and_process(single(AudioFeatures))
+    def track_audio_features(self, track_id: str) -> AudioFeatures:
+        """Get audio feature information for a track."""
+        return self._get("audio-features/" + track_id)
+
+    @scopes()
+    @chunked("track_ids", 1, 100, join_lists)
+    @send_and_process(model_list(AudioFeatures, "audio_features"))
+    def tracks_audio_features(self, track_ids: list) -> ModelList[AudioFeatures]:
+        """
+        Get audio feature information for multiple tracks.
+
+        Feature information for a track may be ``None`` if not available.
+
+        Parameters
+        ----------
+        track_ids
+            track IDs, max 100 without chunking
+        """
+        return self._get("audio-features?ids=" + ",".join(track_ids))
```

### Comparing `tekore-4.5.0/tekore/_client/api/user.py` & `tekore-4.6.0/src/tekore/_client/api/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from ..base import SpotifyBase
-from ..decor import send_and_process, scopes
-from ..process import single
-from tekore._auth import scope
-from tekore.model import PublicUser, PrivateUser
-
-
-class SpotifyUser(SpotifyBase):
-    """User API endpoints."""
-
-    @scopes()
-    @send_and_process(single(PublicUser))
-    def user(self, user_id: str) -> PublicUser:
-        """
-        Get a user's profile.
-
-        Parameters
-        ----------
-        user_id
-            user ID
-        """
-        return self._get('users/' + user_id.replace('#', '%23'))
-
-    @scopes(optional=[scope.user_read_private, scope.user_read_email])
-    @send_and_process(single(PrivateUser))
-    def current_user(self) -> PrivateUser:
-        """
-        Get current user's profile.
-
-        The user-read-private scope allows the user's country and
-        product subscription level to be returned.
-        """
-        return self._get('me/')
+from tekore._auth import scope
+from tekore.model import PrivateUser, PublicUser
+
+from ..base import SpotifyBase
+from ..decor import scopes, send_and_process
+from ..process import single
+
+
+class SpotifyUser(SpotifyBase):
+    """User API endpoints."""
+
+    @scopes()
+    @send_and_process(single(PublicUser))
+    def user(self, user_id: str) -> PublicUser:
+        """
+        Get a user's profile.
+
+        Parameters
+        ----------
+        user_id
+            user ID
+        """
+        return self._get("users/" + user_id.replace("#", "%23"))
+
+    @scopes(optional=[scope.user_read_private, scope.user_read_email])
+    @send_and_process(single(PrivateUser))
+    def current_user(self) -> PrivateUser:
+        """
+        Get current user's profile.
+
+        The user-read-private scope allows the user's country and
+        product subscription level to be returned.
+        """
+        return self._get("me/")
```

### Comparing `tekore-4.5.0/tekore/_client/base.py` & `tekore-4.6.0/src/tekore/_client/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,141 +1,137 @@
-from typing import Optional, Union, Coroutine
-from contextvars import ContextVar
-from tekore._sender import Sender, Client, Request, Response
-
-prefix = 'https://api.spotify.com/v1/'
-
-
-def build_url(url: str) -> str:
-    """Attach API address to endpoint."""
-    if not url.startswith('http'):
-        url = prefix + url
-    return url
-
-
-def parse_url_params(params: Optional[dict]) -> Optional[dict]:
-    """Generate parameter dict and filter Nones."""
-    params = params or {}
-    return {k: v for k, v in params.items() if v is not None} or None
-
-
-class SpotifyBase(Client):
-    """Base client with options and utility functions."""
-
-    _token_cv = ContextVar('_token_cv')
-    _max_limits_on_cv = ContextVar('_max_limits_on_cv')
-    _chunked_on_cv = ContextVar('_chunked_on_cv')
-
-    def __init__(
-            self,
-            token=None,
-            sender: Sender = None,
-            asynchronous: bool = None,
-            max_limits_on: bool = False,
-            chunked_on: bool = False,
-    ):
-        # Docstring in the main client
-        super().__init__(sender, asynchronous)
-        self._token = token
-        self._max_limits_on = max_limits_on
-        self._chunked_on = chunked_on
-
-    @property
-    def token(self):
-        """Token getter."""
-        return self._token_cv.get(self._token)
-
-    @token.setter
-    def token(self, value):
-        try:
-            self._token_cv.get()
-        except LookupError:
-            self._token = value
-        else:
-            self._token_cv.set(value)
-
-    @property
-    def max_limits_on(self):
-        """Max limits getter."""
-        return self._max_limits_on_cv.get(self._max_limits_on)
-
-    @max_limits_on.setter
-    def max_limits_on(self, value):
-        try:
-            self._max_limits_on_cv.get()
-        except LookupError:
-            self._max_limits_on = value
-        else:
-            self._max_limits_on_cv.set(value)
-
-    @property
-    def chunked_on(self):
-        """Chunked getter."""
-        return self._chunked_on_cv.get(self._chunked_on)
-
-    @chunked_on.setter
-    def chunked_on(self, value):
-        try:
-            self._chunked_on_cv.get()
-        except LookupError:
-            self._chunked_on = value
-        else:
-            self._chunked_on_cv.set(value)
-
-    def __repr__(self):
-        options = [
-            f'token={self.token!r}',
-            f'max_limits_on={self.max_limits_on}',
-            f'chunked_on={self.chunked_on}',
-            f'sender={self.sender!r}',
-        ]
-        return type(self).__name__ + '(' + ', '.join(options) + ')'
-
-    def _create_headers(self, content_type: str = 'application/json'):
-        return {
-            'Authorization': f'Bearer {str(self.token)}',
-            'Content-Type': content_type
-        }
-
-    def send(
-        self, request: Request
-    ) -> Union[Response, Coroutine[None, None, Response]]:
-        """
-        Build request url and headers, and send with underlying sender.
-
-        Exposed to easily send arbitrary requests,
-        for custom behavior in some endpoint e.g. for a subclass.
-        It may also come in handy if a bugfix or a feature is not implemented
-        in a timely manner, or in debugging related to the client or Web API.
-        """
-        request.url = build_url(request.url)
-        headers = self._create_headers()
-        if request.headers is not None:
-            headers.update(request.headers)
-        request.headers = headers
-        return self.sender.send(request)
-
-    @staticmethod
-    def _request(
-            method: str,
-            url: str,
-            payload: dict = None,
-            params: dict = None
-    ):
-        return Request(
-            method=method,
-            url=url,
-            params=parse_url_params(params),
-            json=payload,
-        ), ()
-
-    def _get(self, url: str, payload: dict = None, **params):
-        return self._request('GET', url, payload=payload, params=params)
-
-    def _post(self, url: str, payload: dict = None, **params):
-        return self._request('POST', url, payload=payload, params=params)
-
-    def _delete(self, url: str, payload: dict = None, **params):
-        return self._request('DELETE', url, payload=payload, params=params)
-
-    def _put(self, url: str, payload: dict = None, **params):
-        return self._request('PUT', url, payload=payload, params=params)
+from contextvars import ContextVar
+from typing import Coroutine, Optional, Union
+
+from tekore._sender import Client, Request, Response, Sender
+
+prefix = "https://api.spotify.com/v1/"
+
+
+def build_url(url: str) -> str:
+    """Attach API address to endpoint."""
+    if not url.startswith("http"):
+        url = prefix + url
+    return url
+
+
+def parse_url_params(params: Optional[dict]) -> Optional[dict]:
+    """Generate parameter dict and filter Nones."""
+    params = params or {}
+    return {k: v for k, v in params.items() if v is not None} or None
+
+
+class SpotifyBase(Client):
+    """Base client with options and utility functions."""
+
+    _token_cv = ContextVar("_token_cv")
+    _max_limits_on_cv = ContextVar("_max_limits_on_cv")
+    _chunked_on_cv = ContextVar("_chunked_on_cv")
+
+    def __init__(
+        self,
+        token=None,
+        sender: Sender = None,
+        asynchronous: bool = None,
+        max_limits_on: bool = False,
+        chunked_on: bool = False,
+    ):
+        # Docstring in the main client
+        super().__init__(sender, asynchronous)
+        self._token = token
+        self._max_limits_on = max_limits_on
+        self._chunked_on = chunked_on
+
+    @property
+    def token(self):
+        """Token getter."""
+        return self._token_cv.get(self._token)
+
+    @token.setter
+    def token(self, value):
+        try:
+            self._token_cv.get()
+        except LookupError:
+            self._token = value
+        else:
+            self._token_cv.set(value)
+
+    @property
+    def max_limits_on(self):
+        """Max limits getter."""
+        return self._max_limits_on_cv.get(self._max_limits_on)
+
+    @max_limits_on.setter
+    def max_limits_on(self, value):
+        try:
+            self._max_limits_on_cv.get()
+        except LookupError:
+            self._max_limits_on = value
+        else:
+            self._max_limits_on_cv.set(value)
+
+    @property
+    def chunked_on(self):
+        """Chunked getter."""
+        return self._chunked_on_cv.get(self._chunked_on)
+
+    @chunked_on.setter
+    def chunked_on(self, value):
+        try:
+            self._chunked_on_cv.get()
+        except LookupError:
+            self._chunked_on = value
+        else:
+            self._chunked_on_cv.set(value)
+
+    def __repr__(self):
+        options = [
+            f"token={self.token!r}",
+            f"max_limits_on={self.max_limits_on}",
+            f"chunked_on={self.chunked_on}",
+            f"sender={self.sender!r}",
+        ]
+        return type(self).__name__ + "(" + ", ".join(options) + ")"
+
+    def _create_headers(self, content_type: str = "application/json"):
+        return {
+            "Authorization": f"Bearer {str(self.token)}",
+            "Content-Type": content_type,
+        }
+
+    def send(
+        self, request: Request
+    ) -> Union[Response, Coroutine[None, None, Response]]:
+        """
+        Build request url and headers, and send with underlying sender.
+
+        Exposed to easily send arbitrary requests,
+        for custom behavior in some endpoint e.g. for a subclass.
+        It may also come in handy if a bugfix or a feature is not implemented
+        in a timely manner, or in debugging related to the client or Web API.
+        """
+        request.url = build_url(request.url)
+        headers = self._create_headers()
+        if request.headers is not None:
+            headers.update(request.headers)
+        request.headers = headers
+        return self.sender.send(request)
+
+    @staticmethod
+    def _request(method: str, url: str, payload: dict = None, params: dict = None):
+        return (
+            Request(
+                method=method, url=url, params=parse_url_params(params), json=payload
+            ),
+            (),
+        )
+
+    def _get(self, url: str, payload: dict = None, **params):
+        return self._request("GET", url, payload=payload, params=params)
+
+    def _post(self, url: str, payload: dict = None, **params):
+        return self._request("POST", url, payload=payload, params=params)
+
+    def _delete(self, url: str, payload: dict = None, **params):
+        return self._request("DELETE", url, payload=payload, params=params)
+
+    def _put(self, url: str, payload: dict = None, **params):
+        return self._request("PUT", url, payload=payload, params=params)
```

### Comparing `tekore-4.5.0/tekore/_client/chunked.py` & `tekore-4.6.0/src/tekore/_client/chunked.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,150 @@
-from typing import Callable
-from functools import wraps
-
-from tekore.model import ModelList
-
-
-def _chunks(lst: list, n: int, reverse: bool) -> list:
-    """
-    Chunk list into length 'n' sublists.
-
-    Parameters
-    ----------
-    lst
-        list to chunk
-    n
-        length of chunks
-    reverse
-        reverse the order of chunks
-    """
-    rng = range(0, len(lst), n)
-
-    if reverse:
-        rng = rng[::-1]
-
-    for i in rng:
-        yield lst[i:i + n]
-
-
-def _get_arg(position, name, args, kwargs):
-    """Get argument from args or kwargs."""
-    return kwargs.get(name, None) if len(args) <= position else args[position]
-
-
-def _replace_arg(position, name, value, args, kwargs):
-    if len(args) <= position:
-        kwargs[name] = value
-    else:
-        args = args[:position] + (value,) + args[position + 1:]
-    return args, kwargs
-
-
-def chunked(
-        arg_name: str,
-        arg_pos: int,
-        chunk_size: int,
-        process: Callable,
-        reverse: str = None,
-        reverse_pos: int = None,
-        chain: str = None,
-        chain_pos: int = None,
-) -> Callable:
-    """
-    Decorate a function to make multiple calls splitting a list argument.
-
-    Optionally chain the return value of the previous request
-    to the specified variable in the next request.
-
-    Parameters
-    ----------
-    arg_name
-        argument to chunk
-    arg_pos
-        index of argument in the argument list
-    chunk_size
-        size of chunk to send at a time
-    process
-        process response list
-    reverse
-        reverse order of chunks sent when argument defined
-    reverse_pos
-        position of the reverse argument
-    chain
-        variable to chain into the next request
-    chain_pos
-        position of the chain argument
-    """
-    def decorator(function: Callable) -> Callable:
-        nonlocal arg_pos, reverse_pos, chain_pos
-        arg_pos -= 1
-        if reverse_pos is not None:
-            reverse_pos -= 1
-        if chain_pos is not None:
-            chain_pos -= 1
-
-        def replace(arg_val, chain_val, args, kwargs):
-            args, kwargs = _replace_arg(arg_pos, arg_name, arg_val, args, kwargs)
-
-            if chain is not None:
-                args, kwargs = _replace_arg(
-                    chain_pos,
-                    chain,
-                    chain_val,
-                    args,
-                    kwargs
-                )
-
-            return args, kwargs
-
-        async def async_wrapper(self, chunks, chain_val, args, kwargs):
-            responses = []
-            for chunk in chunks:
-                args, kwargs = replace(chunk, chain_val, args, kwargs)
-                chain_val = await function(self, *args, **kwargs)
-                responses.append(chain_val)
-
-            return process(responses)
-
-        @wraps(function)
-        def wrapper(self, *args, **kwargs):
-            arg_val = _get_arg(arg_pos, arg_name, args, kwargs)
-            if not self.chunked_on or arg_val is None:
-                return function(self, *args, **kwargs)
-
-            if chain is not None:
-                chain_val = _get_arg(chain_pos, chain, args, kwargs)
-            else:
-                chain_val = None
-
-            if reverse is not None:
-                reverse_val = _get_arg(reverse_pos, reverse, args, kwargs)
-                reverse_bool = reverse_val is not None
-            else:
-                reverse_bool = False
-
-            chunks = _chunks(arg_val, chunk_size, reverse_bool)
-
-            if self.is_async:
-                return async_wrapper(self, chunks, chain_val, args, kwargs)
-
-            responses = []
-            for chunk in chunks:
-                args, kwargs = replace(chunk, chain_val, args, kwargs)
-                chain_val = function(self, *args, **kwargs)
-                responses.append(chain_val)
-
-            return process(responses)
-        return wrapper
-    return decorator
-
-
-def join_lists(responses):
-    """Join lists of models into ModelList."""
-    return ModelList(sum(responses, []))
-
-
-def return_none(_):
-    """Return None always."""
-    return None
-
-
-def return_last(responses):
-    """Return last item of a list."""
-    return responses[-1] if responses else None
+from functools import wraps
+from typing import Callable
+
+from tekore.model import ModelList
+
+
+def _chunks(lst: list, n: int, reverse: bool) -> list:
+    """
+    Chunk list into length 'n' sublists.
+
+    Parameters
+    ----------
+    lst
+        list to chunk
+    n
+        length of chunks
+    reverse
+        reverse the order of chunks
+    """
+    rng = range(0, len(lst), n)
+
+    if reverse:
+        rng = rng[::-1]
+
+    for i in rng:
+        yield lst[i : i + n]
+
+
+def _get_arg(position, name, args, kwargs):
+    """Get argument from args or kwargs."""
+    return kwargs.get(name, None) if len(args) <= position else args[position]
+
+
+def _replace_arg(position, name, value, args, kwargs):
+    if len(args) <= position:
+        kwargs[name] = value
+    else:
+        args = args[:position] + (value,) + args[position + 1 :]
+    return args, kwargs
+
+
+def chunked(
+    arg_name: str,
+    arg_pos: int,
+    chunk_size: int,
+    process: Callable,
+    reverse: str = None,
+    reverse_pos: int = None,
+    chain: str = None,
+    chain_pos: int = None,
+) -> Callable:
+    """
+    Decorate a function to make multiple calls splitting a list argument.
+
+    Optionally chain the return value of the previous request
+    to the specified variable in the next request.
+
+    Parameters
+    ----------
+    arg_name
+        argument to chunk
+    arg_pos
+        index of argument in the argument list
+    chunk_size
+        size of chunk to send at a time
+    process
+        process response list
+    reverse
+        reverse order of chunks sent when argument defined
+    reverse_pos
+        position of the reverse argument
+    chain
+        variable to chain into the next request
+    chain_pos
+        position of the chain argument
+    """
+
+    def decorator(function: Callable) -> Callable:
+        nonlocal arg_pos, reverse_pos, chain_pos
+        arg_pos -= 1
+        if reverse_pos is not None:
+            reverse_pos -= 1
+        if chain_pos is not None:
+            chain_pos -= 1
+
+        def replace(arg_val, chain_val, args, kwargs):
+            args, kwargs = _replace_arg(arg_pos, arg_name, arg_val, args, kwargs)
+
+            if chain is not None:
+                args, kwargs = _replace_arg(chain_pos, chain, chain_val, args, kwargs)
+
+            return args, kwargs
+
+        async def async_wrapper(self, chunks, chain_val, args, kwargs):
+            responses = []
+            for chunk in chunks:
+                args, kwargs = replace(chunk, chain_val, args, kwargs)
+                chain_val = await function(self, *args, **kwargs)
+                responses.append(chain_val)
+
+            return process(responses)
+
+        @wraps(function)
+        def wrapper(self, *args, **kwargs):
+            arg_val = _get_arg(arg_pos, arg_name, args, kwargs)
+            if not self.chunked_on or arg_val is None:
+                return function(self, *args, **kwargs)
+
+            if chain is not None:
+                chain_val = _get_arg(chain_pos, chain, args, kwargs)
+            else:
+                chain_val = None
+
+            if reverse is not None:
+                reverse_val = _get_arg(reverse_pos, reverse, args, kwargs)
+                reverse_bool = reverse_val is not None
+            else:
+                reverse_bool = False
+
+            chunks = _chunks(arg_val, chunk_size, reverse_bool)
+
+            if self.is_async:
+                return async_wrapper(self, chunks, chain_val, args, kwargs)
+
+            responses = []
+            for chunk in chunks:
+                args, kwargs = replace(chunk, chain_val, args, kwargs)
+                chain_val = function(self, *args, **kwargs)
+                responses.append(chain_val)
+
+            return process(responses)
+
+        return wrapper
+
+    return decorator
+
+
+def join_lists(responses):
+    """Join lists of models into ModelList."""
+    return ModelList(sum(responses, []))
+
+
+def return_none(_):
+    """Return None always."""
+    return None
+
+
+def return_last(responses):
+    """Return last item of a list."""
+    return responses[-1] if responses else None
```

### Comparing `tekore-4.5.0/tekore/_client/decor/__init__.py` & `tekore-4.6.0/src/tekore/_client/decor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,102 @@
-from typing import Callable
-from functools import wraps
-
-from .handle import handle_errors
-from tekore._auth import Scope
-from tekore._sender import send_and_process as _send_and_process
-
-
-def send_and_process(post_func: Callable) -> Callable:
-    """
-    Decorate a Spotify endpoint to send a request and process its content.
-
-    Parameters
-    ----------
-    post_func
-        function to call with response JSON content
-    """
-    def parse_response(request, response):
-        handle_errors(request, response)
-        return post_func(response.content)
-
-    return _send_and_process(parse_response)
-
-
-def maximise_limit(max_limit: int) -> Callable:
-    """
-    Decorate a function to maximise the value of a 'limit' argument.
-
-    Parameters
-    ----------
-    max_limit
-        maximum value of the limit
-    """
-    def decorator(function: Callable) -> Callable:
-        varnames = function.__code__.co_varnames
-        arg_pos = varnames.index('limit') - 1
-
-        @wraps(function)
-        def wrapper(self, *args, **kwargs):
-            if self.max_limits_on and len(args) <= arg_pos:
-                kwargs.setdefault('limit', max_limit)
-            return function(self, *args, **kwargs)
-        return wrapper
-    return decorator
-
-
-def _add_doc_section(doc: str, section: str) -> str:
-    """Add section with correct indentation to docstring."""
-    items = doc.split('\n', maxsplit=2)
-
-    if len(items) == 1:
-        empty = ''
-        head = items[0]
-        body = ''
-    else:
-        empty, head, body = items
-
-    indent = (len(head) - len(head.lstrip(' '))) * ' '
-
-    section = indent + section.replace('\n', '\n' + indent)
-    return '\n'.join([empty, head, '', section, body])
-
-
-def scopes(required: list = None, optional: list = None) -> Callable:
-    """
-    List the scopes that a call uses.
-
-    Provides ``required_scopes``, ``optional_scopes``
-    and their combination ``scopes``.
-    Also modifies the docstring to include scope information.
-
-    Parameters
-    ----------
-    required
-        required scopes
-    optional
-        optional scopes
-    """
-    required = required or []
-    optional = optional or []
-    required_scope = Scope(*required)
-    optional_scope = Scope(*optional)
-    doc_msg = '\n'.join([
-        '| Required :class:`scope`: ' + (str(required_scope) or 'none'),
-        '| Optional :class:`scope`: ' + (str(optional_scope) or 'none')
-    ])
-
-    def decorator(function: Callable) -> Callable:
-        function.required_scope = required_scope
-        function.optional_scope = optional_scope
-        function.scope = required_scope + optional_scope
-        function.__doc__ = _add_doc_section(function.__doc__, doc_msg)
-        return function
-    return decorator
+from functools import wraps
+from typing import Callable
+
+from tekore._auth import Scope
+from tekore._sender import send_and_process as _send_and_process
+
+from .handle import handle_errors
+
+
+def send_and_process(post_func: Callable) -> Callable:
+    """
+    Decorate a Spotify endpoint to send a request and process its content.
+
+    Parameters
+    ----------
+    post_func
+        function to call with response JSON content
+    """
+
+    def parse_response(request, response):
+        handle_errors(request, response)
+        return post_func(response.content)
+
+    return _send_and_process(parse_response)
+
+
+def maximise_limit(max_limit: int) -> Callable:
+    """
+    Decorate a function to maximise the value of a 'limit' argument.
+
+    Parameters
+    ----------
+    max_limit
+        maximum value of the limit
+    """
+
+    def decorator(function: Callable) -> Callable:
+        varnames = function.__code__.co_varnames
+        arg_pos = varnames.index("limit") - 1
+
+        @wraps(function)
+        def wrapper(self, *args, **kwargs):
+            if self.max_limits_on and len(args) <= arg_pos:
+                kwargs.setdefault("limit", max_limit)
+            return function(self, *args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
+def _add_doc_section(doc: str, section: str) -> str:
+    """Add section with correct indentation to docstring."""
+    items = doc.split("\n", maxsplit=2)
+
+    if len(items) == 1:
+        empty = ""
+        head = items[0]
+        body = ""
+    else:
+        empty, head, body = items
+
+    indent = (len(head) - len(head.lstrip(" "))) * " "
+
+    section = indent + section.replace("\n", "\n" + indent)
+    return "\n".join([empty, head, "", section, body])
+
+
+def scopes(required: list = None, optional: list = None) -> Callable:
+    """
+    List the scopes that a call uses.
+
+    Provides ``required_scopes``, ``optional_scopes``
+    and their combination ``scopes``.
+    Also modifies the docstring to include scope information.
+
+    Parameters
+    ----------
+    required
+        required scopes
+    optional
+        optional scopes
+    """
+    required = required or []
+    optional = optional or []
+    required_scope = Scope(*required)
+    optional_scope = Scope(*optional)
+    doc_msg = "\n".join(
+        [
+            "| Required :class:`scope`: " + (str(required_scope) or "none"),
+            "| Optional :class:`scope`: " + (str(optional_scope) or "none"),
+        ]
+    )
+
+    def decorator(function: Callable) -> Callable:
+        function.required_scope = required_scope
+        function.optional_scope = optional_scope
+        function.scope = required_scope + optional_scope
+        function.__doc__ = _add_doc_section(function.__doc__, doc_msg)
+        return function
+
+    return decorator
```

### Comparing `tekore-4.5.0/tekore/_client/decor/handle.py` & `tekore-4.6.0/src/tekore/_client/decor/handle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from tekore._sender.error import get_error
-from tekore._sender import Request, Response
-from tekore.model import PlayerErrorReason
-
-error_format = """Error in {url}:
-{code}: {msg}
-"""
-
-
-def parse_error_reason(response: Response) -> str:
-    """Extract error reason from response content."""
-    reason = getattr(response, 'reason', '')
-
-    if response.content is None:
-        return reason
-
-    error = response.content['error']
-    message = error.get('message', reason)
-    if 'reason' in error:
-        message += '\n' + PlayerErrorReason[error['reason']].value
-    return message
-
-
-def handle_errors(request: Request, response: Response) -> None:
-    """Examine response and raise errors accordingly."""
-    if response.status_code >= 400:
-        error_str = error_format.format(
-            url=response.url,
-            code=response.status_code,
-            msg=parse_error_reason(response)
-        )
-        error_cls = get_error(response.status_code)
-        raise error_cls(error_str, request=request, response=response)
+from tekore._sender import Request, Response
+from tekore._sender.error import get_error
+from tekore.model import PlayerErrorReason
+
+error_format = """Error in {url}:
+{code}: {msg}
+"""
+
+
+def parse_error_reason(response: Response) -> str:
+    """Extract error reason from response content."""
+    reason = getattr(response, "reason", "")
+
+    if response.content is None:
+        return reason
+
+    error = response.content["error"]
+    message = error.get("message", reason)
+    if "reason" in error:
+        message += "\n" + PlayerErrorReason[error["reason"]].value
+    return message
+
+
+def handle_errors(request: Request, response: Response) -> None:
+    """Examine response and raise errors accordingly."""
+    if response.status_code >= 400:
+        error_str = error_format.format(
+            url=response.url,
+            code=response.status_code,
+            msg=parse_error_reason(response),
+        )
+        error_cls = get_error(response.status_code)
+        raise error_cls(error_str, request=request, response=response)
```

### Comparing `tekore-4.5.0/tekore/_client/full.py` & `tekore-4.6.0/src/tekore/_client/full.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-from typing import Generator
-from contextlib import contextmanager
-
-from .paging import SpotifyPaging
-from .api import (
-    SpotifyAlbum,
-    SpotifyArtist,
-    SpotifyAudiobook,
-    SpotifyBrowse,
-    SpotifyChapter,
-    SpotifyEpisode,
-    SpotifyFollow,
-    SpotifyLibrary,
-    SpotifyMarkets,
-    SpotifyPersonalisation,
-    SpotifyPlayer,
-    SpotifyPlaylist,
-    SpotifySearch,
-    SpotifyShow,
-    SpotifyTrack,
-    SpotifyUser,
-)
-
-
-class Spotify(
-    SpotifyAlbum,
-    SpotifyArtist,
-    SpotifyAudiobook,
-    SpotifyBrowse,
-    SpotifyChapter,
-    SpotifyEpisode,
-    SpotifyFollow,
-    SpotifyLibrary,
-    SpotifyMarkets,
-    SpotifyPersonalisation,
-    SpotifyPlayer,
-    SpotifyPlaylist,
-    SpotifySearch,
-    SpotifyShow,
-    SpotifyTrack,
-    SpotifyUser,
-    SpotifyPaging,
-):
-    """
-    Bases: :class:`tekore.Client`.
-
-    Client to Web API endpoints.
-
-    Parameters
-    ----------
-    token
-        bearer token for requests
-    sender
-        request sender
-    asynchronous
-        synchronicity requirement
-    max_limits_on
-        use maximum limits in paging calls, overrided by endpoint arguments
-    chunked_on
-        use chunking when requesting lists of resources
-
-    Attributes
-    ----------
-    token
-        bearer token for requests
-    sender
-        underlying sender
-    max_limits_on
-        use maximum limits in paging calls, overrided by endpoint arguments
-    chunked_on
-        use chunking when requesting lists of resources
-    """
-
-    @contextmanager
-    def token_as(self, token) -> Generator['Spotify', None, None]:
-        """
-        Use a different token with requests. Context manager, async safe.
-
-        Parameters
-        ----------
-        token
-            access token
-
-        Returns
-        -------
-        Generator[Spotify, None, None]
-            self as context
-
-        Examples
-        --------
-        .. code:: python
-
-            spotify = Spotify()
-            with spotify.token_as(token):
-                album = spotify.album(album_id)
-
-            spotify = Spotify(app_token)
-            with spotify.token_as(user_token):
-                user = spotify.current_user()
-        """
-        cv_token = self._token_cv.set(token)
-        yield self
-        self._token_cv.reset(cv_token)
-
-    @contextmanager
-    def max_limits(self, on: bool = True) -> Generator['Spotify', None, None]:
-        """
-        Toggle using maximum limits in paging calls. Context manager, async safe.
-
-        Parameters
-        ----------
-        on
-            enable or disable using maximum limits
-
-        Returns
-        -------
-        Generator[Spotify, None, None]
-            self as context
-
-        Examples
-        --------
-        .. code:: python
-
-            spotify = Spotify(token)
-            with spotify.max_limits(True):
-                tracks, = spotify.search('piano')
-
-            spotify = Spotify(token, max_limits_on=True)
-            with spotify.max_limits(False):
-                tracks, = spotify.search('piano')
-        """
-        cv_token = self._max_limits_on_cv.set(on)
-        yield self
-        self._max_limits_on_cv.reset(cv_token)
-
-    @contextmanager
-    def chunked(self, on: bool = True) -> Generator['Spotify', None, None]:
-        """
-        Toggle chunking lists of resources. Context manager, async safe.
-
-        Parameters
-        ----------
-        on
-            enable or disable chunking
-
-        Returns
-        -------
-        Generator[Spotify, None, None]
-            self as context
-
-        Examples
-        --------
-        .. code:: python
-
-            spotify = Spotify(token)
-            with spotify.chunked(True):
-                tracks = spotify.tracks(many_ids)
-
-            spotify = Spotify(token, chunked_on=True)
-            with spotify.chunked(False):
-                tracks = spotify.search(many_ids[:50])
-        """
-        cv_token = self._chunked_on_cv.set(on)
-        yield self
-        self._chunked_on_cv.reset(cv_token)
+from contextlib import contextmanager
+from typing import Generator
+
+from .api import (
+    SpotifyAlbum,
+    SpotifyArtist,
+    SpotifyAudiobook,
+    SpotifyBrowse,
+    SpotifyChapter,
+    SpotifyEpisode,
+    SpotifyFollow,
+    SpotifyLibrary,
+    SpotifyMarkets,
+    SpotifyPersonalisation,
+    SpotifyPlayer,
+    SpotifyPlaylist,
+    SpotifySearch,
+    SpotifyShow,
+    SpotifyTrack,
+    SpotifyUser,
+)
+from .paging import SpotifyPaging
+
+
+class Spotify(
+    SpotifyAlbum,
+    SpotifyArtist,
+    SpotifyAudiobook,
+    SpotifyBrowse,
+    SpotifyChapter,
+    SpotifyEpisode,
+    SpotifyFollow,
+    SpotifyLibrary,
+    SpotifyMarkets,
+    SpotifyPersonalisation,
+    SpotifyPlayer,
+    SpotifyPlaylist,
+    SpotifySearch,
+    SpotifyShow,
+    SpotifyTrack,
+    SpotifyUser,
+    SpotifyPaging,
+):
+    """
+    Bases: :class:`tekore.Client`.
+
+    Client to Web API endpoints.
+
+    Parameters
+    ----------
+    token
+        bearer token for requests
+    sender
+        request sender
+    asynchronous
+        synchronicity requirement
+    max_limits_on
+        use maximum limits in paging calls, overrided by endpoint arguments
+    chunked_on
+        use chunking when requesting lists of resources
+
+    Attributes
+    ----------
+    token
+        bearer token for requests
+    sender
+        underlying sender
+    max_limits_on
+        use maximum limits in paging calls, overrided by endpoint arguments
+    chunked_on
+        use chunking when requesting lists of resources
+    """
+
+    @contextmanager
+    def token_as(self, token) -> Generator["Spotify", None, None]:
+        """
+        Use a different token with requests. Context manager, async safe.
+
+        Parameters
+        ----------
+        token
+            access token
+
+        Returns
+        -------
+        Generator[Spotify, None, None]
+            self as context
+
+        Examples
+        --------
+        .. code:: python
+
+            spotify = Spotify()
+            with spotify.token_as(token):
+                album = spotify.album(album_id)
+
+            spotify = Spotify(app_token)
+            with spotify.token_as(user_token):
+                user = spotify.current_user()
+        """
+        cv_token = self._token_cv.set(token)
+        yield self
+        self._token_cv.reset(cv_token)
+
+    @contextmanager
+    def max_limits(self, on: bool = True) -> Generator["Spotify", None, None]:
+        """
+        Toggle using maximum limits in paging calls. Context manager, async safe.
+
+        Parameters
+        ----------
+        on
+            enable or disable using maximum limits
+
+        Returns
+        -------
+        Generator[Spotify, None, None]
+            self as context
+
+        Examples
+        --------
+        .. code:: python
+
+            spotify = Spotify(token)
+            with spotify.max_limits(True):
+                tracks, = spotify.search('piano')
+
+            spotify = Spotify(token, max_limits_on=True)
+            with spotify.max_limits(False):
+                tracks, = spotify.search('piano')
+        """
+        cv_token = self._max_limits_on_cv.set(on)
+        yield self
+        self._max_limits_on_cv.reset(cv_token)
+
+    @contextmanager
+    def chunked(self, on: bool = True) -> Generator["Spotify", None, None]:
+        """
+        Toggle chunking lists of resources. Context manager, async safe.
+
+        Parameters
+        ----------
+        on
+            enable or disable chunking
+
+        Returns
+        -------
+        Generator[Spotify, None, None]
+            self as context
+
+        Examples
+        --------
+        .. code:: python
+
+            spotify = Spotify(token)
+            with spotify.chunked(True):
+                tracks = spotify.tracks(many_ids)
+
+            spotify = Spotify(token, chunked_on=True)
+            with spotify.chunked(False):
+                tracks = spotify.search(many_ids[:50])
+        """
+        cv_token = self._chunked_on_cv.set(on)
+        yield self
+        self._chunked_on_cv.reset(cv_token)
```

### Comparing `tekore-4.5.0/tekore/_config.py` & `tekore-4.6.0/src/tekore/_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,230 +1,221 @@
-from os import environ
-from typing import Union, Iterable
-from warnings import warn
-from configparser import ConfigParser
-
-
-class MissingConfigurationWarning(RuntimeWarning):
-    """Missing value read from configuration."""
-
-
-def _read_configuration(conf: dict, return_refresh: bool = False) -> tuple:
-    """
-    Read variables from dictionary.
-
-    Parameters
-    ----------
-    conf
-        dictionary to read from
-    return_refresh
-        return user refresh token
-
-    Returns
-    -------
-    tuple
-        (client ID, client secret, redirect URI), None if not found.
-        If return_refresh is True, also return user refresh token.
-    """
-    from tekore import (
-        client_id_var,
-        client_secret_var,
-        redirect_uri_var,
-        user_refresh_var,
-    )
-    variables = (client_id_var, client_secret_var, redirect_uri_var)
-
-    if return_refresh:
-        variables += (user_refresh_var,)
-
-    values = tuple(conf.get(var, None) for var in variables)
-
-    for var, val in zip(variables, values):
-        if val is None:
-            warn(
-                f'`{var}` missing! None returned instead.',
-                MissingConfigurationWarning,
-                stacklevel=3
-            )
-
-    return values
-
-
-def config_from_environment(return_refresh: bool = False) -> tuple:
-    """
-    Read configuration from environment variables.
-
-    Parameters
-    ----------
-    return_refresh
-        return user refresh token
-
-    Returns
-    -------
-    tuple
-        (client ID, client secret, redirect URI), None if not found.
-        If return_refresh is True, also return user refresh token.
-
-    Raises
-    ------
-    MissingConfigurationWarning
-        when a missing value is encountered
-
-    Examples
-    --------
-    .. code:: python
-
-        client_id, client_secret, redirect_uri = tk.config_from_environment()
-
-        conf = tk.config_from_environment(return_refresh=True)
-        client_id, client_secret, redirect_uri, user_refresh = conf
-    """
-    return _read_configuration(environ, return_refresh)
-
-
-def _read_configfile(file_path: str, force: bool = True) -> ConfigParser:
-    """
-    Read configuration from INI file.
-
-    Parameters
-    ----------
-    file_path
-        path of the configuration file
-    force
-        force reading of the file, fail if not found
-    """
-    c = ConfigParser()
-    c.optionxform = str
-
-    if force:
-        with open(file_path, 'r') as f:
-            c.read_file(f)
-    else:
-        c.read(file_path)
-
-    return c
-
-
-def config_from_file(
-        file_path: str,
-        section: str = 'DEFAULT',
-        return_refresh: bool = False
-) -> tuple:
-    """
-    Read configuration from a config file.
-
-    The configuration must be in INI format
-    as accepted by :class:`configparser.ConfigParser`.
-
-    Parameters
-    ----------
-    file_path
-        path of the file containing the credential variables
-    section
-        name of the section to read variables from
-    return_refresh
-        return user refresh token
-
-    Returns
-    -------
-    tuple
-        (client ID, client secret, redirect URI), None if not found.
-        If return_refresh is True, also return user refresh token.
-
-    Raises
-    ------
-    MissingConfigurationWarning
-        when a missing value is encountered
-
-    Examples
-    --------
-    .. code:: python
-
-        client_id, client_secret, redirect_uri = tk.config_from_file(filename)
-
-        conf = tk.config_from_file(filename, return_refresh=True)
-        client_id, client_secret, redirect_uri, user_refresh = conf
-    """
-    c = _read_configfile(file_path)
-    return _read_configuration(c[section], return_refresh)
-
-
-def config_to_file(
-        file_path: str,
-        values: Union[Iterable, dict],
-        section: str = 'DEFAULT'
-) -> None:
-    """
-    Write configuration to a config file.
-
-    Existing configuration is preserved if it's not in conflict.
-
-    Parameters
-    ----------
-    file_path
-        path of the configuration file
-    values
-        configuration values to write, dict or iterable, see below for examples
-    section
-        name of the section to write to
-
-    Examples
-    --------
-    Configuration can be written in different ways.
-    Pass in an iterable to use the preset variable names.
-    The values should be ordered as returned when reading configuration:
-    ``client_id, client_secret, redirect_uri, user_refresh``.
-
-    .. code:: python
-
-        conf = (client_id, client_secret, redirect_uri, user_refresh)
-        config_to_file(filename, conf)
-
-    A shorter iterable or one containing ``None`` values may be passed.
-    Items missing from the end are ignored and ``None`` values are discarded.
-
-    .. code:: python
-
-        # Write partial information
-        config_to_file(filename, (client_id, client_secret))
-
-        # Fill the missing configuration
-        conf = (None, None, redirect_uri, user_refresh)
-        config_to_file(filename, conf)
-
-    A dictionary is also accepted.
-    In this case the keys are used instead of preset variable names.
-
-    .. code:: python
-
-        config_to_file(filename, {'REFRESH_TOKEN': refresh_token})
-    """
-    if isinstance(values, dict):
-        val_dict = values
-    else:
-        from tekore import (
-            client_id_var,
-            client_secret_var,
-            redirect_uri_var,
-            user_refresh_var,
-        )
-        names = (
-            client_id_var,
-            client_secret_var,
-            redirect_uri_var,
-            user_refresh_var
-        )
-        val_dict = {
-            name: value
-            for name, value in zip(names, values)
-            if value is not None
-        }
-
-    c = _read_configfile(file_path, force=False)
-
-    if section not in c:
-        c[section] = {}
-
-    c[section].update(val_dict)
-
-    with open(file_path, 'w') as f:
-        c.write(f)
+from configparser import ConfigParser
+from os import environ
+from typing import Iterable, Union
+from warnings import warn
+
+
+class MissingConfigurationWarning(RuntimeWarning):
+    """Missing value read from configuration."""
+
+
+def _read_configuration(conf: dict, return_refresh: bool = False) -> tuple:
+    """
+    Read variables from dictionary.
+
+    Parameters
+    ----------
+    conf
+        dictionary to read from
+    return_refresh
+        return user refresh token
+
+    Returns
+    -------
+    tuple
+        (client ID, client secret, redirect URI), None if not found.
+        If return_refresh is True, also return user refresh token.
+    """
+    from tekore import (
+        client_id_var,
+        client_secret_var,
+        redirect_uri_var,
+        user_refresh_var,
+    )
+
+    variables = (client_id_var, client_secret_var, redirect_uri_var)
+
+    if return_refresh:
+        variables += (user_refresh_var,)
+
+    values = tuple(conf.get(var, None) for var in variables)
+
+    for var, val in zip(variables, values):
+        if val is None:
+            warn(
+                f"`{var}` missing! None returned instead.",
+                MissingConfigurationWarning,
+                stacklevel=3,
+            )
+
+    return values
+
+
+def config_from_environment(return_refresh: bool = False) -> tuple:
+    """
+    Read configuration from environment variables.
+
+    Parameters
+    ----------
+    return_refresh
+        return user refresh token
+
+    Returns
+    -------
+    tuple
+        (client ID, client secret, redirect URI), None if not found.
+        If return_refresh is True, also return user refresh token.
+
+    Raises
+    ------
+    MissingConfigurationWarning
+        when a missing value is encountered
+
+    Examples
+    --------
+    .. code:: python
+
+        client_id, client_secret, redirect_uri = tk.config_from_environment()
+
+        conf = tk.config_from_environment(return_refresh=True)
+        client_id, client_secret, redirect_uri, user_refresh = conf
+    """
+    return _read_configuration(environ, return_refresh)
+
+
+def _read_configfile(file_path: str, force: bool = True) -> ConfigParser:
+    """
+    Read configuration from INI file.
+
+    Parameters
+    ----------
+    file_path
+        path of the configuration file
+    force
+        force reading of the file, fail if not found
+    """
+    c = ConfigParser()
+    c.optionxform = str
+
+    if force:
+        with open(file_path, "r") as f:
+            c.read_file(f)
+    else:
+        c.read(file_path)
+
+    return c
+
+
+def config_from_file(
+    file_path: str, section: str = "DEFAULT", return_refresh: bool = False
+) -> tuple:
+    """
+    Read configuration from a config file.
+
+    The configuration must be in INI format
+    as accepted by :class:`configparser.ConfigParser`.
+
+    Parameters
+    ----------
+    file_path
+        path of the file containing the credential variables
+    section
+        name of the section to read variables from
+    return_refresh
+        return user refresh token
+
+    Returns
+    -------
+    tuple
+        (client ID, client secret, redirect URI), None if not found.
+        If return_refresh is True, also return user refresh token.
+
+    Raises
+    ------
+    MissingConfigurationWarning
+        when a missing value is encountered
+
+    Examples
+    --------
+    .. code:: python
+
+        client_id, client_secret, redirect_uri = tk.config_from_file(filename)
+
+        conf = tk.config_from_file(filename, return_refresh=True)
+        client_id, client_secret, redirect_uri, user_refresh = conf
+    """
+    c = _read_configfile(file_path)
+    return _read_configuration(c[section], return_refresh)
+
+
+def config_to_file(
+    file_path: str, values: Union[Iterable, dict], section: str = "DEFAULT"
+) -> None:
+    """
+    Write configuration to a config file.
+
+    Existing configuration is preserved if it's not in conflict.
+
+    Parameters
+    ----------
+    file_path
+        path of the configuration file
+    values
+        configuration values to write, dict or iterable, see below for examples
+    section
+        name of the section to write to
+
+    Examples
+    --------
+    Configuration can be written in different ways.
+    Pass in an iterable to use the preset variable names.
+    The values should be ordered as returned when reading configuration:
+    ``client_id, client_secret, redirect_uri, user_refresh``.
+
+    .. code:: python
+
+        conf = (client_id, client_secret, redirect_uri, user_refresh)
+        config_to_file(filename, conf)
+
+    A shorter iterable or one containing ``None`` values may be passed.
+    Items missing from the end are ignored and ``None`` values are discarded.
+
+    .. code:: python
+
+        # Write partial information
+        config_to_file(filename, (client_id, client_secret))
+
+        # Fill the missing configuration
+        conf = (None, None, redirect_uri, user_refresh)
+        config_to_file(filename, conf)
+
+    A dictionary is also accepted.
+    In this case the keys are used instead of preset variable names.
+
+    .. code:: python
+
+        config_to_file(filename, {'REFRESH_TOKEN': refresh_token})
+    """
+    if isinstance(values, dict):
+        val_dict = values
+    else:
+        from tekore import (
+            client_id_var,
+            client_secret_var,
+            redirect_uri_var,
+            user_refresh_var,
+        )
+
+        names = (client_id_var, client_secret_var, redirect_uri_var, user_refresh_var)
+        val_dict = {
+            name: value for name, value in zip(names, values) if value is not None
+        }
+
+    c = _read_configfile(file_path, force=False)
+
+    if section not in c:
+        c[section] = {}
+
+    c[section].update(val_dict)
+
+    with open(file_path, "w") as f:
+        c.write(f)
```

### Comparing `tekore-4.5.0/tekore/_convert.py` & `tekore-4.6.0/src/tekore/_convert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-import re
-
-from typing import Union, Tuple
-from tekore.model import StrEnum
-
-
-class ConversionError(Exception):
-    """Error in conversion."""
-
-
-class IdentifierType(StrEnum):
-    """Valid types of Spotify IDs."""
-
-    artist = 'artist'
-    album = 'album'
-    episode = 'episode'
-    playlist = 'playlist'
-    show = 'show'
-    track = 'track'
-    user = 'user'
-
-
-def check_type(type_: Union[str, IdentifierType]) -> None:
-    """
-    Validate type of an ID.
-
-    Raises
-    ------
-    ConversionError
-        When type is invalid.
-    """
-    if str(type_) not in IdentifierType.__members__:
-        raise ConversionError(f'Invalid type "{type_}"!')
-
-
-# Match beginning, all base62 characters and end of string
-all_base62 = re.compile('^[0-9a-zA-Z]*$')
-
-
-def check_id(id_: str) -> None:
-    """
-    Validate resource ID to be base 62.
-
-    Note that user IDs can have special characters, so they cannot be validated.
-
-    Raises
-    ------
-    ConversionError
-        When ID is invalid.
-    """
-    if id_ == '' or all_base62.search(id_) is None:
-        raise ConversionError(f'Invalid id: "{id_}"!')
-
-
-def to_uri(type_: Union[str, IdentifierType], id_: str) -> str:
-    """
-    Convert an ID to an URI of the appropriate type.
-
-    Parameters
-    ----------
-    type_
-        valid :class:`IdentifierType`
-    id_
-        resource identifier
-
-    Returns
-    -------
-    str
-        converted URI
-
-    Raises
-    ------
-    ConversionError
-        On invalid type or ID.
-    """
-    check_type(type_)
-    if type_ != IdentifierType.user:
-        check_id(id_)
-    return f'spotify:{type_}:{id_}'
-
-
-def to_url(type_: Union[str, IdentifierType], id_: str) -> str:
-    """
-    Convert an ID to an URL of the appropriate type.
-
-    Parameters
-    ----------
-    type_
-        valid :class:`IdentifierType`
-    id_
-        resource identifier
-
-    Returns
-    -------
-    str
-        converted URL
-
-    Raises
-    ------
-    ConversionError
-        On invalid type or ID.
-    """
-    check_type(type_)
-    if type_ != IdentifierType.user:
-        check_id(id_)
-    else:
-        id_ = id_.replace('#', '%23')
-    return f'https://open.spotify.com/{type_}/{id_}'
-
-
-def from_uri(uri: str) -> Tuple[str, str]:
-    """
-    Parse type and ID from an URI.
-
-    Parameters
-    ----------
-    uri
-        URI to parse
-
-    Returns
-    -------
-    Tuple[str, str]
-        type and ID parsed from the URI
-
-    Raises
-    ------
-    ConversionError
-        On invalid format, prefix, type or ID.
-    """
-    try:
-        spotify, type_, id_ = uri.split(':')
-        if spotify != 'spotify':
-            raise ValueError()
-    except ValueError as e:
-        msg = f'Invalid URI: expected format "spotify:{{type}}:{{id}}", got "{uri}"!'
-        raise ConversionError(msg) from e
-
-    check_type(type_)
-    if type_ != IdentifierType.user:
-        check_id(id_)
-
-    return type_, id_
-
-
-_url_prefixes = (
-    'open.spotify.com',
-    'http://open.spotify.com',
-    'https://open.spotify.com'
-)
-
-
-def from_url(url: str) -> Tuple[str, str]:
-    """
-    Parse type and ID from an URL.
-
-    Any parameters in the URL will be ignored.
-
-    Parameters
-    ----------
-    url
-        URL to parse
-
-    Returns
-    -------
-    Tuple[str, str]
-        type and ID parsed from the URL
-
-    Raises
-    ------
-    ConversionError
-        On invalid format, prefix, type or ID.
-    """
-    try:
-        *prefixes, type_, id_ = url.split('/')
-        prefix = '/'.join(prefixes)
-        if prefix not in _url_prefixes:
-            raise ValueError()
-    except ValueError as e:
-        valid_url = '[http[s]://]open.spotify.com/{type}/{id}'
-        msg = f'Invalid URL: expected format "{valid_url}", got "{url}"!'
-        raise ConversionError(msg) from e
-
-    id_ = id_.split('?')[0]
-    check_type(type_)
-    if type_ != IdentifierType.user:
-        check_id(id_)
-
-    return type_, id_
+import re
+from typing import Tuple, Union
+
+from tekore.model import StrEnum
+
+
+class ConversionError(Exception):
+    """Error in conversion."""
+
+
+class IdentifierType(StrEnum):
+    """Valid types of Spotify IDs."""
+
+    artist = "artist"
+    album = "album"
+    episode = "episode"
+    playlist = "playlist"
+    show = "show"
+    track = "track"
+    user = "user"
+
+
+def check_type(type_: Union[str, IdentifierType]) -> None:
+    """
+    Validate type of an ID.
+
+    Raises
+    ------
+    ConversionError
+        When type is invalid.
+    """
+    if str(type_) not in IdentifierType.__members__:
+        raise ConversionError(f"Invalid type {type_!r}!")
+
+
+# Match beginning, all base62 characters and end of string
+all_base62 = re.compile("^[0-9a-zA-Z]*$")
+
+
+def check_id(id_: str) -> None:
+    """
+    Validate resource ID to be base 62.
+
+    Note that user IDs can have special characters, so they cannot be validated.
+
+    Raises
+    ------
+    ConversionError
+        When ID is invalid.
+    """
+    if id_ == "" or all_base62.search(id_) is None:
+        raise ConversionError(f"Invalid id: {id_!r}!")
+
+
+def to_uri(type_: Union[str, IdentifierType], id_: str) -> str:
+    """
+    Convert an ID to an URI of the appropriate type.
+
+    Parameters
+    ----------
+    type_
+        valid :class:`IdentifierType`
+    id_
+        resource identifier
+
+    Returns
+    -------
+    str
+        converted URI
+
+    Raises
+    ------
+    ConversionError
+        On invalid type or ID.
+    """
+    check_type(type_)
+    if type_ != IdentifierType.user:
+        check_id(id_)
+    return f"spotify:{type_}:{id_}"
+
+
+def to_url(type_: Union[str, IdentifierType], id_: str) -> str:
+    """
+    Convert an ID to an URL of the appropriate type.
+
+    Parameters
+    ----------
+    type_
+        valid :class:`IdentifierType`
+    id_
+        resource identifier
+
+    Returns
+    -------
+    str
+        converted URL
+
+    Raises
+    ------
+    ConversionError
+        On invalid type or ID.
+    """
+    check_type(type_)
+    if type_ != IdentifierType.user:
+        check_id(id_)
+    else:
+        id_ = id_.replace("#", "%23")
+    return f"https://open.spotify.com/{type_}/{id_}"
+
+
+def from_uri(uri: str) -> Tuple[str, str]:
+    """
+    Parse type and ID from an URI.
+
+    Parameters
+    ----------
+    uri
+        URI to parse
+
+    Returns
+    -------
+    Tuple[str, str]
+        type and ID parsed from the URI
+
+    Raises
+    ------
+    ConversionError
+        On invalid format, prefix, type or ID.
+    """
+    try:
+        spotify, type_, id_ = uri.split(":")
+        if spotify != "spotify":
+            raise ValueError()
+    except ValueError as e:
+        msg = f'Invalid URI: expected format "spotify:{{type}}:{{id}}", got {uri!r}!'
+        raise ConversionError(msg) from e
+
+    check_type(type_)
+    if type_ != IdentifierType.user:
+        check_id(id_)
+
+    return type_, id_
+
+
+_url_prefixes = (
+    "open.spotify.com",
+    "http://open.spotify.com",
+    "https://open.spotify.com",
+)
+
+
+def from_url(url: str) -> Tuple[str, str]:
+    """
+    Parse type and ID from an URL.
+
+    Any parameters in the URL will be ignored.
+
+    Parameters
+    ----------
+    url
+        URL to parse
+
+    Returns
+    -------
+    Tuple[str, str]
+        type and ID parsed from the URL
+
+    Raises
+    ------
+    ConversionError
+        On invalid format, prefix, type or ID.
+    """
+    try:
+        *prefixes, type_, id_ = url.split("/")
+        prefix = "/".join(prefixes)
+        if prefix not in _url_prefixes:
+            raise ValueError()
+    except ValueError as e:
+        valid_url = "[http[s]://]open.spotify.com/{type}/{id}"
+        msg = f"Invalid URL: expected format {valid_url!r}, got {url!r}!"
+        raise ConversionError(msg) from e
+
+    id_ = id_.split("?")[0]
+    check_type(type_)
+    if type_ != IdentifierType.user:
+        check_id(id_)
+
+    return type_, id_
```

### Comparing `tekore-4.5.0/tekore/_model/__init__.py` & `tekore-4.6.0/src/tekore/_model/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,114 +1,92 @@
-from .album import (
-    AlbumType,
-    Album,
-    AlbumGroup,
-    SimpleAlbum,
-    SimpleAlbumPaging,
-)
-from .album.full import FullAlbum, SavedAlbum, SavedAlbumPaging
-from .artist import (
-    Artist,
-    SimpleArtist,
-    FullArtist,
-    FullArtistCursorPaging,
-    FullArtistOffsetPaging,
-)
-from .audio_analysis import (
-    AudioAnalysis,
-    TimeInterval,
-    Section,
-    Segment,
-)
-from .audio_features import AudioFeatures
-from .audiobook import (
-    Author,
-    Narrator,
-    SimpleAudiobook,
-    SimpleAudiobookPaging,
-    Audiobook,
-)
-from .audiobook.full import FullAudiobook
-from .base import Identifiable, Item
-from .category import Category, CategoryPaging
-from .chapter import Chapter, SimpleChapterPaging, SimpleChapter
-from .chapter.full import FullChapter
-from .context import ContextType, Context
-from .currently_playing import (
-    CurrentlyPlayingType,
-    CurrentlyPlayingContext,
-    CurrentlyPlaying,
-    RepeatState,
-    Disallows,
-    Actions,
-    Queue,
-)
-from .device import Device, DeviceType
-from .episode import (
-    Episode,
-    SimpleEpisode,
-    SimpleEpisodePaging,
-    FullEpisode,
-    SavedEpisode,
-    SavedEpisodePaging,
-)
-from .error import PlayerErrorReason
-from .local import LocalItem, LocalAlbum, LocalArtist, LocalTrack
-from .member import (
-    ReleaseDatePrecision,
-    Copyright,
-    Followers,
-    Image,
-    Restrictions,
-    ResumePoint,
-)
-from .paging import Paging, OffsetPaging, Cursor, CursorPaging
-from .play_history import (
-    PlayHistory,
-    PlayHistoryCursor,
-    PlayHistoryPaging,
-)
-from .playlist import (
-    PlaylistTrack,
-    PlaylistTrackPaging,
-    Playlist,
-    SimplePlaylist,
-    FullPlaylist,
-    SimplePlaylistPaging,
-    FullPlaylistTrack,
-    FullPlaylistEpisode,
-    LocalPlaylistTrack,
-)
-from .recommendations import (
-    Recommendations,
-    RecommendationSeed,
-    RecommendationAttribute,
-)
-from .show import (
-    Show,
-    SimpleShow,
-    SimpleShowPaging,
-    SavedShow,
-    SavedShowPaging,
-)
-from .show.full import FullShow
-from .track import (
-    TrackLink,
-    Track,
-    Tracks,
-    SimpleTrack,
-    SavedTrack,
-    FullTrack,
-    SimpleTrackPaging,
-    SavedTrackPaging,
-    FullTrackPaging,
-)
-from .user import ExplicitContent, User, PrivateUser, PublicUser
-
-from .serialise import (
-    Model,
-    ModelList,
-    Serialisable,
-    StrEnum,
-    Timestamp,
-    UnknownModelAttributeWarning,
-)
+from .album import Album, AlbumGroup, AlbumType, SimpleAlbum, SimpleAlbumPaging
+from .album.full import FullAlbum, SavedAlbum, SavedAlbumPaging
+from .artist import (
+    Artist,
+    FullArtist,
+    FullArtistCursorPaging,
+    FullArtistOffsetPaging,
+    SimpleArtist,
+)
+from .audio_analysis import AudioAnalysis, Section, Segment, TimeInterval
+from .audio_features import AudioFeatures
+from .audiobook import (
+    Audiobook,
+    Author,
+    Narrator,
+    SimpleAudiobook,
+    SimpleAudiobookPaging,
+)
+from .audiobook.full import FullAudiobook
+from .base import Identifiable, Item
+from .category import Category, CategoryPaging
+from .chapter import Chapter, SimpleChapter, SimpleChapterPaging
+from .chapter.full import FullChapter
+from .context import Context, ContextType
+from .currently_playing import (
+    Actions,
+    CurrentlyPlaying,
+    CurrentlyPlayingContext,
+    CurrentlyPlayingType,
+    Disallows,
+    Queue,
+    RepeatState,
+)
+from .device import Device, DeviceType
+from .episode import (
+    Episode,
+    FullEpisode,
+    SavedEpisode,
+    SavedEpisodePaging,
+    SimpleEpisode,
+    SimpleEpisodePaging,
+)
+from .error import PlayerErrorReason
+from .local import LocalAlbum, LocalArtist, LocalItem, LocalTrack
+from .member import (
+    Copyright,
+    Followers,
+    Image,
+    ReleaseDatePrecision,
+    Restrictions,
+    ResumePoint,
+)
+from .paging import Cursor, CursorPaging, OffsetPaging, Paging
+from .play_history import PlayHistory, PlayHistoryCursor, PlayHistoryPaging
+from .playlist import (
+    FullPlaylist,
+    FullPlaylistEpisode,
+    FullPlaylistTrack,
+    LocalPlaylistTrack,
+    Playlist,
+    PlaylistTrack,
+    PlaylistTrackPaging,
+    SimplePlaylist,
+    SimplePlaylistPaging,
+)
+from .recommendations import (
+    RecommendationAttribute,
+    Recommendations,
+    RecommendationSeed,
+)
+from .serialise import (
+    Model,
+    ModelList,
+    Serialisable,
+    StrEnum,
+    Timestamp,
+    UnknownModelAttributeWarning,
+)
+from .show import SavedShow, SavedShowPaging, Show, SimpleShow, SimpleShowPaging
+from .show.full import FullShow
+from .track import (
+    FullTrack,
+    FullTrackPaging,
+    SavedTrack,
+    SavedTrackPaging,
+    SimpleTrack,
+    SimpleTrackPaging,
+    Track,
+    TrackLink,
+    Tracks,
+)
+from .user import ExplicitContent, PrivateUser, PublicUser, User
```

### Comparing `tekore-4.5.0/tekore/_model/album/__init__.py` & `tekore-4.6.0/src/tekore/_model/album/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import List, Optional
-from dataclasses import dataclass
-
-from ..paging import OffsetPaging
-from ..serialise import StrEnum, ModelList
-from ..album.base import Album, AlbumType
-
-
-class AlbumGroup(StrEnum):
-    """Relationship between artist and album."""
-
-    album = 'album'
-    appears_on = 'appears_on'
-    compilation = 'compilation'
-    single = 'single'
-
-
-@dataclass(repr=False)
-class SimpleAlbum(Album):
-    """
-    Simplified album object.
-
-    :attr:`album_group` is available when getting an artist's albums.
-    :attr:`available_markets` is available when market is not specified.
-
-    The presence of :attr:`is_playable` is undocumented
-    and it appears to only be ``True`` when it is present.
-    """
-
-    album_group: Optional[AlbumGroup] = None
-    available_markets: Optional[List[str]] = None
-    is_playable: Optional[bool] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        if self.album_group is not None:
-            self.album_group = AlbumGroup[self.album_group]
-        if self.available_markets is not None:
-            self.available_markets = ModelList(self.available_markets)
-
-
-@dataclass(repr=False)
-class SimpleAlbumPaging(OffsetPaging):
-    """Paging containing simplified albums."""
-
-    items: List[SimpleAlbum]
-
-    def __post_init__(self):
-        self.items = ModelList(SimpleAlbum.from_kwargs(a) for a in self.items)
+from dataclasses import dataclass
+from typing import List, Optional
+
+from ..album.base import Album, AlbumType
+from ..paging import OffsetPaging
+from ..serialise import ModelList, StrEnum
+
+
+class AlbumGroup(StrEnum):
+    """Relationship between artist and album."""
+
+    album = "album"
+    appears_on = "appears_on"
+    compilation = "compilation"
+    single = "single"
+
+
+@dataclass(repr=False)
+class SimpleAlbum(Album):
+    """
+    Simplified album object.
+
+    :attr:`album_group` is available when getting an artist's albums.
+    :attr:`available_markets` is available when market is not specified.
+
+    The presence of :attr:`is_playable` is undocumented
+    and it appears to only be ``True`` when it is present.
+    """
+
+    album_group: Optional[AlbumGroup] = None
+    available_markets: Optional[List[str]] = None
+    is_playable: Optional[bool] = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        if self.album_group is not None:
+            self.album_group = AlbumGroup[self.album_group]
+        if self.available_markets is not None:
+            self.available_markets = ModelList(self.available_markets)
+
+
+@dataclass(repr=False)
+class SimpleAlbumPaging(OffsetPaging):
+    """Paging containing simplified albums."""
+
+    items: List[SimpleAlbum]
+
+    def __post_init__(self):
+        self.items = ModelList(SimpleAlbum.from_kwargs(a) for a in self.items)
```

### Comparing `tekore-4.5.0/tekore/_model/album/base.py` & `tekore-4.6.0/src/tekore/_model/album/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from typing import List
-from dataclasses import dataclass
-
-from ..base import Item
-from ..artist import SimpleArtist
-from ..member import Image, ReleaseDatePrecision
-from ..serialise import StrEnum, ModelList
-
-
-class AlbumType(StrEnum):
-    """Type of album."""
-
-    album = 'album'
-    compilation = 'compilation'
-    single = 'single'
-
-
-@dataclass(repr=False)
-class Album(Item):
-    """Album base."""
-
-    album_type: AlbumType
-    artists: List[SimpleArtist]
-    external_urls: dict
-    images: List[Image]
-    name: str
-    total_tracks: int
-    release_date: str
-    release_date_precision: ReleaseDatePrecision
-
-    def __post_init__(self):
-        self.album_type = AlbumType[self.album_type.lower()]
-        self.artists = ModelList(SimpleArtist.from_kwargs(a) for a in self.artists)
-        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-        self.release_date_precision = ReleaseDatePrecision[
-            self.release_date_precision
-        ]
+from dataclasses import dataclass
+from typing import List
+
+from ..artist import SimpleArtist
+from ..base import Item
+from ..member import Image, ReleaseDatePrecision
+from ..serialise import ModelList, StrEnum
+
+
+class AlbumType(StrEnum):
+    """Type of album."""
+
+    album = "album"
+    compilation = "compilation"
+    single = "single"
+
+
+@dataclass(repr=False)
+class Album(Item):
+    """Album base."""
+
+    album_type: AlbumType
+    artists: List[SimpleArtist]
+    external_urls: dict
+    images: List[Image]
+    name: str
+    total_tracks: int
+    release_date: str
+    release_date_precision: ReleaseDatePrecision
+
+    def __post_init__(self):
+        self.album_type = AlbumType[self.album_type.lower()]
+        self.artists = ModelList(SimpleArtist.from_kwargs(a) for a in self.artists)
+        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
+        self.release_date_precision = ReleaseDatePrecision[self.release_date_precision]
```

### Comparing `tekore-4.5.0/tekore/_model/audio_analysis.py` & `tekore-4.6.0/src/tekore/_model/audio_analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,89 @@
-from typing import List, Optional
-from dataclasses import dataclass
-from .serialise import Model, ModelList
-
-
-@dataclass(repr=False)
-class TimeInterval(Model):
-    """
-    Generic representation of an interval.
-
-    Attributes are sometimes not available.
-    """
-
-    duration: float
-    start: Optional[float] = None
-    confidence: Optional[float] = None
-
-
-@dataclass(repr=False)
-class Section(Model):
-    """
-    Analysis of a track's section.
-
-    Attributes are sometimes not available.
-    """
-
-    duration: float
-    loudness: float
-    tempo: float
-    tempo_confidence: float
-    key_confidence: float
-    mode_confidence: float
-    time_signature: int
-    time_signature_confidence: float
-    confidence: Optional[float] = None
-    mode: Optional[int] = None
-    key: Optional[int] = None
-    start: Optional[float] = None
-
-
-@dataclass(repr=False)
-class Segment(Model):
-    """
-    Analysis of a track's segment.
-
-    Attributes are sometimes not available.
-    """
-
-    duration: float
-    loudness_start: float
-    loudness_max: float
-    pitches: List[float]
-    timbre: List[float]
-    confidence: Optional[float] = None
-    loudness_end: Optional[float] = None
-    loudness_max_time: Optional[float] = None
-    start: Optional[float] = None
-
-    def __post_init__(self):
-        self.pitches = ModelList(self.pitches)
-        self.timbre = ModelList(self.timbre)
-
-
-@dataclass(repr=False)
-class AudioAnalysis(Model):
-    """
-    Track audio analysis.
-
-    See the Web API
-    `documentation <https://developer.spotify.com/documentation/web-api/\
-    reference/tracks/get-audio-analysis/>`_
-    for more details.
-    """
-
-    bars: List[TimeInterval]
-    beats: List[TimeInterval]
-    sections: List[Section]
-    segments: List[Segment]
-    tatums: List[TimeInterval]
-    meta: dict
-    track: dict
-
-    def __post_init__(self):
-        self.bars = ModelList(TimeInterval.from_kwargs(i) for i in self.bars)
-        self.beats = ModelList(TimeInterval.from_kwargs(i) for i in self.beats)
-        self.sections = ModelList(Section.from_kwargs(s) for s in self.sections)
-        self.segments = ModelList(Segment.from_kwargs(s) for s in self.segments)
-        self.tatums = ModelList(TimeInterval.from_kwargs(i) for i in self.tatums)
+from dataclasses import dataclass
+from typing import List, Optional
+
+from .serialise import Model, ModelList
+
+
+@dataclass(repr=False)
+class TimeInterval(Model):
+    """
+    Generic representation of an interval.
+
+    Attributes are sometimes not available.
+    """
+
+    duration: float
+    start: Optional[float] = None
+    confidence: Optional[float] = None
+
+
+@dataclass(repr=False)
+class Section(Model):
+    """
+    Analysis of a track's section.
+
+    Attributes are sometimes not available.
+    """
+
+    duration: float
+    loudness: float
+    tempo: float
+    tempo_confidence: float
+    key_confidence: float
+    mode_confidence: float
+    time_signature: int
+    time_signature_confidence: float
+    confidence: Optional[float] = None
+    mode: Optional[int] = None
+    key: Optional[int] = None
+    start: Optional[float] = None
+
+
+@dataclass(repr=False)
+class Segment(Model):
+    """
+    Analysis of a track's segment.
+
+    Attributes are sometimes not available.
+    """
+
+    duration: float
+    loudness_start: float
+    loudness_max: float
+    pitches: List[float]
+    timbre: List[float]
+    confidence: Optional[float] = None
+    loudness_end: Optional[float] = None
+    loudness_max_time: Optional[float] = None
+    start: Optional[float] = None
+
+    def __post_init__(self):
+        self.pitches = ModelList(self.pitches)
+        self.timbre = ModelList(self.timbre)
+
+
+@dataclass(repr=False)
+class AudioAnalysis(Model):
+    """
+    Track audio analysis.
+
+    See the Web API
+    `documentation <https://developer.spotify.com/documentation/web-api/\
+    reference/tracks/get-audio-analysis/>`_
+    for more details.
+    """
+
+    bars: List[TimeInterval]
+    beats: List[TimeInterval]
+    sections: List[Section]
+    segments: List[Segment]
+    tatums: List[TimeInterval]
+    meta: dict
+    track: dict
+
+    def __post_init__(self):
+        self.bars = ModelList(TimeInterval.from_kwargs(i) for i in self.bars)
+        self.beats = ModelList(TimeInterval.from_kwargs(i) for i in self.beats)
+        self.sections = ModelList(Section.from_kwargs(s) for s in self.sections)
+        self.segments = ModelList(Segment.from_kwargs(s) for s in self.segments)
+        self.tatums = ModelList(TimeInterval.from_kwargs(i) for i in self.tatums)
```

### Comparing `tekore-4.5.0/tekore/_model/audiobook/base.py` & `tekore-4.6.0/src/tekore/_model/audiobook/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from typing import List
-from dataclasses import dataclass
-
-from ..base import Item
-from ..member import Copyright, Image
-from ..serialise import ModelList, Model
-
-
-@dataclass(repr=False)
-class Author(Model):
-    """Audiobook author."""
-
-    name: str
-
-
-@dataclass(repr=False)
-class Narrator(Model):
-    """Audiobook narrator."""
-
-    name: str
-
-
-@dataclass(repr=False)
-class Audiobook(Item):
-    """Audiobook base."""
-
-    authors: List[Author]
-    copyrights: List[Copyright]
-    description: str
-    edition: str
-    explicit: bool
-    external_urls: dict
-    html_description: str
-    images: List[Image]
-    languages: List[str]
-    media_type: str
-    name: str
-    narrators: List[Narrator]
-    publisher: str
-    total_chapters: int
-
-    def __post_init__(self):
-        self.authors = ModelList(Author.from_kwargs(i) for i in self.authors)
-        self.copyrights = ModelList(Copyright.from_kwargs(i) for i in self.copyrights)
-        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-        self.narrators = ModelList(Narrator.from_kwargs(i) for i in self.narrators)
+from dataclasses import dataclass
+from typing import List
+
+from ..base import Item
+from ..member import Copyright, Image
+from ..serialise import Model, ModelList
+
+
+@dataclass(repr=False)
+class Author(Model):
+    """Audiobook author."""
+
+    name: str
+
+
+@dataclass(repr=False)
+class Narrator(Model):
+    """Audiobook narrator."""
+
+    name: str
+
+
+@dataclass(repr=False)
+class Audiobook(Item):
+    """Audiobook base."""
+
+    authors: List[Author]
+    copyrights: List[Copyright]
+    description: str
+    edition: str
+    explicit: bool
+    external_urls: dict
+    html_description: str
+    images: List[Image]
+    languages: List[str]
+    media_type: str
+    name: str
+    narrators: List[Narrator]
+    publisher: str
+    total_chapters: int
+
+    def __post_init__(self):
+        self.authors = ModelList(Author.from_kwargs(i) for i in self.authors)
+        self.copyrights = ModelList(Copyright.from_kwargs(i) for i in self.copyrights)
+        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
+        self.narrators = ModelList(Narrator.from_kwargs(i) for i in self.narrators)
```

### Comparing `tekore-4.5.0/tekore/_model/category.py` & `tekore-4.6.0/src/tekore/_model/category.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import List
-from dataclasses import dataclass
-
-from .base import Identifiable
-from .member import Image
-from .paging import OffsetPaging
-from .serialise import ModelList
-
-
-@dataclass(repr=False)
-class Category(Identifiable):
-    """Spotify tag category."""
-
-    href: str
-    icons: List[Image]
-    name: str
-
-    def __post_init__(self):
-        self.icons = ModelList(Image.from_kwargs(i) for i in self.icons)
-
-
-@dataclass(repr=False)
-class CategoryPaging(OffsetPaging):
-    """Paging of categories."""
-
-    items: List[Category]
-
-    def __post_init__(self):
-        self.items = ModelList(Category.from_kwargs(c) for c in self.items)
+from dataclasses import dataclass
+from typing import List
+
+from .base import Identifiable
+from .member import Image
+from .paging import OffsetPaging
+from .serialise import ModelList
+
+
+@dataclass(repr=False)
+class Category(Identifiable):
+    """Spotify tag category."""
+
+    href: str
+    icons: List[Image]
+    name: str
+
+    def __post_init__(self):
+        self.icons = ModelList(Image.from_kwargs(i) for i in self.icons)
+
+
+@dataclass(repr=False)
+class CategoryPaging(OffsetPaging):
+    """Paging of categories."""
+
+    items: List[Category]
+
+    def __post_init__(self):
+        self.items = ModelList(Category.from_kwargs(c) for c in self.items)
```

### Comparing `tekore-4.5.0/tekore/_model/chapter/__init__.py` & `tekore-4.6.0/src/tekore/_model/chapter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import List, Optional
-from dataclasses import dataclass
-
-from ..paging import OffsetPaging
-from ..serialise import ModelList
-from ..member import Restrictions
-from .base import Chapter
-
-
-@dataclass(repr=False)
-class SimpleChapter(Chapter):
-    """Simplified chapter."""
-
-    available_markets: List[str] = None
-    is_playable: Optional[bool] = None
-    restriction: Optional[Restrictions] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        if self.restriction:
-            self.restriction = Restrictions.from_kwargs(self.restriction)
-
-
-@dataclass(repr=False)
-class SimpleChapterPaging(OffsetPaging):
-    """Paging of simplified chapters."""
-
-    items = List[SimpleChapter]
-
-    def __post_init__(self):
-        self.items = ModelList(SimpleChapter.from_kwargs(i) for i in self.items)
+from dataclasses import dataclass
+from typing import List, Optional
+
+from ..member import Restrictions
+from ..paging import OffsetPaging
+from ..serialise import ModelList
+from .base import Chapter
+
+
+@dataclass(repr=False)
+class SimpleChapter(Chapter):
+    """Simplified chapter."""
+
+    available_markets: List[str] = None
+    is_playable: Optional[bool] = None
+    restrictions: Optional[Restrictions] = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        if self.restrictions:
+            self.restrictions = Restrictions.from_kwargs(self.restrictions)
+
+
+@dataclass(repr=False)
+class SimpleChapterPaging(OffsetPaging):
+    """Paging of simplified chapters."""
+
+    items = List[SimpleChapter]
+
+    def __post_init__(self):
+        self.items = ModelList(SimpleChapter.from_kwargs(i) for i in self.items)
```

### Comparing `tekore-4.5.0/tekore/_model/chapter/full.py` & `tekore-4.6.0/src/tekore/_model/chapter/full.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Optional
-from dataclasses import dataclass
-
-from .base import Chapter
-from ..member import Restrictions
-from ..audiobook.full import FullAudiobook
-
-
-@dataclass(repr=False)
-class FullChapter(Chapter):
-    """Complete chapter object."""
-
-    audiobook: FullAudiobook
-    is_playable: Optional[bool] = None
-    restriction: Optional[Restrictions] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        self.audiobook = FullAudiobook.from_kwargs(self.audiobook)
-        if self.restriction:
-            self.restriction = Restrictions.from_kwargs(self.restriction)
+from dataclasses import dataclass
+from typing import Optional
+
+from ..audiobook.full import FullAudiobook
+from ..member import Restrictions
+from .base import Chapter
+
+
+@dataclass(repr=False)
+class FullChapter(Chapter):
+    """Complete chapter object."""
+
+    audiobook: FullAudiobook
+    is_playable: Optional[bool] = None
+    restrictions: Optional[Restrictions] = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.audiobook = FullAudiobook.from_kwargs(self.audiobook)
+        if self.restrictions:
+            self.restrictions = Restrictions.from_kwargs(self.restrictions)
```

### Comparing `tekore-4.5.0/tekore/_model/currently_playing.py` & `tekore-4.6.0/src/tekore/_model/currently_playing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,115 @@
-from typing import Optional, Union, List
-from dataclasses import dataclass
-
-from .context import Context
-from .device import Device
-from .track import FullTrack
-from .local import LocalTrack
-from .episode import FullEpisode
-from .serialise import Model, StrEnum, ModelList
-
-
-class CurrentlyPlayingType(StrEnum):
-    """Type of currently playing item."""
-
-    ad = 'ad'
-    episode = 'episode'
-    track = 'track'
-    unknown = 'unknown'
-
-
-class RepeatState(StrEnum):
-    """Playback repeat state."""
-
-    off = 'off'
-    track = 'track'
-    context = 'context'
-
-
-@dataclass(repr=False)
-class Disallows(Model):
-    """Disallowed player actions."""
-
-    interrupting_playback: bool = False
-    pausing: bool = False
-    resuming: bool = False
-    seeking: bool = False
-    skipping_next: bool = False
-    skipping_prev: bool = False
-    toggling_repeat_context: bool = False
-    toggling_shuffle: bool = False
-    toggling_repeat_track: bool = False
-    transferring_playback: bool = False
-
-
-@dataclass(repr=False)
-class Actions(Model):
-    """Player actions."""
-
-    disallows: Disallows
-
-    def __post_init__(self):
-        self.disallows = Disallows.from_kwargs(self.disallows)
-
-
-item_type = {
-    'track': FullTrack,
-    'episode': FullEpisode,
-}
-
-
-def _parse_playback_item(item: dict):
-    if item.get('is_local', False) is True:
-        return LocalTrack.from_kwargs(item)
-    else:
-        return item_type[item['type']].from_kwargs(item)
-
-
-@dataclass(repr=False)
-class CurrentlyPlaying(Model):
-    """
-    Current playback.
-
-    :attr:`context`, :attr:`progress_ms` and :attr:`item` may be ``None``
-    e.g. during a private session.
-    """
-
-    actions: Actions
-    currently_playing_type: CurrentlyPlayingType
-    is_playing: bool
-    timestamp: int
-    context: Optional[Context]
-    progress_ms: Optional[int]
-    item: Union[FullTrack, LocalTrack, FullEpisode, None]
-
-    def __post_init__(self):
-        self.actions = Actions.from_kwargs(self.actions)
-        self.currently_playing_type = CurrentlyPlayingType[
-            self.currently_playing_type
-        ]
-
-        if self.context is not None:
-            self.context = Context.from_kwargs(self.context)
-        if self.item is not None:
-            self.item = _parse_playback_item(self.item)
-
-
-@dataclass(repr=False)
-class CurrentlyPlayingContext(CurrentlyPlaying):
-    """Extended current playback context."""
-
-    device: Device
-    repeat_state: RepeatState
-    shuffle_state: bool
-
-    def __post_init__(self):
-        super().__post_init__()
-        self.device = Device.from_kwargs(self.device)
-        self.repeat_state = RepeatState[self.repeat_state]
-
-
-@dataclass(repr=False)
-class Queue(Model):
-    """Playback queue."""
-
-    currently_playing: Union[FullTrack, LocalTrack, FullEpisode, None]
-    queue: List[FullTrack]
-
-    def __post_init__(self):
-        self.currently_playing = _parse_playback_item(self.currently_playing)
-        self.queue = ModelList(_parse_playback_item(i) for i in self.queue)
+from dataclasses import dataclass
+from typing import List, Optional, Union
+
+from .context import Context
+from .device import Device
+from .episode import FullEpisode
+from .local import LocalTrack
+from .serialise import Model, ModelList, StrEnum
+from .track import FullTrack
+
+
+class CurrentlyPlayingType(StrEnum):
+    """Type of currently playing item."""
+
+    ad = "ad"
+    episode = "episode"
+    track = "track"
+    unknown = "unknown"
+
+
+class RepeatState(StrEnum):
+    """Playback repeat state."""
+
+    off = "off"
+    track = "track"
+    context = "context"
+
+
+@dataclass(repr=False)
+class Disallows(Model):
+    """Disallowed player actions."""
+
+    interrupting_playback: bool = False
+    pausing: bool = False
+    resuming: bool = False
+    seeking: bool = False
+    skipping_next: bool = False
+    skipping_prev: bool = False
+    toggling_repeat_context: bool = False
+    toggling_shuffle: bool = False
+    toggling_repeat_track: bool = False
+    transferring_playback: bool = False
+
+
+@dataclass(repr=False)
+class Actions(Model):
+    """Player actions."""
+
+    disallows: Disallows
+
+    def __post_init__(self):
+        self.disallows = Disallows.from_kwargs(self.disallows)
+
+
+item_type = {"track": FullTrack, "episode": FullEpisode}
+
+
+def _parse_playback_item(item: dict):
+    if item.get("is_local", False) is True:
+        return LocalTrack.from_kwargs(item)
+    else:
+        return item_type[item["type"]].from_kwargs(item)
+
+
+@dataclass(repr=False)
+class CurrentlyPlaying(Model):
+    """
+    Current playback.
+
+    :attr:`context`, :attr:`progress_ms` and :attr:`item` may be ``None``
+    e.g. during a private session.
+    """
+
+    actions: Actions
+    currently_playing_type: CurrentlyPlayingType
+    is_playing: bool
+    timestamp: int
+    context: Optional[Context]
+    progress_ms: Optional[int]
+    item: Union[FullTrack, LocalTrack, FullEpisode, None]
+
+    def __post_init__(self):
+        self.actions = Actions.from_kwargs(self.actions)
+        self.currently_playing_type = CurrentlyPlayingType[self.currently_playing_type]
+
+        if self.context is not None:
+            self.context = Context.from_kwargs(self.context)
+        if self.item is not None:
+            self.item = _parse_playback_item(self.item)
+
+
+@dataclass(repr=False)
+class CurrentlyPlayingContext(CurrentlyPlaying):
+    """Extended current playback context."""
+
+    device: Device
+    repeat_state: RepeatState
+    shuffle_state: bool
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.device = Device.from_kwargs(self.device)
+        self.repeat_state = RepeatState[self.repeat_state]
+
+
+@dataclass(repr=False)
+class Queue(Model):
+    """Playback queue."""
+
+    currently_playing: Union[FullTrack, LocalTrack, FullEpisode, None]
+    queue: List[FullTrack]
+
+    def __post_init__(self):
+        self.currently_playing = _parse_playback_item(self.currently_playing)
+        self.queue = ModelList(_parse_playback_item(i) for i in self.queue)
```

### Comparing `tekore-4.5.0/tekore/_model/local.py` & `tekore-4.6.0/src/tekore/_model/local.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import List
-from dataclasses import dataclass
-
-from .serialise import Model, ModelList
-
-
-@dataclass(repr=False)
-class LocalItem(Model):
-    """Base for local items."""
-
-    id: None
-    href: None
-    name: str
-    type: str
-    uri: None
-
-
-@dataclass(repr=False)
-class LocalAlbum(LocalItem):
-    """Album of a locally saved track."""
-
-    album_type: None
-    artists: List[None]
-    available_markets: List[None]
-    external_urls: dict
-    images: List[None]
-    release_date: None
-    release_date_precision: None
-
-
-@dataclass(repr=False)
-class LocalArtist(LocalItem):
-    """Artist of a locally saved track."""
-
-    external_urls: dict
-
-
-@dataclass(repr=False)
-class LocalTrack(LocalItem):
-    """
-    Locally saved track.
-
-    Locally saved track where most attributes are
-    always None, empty, zero or False.
-    """
-
-    album: LocalAlbum
-    artists: List[LocalArtist]
-    available_markets: List[None]
-    disc_number: int
-    duration_ms: int
-    explicit: bool
-    external_ids: dict
-    external_urls: dict
-    is_local: bool
-    popularity: int
-    preview_url: None
-    track_number: int
-    uri: str
-
-    def __post_init__(self):
-        self.album = LocalAlbum.from_kwargs(self.album)
-        self.artists = ModelList(LocalArtist.from_kwargs(a) for a in self.artists)
+from dataclasses import dataclass
+from typing import List
+
+from .serialise import Model, ModelList
+
+
+@dataclass(repr=False)
+class LocalItem(Model):
+    """Base for local items."""
+
+    id: None
+    href: None
+    name: str
+    type: str
+    uri: None
+
+
+@dataclass(repr=False)
+class LocalAlbum(LocalItem):
+    """Album of a locally saved track."""
+
+    album_type: None
+    artists: List[None]
+    available_markets: List[None]
+    external_urls: dict
+    images: List[None]
+    release_date: None
+    release_date_precision: None
+
+
+@dataclass(repr=False)
+class LocalArtist(LocalItem):
+    """Artist of a locally saved track."""
+
+    external_urls: dict
+
+
+@dataclass(repr=False)
+class LocalTrack(LocalItem):
+    """
+    Locally saved track.
+
+    Locally saved track where most attributes are
+    always None, empty, zero or False.
+    """
+
+    album: LocalAlbum
+    artists: List[LocalArtist]
+    available_markets: List[None]
+    disc_number: int
+    duration_ms: int
+    explicit: bool
+    external_ids: dict
+    external_urls: dict
+    is_local: bool
+    popularity: int
+    preview_url: None
+    track_number: int
+    uri: str
+
+    def __post_init__(self):
+        self.album = LocalAlbum.from_kwargs(self.album)
+        self.artists = ModelList(LocalArtist.from_kwargs(a) for a in self.artists)
```

### Comparing `tekore-4.5.0/tekore/_model/playlist.py` & `tekore-4.6.0/src/tekore/_model/playlist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,149 +1,146 @@
-from typing import List, Union, Optional
-from dataclasses import dataclass
-
-from .base import Item
-from .user import PublicUser
-from .local import LocalTrack
-from .track import FullTrack, Tracks
-from .paging import OffsetPaging
-from .member import Followers, Image
-from .episode import FullEpisode
-from .serialise import Model, ModelList, Timestamp
-
-
-@dataclass(repr=False)
-class FullPlaylistTrack(FullTrack):
-    """
-    Track on a playlist.
-
-    Provides :attr:`episode` and :attr:`track` booleans
-    to easily determine the type of playlist item.
-    """
-
-    episode: bool = False
-    track: bool = True
-
-
-@dataclass(repr=False)
-class FullPlaylistEpisode(FullEpisode):
-    """
-    Episode on a playlist.
-
-    Provides :attr:`episode` and :attr:`track` booleans
-    to easily determine the type of playlist item.
-    """
-
-    episode: bool = True
-    track: bool = False
-
-
-@dataclass(repr=False)
-class LocalPlaylistTrack(LocalTrack):
-    """
-    Local track on a playlist.
-
-    Provides :attr:`episode` and :attr:`track` booleans
-    to easily determine the type of playlist item.
-    """
-
-    episode: bool = False
-    track: bool = True
-
-
-track_type = {
-    'track': FullPlaylistTrack,
-    'episode': FullPlaylistEpisode,
-}
-
-
-@dataclass(repr=False)
-class PlaylistTrack(Model):
-    """Track or episode on a playlist."""
-
-    added_at: Timestamp
-    added_by: PublicUser
-    is_local: bool
-    primary_color: str
-    video_thumbnail: Optional[Image]
-    track: Union[FullPlaylistTrack, LocalPlaylistTrack, FullPlaylistEpisode, None]
-
-    def __post_init__(self):
-        self.added_at = Timestamp.from_string(self.added_at)
-        self.added_by = PublicUser.from_kwargs(self.added_by)
-
-        if self.video_thumbnail is not None:
-            self.video_thumbnail = Image.from_kwargs(self.video_thumbnail)
-
-        if self.track is not None:
-            if self.is_local:
-                self.track = LocalPlaylistTrack.from_kwargs(self.track)
-            else:
-                self.track = track_type[self.track['type']].from_kwargs(self.track)
-
-
-@dataclass(repr=False)
-class PlaylistTrackPaging(OffsetPaging):
-    """Paging of playlist tracks."""
-
-    items: List[PlaylistTrack]
-
-    def __post_init__(self):
-        self.items = ModelList(PlaylistTrack.from_kwargs(t) for t in self.items)
-
-
-@dataclass(repr=False)
-class Playlist(Item):
-    """
-    Playlist base.
-
-    :attr:`owner` can be ``None`` on featured playlists.
-    """
-
-    collaborative: bool
-    external_urls: dict
-    images: List[Image]
-    name: str
-    owner: PublicUser
-    public: bool
-    snapshot_id: str
-    primary_color: str
-    description: str
-
-    def __post_init__(self):
-        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-        if self.owner is not None:
-            self.owner = PublicUser.from_kwargs(self.owner)
-
-
-@dataclass(repr=False)
-class SimplePlaylist(Playlist):
-    """Simplified playlist object."""
-
-    tracks: Tracks
-
-    def __post_init__(self):
-        super().__post_init__()
-        self.tracks = Tracks.from_kwargs(self.tracks)
-
-
-@dataclass(repr=False)
-class FullPlaylist(Playlist):
-    """Complete playlist object."""
-
-    followers: Followers
-    tracks: PlaylistTrackPaging
-
-    def __post_init__(self):
-        super().__post_init__()
-        self.followers = Followers.from_kwargs(self.followers)
-        self.tracks = PlaylistTrackPaging.from_kwargs(self.tracks)
-
-
-@dataclass(repr=False)
-class SimplePlaylistPaging(OffsetPaging):
-    """Paging of simplified playlists."""
-
-    items: List[SimplePlaylist]
-
-    def __post_init__(self):
-        self.items = ModelList(SimplePlaylist.from_kwargs(p) for p in self.items)
+from dataclasses import dataclass
+from typing import List, Optional, Union
+
+from .base import Item
+from .episode import FullEpisode
+from .local import LocalTrack
+from .member import Followers, Image
+from .paging import OffsetPaging
+from .serialise import Model, ModelList, Timestamp
+from .track import FullTrack, Tracks
+from .user import PublicUser
+
+
+@dataclass(repr=False)
+class FullPlaylistTrack(FullTrack):
+    """
+    Track on a playlist.
+
+    Provides :attr:`episode` and :attr:`track` booleans
+    to easily determine the type of playlist item.
+    """
+
+    episode: bool = False
+    track: bool = True
+
+
+@dataclass(repr=False)
+class FullPlaylistEpisode(FullEpisode):
+    """
+    Episode on a playlist.
+
+    Provides :attr:`episode` and :attr:`track` booleans
+    to easily determine the type of playlist item.
+    """
+
+    episode: bool = True
+    track: bool = False
+
+
+@dataclass(repr=False)
+class LocalPlaylistTrack(LocalTrack):
+    """
+    Local track on a playlist.
+
+    Provides :attr:`episode` and :attr:`track` booleans
+    to easily determine the type of playlist item.
+    """
+
+    episode: bool = False
+    track: bool = True
+
+
+track_type = {"track": FullPlaylistTrack, "episode": FullPlaylistEpisode}
+
+
+@dataclass(repr=False)
+class PlaylistTrack(Model):
+    """Track or episode on a playlist."""
+
+    added_at: Timestamp
+    added_by: PublicUser
+    is_local: bool
+    primary_color: str
+    video_thumbnail: Optional[Image]
+    track: Union[FullPlaylistTrack, LocalPlaylistTrack, FullPlaylistEpisode, None]
+
+    def __post_init__(self):
+        self.added_at = Timestamp.from_string(self.added_at)
+        self.added_by = PublicUser.from_kwargs(self.added_by)
+
+        if self.video_thumbnail is not None:
+            self.video_thumbnail = Image.from_kwargs(self.video_thumbnail)
+
+        if self.track is not None:
+            if self.is_local:
+                self.track = LocalPlaylistTrack.from_kwargs(self.track)
+            else:
+                self.track = track_type[self.track["type"]].from_kwargs(self.track)
+
+
+@dataclass(repr=False)
+class PlaylistTrackPaging(OffsetPaging):
+    """Paging of playlist tracks."""
+
+    items: List[PlaylistTrack]
+
+    def __post_init__(self):
+        self.items = ModelList(PlaylistTrack.from_kwargs(t) for t in self.items)
+
+
+@dataclass(repr=False)
+class Playlist(Item):
+    """
+    Playlist base.
+
+    :attr:`owner` can be ``None`` on featured playlists.
+    """
+
+    collaborative: bool
+    external_urls: dict
+    images: List[Image]
+    name: str
+    owner: PublicUser
+    public: bool
+    snapshot_id: str
+    primary_color: str
+    description: str
+
+    def __post_init__(self):
+        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
+        if self.owner is not None:
+            self.owner = PublicUser.from_kwargs(self.owner)
+
+
+@dataclass(repr=False)
+class SimplePlaylist(Playlist):
+    """Simplified playlist object."""
+
+    tracks: Tracks
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.tracks = Tracks.from_kwargs(self.tracks)
+
+
+@dataclass(repr=False)
+class FullPlaylist(Playlist):
+    """Complete playlist object."""
+
+    followers: Followers
+    tracks: PlaylistTrackPaging
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.followers = Followers.from_kwargs(self.followers)
+        self.tracks = PlaylistTrackPaging.from_kwargs(self.tracks)
+
+
+@dataclass(repr=False)
+class SimplePlaylistPaging(OffsetPaging):
+    """Paging of simplified playlists."""
+
+    items: List[SimplePlaylist]
+
+    def __post_init__(self):
+        self.items = ModelList(SimplePlaylist.from_kwargs(p) for p in self.items)
```

### Comparing `tekore-4.5.0/tekore/_model/recommendations.py` & `tekore-4.6.0/src/tekore/_model/recommendations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import List
-from dataclasses import dataclass
-
-from .base import Identifiable
-from .track import FullTrack
-from .serialise import Model, ModelList, StrEnum
-
-
-class RecommendationAttribute(StrEnum):
-    """Attributes available in recommendations."""
-
-    acousticness = 'acousticness'
-    danceability = 'danceability'
-    duration_ms = 'duration_ms'
-    energy = 'energy'
-    instrumentalness = 'instrumentalness'
-    key = 'key'
-    liveness = 'liveness'
-    loudness = 'loudness'
-    mode = 'mode'
-    popularity = 'popularity'
-    speechiness = 'speechiness'
-    tempo = 'tempo'
-    time_signature = 'time_signature'
-    valence = 'valence'
-
-
-@dataclass(repr=False)
-class RecommendationSeed(Identifiable):
-    """Recommendation seeds."""
-
-    afterFilteringSize: int
-    afterRelinkingSize: int
-    href: str
-    initialPoolSize: int
-    type: str
-
-
-@dataclass(repr=False)
-class Recommendations(Model):
-    """Track recommendations."""
-
-    seeds: List[RecommendationSeed]
-    tracks: List[FullTrack]
-
-    def __post_init__(self):
-        self.seeds = ModelList(RecommendationSeed.from_kwargs(s) for s in self.seeds)
-        self.tracks = ModelList(FullTrack.from_kwargs(t) for t in self.tracks)
+from dataclasses import dataclass
+from typing import List
+
+from .base import Identifiable
+from .serialise import Model, ModelList, StrEnum
+from .track import FullTrack
+
+
+class RecommendationAttribute(StrEnum):
+    """Attributes available in recommendations."""
+
+    acousticness = "acousticness"
+    danceability = "danceability"
+    duration_ms = "duration_ms"
+    energy = "energy"
+    instrumentalness = "instrumentalness"
+    key = "key"
+    liveness = "liveness"
+    loudness = "loudness"
+    mode = "mode"
+    popularity = "popularity"
+    speechiness = "speechiness"
+    tempo = "tempo"
+    time_signature = "time_signature"
+    valence = "valence"
+
+
+@dataclass(repr=False)
+class RecommendationSeed(Identifiable):
+    """Recommendation seeds."""
+
+    afterFilteringSize: int
+    afterRelinkingSize: int
+    href: str
+    initialPoolSize: int
+    type: str
+
+
+@dataclass(repr=False)
+class Recommendations(Model):
+    """Track recommendations."""
+
+    seeds: List[RecommendationSeed]
+    tracks: List[FullTrack]
+
+    def __post_init__(self):
+        self.seeds = ModelList(RecommendationSeed.from_kwargs(s) for s in self.seeds)
+        self.tracks = ModelList(FullTrack.from_kwargs(t) for t in self.tracks)
```

### Comparing `tekore-4.5.0/tekore/_model/show/__init__.py` & `tekore-4.6.0/src/tekore/_model/show/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing import List
-from dataclasses import dataclass
-
-from ..paging import OffsetPaging
-from ..show.base import Show
-from ..serialise import Model, ModelList, Timestamp
-
-
-@dataclass(repr=False)
-class SimpleShow(Show):
-    """
-    Simplified show object.
-
-    :attr:`total_episodes` is undocumented by Spotify,
-    so it might be missing or removed in a future version.
-    """
-
-
-@dataclass(repr=False)
-class SimpleShowPaging(OffsetPaging):
-    """Paging of simplified shows."""
-
-    items: List[SimpleShow]
-
-    def __post_init__(self):
-        self.items = ModelList(SimpleShow.from_kwargs(i) for i in self.items)
-
-
-@dataclass(repr=False)
-class SavedShow(Model):
-    """Show saved in library."""
-
-    added_at: Timestamp
-    show: SimpleShow
-
-    def __post_init__(self):
-        self.added_at = Timestamp.from_string(self.added_at)
-        self.show = SimpleShow.from_kwargs(self.show)
-
-
-@dataclass(repr=False)
-class SavedShowPaging(OffsetPaging):
-    """Paging of shows in library."""
-
-    items: List[SavedShow]
-
-    def __post_init__(self):
-        self.items = ModelList(SavedShow.from_kwargs(i) for i in self.items)
+from dataclasses import dataclass
+from typing import List
+
+from ..paging import OffsetPaging
+from ..serialise import Model, ModelList, Timestamp
+from ..show.base import Show
+
+
+@dataclass(repr=False)
+class SimpleShow(Show):
+    """
+    Simplified show object.
+
+    :attr:`total_episodes` is undocumented by Spotify,
+    so it might be missing or removed in a future version.
+    """
+
+
+@dataclass(repr=False)
+class SimpleShowPaging(OffsetPaging):
+    """Paging of simplified shows."""
+
+    items: List[SimpleShow]
+
+    def __post_init__(self):
+        self.items = ModelList(SimpleShow.from_kwargs(i) for i in self.items)
+
+
+@dataclass(repr=False)
+class SavedShow(Model):
+    """Show saved in library."""
+
+    added_at: Timestamp
+    show: SimpleShow
+
+    def __post_init__(self):
+        self.added_at = Timestamp.from_string(self.added_at)
+        self.show = SimpleShow.from_kwargs(self.show)
+
+
+@dataclass(repr=False)
+class SavedShowPaging(OffsetPaging):
+    """Paging of shows in library."""
+
+    items: List[SavedShow]
+
+    def __post_init__(self):
+        self.items = ModelList(SavedShow.from_kwargs(i) for i in self.items)
```

### Comparing `tekore-4.5.0/tekore/_model/show/base.py` & `tekore-4.6.0/src/tekore/_model/show/base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import List, Optional
-from dataclasses import dataclass
-
-from ..base import Item
-from ..member import Copyright, Image
-from ..serialise import ModelList
-
-
-@dataclass(repr=False)
-class Show(Item):
-    """Show base."""
-
-    available_markets: List[str]
-    copyrights: List[Copyright]
-    description: str
-    explicit: bool
-    external_urls: dict
-    images: List[Image]
-    is_externally_hosted: bool
-    languages: List[str]
-    media_type: str
-    name: str
-    publisher: str
-    total_episodes: Optional[int] = None
-    html_description: str = None
-
-    def __post_init__(self):
-        self.available_markets = ModelList(self.available_markets)
-        self.copyrights = ModelList(Copyright.from_kwargs(c) for c in self.copyrights)
-        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-        self.languages = ModelList(self.languages)
+from dataclasses import dataclass
+from typing import List, Optional
+
+from ..base import Item
+from ..member import Copyright, Image
+from ..serialise import ModelList
+
+
+@dataclass(repr=False)
+class Show(Item):
+    """Show base."""
+
+    available_markets: List[str]
+    copyrights: List[Copyright]
+    description: str
+    explicit: bool
+    external_urls: dict
+    images: List[Image]
+    is_externally_hosted: bool
+    languages: List[str]
+    media_type: str
+    name: str
+    publisher: str
+    total_episodes: Optional[int] = None
+    html_description: str = None
+
+    def __post_init__(self):
+        self.available_markets = ModelList(self.available_markets)
+        self.copyrights = ModelList(Copyright.from_kwargs(c) for c in self.copyrights)
+        self.images = ModelList(Image.from_kwargs(i) for i in self.images)
+        self.languages = ModelList(self.languages)
```

### Comparing `tekore-4.5.0/tekore/_model/track.py` & `tekore-4.6.0/src/tekore/_model/track.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from typing import List, Optional
-from dataclasses import dataclass
-
-from .base import Item
-from .album import SimpleAlbum
-from .artist import SimpleArtist
-from .member import Restrictions
-from .paging import OffsetPaging
-from .serialise import Model, ModelList, Timestamp
-
-
-@dataclass(repr=False)
-class TrackLink(Item):
-    """Relinked track."""
-
-    external_urls: dict
-
-
-@dataclass(repr=False)
-class Track(Item):
-    """Track base."""
-
-    artists: List[SimpleArtist]
-    disc_number: int
-    duration_ms: int
-    explicit: bool
-    external_urls: dict
-    name: str
-    preview_url: str
-    track_number: int
-    is_local: bool
-
-    def __post_init__(self):
-        self.artists = ModelList(SimpleArtist.from_kwargs(a) for a in self.artists)
-
-
-@dataclass(repr=False)
-class SimpleTrack(Track):
-    """
-    Simplified track object.
-
-    When market is specified, :attr:`available_markets` is not available.
-    :attr:`is_playable` is not available when market is not specified.
-    :attr:`restrictions` is available if restrictions have been placed on
-    the track, making it unplayable.
-    """
-
-    available_markets: Optional[List[str]] = None
-    linked_from: Optional[TrackLink] = None
-    is_playable: Optional[bool] = None
-    restrictions: Optional[Restrictions] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        if self.available_markets is not None:
-            self.available_markets = ModelList(self.available_markets)
-        if self.linked_from is not None:
-            self.linked_from = TrackLink.from_kwargs(self.linked_from)
-        if self.restrictions is not None:
-            self.restrictions = Restrictions.from_kwargs(self.restrictions)
-
-
-@dataclass(repr=False)
-class FullTrack(Track):
-    """
-    Complete track object.
-
-    When market is specified, :attr:`available_markets` is not available.
-    :attr:`is_playable` is not available when market is not specified.
-    :attr:`restrictions` is available if restrictions have been placed on
-    the track, making it unplayable.
-    """
-
-    album: SimpleAlbum
-    external_ids: dict
-    popularity: int
-    available_markets: Optional[List[str]] = None
-    linked_from: Optional[TrackLink] = None
-    is_playable: Optional[bool] = None
-    restrictions: Optional[Restrictions] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        self.album = SimpleAlbum.from_kwargs(self.album)
-        if self.available_markets is not None:
-            self.available_markets = ModelList(self.available_markets)
-        if self.linked_from is not None:
-            self.linked_from = TrackLink.from_kwargs(self.linked_from)
-        if self.restrictions is not None:
-            self.restrictions = Restrictions.from_kwargs(self.restrictions)
-
-
-@dataclass(repr=False)
-class FullTrackPaging(OffsetPaging):
-    """Paging of full tracks."""
-
-    items: List[FullTrack]
-
-    def __post_init__(self):
-        self.items = ModelList(FullTrack.from_kwargs(t) for t in self.items)
-
-
-@dataclass(repr=False)
-class SimpleTrackPaging(OffsetPaging):
-    """Paging of simplified tracks."""
-
-    items: List[SimpleTrack]
-
-    def __post_init__(self):
-        self.items = ModelList(SimpleTrack.from_kwargs(t) for t in self.items)
-
-
-@dataclass(repr=False)
-class Tracks(Model):
-    """Minimal representation of playlist tracks."""
-
-    href: str
-    total: int
-
-
-@dataclass(repr=False)
-class SavedTrack(Model):
-    """Track saved to library."""
-
-    added_at: Timestamp
-    track: FullTrack
-
-    def __post_init__(self):
-        self.added_at = Timestamp.from_string(self.added_at)
-        self.track = FullTrack.from_kwargs(self.track)
-
-
-@dataclass(repr=False)
-class SavedTrackPaging(OffsetPaging):
-    """Paging of tracks in library."""
-
-    items: List[SavedTrack]
-
-    def __post_init__(self):
-        self.items = ModelList(SavedTrack.from_kwargs(t) for t in self.items)
+from dataclasses import dataclass
+from typing import List, Optional
+
+from .album import SimpleAlbum
+from .artist import SimpleArtist
+from .base import Item
+from .member import Restrictions
+from .paging import OffsetPaging
+from .serialise import Model, ModelList, Timestamp
+
+
+@dataclass(repr=False)
+class TrackLink(Item):
+    """Relinked track."""
+
+    external_urls: dict
+
+
+@dataclass(repr=False)
+class Track(Item):
+    """Track base."""
+
+    artists: List[SimpleArtist]
+    disc_number: int
+    duration_ms: int
+    explicit: bool
+    external_urls: dict
+    name: str
+    preview_url: str
+    track_number: int
+    is_local: bool
+
+    def __post_init__(self):
+        self.artists = ModelList(SimpleArtist.from_kwargs(a) for a in self.artists)
+
+
+@dataclass(repr=False)
+class SimpleTrack(Track):
+    """
+    Simplified track object.
+
+    When market is specified, :attr:`available_markets` is not available.
+    :attr:`is_playable` is not available when market is not specified.
+    :attr:`restrictions` is available if restrictions have been placed on
+    the track, making it unplayable.
+    """
+
+    available_markets: Optional[List[str]] = None
+    linked_from: Optional[TrackLink] = None
+    is_playable: Optional[bool] = None
+    restrictions: Optional[Restrictions] = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        if self.available_markets is not None:
+            self.available_markets = ModelList(self.available_markets)
+        if self.linked_from is not None:
+            self.linked_from = TrackLink.from_kwargs(self.linked_from)
+        if self.restrictions is not None:
+            self.restrictions = Restrictions.from_kwargs(self.restrictions)
+
+
+@dataclass(repr=False)
+class FullTrack(Track):
+    """
+    Complete track object.
+
+    When market is specified, :attr:`available_markets` is not available.
+    :attr:`is_playable` is not available when market is not specified.
+    :attr:`restrictions` is available if restrictions have been placed on
+    the track, making it unplayable.
+    """
+
+    album: SimpleAlbum
+    external_ids: dict
+    popularity: int
+    available_markets: Optional[List[str]] = None
+    linked_from: Optional[TrackLink] = None
+    is_playable: Optional[bool] = None
+    restrictions: Optional[Restrictions] = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.album = SimpleAlbum.from_kwargs(self.album)
+        if self.available_markets is not None:
+            self.available_markets = ModelList(self.available_markets)
+        if self.linked_from is not None:
+            self.linked_from = TrackLink.from_kwargs(self.linked_from)
+        if self.restrictions is not None:
+            self.restrictions = Restrictions.from_kwargs(self.restrictions)
+
+
+@dataclass(repr=False)
+class FullTrackPaging(OffsetPaging):
+    """Paging of full tracks."""
+
+    items: List[FullTrack]
+
+    def __post_init__(self):
+        self.items = ModelList(FullTrack.from_kwargs(t) for t in self.items)
+
+
+@dataclass(repr=False)
+class SimpleTrackPaging(OffsetPaging):
+    """Paging of simplified tracks."""
+
+    items: List[SimpleTrack]
+
+    def __post_init__(self):
+        self.items = ModelList(SimpleTrack.from_kwargs(t) for t in self.items)
+
+
+@dataclass(repr=False)
+class Tracks(Model):
+    """Minimal representation of playlist tracks."""
+
+    href: str
+    total: int
+
+
+@dataclass(repr=False)
+class SavedTrack(Model):
+    """Track saved to library."""
+
+    added_at: Timestamp
+    track: FullTrack
+
+    def __post_init__(self):
+        self.added_at = Timestamp.from_string(self.added_at)
+        self.track = FullTrack.from_kwargs(self.track)
+
+
+@dataclass(repr=False)
+class SavedTrackPaging(OffsetPaging):
+    """Paging of tracks in library."""
+
+    items: List[SavedTrack]
+
+    def __post_init__(self):
+        self.items = ModelList(SavedTrack.from_kwargs(t) for t in self.items)
```

### Comparing `tekore-4.5.0/tekore/_model/user.py` & `tekore-4.6.0/src/tekore/_model/user.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from typing import List, Optional
-from dataclasses import dataclass
-
-from .base import Item
-from .member import Followers, Image
-from .serialise import Model, ModelList
-
-
-@dataclass(repr=False)
-class ExplicitContent(Model):
-    """Explicit content filter of a user."""
-
-    filter_enabled: bool
-    filter_locked: bool
-
-
-@dataclass(repr=False)
-class User(Item):
-    """
-    User base.
-
-    :attr:`display_name`, :attr:`followers` and :attr:`images`
-    may not be available.
-    """
-
-    external_urls: dict
-    display_name: Optional[str] = None
-    followers: Optional[Followers] = None
-    images: Optional[List[Image]] = None
-
-    def __post_init__(self):
-        if self.followers is not None:
-            self.followers = Followers.from_kwargs(self.followers)
-        if self.images is not None:
-            self.images = ModelList(Image.from_kwargs(i) for i in self.images)
-
-
-@dataclass(repr=False)
-class PrivateUser(User):
-    """
-    User with private information.
-
-    :attr:`country`, :attr:`explicit_content` and :attr:`product`
-    require the ``user-read-private`` scope.
-    :attr:`email` requires the ``user-read-email`` scope.
-    :attr:`birthday` is unavailable unless the now-invalid
-    ``user-read-birthdate`` scope was granted to the token.
-    """
-
-    country: Optional[str] = None
-    email: Optional[str] = None
-    explicit_content: Optional[ExplicitContent] = None
-    product: Optional[str] = None
-    birthday: Optional[str] = None
-
-    def __post_init__(self):
-        super().__post_init__()
-        if self.explicit_content is not None:
-            self.explicit_content = ExplicitContent.from_kwargs(self.explicit_content)
-
-
-@dataclass(repr=False)
-class PublicUser(User):
-    """User as viewable by anyone."""
+from dataclasses import dataclass
+from typing import List, Optional
+
+from .base import Item
+from .member import Followers, Image
+from .serialise import Model, ModelList
+
+
+@dataclass(repr=False)
+class ExplicitContent(Model):
+    """Explicit content filter of a user."""
+
+    filter_enabled: bool
+    filter_locked: bool
+
+
+@dataclass(repr=False)
+class User(Item):
+    """
+    User base.
+
+    :attr:`display_name`, :attr:`followers` and :attr:`images`
+    may not be available.
+    """
+
+    external_urls: dict
+    display_name: Optional[str] = None
+    followers: Optional[Followers] = None
+    images: Optional[List[Image]] = None
+
+    def __post_init__(self):
+        if self.followers is not None:
+            self.followers = Followers.from_kwargs(self.followers)
+        if self.images is not None:
+            self.images = ModelList(Image.from_kwargs(i) for i in self.images)
+
+
+@dataclass(repr=False)
+class PrivateUser(User):
+    """
+    User with private information.
+
+    :attr:`country`, :attr:`explicit_content` and :attr:`product`
+    require the ``user-read-private`` scope.
+    :attr:`email` requires the ``user-read-email`` scope.
+    :attr:`birthday` is unavailable unless the now-invalid
+    ``user-read-birthdate`` scope was granted to the token.
+    """
+
+    country: Optional[str] = None
+    email: Optional[str] = None
+    explicit_content: Optional[ExplicitContent] = None
+    product: Optional[str] = None
+    birthday: Optional[str] = None
+
+    def __post_init__(self):
+        super().__post_init__()
+        if self.explicit_content is not None:
+            self.explicit_content = ExplicitContent.from_kwargs(self.explicit_content)
+
+
+@dataclass(repr=False)
+class PublicUser(User):
+    """User as viewable by anyone."""
```

### Comparing `tekore-4.5.0/tekore/_sender/base.py` & `tekore-4.6.0/src/tekore/_sender/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from typing import Optional, Union, Coroutine
-
-
-@dataclass
-class Request:
-    """Wrapper for parameters of a HTTP request."""
-
-    method: str
-    url: str
-    params: Optional[dict] = None
-    headers: Optional[dict] = None
-    data: Optional[dict] = None
-    json: Optional[dict] = None
-    content: Optional[str] = None
-
-
-@dataclass
-class Response:
-    """Wrapper for result of a HTTP request."""
-
-    url: str
-    headers: dict
-    status_code: int
-    content: Optional[dict]
-
-
-class Sender(ABC):
-    """Sender interface for requests."""
-
-    def __repr__(self):
-        return type(self).__name__ + '()'
-
-    @abstractmethod
-    def send(
-        self,
-        request: Request
-    ) -> Union[Response, Coroutine[None, None, Response]]:
-        """
-        Send a request.
-
-        Parameters
-        ----------
-        request
-            request to send
-
-        Returns
-        -------
-        Response
-            resulting response
-        """
-
-    @property
-    @abstractmethod
-    def is_async(self) -> bool:
-        """Sender asynchronicity mode."""
-
-    @abstractmethod
-    def close(self) -> Union[None, Coroutine[None, None, None]]:
-        """Close underlying client."""
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from typing import Coroutine, Optional, Union
+
+
+@dataclass
+class Request:
+    """Wrapper for parameters of a HTTP request."""
+
+    method: str
+    url: str
+    params: Optional[dict] = None
+    headers: Optional[dict] = None
+    data: Optional[dict] = None
+    json: Optional[dict] = None
+    content: Optional[str] = None
+
+
+@dataclass
+class Response:
+    """Wrapper for result of a HTTP request."""
+
+    url: str
+    headers: dict
+    status_code: int
+    content: Optional[dict]
+
+
+class Sender(ABC):
+    """Sender interface for requests."""
+
+    def __repr__(self):
+        return type(self).__name__ + "()"
+
+    @abstractmethod
+    def send(
+        self, request: Request
+    ) -> Union[Response, Coroutine[None, None, Response]]:
+        """
+        Send a request.
+
+        Parameters
+        ----------
+        request
+            request to send
+
+        Returns
+        -------
+        Response
+            resulting response
+        """
+
+    @property
+    @abstractmethod
+    def is_async(self) -> bool:
+        """Sender asynchronicity mode."""
+
+    @abstractmethod
+    def close(self) -> Union[None, Coroutine[None, None, None]]:
+        """Close underlying client."""
```

### Comparing `tekore-4.5.0/tekore/_sender/concrete.py` & `tekore-4.6.0/docs/src/reference/senders.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,90 @@
-from typing import Optional
-from httpx import Client, AsyncClient, Response as HTTPXResponse
-
-from .base import Sender, Request, Response
-
-
-def try_parse_json(response: HTTPXResponse) -> Optional[dict]:
-    """Parse json content or return None if not successful."""
-    try:
-        return response.json()
-    except ValueError:
-        return None
-
-
-class SyncSender(Sender):
-    """
-    Send requests synchronously.
-
-    .. warning::
-
-        The underlying client is *not* closed automatically.
-        Use :code:`sender.client.close()` to close it,
-        particularly if multiple senders are instantiated.
-
-    Parameters
-    ----------
-    client
-        :class:`httpx.Client` to use when sending requests
-    """
-
-    def __init__(self, client: Client = None):
-        self.client = client or Client()
-
-    def send(self, request: Request) -> Response:
-        """Send request with :class:`httpx.Client`."""
-        response = self.client.request(
-            method=request.method,
-            url=request.url,
-            params=request.params,
-            headers=request.headers,
-            data=request.data,
-            json=request.json,
-            content=request.content,
-        )
-        return Response(
-            url=str(response.url),
-            headers=response.headers,
-            status_code=response.status_code,
-            content=try_parse_json(response),
-        )
-
-    @property
-    def is_async(self) -> bool:
-        """Sender asynchronicity, always :class:`False`."""
-        return False
-
-    def close(self) -> None:
-        """Close the underlying synchronous client."""
-        return self.client.close()
-
-
-class AsyncSender(Sender):
-    """
-    Send requests asynchronously.
-
-    .. warning::
-
-        The underlying client is **not** closed automatically.
-        Use :code:`await sender.client.aclose()` to close it,
-        particularly if multiple senders are instantiated.
-
-    Parameters
-    ----------
-    client
-        :class:`httpx.AsyncClient` to use when sending requests
-    """
-
-    def __init__(self, client: AsyncClient = None):
-        self.client = client or AsyncClient()
-
-    async def send(self, request: Request) -> Response:
-        """Send request with :class:`httpx.AsyncClient`."""
-        response = await self.client.request(
-            method=request.method,
-            url=request.url,
-            params=request.params,
-            headers=request.headers,
-            data=request.data,
-            json=request.json,
-            content=request.content,
-        )
-        return Response(
-            url=str(response.url),
-            headers=response.headers,
-            status_code=response.status_code,
-            content=try_parse_json(response),
-        )
-
-    @property
-    def is_async(self) -> bool:
-        """Sender asynchronicity, always :class:`True`."""
-        return True
-
-    async def close(self) -> None:
-        """Close the underlying asynchronous client."""
-        return await self.client.aclose()
+.. _senders:
+
+Senders
+=======
+Manipulate the way clients send requests.
+
+.. currentmodule:: tekore
+.. autosummary::
+   :nosignatures:
+
+   SyncSender
+   AsyncSender
+   RetryingSender
+   CachingSender
+
+See also :ref:`senders-other`.
+
+Senders provide a hook between
+defining a request and sending it to the Web API.
+The sender of a :class:`Client` also determines whether synchronous or
+asynchronous calls are used to send requests and process responses.
+
+Sender instances are passed to a client at initialisation.
+
+.. code:: python
+
+    import tekore as tk
+
+    tk.Credentials(*conf, sender=tk.SyncSender())
+    tk.Spotify(sender=tk.RetryingSender())
+
+Senders wrap around the :mod:`httpx` library
+and accept additional keyword arguments to :meth:`httpx.Client`.
+
+.. code:: python
+
+    proxies = {
+        'http': 'http://10.10.10.10:8000',
+        'https': 'http://10.10.10.10:8000',
+    }
+    tk.SyncSender(proxies=proxies)
+
+Instances of :class:`httpx.Client` or :class:`httpx.AsyncClient`
+can also be passed in for a finer control over sender behaviour.
+
+.. code:: python
+
+    from httpx import Client
+
+    client = Client(proxies=proxies)
+    tk.SyncSender(client)
+
+Concrete senders
+----------------
+Final senders in a possible chain that concretely make the request to Spotify.
+
+.. autoclass:: SyncSender
+.. autoclass:: AsyncSender
+
+Extending senders
+-----------------
+Senders that extend the functionality of other senders.
+
+.. autoclass:: RetryingSender
+.. autoclass:: CachingSender
+
+.. _senders-other:
+
+Other classes
+-------------
+Bases for subclassing or other endeavours.
+
+.. autosummary::
+   :nosignatures:
+
+   Sender
+   ExtendingSender
+   SenderConflictWarning
+   Client
+   Request
+   Response
+
+.. autoclass:: Sender
+.. autoclass:: ExtendingSender
+.. autoclass:: SenderConflictWarning
+.. autoclass:: Client
+.. autoclass:: Request
+   :no-show-inheritance:
+.. autoclass:: Response
+   :no-show-inheritance:
```

### Comparing `tekore-4.5.0/tekore/_sender/error.py` & `tekore-4.6.0/src/tekore/_sender/error.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from .base import Request, Response
-
-
-class HTTPError(Exception):
-    """
-    Base error for all web status errors.
-
-    Attributes
-    ----------
-    request
-        request that led to the error
-    response
-        response from the web server
-    """
-
-    def __init__(self, message: str, request: Request, response: Response):
-        super(HTTPError, self).__init__(message)
-        self.request = request
-        self.response = response
-
-
-class ClientError(HTTPError):
-    """4xx - Base client error."""
-
-
-class ServerError(HTTPError):
-    """5xx - Base server error."""
-
-
-class BadRequest(ClientError):
-    """
-    400 - Bad request.
-
-    The request could not be understood by the server due to malformed syntax.
-    """
-
-
-class Unauthorised(ClientError):
-    """
-    401 - Unauthorised.
-
-    The request requires user authentication or,
-    if the request included authorization credentials,
-    authorization has been refused for those credentials.
-
-    The scopes associated with the call are attached to this class.
-    """
-
-    scope: str
-    required_scope: str
-    optional_scope: str
-
-
-class Forbidden(ClientError):
-    """
-    403 - Forbidden.
-
-    The server understood the request, but is refusing to fulfill it.
-    """
-
-
-class NotFound(ClientError):
-    """
-    404 - Not found.
-
-    The requested resource could not be found.
-    This error can be due to a temporary or permanent condition.
-    """
-
-
-class TooManyRequests(ClientError):
-    """
-    429 - Too many requests.
-
-    Rate limiting has been applied.
-    """
-
-
-class InternalServerError(ServerError):
-    """
-    500 - Internal server error.
-
-    You should never receive this error because the clever coders at Spotify
-    catch them all... But if you are unlucky enough to get one,
-    please report it to Spotify through their GitHub (spotify/web-api).
-    """
-
-
-class BadGateway(ClientError):
-    """
-    502 - Bad gateway.
-
-    The server was acting as a gateway or proxy and received
-    an invalid response from the upstream server.
-    """
-
-
-class ServiceUnavailable(ClientError):
-    """
-    503 - Service unavailable.
-
-    The server is currently unable to handle the request due to a temporary
-    condition which will be alleviated after some delay.
-    You can choose to resend the request again.
-    """
-
-
-errors = {
-    400: BadRequest,
-    401: Unauthorised,
-    403: Forbidden,
-    404: NotFound,
-    429: TooManyRequests,
-    500: InternalServerError,
-    502: BadGateway,
-    503: ServiceUnavailable,
-}
-
-
-def get_error(code):
-    """Get error based on status code or default error."""
-    cls = errors.get(code, None)
-    if cls is None:
-        if code < 500:
-            cls = ClientError
-        else:
-            cls = ServerError
-    return cls
+from .base import Request, Response
+
+
+class HTTPError(Exception):
+    """
+    Base error for all web status errors.
+
+    Attributes
+    ----------
+    request
+        request that led to the error
+    response
+        response from the web server
+    """
+
+    def __init__(self, message: str, request: Request, response: Response):
+        super(HTTPError, self).__init__(message)
+        self.request = request
+        self.response = response
+
+
+class ClientError(HTTPError):
+    """4xx - Base client error."""
+
+
+class ServerError(HTTPError):
+    """5xx - Base server error."""
+
+
+class BadRequest(ClientError):
+    """
+    400 - Bad request.
+
+    The request could not be understood by the server due to malformed syntax.
+    """
+
+
+class Unauthorised(ClientError):
+    """
+    401 - Unauthorised.
+
+    The request requires user authentication or,
+    if the request included authorization credentials,
+    authorization has been refused for those credentials.
+
+    The scopes associated with the call are attached to this class.
+    """
+
+    scope: str
+    required_scope: str
+    optional_scope: str
+
+
+class Forbidden(ClientError):
+    """
+    403 - Forbidden.
+
+    The server understood the request, but is refusing to fulfill it.
+    """
+
+
+class NotFound(ClientError):
+    """
+    404 - Not found.
+
+    The requested resource could not be found.
+    This error can be due to a temporary or permanent condition.
+    """
+
+
+class TooManyRequests(ClientError):
+    """
+    429 - Too many requests.
+
+    Rate limiting has been applied.
+    """
+
+
+class InternalServerError(ServerError):
+    """
+    500 - Internal server error.
+
+    You should never receive this error because the clever coders at Spotify
+    catch them all... But if you are unlucky enough to get one,
+    please report it to Spotify through their GitHub (spotify/web-api).
+    """
+
+
+class BadGateway(ClientError):
+    """
+    502 - Bad gateway.
+
+    The server was acting as a gateway or proxy and received
+    an invalid response from the upstream server.
+    """
+
+
+class ServiceUnavailable(ClientError):
+    """
+    503 - Service unavailable.
+
+    The server is currently unable to handle the request due to a temporary
+    condition which will be alleviated after some delay.
+    You can choose to resend the request again.
+    """
+
+
+errors = {
+    400: BadRequest,
+    401: Unauthorised,
+    403: Forbidden,
+    404: NotFound,
+    429: TooManyRequests,
+    500: InternalServerError,
+    502: BadGateway,
+    503: ServiceUnavailable,
+}
+
+
+def get_error(code):
+    """Get error based on status code or default error."""
+    cls = errors.get(code, None)
+    if cls is None:
+        if code < 500:
+            cls = ClientError
+        else:
+            cls = ServerError
+    return cls
```

### Comparing `tekore-4.5.0/tekore.egg-info/PKG-INFO` & `tekore-4.6.0/src/tekore.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,132 @@
-Metadata-Version: 2.1
-Name: tekore
-Version: 4.5.0
-Summary: Client for the Spotify Web API
-Home-page: https://tekore.readthedocs.io
-Download-URL: https://pypi.org/project/tekore
-Author: Felix Hildén
-Author-email: felix.hilden@gmail.com
-Maintainer: Felix Hildén
-Maintainer-email: felix.hilden@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/felix-hilden/tekore
-Project-URL: Issues, https://github.com/felix-hilden/tekore/issues
-Project-URL: Documentation, https://tekore.readthedocs.io
-Keywords: spotify web api client
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Multimedia :: Sound/Audio
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: tests
-Provides-Extra: checks
-Provides-Extra: dev
-License-File: LICENSE
-
-|logo|
-
-|python| |downloads|
-
-Welcome to the Python Package Index page of Tekore!
-We provide a client for the Spotify Web API for Python,
-complete with all available endpoints and authentication methods,
-async support and loads of additional features.
-Tekore allows you to interact with the API effortlessly.
-Here's five lines to get you full access and start playing your top songs.
-
-.. code:: python
-
-    import tekore as tk
-
-    conf = (client_id, client_secret, redirect_uri)
-    token = tk.prompt_for_user_token(*conf, scope=tk.scope.every)
-
-    spotify = tk.Spotify(token)
-    tracks = spotify.current_user_top_tracks(limit=10)
-    spotify.playback_start_tracks([t.id for t in tracks.items])
-
-See our online documentation on `Read The Docs`_ for tutorials,
-examples, package reference and a detailed description of features.
-If you've found a bug or would like to propose a feature,
-please submit an issue on `GitHub`_.
-Join our `Discord <https://discord.gg/wcRXgJu>`_ community
-to ask for help or discuss just about anything related to Tekore.
-You can also ask a question on
-`Stack Overflow <https://stackoverflow.com/questions/tagged/tekore>`_.
-
-Installation
-============
-Tekore can be installed from the Package Index via ``pip``.
-
-.. code:: sh
-
-    $ pip install tekore
-
-Changelog
-=========
-A detailed changelog can be found on our RTD documentation's
-`Release notes <https://tekore.readthedocs.io/page/release_notes.html>`_.
-
-Versioning
-==========
-When requiring Tekore in projects or other packages,
-please pin the version down to at least a specific major release
-to avoid compatibility issues.
-For example:
-
-.. code:: python
-
-    setup(
-        install_requires=[
-            'tekore~=4.0'
-        ]
-    )
-
-Tekore provides both stable and beta endpoints of the Web API.
-However, beta endpoints may be changed by Spotify without prior notice,
-so older versions of the library may have unintended issues.
-Because of this, Tekore follows a modified form of
-`Semantic Versioning <https://semver.org/>`_.
-Incompatible changes in the library are still introduced in major versions,
-and new features and endpoints are added in minor versions.
-But endpoints removed by Spotify are removed in minor versions and changes
-to endpoints are implemented as bugfixes.
-See the Web API `documentation <web api_>`_ for further information on beta endpoints.
-
-
-.. |logo| image:: https://raw.githubusercontent.com/felix-hilden/tekore/master/docs/src/logo_small.png
-   :alt: logo
-
-.. |python| image:: https://img.shields.io/pypi/pyversions/tekore
-   :alt: python version
-
-.. |downloads| image:: https://pepy.tech/badge/tekore/month
-   :alt: monthly downloads
-
-.. _github: https://github.com/felix-hilden/tekore
-.. _read the docs: https://tekore.readthedocs.io
-.. _web api: https://developer.spotify.com/documentation/web-api
+Metadata-Version: 2.1
+Name: tekore
+Version: 4.6.0
+Summary: Client for the Spotify Web API
+Author-email: Felix Hildén <felix.hilden@gmail.com>
+Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2019-2023 Felix Hildén
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://pypi.org/project/tekore
+Project-URL: Download, https://pypi.org/project/tekore
+Project-URL: Source, https://github.com/felix-hilden/tekore
+Project-URL: Issues, https://github.com/felix-hilden/tekore/issues
+Project-URL: Documentation, https://tekore.rtfd.org
+Keywords: spotify,web,api,client
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+|logo|
+
+|python| |downloads|
+
+Welcome to the Python Package Index page of Tekore!
+We provide a client for the Spotify Web API for Python,
+complete with all available endpoints and authentication methods,
+async support and loads of additional features.
+Tekore allows you to interact with the API effortlessly.
+Here's five lines to get you full access and start playing your top songs.
+
+.. code:: python
+
+    import tekore as tk
+
+    conf = (client_id, client_secret, redirect_uri)
+    token = tk.prompt_for_user_token(*conf, scope=tk.scope.every)
+
+    spotify = tk.Spotify(token)
+    tracks = spotify.current_user_top_tracks(limit=10)
+    spotify.playback_start_tracks([t.id for t in tracks.items])
+
+See our online documentation on `Read The Docs`_ for tutorials,
+examples, package reference and a detailed description of features.
+If you've found a bug or would like to propose a feature,
+please submit an issue on `GitHub`_.
+Join our `Discord <https://discord.gg/wcRXgJu>`_ community
+to ask for help or discuss just about anything related to Tekore.
+You can also ask a question on
+`Stack Overflow <https://stackoverflow.com/questions/tagged/tekore>`_.
+
+Installation
+============
+Tekore can be installed from the Package Index via ``pip``.
+
+.. code:: sh
+
+    $ pip install tekore
+
+Changelog
+=========
+A detailed changelog can be found on our RTD documentation's
+`Release notes <https://tekore.readthedocs.io/page/release_notes.html>`_.
+
+Versioning
+==========
+When requiring Tekore in projects or other packages,
+please pin the version down to at least a specific major release
+to avoid compatibility issues.
+For example:
+
+.. code:: python
+
+    setup(
+        install_requires=[
+            'tekore~=4.0'
+        ]
+    )
+
+Tekore provides both stable and beta endpoints of the Web API.
+However, beta endpoints may be changed by Spotify without prior notice,
+so older versions of the library may have unintended issues.
+Because of this, Tekore follows a modified form of
+`Semantic Versioning <https://semver.org/>`_.
+Incompatible changes in the library are still introduced in major versions,
+and new features and endpoints are added in minor versions.
+But endpoints removed by Spotify are removed in minor versions and changes
+to endpoints are implemented as bugfixes.
+See the Web API `documentation <web api_>`_ for further information on beta endpoints.
+
+
+.. |logo| image:: https://raw.githubusercontent.com/felix-hilden/tekore/master/docs/src/logo_small.png
+   :alt: logo
+
+.. |python| image:: https://img.shields.io/pypi/pyversions/tekore
+   :alt: python version
+
+.. |downloads| image:: https://pepy.tech/badge/tekore/month
+   :alt: monthly downloads
+
+.. _github: https://github.com/felix-hilden/tekore
+.. _read the docs: https://tekore.readthedocs.io
+.. _web api: https://developer.spotify.com/documentation/web-api
```

