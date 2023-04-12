# Comparing `tmp/robotmk-0.0.45.tar.gz` & `tmp/robotmk-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.45.tar", last modified: Wed Apr 12 15:50:45 2023, max compression
+gzip compressed data, was "robotmk-0.0.46.tar", last modified: Wed Apr 12 15:59:27 2023, max compression
```

## Comparing `robotmk-0.0.45.tar` & `robotmk-0.0.46.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      110 2023-04-12 15:50:33.292020 robotmk-0.0.45/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.45/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.45/README.md
--rw-r--r--   0        0        0      672 2023-04-12 15:47:12.533918 robotmk-0.0.45/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.45/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.45/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.45/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.45/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.45/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.45/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.45/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.45/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-12 15:50:33.292020 robotmk-0.0.45/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.45/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.45/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.45/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    15122 2023-04-12 15:30:56.411240 robotmk-0.0.45/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.45/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.45/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.45/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.45/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.45/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.45/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.45/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.45/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.45/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.45/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.45/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.45/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.45/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.45/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.45/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.45/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     6017 2023-04-12 15:49:51.188418 robotmk-0.0.45/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.45/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.45/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     8422 2023-04-12 15:48:14.953328 robotmk-0.0.45/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.45/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2766 2023-04-09 16:54:37.704068 robotmk-0.0.45/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.45/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.45/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.45/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.45/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.45/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.45/src/robotmk/logger.py
--rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.45/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.45/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.45/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.45/tests/config/robotmk.yml
--rw-r--r--   0        0        0     9958 2023-04-12 15:08:57.203733 robotmk-0.0.45/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.45/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.45/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.45/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.45/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.45/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.45/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.45/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.45/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 robotmk-0.0.45/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-12 15:59:18.695061 robotmk-0.0.46/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.46/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.46/README.md
+-rw-r--r--   0        0        0      689 2023-04-12 15:59:06.911172 robotmk-0.0.46/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.46/src/_confitree/__init__.py
+-rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.46/src/_confitree/confitree.py
+-rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.46/src/_confitree/robotmk.yml
+-rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.46/src/_robotmk/__init__.py
+-rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.46/src/_robotmk/__main__.py
+-rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.46/src/_robotmk/cli.py
+-rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/agent/__init__.py
+-rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/agent/agent.py
+-rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/agent/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/output/__init__.py
+-rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/output/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/robot/__init__.py
+-rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/robot/cli.py
+-rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/robotmk.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/specialagent/__init__.py
+-rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.46/src/_robotmk/modes/specialagent/cli.py
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.46/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.46/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-12 15:59:18.691061 robotmk-0.0.46/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.46/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.46/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.46/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    15122 2023-04-12 15:30:56.411240 robotmk-0.0.46/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.46/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.46/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.46/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.46/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.46/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.46/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.46/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.46/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.46/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.46/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.46/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.46/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.46/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.46/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.46/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.46/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     6017 2023-04-12 15:49:51.188418 robotmk-0.0.46/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.46/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.46/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     8422 2023-04-12 15:48:14.953328 robotmk-0.0.46/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.46/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2766 2023-04-09 16:54:37.704068 robotmk-0.0.46/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.46/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.46/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.46/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.46/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.46/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.46/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.46/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.46/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.46/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.46/tests/config/robotmk.yml
+-rw-r--r--   0        0        0     9958 2023-04-12 15:08:57.203733 robotmk-0.0.46/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.46/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.46/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.46/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.46/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.46/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.46/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.46/tests/context/test_cli.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.46/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 robotmk-0.0.46/PKG-INFO
```

### Comparing `robotmk-0.0.45/pyproject.toml` & `robotmk-0.0.46/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 dynamic = ["version", "description"]
 keywords = ["robotmk", "checkmk", "robotframework", "automation", "monitoring"]
 readme = "README.md"
 dependencies = [
     "psutil",
     "click", 
     "robotframework",
-    "loguru"
+    "loguru",
+    "mergedeep"
 ]
 
 [project.scripts]
 robotmk = "robotmk.cli.cli:main"
 # TODO: add more scripts here
 # robotmk-agent
 # robotmk-specialagent (calls internally agent & output!)
```

### Comparing `robotmk-0.0.45/src/_confitree/confitree.py` & `robotmk-0.0.46/src/_confitree/confitree.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_confitree/robotmk.yml` & `robotmk-0.0.46/src/_confitree/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_robotmk/__init__.py` & `robotmk-0.0.46/src/_robotmk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_robotmk/__main__.py` & `robotmk-0.0.46/src/_robotmk/__main__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_robotmk/cli.py` & `robotmk-0.0.46/src/_robotmk/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_robotmk/modes/__init__.py` & `robotmk-0.0.46/src/_robotmk/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_robotmk/modes/agent/agent.py` & `robotmk-0.0.46/src/_robotmk/modes/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/_robotmk/modes/agent/cli.py` & `robotmk-0.0.46/src/_robotmk/modes/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/categories.json` & `robotmk-0.0.46/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/click_tutorial.py` & `robotmk-0.0.46/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/cli/cli.py` & `robotmk-0.0.46/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.46/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/config/config.py` & `robotmk-0.0.46/src/robotmk/config/config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/config/yml.py` & `robotmk-0.0.46/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/abstract.py` & `robotmk-0.0.46/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/context.py` & `robotmk-0.0.46/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/local/cli.py` & `robotmk-0.0.46/src/robotmk/context/local/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/local/local.py` & `robotmk-0.0.46/src/robotmk/context/local/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.46/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.46/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/cli.py` & `robotmk-0.0.46/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.46/src/robotmk/context/suite/strategies/run.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/suite.py` & `robotmk-0.0.46/src/robotmk/context/suite/suite.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.46/src/robotmk/context/suite/target/rcc.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.46/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.46/src/robotmk/context/suite/target/target.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/executor/scheduler.py` & `robotmk-0.0.46/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.46/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/logger.py` & `robotmk-0.0.46/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/src/robotmk/main.py` & `robotmk-0.0.46/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/config/robotmk.yml` & `robotmk-0.0.46/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/config/test_config.py` & `robotmk-0.0.46/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/context/local/test_local_cli.py` & `robotmk-0.0.46/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.46/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/context/suite/robotmk.yml` & `robotmk-0.0.46/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.46/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/context/test_cli.py` & `robotmk-0.0.46/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.45/tests/yml/robotmk.yml` & `robotmk-0.0.46/tests/yml/robotmk.yml`

 * *Files identical despite different names*

