# Comparing `tmp/robotmk-0.0.44.tar.gz` & `tmp/robotmk-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.44.tar", last modified: Sat Apr  8 15:02:08 2023, max compression
+gzip compressed data, was "robotmk-0.0.45.tar", last modified: Wed Apr 12 15:50:45 2023, max compression
```

## Comparing `robotmk-0.0.44.tar` & `robotmk-0.0.45.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      110 2023-04-08 14:53:58.218752 robotmk-0.0.44/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.44/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.44/README.md
--rw-r--r--   0        0        0      622 2023-03-04 18:42:56.325941 robotmk-0.0.44/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.44/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.44/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.44/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.44/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.44/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.44/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.44/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.44/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.44/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-08 14:53:58.218752 robotmk-0.0.44/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.44/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.44/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.44/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0     9964 2023-04-04 09:19:31.690886 robotmk-0.0.44/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.44/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.44/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.44/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.44/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.44/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.44/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.44/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.44/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.44/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.44/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.44/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.44/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.44/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.44/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.44/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.44/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     5970 2023-04-04 09:03:29.956051 robotmk-0.0.44/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.44/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.44/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     3861 2023-04-08 14:40:57.514315 robotmk-0.0.44/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.44/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5538 2023-04-03 13:26:37.965696 robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6441 2023-04-08 13:19:40.304088 robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4652 2023-04-04 09:55:55.820622 robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     4613 2023-04-04 11:57:23.004746 robotmk-0.0.44/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.44/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.44/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.44/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.44/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.44/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.44/src/robotmk/logger.py
--rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.44/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.44/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-03-14 14:11:06.828625 robotmk-0.0.44/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.44/tests/config/robotmk.yml
--rw-r--r--   0        0        0     4465 2023-04-01 17:34:04.588583 robotmk-0.0.44/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.44/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.44/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.44/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.44/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.44/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.44/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.44/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.44/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 robotmk-0.0.44/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-12 15:50:33.292020 robotmk-0.0.45/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.45/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.45/README.md
+-rw-r--r--   0        0        0      672 2023-04-12 15:47:12.533918 robotmk-0.0.45/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.45/src/_confitree/__init__.py
+-rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.45/src/_confitree/confitree.py
+-rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.45/src/_confitree/robotmk.yml
+-rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.45/src/_robotmk/__init__.py
+-rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.45/src/_robotmk/__main__.py
+-rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.45/src/_robotmk/cli.py
+-rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/agent/__init__.py
+-rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/agent/agent.py
+-rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/agent/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/output/__init__.py
+-rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/output/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/robot/__init__.py
+-rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/robot/cli.py
+-rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/robotmk.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/specialagent/__init__.py
+-rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.45/src/_robotmk/modes/specialagent/cli.py
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.45/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.45/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-12 15:50:33.292020 robotmk-0.0.45/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.45/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.45/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.45/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    15122 2023-04-12 15:30:56.411240 robotmk-0.0.45/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.45/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.45/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.45/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.45/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.45/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.45/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.45/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.45/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.45/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.45/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.45/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.45/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.45/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.45/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.45/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.45/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     6017 2023-04-12 15:49:51.188418 robotmk-0.0.45/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.45/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.45/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     8422 2023-04-12 15:48:14.953328 robotmk-0.0.45/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.45/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2766 2023-04-09 16:54:37.704068 robotmk-0.0.45/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.45/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.45/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.45/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.45/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.45/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.45/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.45/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.45/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.45/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.45/tests/config/robotmk.yml
+-rw-r--r--   0        0        0     9958 2023-04-12 15:08:57.203733 robotmk-0.0.45/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.45/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.45/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.45/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.45/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.45/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.45/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.45/tests/context/test_cli.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.45/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 robotmk-0.0.45/PKG-INFO
```

### Comparing `robotmk-0.0.44/pyproject.toml` & `robotmk-0.0.45/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 name = "robotmk"
 authors = [{name = "Simon Meggle", email = "simon.meggle@elabit.de"}]
 classifiers = ["License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"]
 dynamic = ["version", "description"]
 keywords = ["robotmk", "checkmk", "robotframework", "automation", "monitoring"]
 readme = "README.md"
 dependencies = [
-    "psutil"
+    "psutil",
+    "click", 
+    "robotframework",
+    "loguru"
 ]
 
 [project.scripts]
 robotmk = "robotmk.cli.cli:main"
 # TODO: add more scripts here
 # robotmk-agent
 # robotmk-specialagent (calls internally agent & output!)
```

### Comparing `robotmk-0.0.44/src/_confitree/confitree.py` & `robotmk-0.0.45/src/_confitree/confitree.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_confitree/robotmk.yml` & `robotmk-0.0.45/src/_confitree/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_robotmk/__init__.py` & `robotmk-0.0.45/src/_robotmk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_robotmk/__main__.py` & `robotmk-0.0.45/src/_robotmk/__main__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_robotmk/cli.py` & `robotmk-0.0.45/src/_robotmk/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_robotmk/modes/__init__.py` & `robotmk-0.0.45/src/_robotmk/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_robotmk/modes/agent/agent.py` & `robotmk-0.0.45/src/_robotmk/modes/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/_robotmk/modes/agent/cli.py` & `robotmk-0.0.45/src/_robotmk/modes/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/categories.json` & `robotmk-0.0.45/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/click_tutorial.py` & `robotmk-0.0.45/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/cli/cli.py` & `robotmk-0.0.45/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.45/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/config/yml.py` & `robotmk-0.0.45/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/abstract.py` & `robotmk-0.0.45/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/context.py` & `robotmk-0.0.45/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/local/cli.py` & `robotmk-0.0.45/src/robotmk/context/local/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/local/local.py` & `robotmk-0.0.45/src/robotmk/context/local/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.45/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.45/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/cli.py` & `robotmk-0.0.45/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.45/src/robotmk/context/suite/strategies/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         super().__init__(target)
 
     def prepare(self) -> int:
         # nothing to do
         return 0
 
     def execute(self) -> int:
+        # DEBUG: " ".join(self.target.command)
         result = subprocess.run(self.target.command, capture_output=True)
         stdout_str = result.stdout.decode("utf-8").splitlines()
         stderr_str = result.stderr.decode("utf-8").splitlines()
         result_dict = {
             "args": result.args,
             "returncode": result.returncode,
             "stdout": stdout_str,
```

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/suite.py` & `robotmk-0.0.45/src/robotmk/context/suite/suite.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def __init__(self, target):
         self.target = target
         self.run = self.target.run_strategy.run
 
     def create(self):
         """Create the execution strategy"""
-        strategy = self.target.suitecfg.get("retry_failed.strategy", "complete")
+        strategy = self.target.config.get("suitecfg.retry_failed.strategy", "complete")
         if strategy == "complete":
             return CompleteRetry(self.target)
         elif strategy == "incremental":
             return IncrementalRetry(self.target)
         else:
             raise Exception("Unknown retry strategy: %s" % strategy)
 
@@ -29,15 +29,15 @@
     def __init__(self, target):
         self.target = target
         self.target.attempt = 1
 
     @property
     def max_attempts(self):
         """Maximum number of attempts to execute a suite (1st + retries)"""
-        return 1 + self.target.suitecfg.get("retry_failed.retry_attempts", 0)
+        return 1 + self.target.config.get("suitecfg.retry_failed.retry_attempts", 0)
 
     def run(self):
         """Run the suite and retry failed tests if necessary."""
 
         # TODO: set TIC
 
         for attempt in range(1, self.max_attempts + 1):
@@ -144,11 +144,11 @@
         """Reparametrize the suite for the next attempt.
 
         The next attempt needs the XML file of the last attempt as input.
         From there it will read failed tests and re-execute them only."""
         # Chance for next try. Attempt gets increased, output files get bumped
         failed_xml = Path(self.target.logdir).joinpath(self.target.output_xml)
         self.target.robotmk_params.update({"rerunfailed": str(failed_xml)})
-        rerun_selection = self.target.suitecfg.get(
-            "retry_failed.rerun_selection", {}
+        rerun_selection = self.target.config.get(
+            "suitecfg.retry_failed.rerun_selection", {}
         ).asdict()
         self.target.robotmk_params.update(rerun_selection)
```

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             {
                 "log": self.log_html,
                 "output": self.output_xml,
             }
         )
 
         suite_params = mergedeep.merge(
-            self.suitecfg.get("params").asdict(), self.robotmk_params
+            self.config.get("suitecfg.params").asdict(), self.robotmk_params
         )
         arglist = ["robot"]
         for k, v in suite_params.items():
             arg = f"--{k}"
             # create something we can iterate over
             if isinstance(v, str):
                 # key:value    => convert to 1 el list
```

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.45/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return {
             "suiteuname": self.target.suiteuname,
             "uuid": self.target.uuid,
             "rc": self.target.rc,
             "start_time": self._start_time.isoformat(),
             "end_time": self._end_time.isoformat(),
             "runtime": self._runtime.total_seconds(),
-            "piggybackhost": self.target.suitecfg.get("piggybackhost", None),
+            "piggybackhost": self.target.config.get("suiteconfig.piggybackhost", None),
             "output": {
                 "html": {
                     "path": self.target.log_html_fullpath,
                 },
                 "xml": {
                     "path": self.target.output_xml_fullpath,
                     "base64": self.encode(
```

### Comparing `robotmk-0.0.44/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.45/src/robotmk/context/suite/target/target.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     - a local Robot suite or ("target: local")
     - an API call to an external platform ("target: remote") like Robocorp or Kubernetes
     """
 
     def __init__(self, suiteuname: str, config: DotMap, logger: RobotmkLogger):
         self.suiteuname = suiteuname
         self.config = config
-        self.suitecfg = self.config.get("suites.%s" % suiteuname)
+
         self.commoncfg = self.config.get("common")
 
         self._logger = logger
         # TODO: Boilerplate alarm
         self.debug = self._logger.debug
         self.info = self._logger.info
         self.warning = self._logger.warning
@@ -38,15 +38,15 @@
     @abstractmethod
     def output(self):
         """Abstract method to get the output of a suite/target."""
         pass
 
 
 class LocalTarget(Target):
-    """A local target is a single Robot Fremework suite or a RCC task for this suite.
+    """A local target is a single Robot Framework suite or a RCC task for this suite.
 
     It also encapsulates the implementation details of the RUN strategy, which is
     either a headless or a headed execution (RDP, XVFB, Scheduled Task)."""
 
     def __init__(
         self,
         suiteuname: str,
@@ -57,23 +57,23 @@
 
         # Store RCC and RF logs in separate folders
         self.config.set(
             "common.logdir", "%s/%s" % (self.config.get("common.logdir"), str(self))
         )
 
         self.path = Path(self.config.get("common.robotdir")).joinpath(
-            self.suitecfg.get("path")
+            self.config.get("suitecfg.path")
         )
         self.run_strategy = RunStrategyFactory(self).create()
         # list of subprocess' results and console output
         self.console_results = {}
 
     @property
     def uuid(self):
-        return self.suitecfg.get("uuid", uuid4().hex)
+        return self.config.get("suitecfg.uuid", uuid4().hex)
 
     @property
     def logdir(self):
         return self.config.get("common.logdir")
 
     @property
     def is_disabled_by_flagfile(self):
@@ -85,69 +85,7 @@
     def run(self):
         pass
 
     def output(self):
         # None of the run strategies used for "run" are needed to get the output,
         # so we can just read the result artifacts from the filesystem.
         pass
-
-
-# ---
-
-
-# class LocalSuite(Target):
-#     """A single Robot Framework suite on Linux and Windows.
-
-#     Also encapsulates the implementation details of
-#     whether to run the suite with the OS Python or within
-#     a RCC environment."""
-
-#     # self.suitecfg = getattr(self.config.suites, self.suitename)
-
-#     def __init__(self, name: str, config: dict):
-#         super().__init__(name, config)
-#         self._set_python_strategy()
-#         self._set_head_strategy()
-#         pass
-
-#     @property
-#     def abspath(self):
-#         return Path(self.config.path).resolve()
-
-#     def run(self):
-#         pass
-
-#     def _set_python_strategy(self):
-#         """Sets the python execution strategy.
-
-#         Execution with `RCC` is possible when
-#         # 1. the suite is RCC compatible (conda.yml)
-#         # 2. feature is available (binary check)
-#         # 3. RCC is not disallowed in robotmk.yml
-#         # 4. `share-python` is not set on cli (would enforce the same Python)"""
-
-#     def _set_head_strategy(self):
-#         """Sets the strategy for this suite:
-#         - HeadedWinExecStrategy
-#         - HeadedLinExecutionStrategy
-#         - HeadlessExecutionStrategy"""
-#         self._strategy = strategy
-#         self.prepare = self._strategy.prepare
-#         self.execute = self._strategy.execute
-#         self.cleanup = self._strategy.cleanup
-
-
-# class RemoteSuite(Target):
-#     """A single Robot Framework suite on a remote platform.
-
-#     Its execution is triggered via an API call."""
-
-#     def __init__(self, name: str, config: dict):
-#         super().__init__(name)
-#         self.config = config
-
-#     def get_jobs_running(self):
-#         """Returns the number of running jobs currently."""
-#         pass
-
-#     def kill_job(self):
-#         pass
```

### Comparing `robotmk-0.0.44/src/robotmk/executor/scheduler.py` & `robotmk-0.0.45/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.45/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/logger.py` & `robotmk-0.0.45/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/src/robotmk/main.py` & `robotmk-0.0.45/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/config/robotmk.yml` & `robotmk-0.0.45/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/context/local/test_local_cli.py` & `robotmk-0.0.45/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.45/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/context/suite/robotmk.yml` & `robotmk-0.0.45/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.45/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/context/test_cli.py` & `robotmk-0.0.45/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.44/tests/yml/robotmk.yml` & `robotmk-0.0.45/tests/yml/robotmk.yml`

 * *Files identical despite different names*

