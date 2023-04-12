# Comparing `tmp/code42cli-1.8.1.tar.gz` & `tmp/code42cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code42cli-1.8.1.tar", last modified: Wed Jul 14 15:51:05 2021, max compression
+gzip compressed data, was "code42cli-1.9.0.tar", last modified: Thu Aug 19 19:04:45 2021, max compression
```

## Comparing `code42cli-1.8.1.tar` & `code42cli-1.9.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.277141 code42cli-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)    22734 2021-07-14 15:50:54.000000 code42cli-1.8.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-07-14 15:50:54.000000 code42cli-1.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-07-14 15:50:54.000000 code42cli-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12323 2021-07-14 15:51:05.277141 code42cli-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9096 2021-07-14 15:50:54.000000 code42cli-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-07-14 15:51:05.277141 code42cli-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-07-14 15:50:54.000000 code42cli-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.269142 code42cli-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6125 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli/click_ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/click_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/click_ext/groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/click_ext/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     4920 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/click_ext/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/alert_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)    12310 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/alerts.py
--rw-r--r--   0 runner    (1001) docker     (121)     7966 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/auditlogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9161 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/cases.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/departing_employee.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli/cmds/detectionlists/
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/detectionlists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/detectionlists/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    20159 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     6444 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/high_risk_employee.py
--rw-r--r--   0 runner    (1001) docker     (121)     9149 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/legal_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)     6503 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli/cmds/search/
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/search/cursor_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     5761 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/search/extraction.py
--rw-r--r--   0 runner    (1001) docker     (121)     5831 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/search/options.py
--rw-r--r--   0 runner    (1001) docker     (121)    12356 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/securitydata.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/shared.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     9790 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/cmds/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/date_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/file_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.277141 code42cli-1.8.1/src/code42cli/logger/
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/logger/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     4861 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/logger/formatters.py
--rw-r--r--   0 runner    (1001) docker     (121)     5233 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/logger/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/maps.py
--rw-r--r--   0 runner    (1001) docker     (121)     6084 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     6473 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/output_formats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/password.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/sdk_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5729 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     4745 2021-07-14 15:50:54.000000 code42cli-1.8.1/src/code42cli/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-14 15:51:05.273141 code42cli-1.8.1/src/code42cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12323 2021-07-14 15:51:04.000000 code42cli-1.8.1/src/code42cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2021-07-14 15:51:05.000000 code42cli-1.8.1/src/code42cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 15:51:04.000000 code42cli-1.8.1/src/code42cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-07-14 15:51:04.000000 code42cli-1.8.1/src/code42cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-14 15:51:04.000000 code42cli-1.8.1/src/code42cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      258 2021-07-14 15:51:04.000000 code42cli-1.8.1/src/code42cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-07-14 15:51:04.000000 code42cli-1.8.1/src/code42cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-07-14 15:50:54.000000 code42cli-1.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.094608 code42cli-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    23529 2021-08-19 19:04:34.000000 code42cli-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-08-19 19:04:34.000000 code42cli-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-08-19 19:04:34.000000 code42cli-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    12323 2021-08-19 19:04:45.094608 code42cli-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9096 2021-08-19 19:04:34.000000 code42cli-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2021-08-19 19:04:45.094608 code42cli-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-08-19 19:04:34.000000 code42cli-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.086608 code42cli-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6125 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli/click_ext/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/click_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5382 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/click_ext/groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/click_ext/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5401 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/click_ext/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5683 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/alert_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12310 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7966 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/auditlogs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9161 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/cases.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5261 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/departing_employee.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli/cmds/detectionlists/
+-rw-r--r--   0 runner    (1001) docker     (121)     3216 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/detectionlists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/detectionlists/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20159 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6444 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/high_risk_employee.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9149 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/legal_hold.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6850 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli/cmds/search/
+-rw-r--r--   0 runner    (1001) docker     (121)     1589 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3449 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/search/cursor_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5761 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/search/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5831 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/search/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17722 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/securitydata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/shared.py
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/shell.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9790 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/cmds/users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5492 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/date_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2680 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/file_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.094608 code42cli-1.9.0/src/code42cli/logger/
+-rw-r--r--   0 runner    (1001) docker     (121)     4391 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/logger/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4861 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/logger/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5233 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/logger/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2176 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/maps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6148 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6473 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/output_formats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1297 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/password.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/sdk_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5729 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4745 2021-08-19 19:04:34.000000 code42cli-1.9.0/src/code42cli/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-19 19:04:45.090608 code42cli-1.9.0/src/code42cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12323 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-08-19 19:04:44.000000 code42cli-1.9.0/src/code42cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-08-19 19:04:34.000000 code42cli-1.9.0/tox.ini
```

### Comparing `code42cli-1.8.1/CHANGELOG.md` & `code42cli-1.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,34 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 The intended audience of this file is for py42 consumers -- as such, changes that don't affect
 how a consumer would use the library (e.g. adding unit tests, updating documentation, etc) are not captured here.
 
+## 1.9.0 - 2021-08-19
+
+### Added
+
+- `code42 profile` commands that validate passwords (`create`, `update`, `reset-pw`) now have the `--debug` option available, and `create` and `update` can now also pass in `--totp` as an option.
+
+- New command options for `code42 security-data search`
+    - `--risk-indicator` to filter events by risk indicators.
+    - `--risk-severity` to filter events by risk severity.
+
+### Changed
+
+- A TOTP token is now required on `code42 profile` commands that check for password validity when a user has MFA enabled.
+
+- Updated minimum version of py42 to `1.18.0` to provide access to `FIRST_DESTINATION_USE` and `RARE_DESTINATION_USE` search filters.
+
+### Fixed
+
+- `code42 profile delete` command now prints a clear error message when deletion target doesn't exist.
+
 ## 1.8.1 - 2021-07-14
 
 ### Fixed
 
 - The `chardet` library is now an explicit dependency, resolving dependency issues for fresh installations using latest `requests` v.2.26.0
 
 ## 1.8.0 - 2021-07-08
```

### Comparing `code42cli-1.8.1/LICENSE.md` & `code42cli-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/PKG-INFO` & `code42cli-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code42cli
-Version: 1.8.1
+Version: 1.9.0
 Summary: The official command line tool for interacting with Code42
 Home-page: https://github.com/code42/py42
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/code42/code42cli/issues
 Project-URL: Documentation, https://clidocs.code42.com/
 Project-URL: Source Code, https://github.com/code42/code42cli
 Description: # The Code42 CLI
```

### Comparing `code42cli-1.8.1/README.md` & `code42cli-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/setup.py` & `code42cli-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     long_description_content_type="text/markdown",
     packages=find_packages("src"),
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
     python_requires=">3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, <4",
     install_requires=[
-        "chardet>=4.0.0",
+        "chardet",
         "click>=7.1.1, <8",
         "click_plugins>=1.1.1",
         "colorama>=0.4.3",
         "c42eventextractor==0.4.1",
         "keyring==18.0.1",
         "keyrings.alt==3.2.0",
         "ipython>=7.16.1",
         "pandas>=1.1.3",
-        "py42>=1.16.0",
+        "py42>=1.18.0",
     ],
     extras_require={
         "dev": [
             "flake8==3.8.3",
             "pytest==4.6.11",
             "pytest-cov==2.10.0",
             "pytest-mock==2.0.0",
```

### Comparing `code42cli-1.8.1/src/code42cli/bulk.py` & `code42cli-1.9.0/src/code42cli/bulk.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/click_ext/groups.py` & `code42cli-1.9.0/src/code42cli/click_ext/groups.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/click_ext/options.py` & `code42cli-1.9.0/src/code42cli/click_ext/options.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/click_ext/types.py` & `code42cli-1.9.0/src/code42cli/click_ext/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,8 +143,26 @@
     def __init__(self, choices, extras_map, **kwargs):
         self.extras_map = extras_map
         super().__init__(choices, **kwargs)
 
     def convert(self, value, param, ctx):
         if value in self.extras_map:
             value = self.extras_map[value]
+
         return super().convert(value, param, ctx)
+
+
+class TOTP(click.ParamType):
+    """Validates param to be a 6-digit integer, which is what all Code42 TOTP tokens will be."""
+
+    def get_metavar(self, param):
+        return "TEXT"
+
+    def convert(self, value, param, ctx):
+        try:
+            int(value)
+            assert len(value) == 6
+            return value
+        except Exception:
+            raise BadParameter(
+                f"TOTP tokens should be a 6-digit integer. '{value}' was provided."
+            )
```

### Comparing `code42cli-1.8.1/src/code42cli/cmds/alert_rules.py` & `code42cli-1.9.0/src/code42cli/cmds/alert_rules.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/alerts.py` & `code42cli-1.9.0/src/code42cli/cmds/alerts.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/auditlogs.py` & `code42cli-1.9.0/src/code42cli/cmds/auditlogs.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/cases.py` & `code42cli-1.9.0/src/code42cli/cmds/cases.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/departing_employee.py` & `code42cli-1.9.0/src/code42cli/cmds/departing_employee.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/detectionlists/__init__.py` & `code42cli-1.9.0/src/code42cli/cmds/detectionlists/__init__.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/devices.py` & `code42cli-1.9.0/src/code42cli/cmds/devices.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/high_risk_employee.py` & `code42cli-1.9.0/src/code42cli/cmds/high_risk_employee.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/legal_hold.py` & `code42cli-1.9.0/src/code42cli/cmds/legal_hold.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/profile.py` & `code42cli-1.9.0/src/code42cli/cmds/profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from getpass import getpass
 
 import click
 from click import echo
 from click import secho
-from py42.exceptions import Py42MFARequiredError
 
 import code42cli.profile as cliprofile
+from code42cli.click_ext.types import TOTP
 from code42cli.errors import Code42CLIError
 from code42cli.options import yes_option
 from code42cli.profile import CREATE_PROFILE_HELP
 from code42cli.sdk_client import create_sdk
 from code42cli.util import does_user_agree
 
 
 @click.group()
 def profile():
     """Manage Code42 connection settings."""
     pass
 
 
+debug_option = click.option(
+    "-d", "--debug", is_flag=True, help="Turn on debug logging.",
+)
+totp_option = click.option(
+    "--totp", help="TOTP token for multi-factor authentication.", type=TOTP()
+)
+
+
 def profile_name_arg(required=False):
     return click.argument("profile_name", required=required)
 
 
 def name_option(required=False):
     return click.option(
         "-n",
@@ -81,59 +89,63 @@
 
 
 @profile.command()
 @name_option(required=True)
 @server_option(required=True)
 @username_option(required=True)
 @password_option
+@totp_option
 @yes_option(hidden=True)
 @disable_ssl_option
-def create(name, server, username, password, disable_ssl_errors):
+@debug_option
+def create(name, server, username, password, disable_ssl_errors, debug, totp):
     """Create profile settings. The first profile created will be the default."""
     cliprofile.create_profile(name, server, username, disable_ssl_errors)
+    password = password or _prompt_for_password(name)
     if password:
-        _set_pw(name, password)
-    else:
-        _prompt_for_allow_password_set(name)
+        _set_pw(name, password, debug, totp=totp)
     echo(f"Successfully created profile '{name}'.")
 
 
 @profile.command()
 @name_option()
 @server_option()
 @username_option()
 @password_option
+@totp_option
 @disable_ssl_option
-def update(name, server, username, password, disable_ssl_errors):
+@debug_option
+def update(name, server, username, password, disable_ssl_errors, debug, totp):
     """Update an existing profile."""
     c42profile = cliprofile.get_profile(name)
 
     if not server and not username and not password and disable_ssl_errors is None:
         raise click.UsageError(
             "Must provide at least one of `--username`, `--server`, `--password`, or "
             "`--disable-ssl-errors` when updating a profile."
         )
 
     cliprofile.update_profile(c42profile.name, server, username, disable_ssl_errors)
+    if not password and not c42profile.has_stored_password:
+        password = _prompt_for_password(c42profile.name)
     if password:
-        _set_pw(name, password)
-    elif not c42profile.has_stored_password:
-        _prompt_for_allow_password_set(c42profile.name)
+        _set_pw(name, password, debug, totp=totp)
 
     echo(f"Profile '{c42profile.name}' has been updated.")
 
 
 @profile.command()
 @profile_name_arg()
-def reset_pw(profile_name):
+@debug_option
+def reset_pw(profile_name, debug):
     """\b
     Change the stored password for a profile. Only affects what's stored in the local profile,
     does not make any changes to the Code42 user account."""
     password = getpass()
-    profile_name_saved = _set_pw(profile_name, password)
+    profile_name_saved = _set_pw(profile_name, password, debug)
     echo(f"Password updated for profile '{profile_name_saved}'.")
 
 
 @profile.command("list")
 def _list():
     """Show all existing stored profiles."""
     profiles = cliprofile.get_all_profiles()
@@ -152,14 +164,18 @@
 
 
 @profile.command()
 @yes_option()
 @profile_name_arg(required=True)
 def delete(profile_name):
     """Deletes a profile and its stored password (if any)."""
+    try:
+        cliprofile.get_profile(profile_name)
+    except Code42CLIError:
+        raise Code42CLIError(f"Profile '{profile_name}' does not exist.")
     message = (
         "\nDeleting this profile will also delete any stored passwords and checkpoints. "
         "Are you sure? (y/n): "
     )
     if cliprofile.is_default_profile(profile_name):
         message = f"\n'{profile_name}' is currently the default profile!\n{message}"
     if does_user_agree(message):
@@ -184,26 +200,22 @@
             for profile_obj in existing_profiles:
                 cliprofile.delete_profile(profile_obj.name)
                 echo(f"Profile '{profile_obj.name}' has been deleted.")
     else:
         echo("\nNo profiles exist. Nothing to delete.")
 
 
-def _prompt_for_allow_password_set(profile_name):
+def _prompt_for_password(profile_name):
     if does_user_agree("Would you like to set a password? (y/n): "):
         password = getpass()
-        _set_pw(profile_name, password)
+        return password
 
 
-def _set_pw(profile_name, password):
+def _set_pw(profile_name, password, debug, totp=None):
     c42profile = cliprofile.get_profile(profile_name)
     try:
-        create_sdk(c42profile, is_debug_mode=False, password=password)
-    except Py42MFARequiredError:
-        echo(
-            "Multi-factor account detected. `--totp <token>` option will be required for all code42 invocations."
-        )
+        create_sdk(c42profile, is_debug_mode=debug, password=password, totp=totp)
     except Exception:
         secho("Password not stored!", bold=True)
         raise
     cliprofile.set_password(password, c42profile.name)
     return c42profile.name
```

### Comparing `code42cli-1.8.1/src/code42cli/cmds/search/__init__.py` & `code42cli-1.9.0/src/code42cli/cmds/search/__init__.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/search/cursor_store.py` & `code42cli-1.9.0/src/code42cli/cmds/search/cursor_store.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/search/extraction.py` & `code42cli-1.9.0/src/code42cli/cmds/search/extraction.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/search/options.py` & `code42cli-1.9.0/src/code42cli/cmds/search/options.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/securitydata.py` & `code42cli-1.9.0/src/code42cli/cmds/securitydata.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import click
 import py42.sdk.queries.fileevents.filters as f
 from c42eventextractor.extractors import FileEventExtractor
 from click import echo
 from py42.sdk.queries.fileevents.filters.exposure_filter import ExposureType
 from py42.sdk.queries.fileevents.filters.file_filter import FileCategory
+from py42.sdk.queries.fileevents.filters.risk_filter import RiskIndicator
+from py42.sdk.queries.fileevents.filters.risk_filter import RiskSeverity
 
 import code42cli.cmds.search.extraction as ext
 import code42cli.cmds.search.options as searchopt
 import code42cli.errors as errors
 import code42cli.options as opt
 from code42cli.click_ext.groups import OrderedGroup
 from code42cli.click_ext.options import incompatible_with
@@ -139,14 +141,110 @@
 include_non_exposure_option = click.option(
     "--include-non-exposure",
     is_flag=True,
     callback=searchopt.exists_filter(f.ExposureType),
     cls=incompatible_with(["advanced_query", "type", "saved_search"]),
     help="Get all events including non-exposure events.",
 )
+risk_indicator_map = {
+    "PUBLIC_CORPORATE_BOX": RiskIndicator.CloudDataExposures.PUBLIC_CORPORATE_BOX,
+    "PUBLIC_CORPORATE_GOOGLE": RiskIndicator.CloudDataExposures.PUBLIC_CORPORATE_GOOGLE_DRIVE,
+    "PUBLIC_CORPORATE_ONEDRIVE": RiskIndicator.CloudDataExposures.PUBLIC_CORPORATE_ONEDRIVE,
+    "SENT_CORPORATE_GMAIL": RiskIndicator.CloudDataExposures.SENT_CORPORATE_GMAIL,
+    "SHARED_CORPORATE_BOX": RiskIndicator.CloudDataExposures.SHARED_CORPORATE_BOX,
+    "SHARED_CORPORATE_GOOGLE_DRIVE": RiskIndicator.CloudDataExposures.SHARED_CORPORATE_GOOGLE_DRIVE,
+    "SHARED_CORPORATE_ONEDRIVE": RiskIndicator.CloudDataExposures.SHARED_CORPORATE_ONEDRIVE,
+    "AMAZON_DRIVE": RiskIndicator.CloudStorageUploads.AMAZON_DRIVE,
+    "BOX": RiskIndicator.CloudStorageUploads.BOX,
+    "DROPBOX": RiskIndicator.CloudStorageUploads.DROPBOX,
+    "GOOGLE_DRIVE": RiskIndicator.CloudStorageUploads.GOOGLE_DRIVE,
+    "ICLOUD": RiskIndicator.CloudStorageUploads.ICLOUD,
+    "MEGA": RiskIndicator.CloudStorageUploads.MEGA,
+    "ONEDRIVE": RiskIndicator.CloudStorageUploads.ONEDRIVE,
+    "ZOHO": RiskIndicator.CloudStorageUploads.ZOHO,
+    "BITBUCKET": RiskIndicator.CodeRepositoryUploads.BITBUCKET,
+    "GITHUB": RiskIndicator.CodeRepositoryUploads.GITHUB,
+    "GITLAB": RiskIndicator.CodeRepositoryUploads.GITLAB,
+    "SOURCEFORGE": RiskIndicator.CodeRepositoryUploads.SOURCEFORGE,
+    "STASH": RiskIndicator.CodeRepositoryUploads.STASH,
+    "163.COM": RiskIndicator.EmailServiceUploads.ONESIXTHREE_DOT_COM,
+    "126.COM": RiskIndicator.EmailServiceUploads.ONETWOSIX_DOT_COM,
+    "AOL": RiskIndicator.EmailServiceUploads.AOL,
+    "COMCAST": RiskIndicator.EmailServiceUploads.COMCAST,
+    "GMAIL": RiskIndicator.EmailServiceUploads.GMAIL,
+    "ICLOUD_MAIL": RiskIndicator.EmailServiceUploads.ICLOUD,
+    "MAIL.COM": RiskIndicator.EmailServiceUploads.MAIL_DOT_COM,
+    "OUTLOOK": RiskIndicator.EmailServiceUploads.OUTLOOK,
+    "PROTONMAIL": RiskIndicator.EmailServiceUploads.PROTONMAIL,
+    "QQMAIL": RiskIndicator.EmailServiceUploads.QQMAIL,
+    "SINA_MAIL": RiskIndicator.EmailServiceUploads.SINA_MAIL,
+    "SOHU_MAIL": RiskIndicator.EmailServiceUploads.SOHU_MAIL,
+    "YAHOO": RiskIndicator.EmailServiceUploads.YAHOO,
+    "ZOHO_MAIL": RiskIndicator.EmailServiceUploads.ZOHO_MAIL,
+    "AIRDROP": RiskIndicator.ExternalDevices.AIRDROP,
+    "REMOVABLE_MEDIA": RiskIndicator.ExternalDevices.REMOVABLE_MEDIA,
+    "AUDIO": RiskIndicator.FileCategories.AUDIO,
+    "DOCUMENT": RiskIndicator.FileCategories.DOCUMENT,
+    "EXECUTABLE": RiskIndicator.FileCategories.EXECUTABLE,
+    "IMAGE": RiskIndicator.FileCategories.IMAGE,
+    "PDF": RiskIndicator.FileCategories.PDF,
+    "PRESENTATION": RiskIndicator.FileCategories.PRESENTATION,
+    "SCRIPT": RiskIndicator.FileCategories.SCRIPT,
+    "SOURCE_CODE": RiskIndicator.FileCategories.SOURCE_CODE,
+    "SPREADSHEET": RiskIndicator.FileCategories.SPREADSHEET,
+    "VIDEO": RiskIndicator.FileCategories.VIDEO,
+    "VIRTUAL_DISK_IMAGE": RiskIndicator.FileCategories.VIRTUAL_DISK_IMAGE,
+    "ZIP": RiskIndicator.FileCategories.ZIP,
+    "FACEBOOK_MESSENGER": RiskIndicator.MessagingServiceUploads.FACEBOOK_MESSENGER,
+    "MICROSOFT_TEAMS": RiskIndicator.MessagingServiceUploads.MICROSOFT_TEAMS,
+    "SLACK": RiskIndicator.MessagingServiceUploads.SLACK,
+    "WHATSAPP": RiskIndicator.MessagingServiceUploads.WHATSAPP,
+    "OTHER": RiskIndicator.Other.OTHER,
+    "UNKNOWN": RiskIndicator.Other.UNKNOWN,
+    "FACEBOOK": RiskIndicator.SocialMediaUploads.FACEBOOK,
+    "LINKEDIN": RiskIndicator.SocialMediaUploads.LINKEDIN,
+    "REDDIT": RiskIndicator.SocialMediaUploads.REDDIT,
+    "TWITTER": RiskIndicator.SocialMediaUploads.TWITTER,
+    "FILE_MISMATCH": RiskIndicator.UserBehavior.FILE_MISMATCH,
+    "OFF_HOURS": RiskIndicator.UserBehavior.OFF_HOURS,
+    "REMOTE": RiskIndicator.UserBehavior.REMOTE,
+    "FIRST_DESTINATION_USE": RiskIndicator.UserBehavior.FIRST_DESTINATION_USE,
+    "RARE_DESTINATION_USE": RiskIndicator.UserBehavior.RARE_DESTINATION_USE,
+}
+risk_indicator_map_reversed = {v: k for k, v in risk_indicator_map.items()}
+
+
+def risk_indicator_callback(filter_cls):
+    def callback(ctx, param, arg):
+        if arg:
+            mapped_args = tuple(risk_indicator_map[i] for i in arg)
+            filter_func = searchopt.is_in_filter(filter_cls)
+            return filter_func(ctx, param, mapped_args)
+
+    return callback
+
+
+risk_indicator_option = click.option(
+    "--risk-indicator",
+    multiple=True,
+    type=MapChoice(
+        choices=list(risk_indicator_map.keys()), extras_map=risk_indicator_map_reversed,
+    ),
+    callback=risk_indicator_callback(f.RiskIndicator),
+    cls=searchopt.AdvancedQueryAndSavedSearchIncompatible,
+    help="Limits events to those classified by the given risk indicator categories.",
+)
+risk_severity_option = click.option(
+    "--risk-severity",
+    multiple=True,
+    type=click.Choice(list(RiskSeverity.choices())),
+    callback=searchopt.is_in_filter(f.RiskSeverity),
+    cls=searchopt.AdvancedQueryAndSavedSearchIncompatible,
+    help="Limits events to those classified by the given risk severity.",
+)
 begin_option = opt.begin_option(
     SECURITY_DATA_KEYWORD,
     callback=lambda ctx, param, arg: convert_datetime_to_timestamp(
         limit_date_range(arg, max_days_back=90)
     ),
 )
 end_option = opt.end_option(SECURITY_DATA_KEYWORD)
@@ -182,14 +280,16 @@
         "eventType": "Type",
         "eventTimestamp": "EventTimestamp",
         "fileCategory": "FileCategory",
         "fileSize": "FileSize",
         "fileOwner": "FileOwner",
         "md5Checksum": "MD5Checksum",
         "sha256Checksum": "SHA256Checksum",
+        "riskIndicators": "RiskIndicator",
+        "riskSeverity": "RiskSeverity",
     }
 
 
 def search_options(f):
     f = checkpoint_option(f)
     f = advanced_query_option(f)
     f = end_option(f)
@@ -206,14 +306,16 @@
     f = source_option(f)
     f = file_name_option(f)
     f = file_path_option(f)
     f = file_category_option(f)
     f = process_owner_option(f)
     f = tab_url_option(f)
     f = include_non_exposure_option(f)
+    f = risk_indicator_option(f)
+    f = risk_severity_option(f)
     f = _get_saved_search_option()(f)
     return f
 
 
 @click.group(cls=OrderedGroup)
 @sdk_options(hidden=True)
 def security_data(state):
```

### Comparing `code42cli-1.8.1/src/code42cli/cmds/shared.py` & `code42cli-1.9.0/src/code42cli/cmds/shared.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/cmds/users.py` & `code42cli-1.9.0/src/code42cli/cmds/users.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/config.py` & `code42cli-1.9.0/src/code42cli/config.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/date_helper.py` & `code42cli-1.9.0/src/code42cli/date_helper.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/errors.py` & `code42cli-1.9.0/src/code42cli/errors.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/extensions/__init__.py` & `code42cli-1.9.0/src/code42cli/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/file_readers.py` & `code42cli-1.9.0/src/code42cli/file_readers.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/logger/__init__.py` & `code42cli-1.9.0/src/code42cli/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/logger/formatters.py` & `code42cli-1.9.0/src/code42cli/logger/formatters.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/logger/handlers.py` & `code42cli-1.9.0/src/code42cli/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/main.py` & `code42cli-1.9.0/src/code42cli/main.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/maps.py` & `code42cli-1.9.0/src/code42cli/maps.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/options.py` & `code42cli-1.9.0/src/code42cli/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
 
 from code42cli.click_ext.types import MagicDate
+from code42cli.click_ext.types import TOTP
 from code42cli.cmds.search.options import AdvancedQueryAndSavedSearchIncompatible
 from code42cli.cmds.search.options import BeginOption
 from code42cli.date_helper import convert_datetime_to_timestamp
 from code42cli.date_helper import round_datetime_to_day_end
 from code42cli.date_helper import round_datetime_to_day_start
 from code42cli.errors import Code42CLIError
 from code42cli.logger.enums import ServerProtocol
@@ -111,14 +112,15 @@
     )
     return opt
 
 
 def totp_option(hidden=False):
     opt = click.option(
         "--totp",
+        type=TOTP(),
         expose_value=False,
         callback=set_totp,
         hidden=hidden,
         help="TOTP token for multi-factor authentication.",
     )
     return opt
```

### Comparing `code42cli-1.8.1/src/code42cli/output_formats.py` & `code42cli-1.9.0/src/code42cli/output_formats.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/password.py` & `code42cli-1.9.0/src/code42cli/password.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/profile.py` & `code42cli-1.9.0/src/code42cli/profile.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/sdk_client.py` & `code42cli-1.9.0/src/code42cli/sdk_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import py42.sdk
 import py42.settings
 import py42.settings.debug as debug
 import requests
 from click import prompt
 from click import secho
-from py42.exceptions import Py42MFARequiredError
 from py42.exceptions import Py42UnauthorizedError
 from requests.exceptions import ConnectionError
 from requests.exceptions import SSLError
 
+from code42cli.click_ext.types import TOTP
 from code42cli.errors import Code42CLIError
 from code42cli.errors import LoggedCLIError
 from code42cli.logger import get_main_cli_logger
 
 py42.settings.items_per_page = 500
 
 logger = get_main_cli_logger()
@@ -43,19 +43,24 @@
         logger.log_error(err)
         raise LoggedCLIError(
             f"Problem connecting to {authority_url}, SSL certificate verification failed.\nUpdate profile with --disable-ssl-errors to bypass certificate checks (not recommended!)."
         )
     except ConnectionError as err:
         logger.log_error(err)
         raise LoggedCLIError(f"Problem connecting to {authority_url}.")
-    except Py42MFARequiredError:
-        totp = prompt("Multi-factor authentication required. Enter TOTP", type=int)
-        return _validate_connection(authority_url, username, password, totp)
     except Py42UnauthorizedError as err:
         logger.log_error(err)
-        if "INVALID_TIME_BASED_ONE_TIME_PASSWORD" in err.response.text:
-            raise Code42CLIError(f"Invalid TOTP token for user {username}.")
+        if "LoginConfig: LOCAL_2FA" in str(err):
+            if totp is None:
+                totp = prompt(
+                    "Multi-factor authentication required. Enter TOTP", type=TOTP()
+                )
+                return _validate_connection(authority_url, username, password, totp)
+            else:
+                raise Code42CLIError(
+                    f"Invalid credentials or TOTP token for user {username}."
+                )
         else:
             raise Code42CLIError(f"Invalid credentials for user {username}.")
     except Exception as err:
         logger.log_error(err)
         raise LoggedCLIError("Unknown problem validating connection.")
```

### Comparing `code42cli-1.8.1/src/code42cli/util.py` & `code42cli-1.9.0/src/code42cli/util.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli/worker.py` & `code42cli-1.9.0/src/code42cli/worker.py`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/src/code42cli.egg-info/PKG-INFO` & `code42cli-1.9.0/src/code42cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code42cli
-Version: 1.8.1
+Version: 1.9.0
 Summary: The official command line tool for interacting with Code42
 Home-page: https://github.com/code42/py42
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/code42/code42cli/issues
 Project-URL: Documentation, https://clidocs.code42.com/
 Project-URL: Source Code, https://github.com/code42/code42cli
 Description: # The Code42 CLI
```

### Comparing `code42cli-1.8.1/src/code42cli.egg-info/SOURCES.txt` & `code42cli-1.9.0/src/code42cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `code42cli-1.8.1/tox.ini` & `code42cli-1.9.0/tox.ini`

 * *Files identical despite different names*

