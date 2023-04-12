# Comparing `tmp/gchar-0.0.7.tar.gz` & `tmp/gchar-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gchar-0.0.7.tar", last modified: Wed Apr 12 05:51:24 2023, max compression
+gzip compressed data, was "gchar-0.0.8.tar", last modified: Wed Apr 12 06:23:48 2023, max compression
```

## Comparing `gchar-0.0.7.tar` & `gchar-0.0.8.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.310284 gchar-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 05:50:26.000000 gchar-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 05:50:26.000000 gchar-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-12 05:51:24.306284 gchar-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-12 05:50:26.000000 gchar-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.278282 gchar-0.0.7/gchar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.278282 gchar-0.0.7/gchar/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.278282 gchar-0.0.7/gchar/games/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.282283 gchar-0.0.7/gchar/games/arknights/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/arknights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/arknights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/arknights/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   259285 2023-04-12 05:51:10.000000 gchar-0.0.7/gchar/games/arknights/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)   719302 2023-04-12 05:51:10.000000 gchar-0.0.7/gchar/games/arknights/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/arknights/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/arknights/name.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 05:51:10.000000 gchar-0.0.7/gchar/games/arknights/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    41356 2023-04-12 05:51:11.000000 gchar-0.0.7/gchar/games/arknights/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   285011 2023-04-12 05:51:11.000000 gchar-0.0.7/gchar/games/arknights/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/arknights/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.290283 gchar-0.0.7/gchar/games/azurlane/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/azurlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/azurlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/azurlane/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   571310 2023-04-12 05:51:12.000000 gchar-0.0.7/gchar/games/azurlane/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)  1261211 2023-04-12 05:51:11.000000 gchar-0.0.7/gchar/games/azurlane/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/azurlane/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/azurlane/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 05:51:12.000000 gchar-0.0.7/gchar/games/azurlane/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    91373 2023-04-12 05:51:12.000000 gchar-0.0.7/gchar/games/azurlane/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   537386 2023-04-12 05:51:12.000000 gchar-0.0.7/gchar/games/azurlane/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/azurlane/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.290283 gchar-0.0.7/gchar/games/base/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/character.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/moegirl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/base/skin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.290283 gchar-0.0.7/gchar/games/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/dispatch/access.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.294283 gchar-0.0.7/gchar/games/fgo/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/fgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/fgo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/fgo/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   631491 2023-04-12 05:51:09.000000 gchar-0.0.7/gchar/games/fgo/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)  1166076 2023-04-12 05:51:09.000000 gchar-0.0.7/gchar/games/fgo/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/fgo/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/fgo/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-12 05:51:09.000000 gchar-0.0.7/gchar/games/fgo/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    55053 2023-04-12 05:51:10.000000 gchar-0.0.7/gchar/games/fgo/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   281606 2023-04-12 05:51:10.000000 gchar-0.0.7/gchar/games/fgo/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/fgo/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.298283 gchar-0.0.7/gchar/games/genshin/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/genshin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/genshin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/genshin/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   143310 2023-04-12 05:51:13.000000 gchar-0.0.7/gchar/games/genshin/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)    71892 2023-04-12 05:51:12.000000 gchar-0.0.7/gchar/games/genshin/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/genshin/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/genshin/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 05:51:13.000000 gchar-0.0.7/gchar/games/genshin/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-04-12 05:51:13.000000 gchar-0.0.7/gchar/games/genshin/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)    71914 2023-04-12 05:51:13.000000 gchar-0.0.7/gchar/games/genshin/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/genshin/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.302284 gchar-0.0.7/gchar/games/girlsfrontline/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/girlsfrontline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/girlsfrontline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/girlsfrontline/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   364422 2023-04-12 05:51:14.000000 gchar-0.0.7/gchar/games/girlsfrontline/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)   589632 2023-04-12 05:51:13.000000 gchar-0.0.7/gchar/games/girlsfrontline/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/girlsfrontline/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/girlsfrontline/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 05:51:14.000000 gchar-0.0.7/gchar/games/girlsfrontline/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    59325 2023-04-12 05:51:14.000000 gchar-0.0.7/gchar/games/girlsfrontline/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)   270008 2023-04-12 05:51:14.000000 gchar-0.0.7/gchar/games/girlsfrontline/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/girlsfrontline/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.302284 gchar-0.0.7/gchar/games/neuralcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/neuralcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/neuralcloud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/neuralcloud/character.py
--rw-r--r--   0 runner    (1001) docker     (123)   391243 2023-04-12 05:51:15.000000 gchar-0.0.7/gchar/games/neuralcloud/danbooru_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)   147890 2023-04-12 05:51:14.000000 gchar-0.0.7/gchar/games/neuralcloud/index.json
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/neuralcloud/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/neuralcloud/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 05:51:15.000000 gchar-0.0.7/gchar/games/neuralcloud/pixiv_alias.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-04-12 05:51:15.000000 gchar-0.0.7/gchar/games/neuralcloud/pixiv_characters.json
--rw-r--r--   0 runner    (1001) docker     (123)    42560 2023-04-12 05:51:15.000000 gchar-0.0.7/gchar/games/neuralcloud/pixiv_names.json
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/games/neuralcloud/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.306284 gchar-0.0.7/gchar/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.306284 gchar-0.0.7/gchar/resources/danbooru/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/danbooru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/danbooru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/danbooru/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/danbooru/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/danbooru/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.306284 gchar-0.0.7/gchar/resources/pixiv/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/pixiv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/pixiv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/pixiv/games.py
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/pixiv/keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/pixiv/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/resources/pixiv/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.306284 gchar-0.0.7/gchar/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-12 05:50:26.000000 gchar-0.0.7/gchar/utils/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.278282 gchar-0.0.7/gchar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-12 05:51:24.000000 gchar-0.0.7/gchar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-12 05:51:24.000000 gchar-0.0.7/gchar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:51:24.000000 gchar-0.0.7/gchar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 05:51:24.000000 gchar-0.0.7/gchar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 05:51:24.000000 gchar-0.0.7/gchar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 05:50:26.000000 gchar-0.0.7/requirements-crawl.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 05:50:26.000000 gchar-0.0.7/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 05:50:26.000000 gchar-0.0.7/requirements-speedup.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 05:50:26.000000 gchar-0.0.7/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 05:50:26.000000 gchar-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:51:24.310284 gchar-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-12 05:50:26.000000 gchar-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:51:24.306284 gchar-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-12 05:50:26.000000 gchar-0.0.7/test/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.411107 gchar-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 06:22:51.000000 gchar-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 06:22:51.000000 gchar-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-12 06:23:48.411107 gchar-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-04-12 06:22:51.000000 gchar-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.383107 gchar-0.0.8/gchar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7646 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.383107 gchar-0.0.8/gchar/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.383107 gchar-0.0.8/gchar/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.387107 gchar-0.0.8/gchar/games/arknights/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/arknights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/arknights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/arknights/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)   259285 2023-04-12 06:23:34.000000 gchar-0.0.8/gchar/games/arknights/danbooru_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)   719302 2023-04-12 06:23:34.000000 gchar-0.0.8/gchar/games/arknights/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/arknights/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/arknights/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 06:23:34.000000 gchar-0.0.8/gchar/games/arknights/pixiv_alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    41356 2023-04-12 06:23:35.000000 gchar-0.0.8/gchar/games/arknights/pixiv_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   285011 2023-04-12 06:23:35.000000 gchar-0.0.8/gchar/games/arknights/pixiv_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/arknights/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.391107 gchar-0.0.8/gchar/games/azurlane/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/azurlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/azurlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/azurlane/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)   571310 2023-04-12 06:23:35.000000 gchar-0.0.8/gchar/games/azurlane/danbooru_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1261211 2023-04-12 06:23:35.000000 gchar-0.0.8/gchar/games/azurlane/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/azurlane/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/azurlane/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 06:23:36.000000 gchar-0.0.8/gchar/games/azurlane/pixiv_alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    91373 2023-04-12 06:23:36.000000 gchar-0.0.8/gchar/games/azurlane/pixiv_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   537386 2023-04-12 06:23:36.000000 gchar-0.0.8/gchar/games/azurlane/pixiv_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/azurlane/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.395107 gchar-0.0.8/gchar/games/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/moegirl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/base/skin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.395107 gchar-0.0.8/gchar/games/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/dispatch/access.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.399107 gchar-0.0.8/gchar/games/fgo/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/fgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/fgo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/fgo/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)   631491 2023-04-12 06:23:33.000000 gchar-0.0.8/gchar/games/fgo/danbooru_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1166076 2023-04-12 06:23:32.000000 gchar-0.0.8/gchar/games/fgo/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/fgo/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/fgo/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-12 06:23:33.000000 gchar-0.0.8/gchar/games/fgo/pixiv_alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    55053 2023-04-12 06:23:34.000000 gchar-0.0.8/gchar/games/fgo/pixiv_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   281606 2023-04-12 06:23:33.000000 gchar-0.0.8/gchar/games/fgo/pixiv_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/fgo/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.399107 gchar-0.0.8/gchar/games/genshin/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/genshin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/genshin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/genshin/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143310 2023-04-12 06:23:36.000000 gchar-0.0.8/gchar/games/genshin/danbooru_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71892 2023-04-12 06:23:36.000000 gchar-0.0.8/gchar/games/genshin/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/genshin/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/genshin/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 06:23:37.000000 gchar-0.0.8/gchar/games/genshin/pixiv_alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-04-12 06:23:37.000000 gchar-0.0.8/gchar/games/genshin/pixiv_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71914 2023-04-12 06:23:37.000000 gchar-0.0.8/gchar/games/genshin/pixiv_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/genshin/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.403107 gchar-0.0.8/gchar/games/girlsfrontline/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/girlsfrontline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/girlsfrontline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/girlsfrontline/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)   364422 2023-04-12 06:23:38.000000 gchar-0.0.8/gchar/games/girlsfrontline/danbooru_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)   589632 2023-04-12 06:23:37.000000 gchar-0.0.8/gchar/games/girlsfrontline/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/girlsfrontline/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/girlsfrontline/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 06:23:38.000000 gchar-0.0.8/gchar/games/girlsfrontline/pixiv_alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    59325 2023-04-12 06:23:38.000000 gchar-0.0.8/gchar/games/girlsfrontline/pixiv_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)   270008 2023-04-12 06:23:38.000000 gchar-0.0.8/gchar/games/girlsfrontline/pixiv_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/girlsfrontline/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.407107 gchar-0.0.8/gchar/games/neuralcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/neuralcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/neuralcloud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/neuralcloud/character.py
+-rw-r--r--   0 runner    (1001) docker     (123)   391243 2023-04-12 06:23:39.000000 gchar-0.0.8/gchar/games/neuralcloud/danbooru_tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147890 2023-04-12 06:23:38.000000 gchar-0.0.8/gchar/games/neuralcloud/index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/neuralcloud/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/neuralcloud/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 06:23:39.000000 gchar-0.0.8/gchar/games/neuralcloud/pixiv_alias.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-04-12 06:23:39.000000 gchar-0.0.8/gchar/games/neuralcloud/pixiv_characters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42560 2023-04-12 06:23:39.000000 gchar-0.0.8/gchar/games/neuralcloud/pixiv_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/games/neuralcloud/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.407107 gchar-0.0.8/gchar/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.407107 gchar-0.0.8/gchar/resources/danbooru/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/danbooru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/danbooru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/danbooru/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/danbooru/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/danbooru/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.411107 gchar-0.0.8/gchar/resources/pixiv/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/pixiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/pixiv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/pixiv/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/pixiv/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/pixiv/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/resources/pixiv/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.411107 gchar-0.0.8/gchar/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-12 06:22:51.000000 gchar-0.0.8/gchar/utils/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.383107 gchar-0.0.8/gchar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-04-12 06:23:48.000000 gchar-0.0.8/gchar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-12 06:23:48.000000 gchar-0.0.8/gchar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 06:23:48.000000 gchar-0.0.8/gchar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 06:23:48.000000 gchar-0.0.8/gchar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 06:23:48.000000 gchar-0.0.8/gchar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-12 06:22:51.000000 gchar-0.0.8/requirements-crawl.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 06:22:51.000000 gchar-0.0.8/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 06:22:51.000000 gchar-0.0.8/requirements-speedup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 06:22:51.000000 gchar-0.0.8/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 06:22:51.000000 gchar-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 06:23:48.411107 gchar-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-12 06:22:51.000000 gchar-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 06:23:48.411107 gchar-0.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-12 06:22:51.000000 gchar-0.0.8/test/test_entry.py
```

### Comparing `gchar-0.0.7/LICENSE` & `gchar-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/PKG-INFO` & `gchar-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gchar
-Version: 0.0.7
+Version: 0.0.8
 Summary: Game character manager.
 Home-page: https://github.com/narugo1992/gchar
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gchar-0.0.7/README.md` & `gchar-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/__main__.py` & `gchar-0.0.8/gchar/__main__.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/character.py` & `gchar-0.0.8/gchar/games/arknights/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/danbooru_tags.json` & `gchar-0.0.8/gchar/games/arknights/danbooru_tags.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/index.json` & `gchar-0.0.8/gchar/games/arknights/index.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/index.py` & `gchar-0.0.8/gchar/games/arknights/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/name.py` & `gchar-0.0.8/gchar/games/arknights/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/pixiv_characters.json` & `gchar-0.0.8/gchar/games/arknights/pixiv_characters.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/pixiv_names.json` & `gchar-0.0.8/gchar/games/arknights/pixiv_names.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/arknights/property.py` & `gchar-0.0.8/gchar/games/arknights/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/character.py` & `gchar-0.0.8/gchar/games/azurlane/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/danbooru_tags.json` & `gchar-0.0.8/gchar/games/azurlane/danbooru_tags.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/index.json` & `gchar-0.0.8/gchar/games/azurlane/index.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/index.py` & `gchar-0.0.8/gchar/games/azurlane/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/name.py` & `gchar-0.0.8/gchar/games/azurlane/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/pixiv_characters.json` & `gchar-0.0.8/gchar/games/azurlane/pixiv_characters.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/pixiv_names.json` & `gchar-0.0.8/gchar/games/azurlane/pixiv_names.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/azurlane/property.py` & `gchar-0.0.8/gchar/games/azurlane/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/base/character.py` & `gchar-0.0.8/gchar/games/base/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/base/index.py` & `gchar-0.0.8/gchar/games/base/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/base/moegirl.py` & `gchar-0.0.8/gchar/games/base/moegirl.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/base/name.py` & `gchar-0.0.8/gchar/games/base/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/base/property.py` & `gchar-0.0.8/gchar/games/base/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/dispatch/access.py` & `gchar-0.0.8/gchar/games/dispatch/access.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/character.py` & `gchar-0.0.8/gchar/games/fgo/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/danbooru_tags.json` & `gchar-0.0.8/gchar/games/fgo/danbooru_tags.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/index.json` & `gchar-0.0.8/gchar/games/fgo/index.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/index.py` & `gchar-0.0.8/gchar/games/fgo/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/name.py` & `gchar-0.0.8/gchar/games/fgo/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/pixiv_alias.yaml` & `gchar-0.0.8/gchar/games/fgo/pixiv_alias.yaml`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/pixiv_characters.json` & `gchar-0.0.8/gchar/games/fgo/pixiv_characters.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/pixiv_names.json` & `gchar-0.0.8/gchar/games/fgo/pixiv_names.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/fgo/property.py` & `gchar-0.0.8/gchar/games/fgo/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/character.py` & `gchar-0.0.8/gchar/games/genshin/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/danbooru_tags.json` & `gchar-0.0.8/gchar/games/genshin/danbooru_tags.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/index.json` & `gchar-0.0.8/gchar/games/genshin/index.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/index.py` & `gchar-0.0.8/gchar/games/genshin/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/pixiv_characters.json` & `gchar-0.0.8/gchar/games/genshin/pixiv_characters.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/pixiv_names.json` & `gchar-0.0.8/gchar/games/genshin/pixiv_names.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/genshin/property.py` & `gchar-0.0.8/gchar/games/genshin/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/character.py` & `gchar-0.0.8/gchar/games/girlsfrontline/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/danbooru_tags.json` & `gchar-0.0.8/gchar/games/girlsfrontline/danbooru_tags.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/index.json` & `gchar-0.0.8/gchar/games/girlsfrontline/index.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/index.py` & `gchar-0.0.8/gchar/games/girlsfrontline/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/name.py` & `gchar-0.0.8/gchar/games/girlsfrontline/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/pixiv_characters.json` & `gchar-0.0.8/gchar/games/girlsfrontline/pixiv_characters.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/pixiv_names.json` & `gchar-0.0.8/gchar/games/girlsfrontline/pixiv_names.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/girlsfrontline/property.py` & `gchar-0.0.8/gchar/games/girlsfrontline/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/character.py` & `gchar-0.0.8/gchar/games/neuralcloud/character.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/danbooru_tags.json` & `gchar-0.0.8/gchar/games/neuralcloud/danbooru_tags.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/index.json` & `gchar-0.0.8/gchar/games/neuralcloud/index.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/index.py` & `gchar-0.0.8/gchar/games/neuralcloud/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/name.py` & `gchar-0.0.8/gchar/games/neuralcloud/name.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/pixiv_characters.json` & `gchar-0.0.8/gchar/games/neuralcloud/pixiv_characters.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/pixiv_names.json` & `gchar-0.0.8/gchar/games/neuralcloud/pixiv_names.json`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/games/neuralcloud/property.py` & `gchar-0.0.8/gchar/games/neuralcloud/property.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/danbooru/__main__.py` & `gchar-0.0.8/gchar/resources/danbooru/__main__.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/danbooru/games.py` & `gchar-0.0.8/gchar/resources/danbooru/games.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/danbooru/index.py` & `gchar-0.0.8/gchar/resources/danbooru/index.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/danbooru/tag.py` & `gchar-0.0.8/gchar/resources/danbooru/tag.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/pixiv/__main__.py` & `gchar-0.0.8/gchar/resources/pixiv/__main__.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/pixiv/games.py` & `gchar-0.0.8/gchar/resources/pixiv/games.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/pixiv/keyword.py` & `gchar-0.0.8/gchar/resources/pixiv/keyword.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/pixiv/session.py` & `gchar-0.0.8/gchar/resources/pixiv/session.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/resources/pixiv/tag.py` & `gchar-0.0.8/gchar/resources/pixiv/tag.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/utils/cli.py` & `gchar-0.0.8/gchar/utils/cli.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/utils/compare.py` & `gchar-0.0.8/gchar/utils/compare.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/utils/download.py` & `gchar-0.0.8/gchar/utils/download.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/utils/huggingface.py` & `gchar-0.0.8/gchar/utils/huggingface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import time
 from hashlib import sha256, sha1
 
 import requests
-from huggingface_hub import hf_hub_url, HfApi
-from huggingface_hub.utils import HfHubHTTPError
 
 
 def hf_resource_check(local_filename, repo_id: str, file_in_repo: str, repo_type='model', revision='main',
                       chunk_for_hash: int = 1 << 20):
     response = requests.post(
         f"https://huggingface.co/api/{repo_type}s/{repo_id}/paths-info/{revision}",
         json={"paths": [file_in_repo]},
@@ -35,30 +33,33 @@
                 break
             sha.update(data)
 
     return sha.hexdigest() == oid
 
 
 def hf_file_exist(repo_id: str, file_in_repo: str, repo_type='model', revision='main'):
+    from huggingface_hub import hf_hub_url
     from .session import srequest, get_requests_session
     url = hf_hub_url(repo_id, file_in_repo, repo_type=repo_type, revision=revision)
     return srequest(get_requests_session(), 'HEAD', url, raise_for_status=False).ok
 
 
 def hf_need_upload(local_filename, repo_id: str, file_in_repo: str, repo_type='model', revision='main',
                    chunk_for_hash: int = 1 << 20, **kwargs):
+    from huggingface_hub import hf_hub_url
     _ = kwargs
     if requests.head(hf_hub_url(repo_id, file_in_repo, repo_type=repo_type, revision=revision)).ok:
         return not hf_resource_check(local_filename, repo_id, file_in_repo, repo_type, revision, chunk_for_hash)
     else:
         return True
 
 
-def hf_upload_file_if_need(api: HfApi, local_filename, path_in_repo: str, repo_id: str,
+def hf_upload_file_if_need(api, local_filename, path_in_repo: str, repo_id: str,
                            max_attempts: int = 10, wait_before_retry: int = 1, **kwargs):
+    from huggingface_hub.utils import HfHubHTTPError
     attempt = 0
     while True:
         attempt += 1
         try:
             if hf_need_upload(local_filename, repo_id, path_in_repo, **kwargs):
                 api.upload_file(
                     path_or_fileobj=local_filename,
```

### Comparing `gchar-0.0.7/gchar/utils/notebook.py` & `gchar-0.0.8/gchar/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar/utils/session.py` & `gchar-0.0.8/gchar/utils/session.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar.egg-info/PKG-INFO` & `gchar-0.0.8/gchar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gchar
-Version: 0.0.7
+Version: 0.0.8
 Summary: Game character manager.
 Home-page: https://github.com/narugo1992/gchar
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gchar-0.0.7/gchar.egg-info/SOURCES.txt` & `gchar-0.0.8/gchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/gchar.egg-info/requires.txt` & `gchar-0.0.8/gchar.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/setup.py` & `gchar-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `gchar-0.0.7/test/test_entry.py` & `gchar-0.0.8/test/test_entry.py`

 * *Files identical despite different names*

