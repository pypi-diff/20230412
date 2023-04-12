# Comparing `tmp/splight-lib-2.2.4.tar.gz` & `tmp/splight-lib-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.2.4.tar", last modified: Mon Apr 10 22:04:45 2023, max compression
+gzip compressed data, was "splight-lib-2.2.5.tar", last modified: Wed Apr 12 14:35:08 2023, max compression
```

## Comparing `splight-lib-2.2.4.tar` & `splight-lib-2.2.5.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.648274 splight-lib-2.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.000000 splight-lib-2.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 22:04:45.648274 splight-lib-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-10 22:04:45.000000 splight-lib-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-10 22:04:45.000000 splight-lib-2.2.4/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 22:04:45.648274 splight-lib-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-10 22:04:45.000000 splight-lib-2.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.632274 splight-lib-2.2.4/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.636273 splight-lib-2.2.4/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.640274 splight-lib-2.2.4/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.640274 splight-lib-2.2.4/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.640274 splight-lib-2.2.4/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.640274 splight-lib-2.2.4/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.640274 splight-lib-2.2.4/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.644274 splight-lib-2.2.4/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.644274 splight-lib-2.2.4/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.644274 splight-lib-2.2.4/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.644274 splight-lib-2.2.4/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.644274 splight-lib-2.2.4/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.644274 splight-lib-2.2.4/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/restclient/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.640274 splight-lib-2.2.4/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.648274 splight-lib-2.2.4/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 22:04:45.648274 splight-lib-2.2.4/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-10 22:04:45.000000 splight-lib-2.2.4/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:07.000000 splight-lib-2.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 14:35:08.745650 splight-lib-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-12 14:35:07.000000 splight-lib-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-12 14:35:07.000000 splight-lib-2.2.5/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:35:08.745650 splight-lib-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 14:35:07.000000 splight-lib-2.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.737650 splight-lib-2.2.5/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/restclient/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.741650 splight-lib-2.2.5/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-12 14:35:08.000000 splight-lib-2.2.5/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-12 14:35:08.000000 splight-lib-2.2.5/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:35:08.000000 splight-lib-2.2.5/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:35:08.000000 splight-lib-2.2.5/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 14:35:08.000000 splight-lib-2.2.5/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 14:35:08.000000 splight-lib-2.2.5/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:35:08.745650 splight-lib-2.2.5/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-12 14:35:07.000000 splight-lib-2.2.5/splight_models/webhook.py
```

### Comparing `splight-lib-2.2.4/PKG-INFO` & `splight-lib-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.4
+Version: 2.2.5
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 License-File: LICENSE.txt
```

### Comparing `splight-lib-2.2.4/remote_splight_lib/communication/client.py` & `splight-lib-2.2.5/remote_splight_lib/communication/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/remote_splight_lib/database/classmap.py` & `splight-lib-2.2.5/remote_splight_lib/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/remote_splight_lib/database/client.py` & `splight-lib-2.2.5/remote_splight_lib/database/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/remote_splight_lib/datalake/client.py` & `splight-lib-2.2.5/remote_splight_lib/datalake/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/remote_splight_lib/hub/client.py` & `splight-lib-2.2.5/remote_splight_lib/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/remote_splight_lib/settings.py` & `splight-lib-2.2.5/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/setup.py` & `splight-lib-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 dependency_links = [
     # External repoitories different from pypi
 ]
 
 setup(
     name='splight-lib',
-    version='2.2.4',
+    version='2.2.5',
     author='Splight',
     author_email='factory@splight-ae.com',
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.2.4/splight_abstract/auth/abstract.py` & `splight-lib-2.2.5/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/auth/exceptions.py` & `splight-lib-2.2.5/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/cache/abstract.py` & `splight-lib-2.2.5/splight_abstract/cache/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/client/abstract.py` & `splight-lib-2.2.5/splight_abstract/client/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/client/filter.py` & `splight-lib-2.2.5/splight_abstract/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/client/hooks.py` & `splight-lib-2.2.5/splight_abstract/client/hooks.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/communication/abstract.py` & `splight-lib-2.2.5/splight_abstract/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/database/abstract.py` & `splight-lib-2.2.5/splight_abstract/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/datalake/abstract.py` & `splight-lib-2.2.5/splight_abstract/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/deployment/abstract.py` & `splight-lib-2.2.5/splight_abstract/deployment/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/endpoints/__init__.py` & `splight-lib-2.2.5/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/hub/abstract.py` & `splight-lib-2.2.5/splight_abstract/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_abstract/storage/abstract.py` & `splight-lib-2.2.5/splight_abstract/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/auth/mac_auth.py` & `splight-lib-2.2.5/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/database/classmap.py` & `splight-lib-2.2.5/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/database/local_client.py` & `splight-lib-2.2.5/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/database/remote_client.py` & `splight-lib-2.2.5/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/datalake/local_client.py` & `splight-lib-2.2.5/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.2.5/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/exceptions.py` & `splight-lib-2.2.5/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/file_handler.py` & `splight-lib-2.2.5/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/filter.py` & `splight-lib-2.2.5/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/client/settings.py` & `splight-lib-2.2.5/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/component/abstract.py` & `splight-lib-2.2.5/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/encryption.py` & `splight-lib-2.2.5/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/execution.py` & `splight-lib-2.2.5/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/logging.py` & `splight-lib-2.2.5/splight_lib/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/restclient/client.py` & `splight-lib-2.2.5/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/restclient/exceptions.py` & `splight-lib-2.2.5/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/restclient/types.py` & `splight-lib-2.2.5/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/settings.py` & `splight-lib-2.2.5/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib/webhook.py` & `splight-lib-2.2.5/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.2.5/splight_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.2.4
+Version: 2.2.5
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 License-File: LICENSE.txt
```

### Comparing `splight-lib-2.2.4/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.2.5/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/__init__.py` & `splight-lib-2.2.5/splight_models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/alert.py` & `splight-lib-2.2.5/splight_models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/blockchain.py` & `splight-lib-2.2.5/splight_models/blockchain.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/communication/context.py` & `splight-lib-2.2.5/splight_models/communication/context.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/communication/events.py` & `splight-lib-2.2.5/splight_models/communication/events.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/component.py` & `splight-lib-2.2.5/splight_models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/constants.py` & `splight-lib-2.2.5/splight_models/constants.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/datalake.py` & `splight-lib-2.2.5/splight_models/datalake.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/deployment.py` & `splight-lib-2.2.5/splight_models/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/exception.py` & `splight-lib-2.2.5/splight_models/exception.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/file.py` & `splight-lib-2.2.5/splight_models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/graph.py` & `splight-lib-2.2.5/splight_models/graph.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/hub.py` & `splight-lib-2.2.5/splight_models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/notification.py` & `splight-lib-2.2.5/splight_models/notification.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/query.py` & `splight-lib-2.2.5/splight_models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/setpoint.py` & `splight-lib-2.2.5/splight_models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/user.py` & `splight-lib-2.2.5/splight_models/user.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/variable.py` & `splight-lib-2.2.5/splight_models/variable.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.2.4/splight_models/webhook.py` & `splight-lib-2.2.5/splight_models/webhook.py`

 * *Files identical despite different names*

