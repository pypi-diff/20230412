# Comparing `tmp/jira-select-3.0.0a1.tar.gz` & `tmp/jira-select-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jira-select-3.0.0a1.tar", last modified: Tue Apr 11 05:39:48 2023, max compression
+gzip compressed data, was "jira-select-3.0.0a2.tar", last modified: Wed Apr 12 03:59:59 2023, max compression
```

## Comparing `jira-select-3.0.0a1.tar` & `jira-select-3.0.0a2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/PKG-INFO
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       25 2023-04-11 05:39:25.000000 jira-select-3.0.0a1/jira_select/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/__main__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/cache.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.0.0a1/jira_select/cmdline.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select/commands/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/build_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/configure.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.0.0a1/jira_select/commands/functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/install_user_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/remove_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.0.0a1/jira_select/commands/run.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/run_script.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.0.0a1/jira_select/commands/schema.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/setup_instance.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/commands/shell.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.0.0a1/jira_select/commands/show_instances.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/commands/store_password.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/constants.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/exceptions.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select/formatters/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/formatters/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/formatters/csv.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/formatters/html.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.0.0a1/jira_select/formatters/json.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      381 2023-04-11 05:13:38.000000 jira-select-3.0.0a1/jira_select/formatters/raw.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.0.0a1/jira_select/formatters/table.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/formatters/tsv.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/jira_select/functions/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.0.0a1/jira_select/functions/estimate_to_days.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/extract.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/field_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/functions/flatten_changelog.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/flatten_list.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.0.0a1/jira_select/functions/get_issue.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3602 2023-04-11 03:48:08.000000 jira-select-3.0.0a1/jira_select/functions/get_issue_snapshot_on_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/get_sprint_by_id.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/get_sprint_by_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.0.0a1/jira_select/functions/interval_business_hours.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1125 2023-04-10 23:10:31.000000 jira-select-3.0.0a1/jira_select/functions/interval_matching.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.0.0a1/jira_select/functions/interval_size.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.0.0a1/jira_select/functions/json_dumps.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/functions/parse_date.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/parse_datetime.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.0.0a1/jira_select/functions/simple_filter.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/simple_filter_any.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/sprint_details.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/functions/sprint_name.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1506 2023-04-10 03:30:19.000000 jira-select-3.0.0a1/jira_select/functions/subquery.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.0.0a1/jira_select/functions/union.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.0.0a1/jira_select/functions/workdays_in_state.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     9642 2023-04-10 03:28:45.000000 jira-select-3.0.0a1/jira_select/plugin.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    20521 2023-04-11 05:00:17.000000 jira-select-3.0.0a1/jira_select/query.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/jira_select/sources/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/jira_select/sources/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/sources/boards.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3865 2023-04-10 23:39:17.000000 jira-select-3.0.0a1/jira_select/sources/issues.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.0.0a1/jira_select/sources/sprints.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2176 2023-04-11 05:19:20.000000 jira-select-3.0.0a1/jira_select/types.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10219 2023-04-11 04:51:08.000000 jira-select-3.0.0a1/jira_select/utils.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.568680 jira-select-3.0.0a1/jira_select.egg-info/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/PKG-INFO
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2322 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/SOURCES.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/dependency_links.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2594 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/entry_points.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.0.0a1/jira_select.egg-info/not-zip-safe
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      395 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/requires.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-04-11 05:39:48.000000 jira-select-3.0.0a1/jira_select.egg-info/top_level.txt
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/setup.cfg
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5718 2023-04-11 05:39:25.000000 jira-select-3.0.0a1/setup.py
-drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-11 05:39:48.572680 jira-select-3.0.0a1/tests/
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/tests/__init__.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/tests/base.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.0.0a1/tests/conftest.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.0.0a1/tests/test_functions.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.0.0a1/tests/test_query.py
--rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.0.0a1/tests/test_utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/PKG-INFO
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       25 2023-04-12 03:59:42.000000 jira-select-3.0.0a2/jira_select/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       98 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/__main__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4180 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/cache.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4595 2023-04-10 16:55:25.000000 jira-select-3.0.0a2/jira_select/cmdline.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select/commands/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1815 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/build_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3473 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/configure.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4371 2023-04-09 01:41:06.000000 jira-select-3.0.0a2/jira_select/commands/functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2971 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/install_user_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      411 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/remove_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4181 2023-04-10 03:27:31.000000 jira-select-3.0.0a2/jira_select/commands/run.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      899 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/run_script.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     4031 2023-04-09 01:41:06.000000 jira-select-3.0.0a2/jira_select/commands/schema.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2706 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/setup_instance.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6891 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/commands/shell.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1687 2023-04-09 01:41:06.000000 jira-select-3.0.0a2/jira_select/commands/show_instances.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      759 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/commands/store_password.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      442 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/constants.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      343 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/exceptions.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select/formatters/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/formatters/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      974 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/formatters/csv.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1895 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/formatters/html.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      706 2023-04-09 01:40:24.000000 jira-select-3.0.0a2/jira_select/formatters/json.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      386 2023-04-12 03:52:31.000000 jira-select-3.0.0a2/jira_select/formatters/raw.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1061 2023-01-26 02:12:26.000000 jira-select-3.0.0a2/jira_select/formatters/table.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      176 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/formatters/tsv.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/jira_select/functions/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      944 2023-03-24 16:42:35.000000 jira-select-3.0.0a2/jira_select/functions/estimate_to_days.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1010 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/extract.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1085 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/field_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1833 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/functions/flatten_changelog.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      261 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/flatten_list.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      427 2023-04-11 05:23:23.000000 jira-select-3.0.0a2/jira_select/functions/get_issue.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3339 2023-04-12 02:18:27.000000 jira-select-3.0.0a2/jira_select/functions/get_issue_snapshot_on_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      788 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/get_sprint_by_id.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3371 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/get_sprint_by_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2010 2023-04-11 05:15:10.000000 jira-select-3.0.0a2/jira_select/functions/interval_business_hours.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      859 2023-04-12 01:44:30.000000 jira-select-3.0.0a2/jira_select/functions/interval_matching.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      578 2023-04-10 23:51:45.000000 jira-select-3.0.0a2/jira_select/functions/interval_size.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      366 2023-04-09 01:37:57.000000 jira-select-3.0.0a2/jira_select/functions/json_dumps.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      628 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/functions/parse_date.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      776 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/parse_datetime.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      718 2023-04-09 01:20:37.000000 jira-select-3.0.0a2/jira_select/functions/simple_filter.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      592 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/simple_filter_any.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2834 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/sprint_details.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      473 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/functions/sprint_name.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     1574 2023-04-12 03:38:13.000000 jira-select-3.0.0a2/jira_select/functions/subquery.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      355 2023-04-10 04:56:24.000000 jira-select-3.0.0a2/jira_select/functions/union.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3454 2023-04-10 15:58:21.000000 jira-select-3.0.0a2/jira_select/functions/workdays_in_state.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10116 2023-04-12 02:18:19.000000 jira-select-3.0.0a2/jira_select/plugin.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    23021 2023-04-12 03:57:45.000000 jira-select-3.0.0a2/jira_select/query.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/jira_select/sources/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/jira_select/sources/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2300 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/sources/boards.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3983 2023-04-12 03:22:28.000000 jira-select-3.0.0a2/jira_select/sources/issues.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3576 2023-03-04 07:50:34.000000 jira-select-3.0.0a2/jira_select/sources/sprints.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2254 2023-04-12 02:50:17.000000 jira-select-3.0.0a2/jira_select/types.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10349 2023-04-12 03:32:48.000000 jira-select-3.0.0a2/jira_select/utils.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.301308 jira-select-3.0.0a2/jira_select.egg-info/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     3984 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/PKG-INFO
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2322 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     2594 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/entry_points.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        1 2022-09-19 22:12:27.000000 jira-select-3.0.0a2/jira_select.egg-info/not-zip-safe
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      393 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/requires.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)       18 2023-04-12 03:59:59.000000 jira-select-3.0.0a2/jira_select.egg-info/top_level.txt
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      775 2023-04-12 03:59:59.309309 jira-select-3.0.0a2/setup.cfg
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     5718 2023-04-12 03:59:42.000000 jira-select-3.0.0a2/setup.py
+drwxrwxr-x   0 acoddington  (1000) acoddington  (1000)        0 2023-04-12 03:59:59.305309 jira-select-3.0.0a2/tests/
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)        0 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/tests/__init__.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      892 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/tests/base.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)      452 2022-05-20 02:53:24.000000 jira-select-3.0.0a2/tests/conftest.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    10342 2023-04-11 05:12:36.000000 jira-select-3.0.0a2/tests/test_functions.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)    13320 2023-04-11 05:12:47.000000 jira-select-3.0.0a2/tests/test_query.py
+-rw-rw-r--   0 acoddington  (1000) acoddington  (1000)     6901 2023-04-11 05:12:28.000000 jira-select-3.0.0a2/tests/test_utils.py
```

### Comparing `jira-select-3.0.0a1/PKG-INFO` & `jira-select-3.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
```

### Comparing `jira-select-3.0.0a1/jira_select/cache.py` & `jira-select-3.0.0a2/jira_select/cache.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/cmdline.py` & `jira-select-3.0.0a2/jira_select/cmdline.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/build_query.py` & `jira-select-3.0.0a2/jira_select/commands/build_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/configure.py` & `jira-select-3.0.0a2/jira_select/commands/configure.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/functions.py` & `jira-select-3.0.0a2/jira_select/commands/functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/install_user_script.py` & `jira-select-3.0.0a2/jira_select/commands/install_user_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/run.py` & `jira-select-3.0.0a2/jira_select/commands/run.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/run_script.py` & `jira-select-3.0.0a2/jira_select/commands/run_script.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/schema.py` & `jira-select-3.0.0a2/jira_select/commands/schema.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/setup_instance.py` & `jira-select-3.0.0a2/jira_select/commands/setup_instance.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/shell.py` & `jira-select-3.0.0a2/jira_select/commands/shell.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/show_instances.py` & `jira-select-3.0.0a2/jira_select/commands/show_instances.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/commands/store_password.py` & `jira-select-3.0.0a2/jira_select/commands/store_password.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/formatters/csv.py` & `jira-select-3.0.0a2/jira_select/formatters/csv.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/formatters/html.py` & `jira-select-3.0.0a2/jira_select/formatters/html.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/formatters/json.py` & `jira-select-3.0.0a2/jira_select/formatters/json.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/formatters/table.py` & `jira-select-3.0.0a2/jira_select/formatters/table.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/estimate_to_days.py` & `jira-select-3.0.0a2/jira_select/functions/estimate_to_days.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/extract.py` & `jira-select-3.0.0a2/jira_select/functions/extract.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/field_by_name.py` & `jira-select-3.0.0a2/jira_select/functions/field_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/flatten_changelog.py` & `jira-select-3.0.0a2/jira_select/functions/flatten_changelog.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/get_issue_snapshot_on_date.py` & `jira-select-3.0.0a2/jira_select/functions/get_issue_snapshot_on_date.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 import copy
 import datetime
 from typing import Any
 from typing import Iterator
 
 from dateutil.parser import parse as parse_datetime
 from dotmap import DotMap
-from jira import JIRA
 from jira.resources import Issue
 from pytz import UTC
 
 from jira_select.plugin import BaseFunction
-from jira_select.plugin import get_installed_sources
 
+from ..exceptions import QueryError
 from .flatten_changelog import flatten_changelog
 
 
 class IssueSnapshotContainer(dict):
     _name_map: dict[str, Any] = {}
 
     def __init__(self, field_dict: dict[str, Any], name_map: dict[str, str]) -> None:
@@ -34,19 +33,14 @@
     def __setitem__(self, item: str, value: Any) -> None:
         if item not in self and item in self._name_map:
             return super().__setitem__(self._name_map[item], value)
 
         return super().__setitem__(item, value)
 
 
-def get_customfield_to_name_mapping(jira: JIRA) -> dict[str, str]:
-    schema = get_installed_sources()["issues"].get_schema(jira)
-    return {row.description: row.id for row in schema if row.description}
-
-
 def snapshot_iterator(issue: Issue, field_name_map: dict[str, str]) -> Iterator[DotMap]:
     non_snapshottable = [
         "changelog",
         "components",
         "comment",
         "expand",
         "parent",
@@ -65,19 +59,25 @@
             for k, v in issue.as_dict().items()
             if not callable(v) and k not in non_snapshottable
         },
         field_name_map,
     )
     snapshot_validity_end = datetime.datetime.utcnow().replace(tzinfo=UTC)
 
-    flattened_changelog = sorted(
-        flatten_changelog(issue.changelog),
-        key=lambda row: row.created if row.created else datetime.date(1, 1, 1),
-        reverse=True,
-    )
+    try:
+        flattened_changelog = sorted(
+            flatten_changelog(issue.changelog),
+            key=lambda row: row.created if row.created else datetime.date(1, 1, 1),
+            reverse=True,
+        )
+    except AttributeError as exc:
+        raise QueryError(
+            "'expand' option of 'changelog' is required for snapshot iteration; "
+        ) from exc
+
     for entry in flattened_changelog:
         if entry.field in non_snapshottable:
             continue
 
         snapshot.update(
             {
                 "validity_start": entry.created,
@@ -96,28 +96,22 @@
 
 
 class Function(BaseFunction):
     """Returns an IssueSnapshot representing the Jira Issue's state on a particular date."""
 
     _field_name_map = None
 
-    def get_customfield_to_name_mapping(self) -> dict[str, str]:
-        if self._field_name_map is None:
-            self._field_name_map = get_customfield_to_name_mapping(self.jira)
-
-        return self._field_name_map
-
     def __call__(  # type: ignore[override]
         self, issue: Issue, date: datetime.datetime
     ) -> DotMap:
         last_snapshot: DotMap = DotMap({})
 
         if date > parse_datetime(issue.created):
-            mapping = self.get_customfield_to_name_mapping()
-
-            for snapshot in snapshot_iterator(issue, mapping):
+            for snapshot in snapshot_iterator(
+                issue, self.executor.field_name_map if self.executor else {}
+            ):
                 if parse_datetime(snapshot.created) < date:
                     return last_snapshot
 
                 last_snapshot = snapshot
 
         return last_snapshot
```

### Comparing `jira-select-3.0.0a1/jira_select/functions/get_sprint_by_id.py` & `jira-select-3.0.0a2/jira_select/functions/get_sprint_by_id.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/get_sprint_by_name.py` & `jira-select-3.0.0a2/jira_select/functions/get_sprint_by_name.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/interval_business_hours.py` & `jira-select-3.0.0a2/jira_select/functions/interval_business_hours.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/interval_size.py` & `jira-select-3.0.0a2/jira_select/functions/interval_size.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/parse_date.py` & `jira-select-3.0.0a2/jira_select/functions/parse_date.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/parse_datetime.py` & `jira-select-3.0.0a2/jira_select/functions/parse_datetime.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/simple_filter.py` & `jira-select-3.0.0a2/jira_select/functions/simple_filter.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/simple_filter_any.py` & `jira-select-3.0.0a2/jira_select/functions/simple_filter_any.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/sprint_details.py` & `jira-select-3.0.0a2/jira_select/functions/sprint_details.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/functions/subquery.py` & `jira-select-3.0.0a2/jira_select/functions/subquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             query_definition.cache = self.query.cache
 
         query = Executor(
             self.jira,
             query_definition,
             progress_bar=False,
             parameters=params,
+            schema=self.executor.schema if self.executor else None,
         )
         for row in query:
             row_values = list(row.values())
             if len(query_definition.select) == 1:
                 results.append(row_values[0])
             else:
                 results.append(row_values)
```

### Comparing `jira-select-3.0.0a1/jira_select/functions/workdays_in_state.py` & `jira-select-3.0.0a2/jira_select/functions/workdays_in_state.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/plugin.py` & `jira-select-3.0.0a2/jira_select/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Type
+from weakref import proxy
 
 import keyring
+import portion
 from jira import JIRA
 from rich.console import Console
 from rich.progress import TaskID
 from safdie import BaseCommand as SafdieBaseCommand
 from safdie import get_entrypoints
 from urllib3 import disable_warnings
 
@@ -98,14 +100,19 @@
     # Random
     **get_functions_for_module(
         random,
         ["random", "randrange", "randint", "choice"],
     ),
     # JSON
     "json_loads": json.loads,
+    "empty_interval": portion.empty,
+    "closed_interval": portion.closed,
+    "open_interval": portion.open,
+    "openclosed_interval": portion.openclosed,
+    "closedopen_interval": portion.closedopen,
 }
 REGISTERED_FUNCTIONS: Dict[str, Callable] = {}
 
 
 class BaseCommand(SafdieBaseCommand):
     _jira: Optional[JIRA] = None
 
@@ -168,26 +175,28 @@
             self._jira = JIRA(
                 options={
                     "agile_rest_path": "agile",
                     "server": instance_url,
                     "verify": verify,
                 },
                 basic_auth=(username, password),
+                validate=False,
+                get_server_info=False,
             )
 
         return self._jira
 
 
 def get_installed_formatters() -> Dict[str, Type[BaseFormatter]]:
     return get_entrypoints(FORMATTER_ENTRYPOINT, BaseFormatter)
 
 
 class BaseFormatter(metaclass=ABCMeta):
     def __init__(self, executor: Executor, stream: IO[bytes]):
-        self._executor = executor
+        self._executor = proxy(executor)
         self._stream = stream
 
     @classmethod
     @abstractmethod
     def get_file_extension(cls) -> str:
         ...
 
@@ -220,15 +229,15 @@
 
 def register_function(fn: Callable):
     """Register a callable to be a function available in queries."""
     REGISTERED_FUNCTIONS[fn.__name__] = fn
 
 
 def get_installed_functions(
-    jira: JIRA = None, query: Query = None
+    jira: JIRA = None, executor: Executor = None
 ) -> Dict[str, Callable]:
     possible_commands: Dict[str, Callable] = copy.copy(BUILTIN_FUNCTIONS)
 
     # Import any modules in the custom functions directory; as a
     # side-effect of this, the functions will become listed within
     # REGISTERED_FUNCTIONS
     function_dir = get_custom_function_dir()
@@ -256,27 +265,31 @@
                     spec.loader.exec_module(user_module)  # type: ignore
                 except Exception as e:
                     logger.error("Could not import user script at %s: %s", full_path, e)
 
     possible_commands.update(REGISTERED_FUNCTIONS)
 
     for fn_name, fn in get_entrypoints(FUNCTION_ENTRYPOINT, BaseFunction).items():
-        possible_commands[fn_name] = fn(jira, query=query)
+        possible_commands[fn_name] = fn(jira, executor=executor)
 
     return possible_commands
 
 
 class BaseFunction(metaclass=ABCMeta):
-    def __init__(self, jira: Optional[JIRA], query: Optional[Query]):
+    def __init__(self, jira: Optional[JIRA], executor: Optional[Executor]):
         self._jira = jira
-        self._query = query
+        self._executor = executor
 
     @property
     def query(self) -> Optional[Query]:
-        return self._query
+        return self.executor.query if self.executor else None
+
+    @property
+    def executor(self) -> Optional[Executor]:
+        return self._executor
 
     @property
     def jira(self):
         assert self._jira
 
         return self._jira
```

### Comparing `jira-select-3.0.0a1/jira_select/query.py` & `jira-select-3.0.0a2/jira_select/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,37 +15,42 @@
 from typing import Tuple
 from typing import Type
 from typing import Union
 from typing import cast
 
 from dotmap import DotMap
 from jira import JIRA
+from pydantic import BaseModel
 from rich.progress import BarColumn
 from rich.progress import Progress
 from rich.progress import TaskID
 from rich.progress import TimeRemainingColumn
 
+from . import __version__
 from .cache import MinimumRecencyCache
 from .exceptions import ExpressionParameterMissing
 from .plugin import BaseSource
 from .plugin import get_installed_functions
 from .plugin import get_installed_sources
 from .types import Expression
 from .types import ExpressionList
 from .types import Field
 from .types import JqlList
 from .types import QueryDefinition
+from .types import SchemaRow
 from .types import SelectFieldDefinition
 from .types import WhereParamDict
 from .utils import calculate_result_hash
+from .utils import evaluate_expression
 from .utils import expression_includes_group_by
 from .utils import find_missing_parameters
 from .utils import get_cache_path
 from .utils import get_field_data
 from .utils import get_row_dict
+from .utils import normalize_value
 from .utils import parse_select_definition
 from .utils import parse_sort_by_definition
 
 
 @total_ordering
 class NullAcceptableSort:
     def __init__(self, value: Any):
@@ -69,14 +74,17 @@
             return False
 
     def __str__(self):
         return str(self._value)
 
 
 class Result(metaclass=ABCMeta):
+    def __init__(self):
+        self._overlay: dict[str, Any] = {}
+
     def __getattr__(self, name):
         result = self.as_dict()
 
         if name not in result:
             raise AttributeError(name)
 
         return result[name]
@@ -122,22 +130,22 @@
         return get_field_data(
             row_source,
             expression,
             functions=functions,
             interpolations=field_name_map,
         )
 
+    def __setitem__(self, name, value):
+        self._overlay[name] = value
+
 
 class SingleResult(Result):
     def __init__(self, row: Any):
         self._row = row
-        self._overlay: dict[str, Any] = {}
-
-    def __setitem__(self, name, value):
-        self._overlay[name] = value
+        super().__init__()
 
     def as_dict(self) -> Dict[str, Any]:
         return get_row_dict(self._row, self._overlay)
 
     def single(self) -> SingleResult:
         return self
 
@@ -179,14 +187,15 @@
         self._rows.append(record)
 
     def single(self) -> SingleResult:
         return self.rows[0]
 
     def as_dict(self) -> Dict[str, Any]:
         result: Dict[str, Any] = {}
+        result.update(self._overlay)
 
         for field in self.all_fields:
             # Exclude empty rows -- in SQL when you run an aggregation
             # function on a set of rows, NULL rows are skipped, so we
             # should probably do the same?
             result[field] = GroupedFieldContainer(
                 [
@@ -195,14 +204,19 @@
                     if row.as_dict().get(field) is not None
                 ]
             )
 
         return result
 
 
+class CachedResults(BaseModel):
+    source_schema: List[SchemaRow]
+    rows: List[Dict]
+
+
 class Query:
     def __init__(self, jira: JIRA, definition: QueryDefinition):
         self._jira = jira
         self._definition = definition
 
     def _ensure_str(self, iterable=Iterable[Any]) -> List[str]:
         return [str(item) for item in iterable]
@@ -245,14 +259,18 @@
         return fields
 
     @property
     def select(self) -> List[SelectFieldDefinition]:
         return self._get_select_calculate_fields(self._definition.select)
 
     @property
+    def static(self) -> List[SelectFieldDefinition]:
+        return self._get_select_calculate_fields(self._definition.static)
+
+    @property
     def calculate(self) -> List[SelectFieldDefinition]:
         return self._get_select_calculate_fields(self._definition.calculate)
 
     @property
     def from_(self) -> str:
         return self._definition.from_
 
@@ -362,33 +380,37 @@
     def __init__(
         self,
         jira: JIRA,
         definition: QueryDefinition,
         enable_cache: bool = True,
         progress_bar: bool = False,
         parameters: Optional[Dict[str, Any]] = None,
+        schema: Optional[List[SchemaRow]] = None,
     ):
         self._query: Query = Query(jira, definition)
         self._jira: JIRA = jira
-        self._functions: Dict[str, Callable] = get_installed_functions(
-            jira, self._query
-        )
+        self._functions: Dict[str, Callable] = get_installed_functions(jira, self)
         self._progress_bar_enabled = progress_bar
 
+        self._enable_cache = enable_cache
         self._cache = MinimumRecencyCache(get_cache_path())
+        self._source_schema: List[SchemaRow] = schema if schema is not None else []
+        self._field_name_map: Dict[str, str] = FieldNameMap()
 
-        self._enable_cache = enable_cache
         self._parameters: Dict[str, Any] = parameters or {}
-        self._field_name_map: Dict[str, str] = FieldNameMap()
 
     @property
     def jira(self) -> JIRA:
         return self._jira
 
     @property
+    def schema(self) -> List[SchemaRow]:
+        return self._source_schema
+
+    @property
     def cache(self) -> MinimumRecencyCache:
         return self._cache
 
     @property
     def query(self) -> Query:
         return self._query
 
@@ -396,63 +418,111 @@
     def functions(self) -> Dict[str, Callable]:
         return self._functions
 
     @property
     def parameters(self) -> Dict[str, Any]:
         return self._parameters
 
+    def get_source_schema(self) -> List[SchemaRow]:
+        if not self._source_schema:
+            sources = get_installed_sources()
+            source = sources[self.query.from_]
+
+            self._source_schema = source.get_schema(self.jira)
+
+        return self._source_schema
+
     @property
     def field_name_map(self) -> Dict[str, Any]:
         if not self._field_name_map:
-            for jira_field in self.jira.fields():
-                self._field_name_map[jira_field["name"]] = jira_field["id"]
+            for schema_row in self.get_source_schema():
+                if not schema_row.description:
+                    continue
+
+                self._field_name_map[schema_row.description] = schema_row.id
 
             self._field_name_map["params"] = DotMap(self._parameters)
 
         return self._field_name_map
 
     def _get_cached(self, source: BaseSource) -> Iterator[Result]:
         cache_key = ":".join(
             [
+                __version__,
                 str(self.jira.client_info()),
                 str(self.query.from_),
                 str(self.query.where),
                 str(self.query.order_by),
                 str(self.query.limit),
                 str(self.query.expand),
+                str(self.parameters),
             ]
         )
 
         if self.query.cache and self._enable_cache:
             try:
                 min_recency, _ = self.query.cache
                 if min_recency is None:
                     raise KeyError(cache_key)
-                cached_results = self.cache.get(cache_key, min_recency=min_recency)
-                if not cached_results:
+                cached_results_raw = self.cache.get(cache_key, min_recency=min_recency)
+                if not cached_results_raw:
                     raise KeyError(cache_key)
 
-                source.update_count(len(cached_results))
+                cached_results = CachedResults.parse_obj(cached_results_raw)
+
+                self._source_schema = cached_results.source_schema
+
+                source.update_count(len(cached_results.rows))
                 source.remove_progress()
-                for result in cached_results:
+                for result in cached_results.rows:
                     yield SingleResult(source.rehydrate(result))
                 return
             except KeyError:
                 pass
 
-        cache = []
+        cached_rows = []
+        cached_schema = self.get_source_schema()
 
         for result in source:
-            cache.append(result)
+            cached_rows.append(result)
             yield SingleResult(source.rehydrate(result))
 
         if self.query.cache:
             _, max_store = self.query.cache
             if max_store is not None:
-                self.cache.set(cache_key, cache, expire=max_store)
+                self.cache.set(
+                    cache_key,
+                    CachedResults(source_schema=cached_schema, rows=cached_rows).dict(),
+                    expire=max_store,
+                )
+
+    def _get_static_results(
+        self,
+    ) -> Dict[str, Any]:
+        shared: Dict[str, Any] = {}
+
+        for definition in self.query.static:
+            if missing := find_missing_parameters(
+                definition.expression, list(self.parameters.keys())
+            ):
+                raise ExpressionParameterMissing(
+                    "Parameter {params.%s} found in expression, but no parameter was specified!"
+                    % missing[0]
+                )
+
+            shared[definition.column] = normalize_value(
+                evaluate_expression(
+                    definition.expression,
+                    names={},
+                    functions=self.functions,
+                    interpolations={"params": DotMap(self.parameters)},
+                )
+            )
+
+        return shared
 
     def _process_calculate(
         self,
         iterator: Iterator[Result],
         task: TaskID,
         input_channel: CounterChannel,
         output_channel: CounterChannel,
@@ -583,14 +653,16 @@
             )
 
         return result
 
     def _get_iterator(self) -> Generator[Dict[str, Any], None, None]:
         sources = get_installed_sources()
 
+        static_results = self._get_static_results()
+
         try:
             iterator = sources[self.query.from_]
         except KeyError:
             raise NotImplementedError(
                 f"No search for source {self.query.from_} implemented."
             )
 
@@ -654,14 +726,18 @@
         for phase, task_id in phases:
             output_channel = CounterChannel()
             cursor = phase(cursor, task_id, channel, output_channel)
             channel = output_channel
 
         for row in cursor:
             self.progress.update(select_task, total=channel.get(), visible=True)
+
+            for shared_result_name, shared_result_value in static_results.items():
+                row[shared_result_name] = shared_result_value
+
             yield self._generate_row_dict(row)
             self.progress.update(select_task, advance=1)
 
     @property
     def progress(self) -> Union[Progress, NullProgressbar]:
         return self._progress_bar
```

### Comparing `jira-select-3.0.0a1/jira_select/sources/boards.py` & `jira-select-3.0.0a2/jira_select/sources/boards.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/sources/issues.py` & `jira-select-3.0.0a2/jira_select/sources/issues.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterator
 from typing import List
 
 from dotmap import DotMap
@@ -13,14 +14,16 @@
 from ..exceptions import QueryError
 from ..plugin import BaseSource
 from ..plugin import get_installed_functions
 from ..types import SchemaRow
 from ..utils import evaluate_expression
 from ..utils import find_missing_parameters
 
+logger = logging.getLogger(__name__)
+
 
 class Source(BaseSource):
     SCHEMA: List[SchemaRow] = [
         SchemaRow.parse_obj({"id": "key", "type": "str"}),
         SchemaRow.parse_obj({"id": "id", "type": "int"}),
     ]
 
@@ -79,14 +82,16 @@
         query = query.format(params=DotMap(self._executor.parameters))
 
         order_by_fields = ", ".join(self.query.order_by)
 
         if order_by_fields:
             query = f"{query} ORDER BY {order_by_fields}"
 
+        logger.debug("Executing JIRA query with JQL %s", query)
+
         return query
 
     def __iter__(self) -> Iterator[Dict]:
         start_at = 0
         max_results = 2**32
         result_limit = self.query.limit or 2**32
```

### Comparing `jira-select-3.0.0a1/jira_select/sources/sprints.py` & `jira-select-3.0.0a2/jira_select/sources/sprints.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select/types.py` & `jira-select-3.0.0a2/jira_select/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 Expression = str
 
 ExpressionList = List[Expression]
 
 
 class QueryDefinition(BaseModel):
     select: Union[List[Field], Dict[str, Optional[str]]]
+    static: Dict[str, str] = ModelField(default_factory=dict, alias="static")
     calculate: Dict[str, str] = ModelField(default_factory=dict)
     from_: str = ModelField(alias="from")
     subqueries: Dict[str, "QueryDefinition"] = ModelField(default_factory=dict)
     where: Union[JqlList, WhereParamDict] = ModelField(default_factory=list)
     order_by: JqlList = ModelField(default_factory=list)
     filter_: ExpressionList = ModelField(alias="filter", default_factory=list)
     having: ExpressionList = ModelField(default_factory=list)
```

### Comparing `jira-select-3.0.0a1/jira_select/utils.py` & `jira-select-3.0.0a2/jira_select/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,21 @@
     if hasattr(row, "fields"):
         for field_name in dir(row.fields):
             if not field_name.startswith("_"):
                 names[field_name] = getattr(row.fields, field_name)
 
     # Gather any top-level keys, too, to make sure we fetch any expansions
     for key in dir(row):
-        if key != "fields" and not key.startswith("_") and not key.upper() == key:
+        field_value = getattr(row, key)
+        if (
+            key != "fields"
+            and not key.startswith("_")
+            and not key.upper() == key
+            and not callable(field_value)
+        ):
             names[key] = getattr(row, key)
 
     names.update(overlay if overlay is not None else {})
 
     return names
```

### Comparing `jira-select-3.0.0a1/jira_select.egg-info/PKG-INFO` & `jira-select-3.0.0a2/jira_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jira-select
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Easily run complex SQL-like queries far beyond what Jira's standard JQL query language can provide.
 Home-page: https://github.com/coddingtonbear/jira-select
 Author: Adam Coddington
 Author-email: me@adamcoddington.net
 License: MIT
 Project-URL: Issue Tracker, https://github.com/coddingtonbear/jira-select/issues
 Keywords: jira,csv,sql
```

### Comparing `jira-select-3.0.0a1/jira_select.egg-info/SOURCES.txt` & `jira-select-3.0.0a2/jira_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/jira_select.egg-info/entry_points.txt` & `jira-select-3.0.0a2/jira_select.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/setup.cfg` & `jira-select-3.0.0a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/setup.py` & `jira-select-3.0.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="jira-select",
-    version="3.0.0.a1",
+    version="3.0.0.a2",
     license="MIT",
     description=(
         "Easily run complex SQL-like queries far beyond what "
         "Jira's standard JQL query language can provide."
     ),
     long_description_content_type="text/markdown",
     long_description=read("readme.md"),
```

### Comparing `jira-select-3.0.0a1/tests/base.py` & `jira-select-3.0.0a2/tests/base.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/tests/test_functions.py` & `jira-select-3.0.0a2/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/tests/test_query.py` & `jira-select-3.0.0a2/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `jira-select-3.0.0a1/tests/test_utils.py` & `jira-select-3.0.0a2/tests/test_utils.py`

 * *Files identical despite different names*

