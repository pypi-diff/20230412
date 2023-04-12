# Comparing `tmp/aomaker-2.2.0.tar.gz` & `tmp/aomaker-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aomaker-2.2.0.tar", last modified: Tue Apr 11 14:14:48 2023, max compression
+gzip compressed data, was "aomaker-2.2.1.tar", last modified: Wed Apr 12 10:31:21 2023, max compression
```

## Comparing `aomaker-2.2.0.tar` & `aomaker-2.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.484575 aomaker-2.2.0/
--rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.0/LICENSE
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       37 2022-11-30 11:05:04.000000 aomaker-2.2.0/MANIFEST.in
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-11 14:14:48.484382 aomaker-2.2.0/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.0/README.md
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.478322 aomaker-2.2.0/aomaker/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-04-09 15:54:39.000000 aomaker-2.2.0/aomaker/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9297 2023-04-10 15:50:41.000000 aomaker-2.2.0/aomaker/_aomaker.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.0/aomaker/_constants.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/_log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.0/aomaker/aomaker.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.479573 aomaker-2.2.0/aomaker/base/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/base/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.0/aomaker/base/base_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/base/base_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.0/aomaker/cache.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.0/aomaker/cli.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.480404 aomaker-2.2.0/aomaker/database/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/database/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.0/aomaker/database/base_db.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/database/mysql.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/database/sqlite.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.0/aomaker/exceptions.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.480537 aomaker-2.2.0/aomaker/extension/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/__init__.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.480846 aomaker-2.2.0/aomaker/extension/har_parse/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.0/aomaker/extension/har_parse/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/har_parse/har_parse.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.481401 aomaker-2.2.0/aomaker/extension/recording/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.0/aomaker/extension/recording/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/recording/addons.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/extension/recording/recording.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/field.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3000 2023-03-23 05:16:42.000000 aomaker-2.2.0/aomaker/fixture.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.0/aomaker/hook_manager.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.482295 aomaker-2.2.0/aomaker/html/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.0/aomaker/html/heading.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.0/aomaker/html/report.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2022-12-22 09:57:22.000000 aomaker-2.2.0/aomaker/html/template.html
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.0/aomaker/log.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/make.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/make_api.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/make_testcase.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/models.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.0/aomaker/param_types.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/path.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     3002 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8814 2023-04-10 03:38:53.000000 aomaker-2.2.0/aomaker/runner.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.0/aomaker/scaffold.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.483012 aomaker-2.2.0/aomaker/send_msg/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/send_msg/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/send_msg/wechat.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/swagger2yaml.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/template.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.483874 aomaker-2.2.0/aomaker/utils/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/utils/__init__.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     9343 2023-02-01 03:18:54.000000 aomaker-2.2.0/aomaker/utils/gen_allure_report.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.0/aomaker/utils/utils.py
--rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.0/aomaker/yaml2case.py
-drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-11 14:14:48.479056 aomaker-2.2.0/aomaker.egg-info/
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/PKG-INFO
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1329 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/entry_points.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/requires.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-04-11 14:14:48.000000 aomaker-2.2.0/aomaker.egg-info/top_level.txt
--rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-04-11 14:14:48.484629 aomaker-2.2.0/setup.cfg
--rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-04-09 15:54:39.000000 aomaker-2.2.0/setup.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.934692 aomaker-2.2.1/
+-rw-r-----   0 zhanglinsen   (501) staff       (20)    11509 2022-11-30 11:05:02.000000 aomaker-2.2.1/LICENSE
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       37 2022-11-30 11:05:04.000000 aomaker-2.2.1/MANIFEST.in
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-12 10:31:21.934559 aomaker-2.2.1/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      607 2022-11-03 10:41:01.000000 aomaker-2.2.1/README.md
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.929968 aomaker-2.2.1/aomaker/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1426 2023-04-12 10:31:01.000000 aomaker-2.2.1/aomaker/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9285 2023-04-12 10:30:39.000000 aomaker-2.2.1/aomaker/_aomaker.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      794 2023-04-10 14:08:17.000000 aomaker-2.2.1/aomaker/_constants.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2356 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/_log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      237 2023-04-10 15:38:20.000000 aomaker-2.2.1/aomaker/aomaker.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.931193 aomaker-2.2.1/aomaker/base/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/base/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4395 2023-04-10 14:57:25.000000 aomaker-2.2.1/aomaker/base/base_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3296 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/base/base_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     6167 2023-04-10 07:53:59.000000 aomaker-2.2.1/aomaker/cache.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9697 2023-03-23 05:48:22.000000 aomaker-2.2.1/aomaker/cli.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.931890 aomaker-2.2.1/aomaker/database/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/database/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1654 2023-03-24 06:30:20.000000 aomaker-2.2.1/aomaker/database/base_db.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1059 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/database/mysql.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2734 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/database/sqlite.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1394 2022-12-05 05:36:42.000000 aomaker-2.2.1/aomaker/exceptions.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.932012 aomaker-2.2.1/aomaker/extension/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        0 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/__init__.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.932297 aomaker-2.2.1/aomaker/extension/har_parse/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2284 2023-03-22 14:18:38.000000 aomaker-2.2.1/aomaker/extension/har_parse/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    10792 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/har_parse/har_parse.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.932812 aomaker-2.2.1/aomaker/extension/recording/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4517 2023-03-21 15:15:18.000000 aomaker-2.2.1/aomaker/extension/recording/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      170 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/recording/addons.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5679 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/extension/recording/recording.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1276 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/field.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3000 2023-03-23 05:16:42.000000 aomaker-2.2.1/aomaker/fixture.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      965 2023-03-22 10:18:59.000000 aomaker-2.2.1/aomaker/hook_manager.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.933369 aomaker-2.2.1/aomaker/html/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9937 2022-12-22 09:57:22.000000 aomaker-2.2.1/aomaker/html/heading.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     4302 2022-12-22 09:57:22.000000 aomaker-2.2.1/aomaker/html/report.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    11555 2022-12-22 09:57:22.000000 aomaker-2.2.1/aomaker/html/template.html
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3816 2023-03-22 11:04:05.000000 aomaker-2.2.1/aomaker/log.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1476 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/make.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7940 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/make_api.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1216 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/make_testcase.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     2118 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/models.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      450 2023-03-16 15:19:31.000000 aomaker-2.2.1/aomaker/param_types.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      691 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/path.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     3002 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8814 2023-04-10 03:38:53.000000 aomaker-2.2.1/aomaker/runner.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8576 2023-04-10 14:08:17.000000 aomaker-2.2.1/aomaker/scaffold.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.933719 aomaker-2.2.1/aomaker/send_msg/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/send_msg/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     8329 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/send_msg/wechat.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     7672 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/swagger2yaml.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9148 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/template.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.934183 aomaker-2.2.1/aomaker/utils/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       19 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/utils/__init__.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     9343 2023-02-01 03:18:54.000000 aomaker-2.2.1/aomaker/utils/gen_allure_report.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     5120 2023-02-02 04:06:40.000000 aomaker-2.2.1/aomaker/utils/utils.py
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)    16987 2022-11-03 10:41:01.000000 aomaker-2.2.1/aomaker/yaml2case.py
+drwxr-xr-x   0 zhanglinsen   (501) staff       (20)        0 2023-04-12 10:31:21.930641 aomaker-2.2.1/aomaker.egg-info/
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1038 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1329 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        1 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      154 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)      173 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/requires.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)        8 2023-04-12 10:31:21.000000 aomaker-2.2.1/aomaker.egg-info/top_level.txt
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)       38 2023-04-12 10:31:21.934736 aomaker-2.2.1/setup.cfg
+-rw-r--r--   0 zhanglinsen   (501) staff       (20)     1282 2023-04-12 10:31:01.000000 aomaker-2.2.1/setup.py
```

### Comparing `aomaker-2.2.0/LICENSE` & `aomaker-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/PKG-INFO` & `aomaker-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.2.0
+Version: 2.2.1
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.2.0/README.md` & `aomaker-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/__init__.py` & `aomaker-2.2.1/aomaker/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from emoji import emojize
 
-__version__ = "2.2.0"
+__version__ = "2.2.1"
 __description__ = "Quickly Arrange,Quickly Test!"
 __image__ = emojize(fr"""
               :----.                                                             ::::
              .------            .:::::::::::::::::::::::::::::::::::::::::::::. :---:  ::::::::::::::::::::::::::
             .---::--:                                                           ----
             ----  :--:          ..::::.      :.:..::::  .::::     ..:::. .:::  :---: ...:.    .::::.     .:.:..::
            :---    :::        .---------:   :-----------------   :----------:  ----.:---:   :---::---:   -------:
```

### Comparing `aomaker-2.2.0/aomaker/_aomaker.py` & `aomaker-2.2.1/aomaker/_aomaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         @wraps(func)
         def wrapper(*args, **kwargs):
             resp = func(*args, **kwargs)
             api_name = func.__name__
             if cache.get(var_name):
                 logger.info(f"==========cache变量<{var_name}>开始更新==========")
                 api_info = cache.get(var_name, select_field="api_info")
-                dependence_res = _call_dependence_for_update(json.loads(api_info), *out_args, **out_kwargs)
+                dependence_res = _call_dependence_for_update(api_info, *out_args, **out_kwargs)
                 cache.update(var_name, dependence_res)
                 logger.info(f"==========<{api_name}>cache更新<{api_info.get('name')}>结束==========")
             return resp
 
         return wrapper
 
     return decorator
```

### Comparing `aomaker-2.2.0/aomaker/_constants.py` & `aomaker-2.2.1/aomaker/_constants.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/_log.py` & `aomaker-2.2.1/aomaker/_log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/base/base_api.py` & `aomaker-2.2.1/aomaker/base/base_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/base/base_testcase.py` & `aomaker-2.2.1/aomaker/base/base_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/cache.py` & `aomaker-2.2.1/aomaker/cache.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/cli.py` & `aomaker-2.2.1/aomaker/cli.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/database/base_db.py` & `aomaker-2.2.1/aomaker/database/base_db.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/database/mysql.py` & `aomaker-2.2.1/aomaker/database/mysql.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/database/sqlite.py` & `aomaker-2.2.1/aomaker/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/exceptions.py` & `aomaker-2.2.1/aomaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/extension/har_parse/__init__.py` & `aomaker-2.2.1/aomaker/extension/har_parse/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/extension/har_parse/har_parse.py` & `aomaker-2.2.1/aomaker/extension/har_parse/har_parse.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/extension/recording/__init__.py` & `aomaker-2.2.1/aomaker/extension/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/extension/recording/recording.py` & `aomaker-2.2.1/aomaker/extension/recording/recording.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/field.py` & `aomaker-2.2.1/aomaker/field.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/fixture.py` & `aomaker-2.2.1/aomaker/fixture.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/hook_manager.py` & `aomaker-2.2.1/aomaker/hook_manager.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/html/heading.html` & `aomaker-2.2.1/aomaker/html/heading.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/html/report.html` & `aomaker-2.2.1/aomaker/html/report.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/html/template.html` & `aomaker-2.2.1/aomaker/html/template.html`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/log.py` & `aomaker-2.2.1/aomaker/log.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/make.py` & `aomaker-2.2.1/aomaker/make.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/make_api.py` & `aomaker-2.2.1/aomaker/make_api.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/make_testcase.py` & `aomaker-2.2.1/aomaker/make_testcase.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/models.py` & `aomaker-2.2.1/aomaker/models.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/path.py` & `aomaker-2.2.1/aomaker/path.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/report.py` & `aomaker-2.2.1/aomaker/report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/runner.py` & `aomaker-2.2.1/aomaker/runner.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/scaffold.py` & `aomaker-2.2.1/aomaker/scaffold.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/send_msg/wechat.py` & `aomaker-2.2.1/aomaker/send_msg/wechat.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/swagger2yaml.py` & `aomaker-2.2.1/aomaker/swagger2yaml.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/template.py` & `aomaker-2.2.1/aomaker/template.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/utils/gen_allure_report.py` & `aomaker-2.2.1/aomaker/utils/gen_allure_report.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/utils/utils.py` & `aomaker-2.2.1/aomaker/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker/yaml2case.py` & `aomaker-2.2.1/aomaker/yaml2case.py`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/aomaker.egg-info/PKG-INFO` & `aomaker-2.2.1/aomaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aomaker
-Version: 2.2.0
+Version: 2.2.1
 Summary: An api testing framework
 Home-page: https://github.com/ae86sen/aomaker
 Author: ancientone
 Author-email: listeningsss@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aomaker-2.2.0/aomaker.egg-info/SOURCES.txt` & `aomaker-2.2.1/aomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aomaker-2.2.0/setup.py` & `aomaker-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # --coding:utf-8--
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="aomaker",
-    version="2.2.0",
+    version="2.2.1",
     author="ancientone",
     author_email="listeningsss@163.com",
     description="An api testing framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ae86sen/aomaker",
     packages=setuptools.find_packages(),
```

