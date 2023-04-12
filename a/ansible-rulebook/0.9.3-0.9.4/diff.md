# Comparing `tmp/ansible_rulebook-0.9.3.tar.gz` & `tmp/ansible_rulebook-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_rulebook-0.9.3.tar", last modified: Tue Oct 18 14:23:59 2022, max compression
+gzip compressed data, was "ansible_rulebook-0.9.4.tar", last modified: Tue Oct 18 14:33:50 2022, max compression
```

## Comparing `ansible_rulebook-0.9.3.tar` & `ansible_rulebook-0.9.4.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.859663 ansible_rulebook-0.9.3/
--rw-r--r--   0 ben        (501) staff       (20)     5536 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/CONTRIBUTING.rst
--rw-r--r--   0 ben        (501) staff       (20)       89 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/HISTORY.rst
--rw-r--r--   0 ben        (501) staff       (20)    11358 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      295 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     6157 2022-10-18 14:23:59.859791 ansible_rulebook-0.9.3/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     5418 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/README.rst
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.775376 ansible_rulebook-0.9.3/ansible_rulebook/
--rw-r--r--   0 ben        (501) staff       (20)       83 2022-10-18 14:20:38.000000 ansible_rulebook-0.9.3/ansible_rulebook/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)       46 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/__main__.py
--rw-r--r--   0 ben        (501) staff       (20)       63 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/ansible_events.py
--rw-r--r--   0 ben        (501) staff       (20)     4567 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/ansible_rulebook/app.py
--rw-r--r--   0 ben        (501) staff       (20)    16870 2022-10-18 14:18:43.000000 ansible_rulebook-0.9.3/ansible_rulebook/builtin.py
--rw-r--r--   0 ben        (501) staff       (20)     3967 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/ansible_rulebook/cli.py
--rw-r--r--   0 ben        (501) staff       (20)     2696 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/ansible_rulebook/collection.py
--rw-r--r--   0 ben        (501) staff       (20)     3524 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/condition_parser.py
--rw-r--r--   0 ben        (501) staff       (20)      689 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/condition_types.py
--rw-r--r--   0 ben        (501) staff       (20)      124 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/conf.py
--rw-r--r--   0 ben        (501) staff       (20)     3783 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/durability.py
--rw-r--r--   0 ben        (501) staff       (20)    12574 2022-10-18 14:19:08.000000 ansible_rulebook-0.9.3/ansible_rulebook/engine.py
--rw-r--r--   0 ben        (501) staff       (20)      156 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/ansible_rulebook/exception.py
--rw-r--r--   0 ben        (501) staff       (20)      668 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/inventory.py
--rw-r--r--   0 ben        (501) staff       (20)     8641 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/json_generator.py
--rw-r--r--   0 ben        (501) staff       (20)      960 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/key.py
--rw-r--r--   0 ben        (501) staff       (20)       70 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/ansible_rulebook/messages.py
--rw-r--r--   0 ben        (501) staff       (20)     9368 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.3/ansible_rulebook/rule_generator.py
--rw-r--r--   0 ben        (501) staff       (20)     1449 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.3/ansible_rulebook/rule_types.py
--rw-r--r--   0 ben        (501) staff       (20)     3740 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/ansible_rulebook/rules_parser.py
--rw-r--r--   0 ben        (501) staff       (20)     3142 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/ansible_rulebook/util.py
--rw-r--r--   0 ben        (501) staff       (20)     3555 2022-10-15 18:36:10.000000 ansible_rulebook-0.9.3/ansible_rulebook/websocket.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.777867 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     6157 2022-10-18 14:23:59.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     7492 2022-10-18 14:23:59.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-10-18 14:23:59.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       63 2022-10-18 14:23:59.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/entry_points.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-10-11 23:07:19.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/not-zip-safe
--rw-r--r--   0 ben        (501) staff       (20)      110 2022-10-18 14:23:59.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       17 2022-10-18 14:23:59.000000 ansible_rulebook-0.9.3/ansible_rulebook.egg-info/top_level.txt
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.787073 ansible_rulebook-0.9.3/docs/
--rw-r--r--   0 ben        (501) staff       (20)      617 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/docs/Makefile
--rw-r--r--   0 ben        (501) staff       (20)      590 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/docs/actions.rst
--rw-r--r--   0 ben        (501) staff       (20)       28 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/authors.rst
--rw-r--r--   0 ben        (501) staff       (20)       39 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/collections.rst
--rw-r--r--   0 ben        (501) staff       (20)     1202 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/conditions.rst
--rwxr-xr-x   0 ben        (501) staff       (20)     4898 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/docs/conf.py
--rw-r--r--   0 ben        (501) staff       (20)       33 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/contributing.rst
--rw-r--r--   0 ben        (501) staff       (20)       42 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/environments.rst
--rw-r--r--   0 ben        (501) staff       (20)      342 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/filters.rst
--rw-r--r--   0 ben        (501) staff       (20)       28 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/history.rst
--rw-r--r--   0 ben        (501) staff       (20)      564 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/host_limit.rst
--rw-r--r--   0 ben        (501) staff       (20)      403 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/docs/index.rst
--rw-r--r--   0 ben        (501) staff       (20)     1113 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/docs/installation.rst
--rw-r--r--   0 ben        (501) staff       (20)      778 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/docs/make.bat
--rw-r--r--   0 ben        (501) staff       (20)     1582 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/multi_events.rst
--rw-r--r--   0 ben        (501) staff       (20)      801 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/multi_sources.rst
--rw-r--r--   0 ben        (501) staff       (20)       27 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/readme.rst
--rw-r--r--   0 ben        (501) staff       (20)    19540 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/docs/rules.rst
--rw-r--r--   0 ben        (501) staff       (20)       24 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/docs/runner.rst
--rw-r--r--   0 ben        (501) staff       (20)     4406 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/docs/sources.rst
--rw-r--r--   0 ben        (501) staff       (20)     2344 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/docs/usage.rst
--rw-r--r--   0 ben        (501) staff       (20)      277 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/pyproject.toml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.787386 ansible_rulebook-0.9.3/schema/
--rw-r--r--   0 ben        (501) staff       (20)     5868 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/schema/ruleset_schema.json
--rw-r--r--   0 ben        (501) staff       (20)     1468 2022-10-18 14:23:59.860403 ansible_rulebook-0.9.3/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.792086 ansible_rulebook-0.9.3/tests/
--rw-r--r--   0 ben        (501) staff       (20)       46 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/tests/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.815358 ansible_rulebook-0.9.3/tests/asts/
--rw-r--r--   0 ben        (501) staff       (20)      516 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/01_noop.yml
--rw-r--r--   0 ben        (501) staff       (20)      510 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/02_debug.yml
--rw-r--r--   0 ben        (501) staff       (20)      522 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/03_print_event.yml
--rw-r--r--   0 ben        (501) staff       (20)      888 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/04_set_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      890 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/05_post_event.yml
--rw-r--r--   0 ben        (501) staff       (20)     1183 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/06_retract_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      772 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/07_and.yml
--rw-r--r--   0 ben        (501) staff       (20)      770 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/08_or.yml
--rw-r--r--   0 ben        (501) staff       (20)      522 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/09_gt.yml
--rw-r--r--   0 ben        (501) staff       (20)      516 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/10_lt.yml
--rw-r--r--   0 ben        (501) staff       (20)      537 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/11_le.yml
--rw-r--r--   0 ben        (501) staff       (20)      543 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/12_ge.yml
--rw-r--r--   0 ben        (501) staff       (20)      662 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/13_add.yml
--rw-r--r--   0 ben        (501) staff       (20)      670 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/14_sub.yml
--rw-r--r--   0 ben        (501) staff       (20)      683 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/15_multiple_events_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      683 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/16_multiple_events_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      783 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/17_multiple_sources_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      787 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/18_multiple_sources_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      802 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/19_is_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)     1100 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/20_is_not_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)      561 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/21_run_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      565 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/23_nested_data.yml
--rw-r--r--   0 ben        (501) staff       (20)      563 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/24_max_attributes.yml
--rw-r--r--   0 ben        (501) staff       (20)      604 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/25_max_attributes_nested.yml
--rw-r--r--   0 ben        (501) staff       (20)      643 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/26_print_events.yml
--rw-r--r--   0 ben        (501) staff       (20)     1066 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/27_var_root.yml
--rw-r--r--   0 ben        (501) staff       (20)      769 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/28_right_side_condition_template.yml
--rw-r--r--   0 ben        (501) staff       (20)      621 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/29_run_module.yml
--rw-r--r--   0 ben        (501) staff       (20)      619 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/30_run_module_missing.yml
--rw-r--r--   0 ben        (501) staff       (20)      626 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/31_run_module_missing_args.yml
--rw-r--r--   0 ben        (501) staff       (20)      641 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/32_run_module_fail.yml
--rw-r--r--   0 ben        (501) staff       (20)      649 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/33_run_playbook_retry.yml
--rw-r--r--   0 ben        (501) staff       (20)      625 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/34_run_playbook_retries.yml
--rw-r--r--   0 ben        (501) staff       (20)     1521 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)     1537 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)     1090 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/37_hosts_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)      534 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/asts/38_shutdown.yml
--rw-r--r--   0 ben        (501) staff       (20)     2984 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/rules.yml
--rw-r--r--   0 ben        (501) staff       (20)      708 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)      707 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_assignment2.yml
--rw-r--r--   0 ben        (501) staff       (20)      923 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_multiple_conditions.yml
--rw-r--r--   0 ben        (501) staff       (20)      924 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_multiple_conditions2.yml
--rw-r--r--   0 ben        (501) staff       (20)     1440 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_multiple_conditions3.yml
--rw-r--r--   0 ben        (501) staff       (20)     1601 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_time.yml
--rw-r--r--   0 ben        (501) staff       (20)     2380 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_timestamp.yml
--rw-r--r--   0 ben        (501) staff       (20)      915 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_with_vars.yml
--rw-r--r--   0 ben        (501) staff       (20)      579 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.3/tests/asts/rules_without_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)     1634 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_filters.yml
--rw-r--r--   0 ben        (501) staff       (20)     1958 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_host_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)     1950 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)     2017 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_rules_multiple_hosts.yml
--rw-r--r--   0 ben        (501) staff       (20)      529 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_rules_multiple_hosts2.yml
--rw-r--r--   0 ben        (501) staff       (20)      529 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_rules_multiple_hosts3.yml
--rw-r--r--   0 ben        (501) staff       (20)     1286 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_set_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)     1548 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/asts/test_simple.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.817321 ansible_rulebook-0.9.3/tests/event_filters/
--rw-r--r--   0 ben        (501) staff       (20)     1027 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/event_filters/dashes_to_underscores.py
--rw-r--r--   0 ben        (501) staff       (20)     1376 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/event_filters/json_filter.py
--rw-r--r--   0 ben        (501) staff       (20)      103 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/event_filters/noop.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.832163 ansible_rulebook-0.9.3/tests/examples/
--rw-r--r--   0 ben        (501) staff       (20)      182 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/01_noop.yml
--rw-r--r--   0 ben        (501) staff       (20)      176 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/02_debug.yml
--rw-r--r--   0 ben        (501) staff       (20)      188 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/03_print_event.yml
--rw-r--r--   0 ben        (501) staff       (20)      324 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/04_set_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      326 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/05_post_event.yml
--rw-r--r--   0 ben        (501) staff       (20)      458 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/06_retract_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)      210 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/07_and.yml
--rw-r--r--   0 ben        (501) staff       (20)      208 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/08_or.yml
--rw-r--r--   0 ben        (501) staff       (20)      165 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/09_gt.yml
--rw-r--r--   0 ben        (501) staff       (20)      162 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/10_lt.yml
--rw-r--r--   0 ben        (501) staff       (20)      175 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/11_le.yml
--rw-r--r--   0 ben        (501) staff       (20)      178 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/12_ge.yml
--rw-r--r--   0 ben        (501) staff       (20)      203 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/13_add.yml
--rw-r--r--   0 ben        (501) staff       (20)      208 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/14_sub.yml
--rw-r--r--   0 ben        (501) staff       (20)      259 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/15_multiple_events_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      259 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/16_multiple_events_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      258 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/17_multiple_sources_any.yml
--rw-r--r--   0 ben        (501) staff       (20)      262 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/18_multiple_sources_all.yml
--rw-r--r--   0 ben        (501) staff       (20)      291 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/19_is_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)      431 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/20_is_not_defined.yml
--rw-r--r--   0 ben        (501) staff       (20)      216 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/21_run_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      249 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/22_run_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      222 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/23_nested_data.yml
--rw-r--r--   0 ben        (501) staff       (20)      220 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/24_max_attributes.yml
--rw-r--r--   0 ben        (501) staff       (20)      261 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/25_max_attributes_nested.yml
--rw-r--r--   0 ben        (501) staff       (20)      240 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/26_print_events.yml
--rw-r--r--   0 ben        (501) staff       (20)      423 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/27_var_root.yml
--rw-r--r--   0 ben        (501) staff       (20)      349 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/28_right_side_condition_template.yml
--rw-r--r--   0 ben        (501) staff       (20)      270 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/29_run_module.yml
--rw-r--r--   0 ben        (501) staff       (20)      268 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/30_run_module_missing.yml
--rw-r--r--   0 ben        (501) staff       (20)      275 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/31_run_module_missing_args.yml
--rw-r--r--   0 ben        (501) staff       (20)      278 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/32_run_module_fail.yml
--rw-r--r--   0 ben        (501) staff       (20)      288 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/33_run_playbook_retry.yml
--rw-r--r--   0 ben        (501) staff       (20)      268 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/34_run_playbook_retries.yml
--rw-r--r--   0 ben        (501) staff       (20)      575 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/35_multiple_rulesets_1_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)      591 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/36_multiple_rulesets_both_fired.yml
--rw-r--r--   0 ben        (501) staff       (20)      402 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/37_hosts_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)      206 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/examples/38_shutdown.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.760773 ansible_rulebook-0.9.3/tests/examples/replays/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.836495 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/
--rw-r--r--   0 ben        (501) staff       (20)       73 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/00.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/01.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/02.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/03.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/04.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/05.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/06.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/07.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/08.json
--rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/09.json
--rwxr-xr-x   0 ben        (501) staff       (20)      245 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/23_nested_data/generate_data.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.837254 ansible_rulebook-0.9.3/tests/examples/replays/24_max_attributes/
--rw-r--r--   0 ben        (501) staff       (20)     5032 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/24_max_attributes/00.json
--rwxr-xr-x   0 ben        (501) staff       (20)      310 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/24_max_attributes/generate_data.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.838086 ansible_rulebook-0.9.3/tests/examples/replays/25_max_attributes_nested/
--rw-r--r--   0 ben        (501) staff       (20)     3791 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/25_max_attributes_nested/00.json
--rwxr-xr-x   0 ben        (501) staff       (20)      519 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/examples/replays/25_max_attributes_nested/generate_data.py
--rwxr-xr-x   0 ben        (501) staff       (20)     1108 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.3/tests/generate_asts.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.841696 ansible_rulebook-0.9.3/tests/playbooks/
--rw-r--r--   0 ben        (501) staff       (20)      616 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/check_facts_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)      302 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/compare_value.yml
--rw-r--r--   0 ben        (501) staff       (20)      825 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/fail_and_succeed.yml
--rw-r--r--   0 ben        (501) staff       (20)      221 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/hello.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/hello_events.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/hello_world_set_fact.yml
--rw-r--r--   0 ben        (501) staff       (20)       62 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/inventory.yml
--rw-r--r--   0 ben        (501) staff       (20)      111 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/inventory1.yml
--rw-r--r--   0 ben        (501) staff       (20)      362 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/validate_args_playbook.yml
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/playbooks/vars.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.851698 ansible_rulebook-0.9.3/tests/rules/
--rw-r--r--   0 ben        (501) staff       (20)     1410 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/rules.yml
--rw-r--r--   0 ben        (501) staff       (20)      267 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)      266 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_assignment2.yml
--rw-r--r--   0 ben        (501) staff       (20)      307 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_multiple_conditions.yml
--rw-r--r--   0 ben        (501) staff       (20)      308 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_multiple_conditions2.yml
--rw-r--r--   0 ben        (501) staff       (20)      475 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_multiple_conditions3.yml
--rw-r--r--   0 ben        (501) staff       (20)      741 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_time.yml
--rw-r--r--   0 ben        (501) staff       (20)     1070 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_timestamp.yml
--rw-r--r--   0 ben        (501) staff       (20)      281 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_with_vars.yml
--rw-r--r--   0 ben        (501) staff       (20)      244 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/rules_without_assignment.yml
--rw-r--r--   0 ben        (501) staff       (20)      286 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_duplicate_rule_names.yml
--rw-r--r--   0 ben        (501) staff       (20)      199 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_empty_rule_names.yml
--rw-r--r--   0 ben        (501) staff       (20)      618 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_filters.yml
--rw-r--r--   0 ben        (501) staff       (20)      754 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_host_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)     1463 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_kafka.yml
--rw-r--r--   0 ben        (501) staff       (20)      189 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_missing_rule_names.yml
--rw-r--r--   0 ben        (501) staff       (20)      337 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/test_multiple_sources.yml
--rw-r--r--   0 ben        (501) staff       (20)      746 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_rules.yml
--rw-r--r--   0 ben        (501) staff       (20)      461 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/test_rules_expanded_conditions.yml
--rw-r--r--   0 ben        (501) staff       (20)      813 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_rules_multiple_hosts.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_rules_multiple_hosts2.yml
--rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_rules_multiple_hosts3.yml
--rw-r--r--   0 ben        (501) staff       (20)      244 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/test_rules_playbooks.yml
--rw-r--r--   0 ben        (501) staff       (20)      688 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_set_facts.yml
--rw-r--r--   0 ben        (501) staff       (20)      587 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_simple.yml
--rw-r--r--   0 ben        (501) staff       (20)      985 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/rules/test_states.yml
--rw-r--r--   0 ben        (501) staff       (20)      944 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/rules/webserver_down.yml
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.857454 ansible_rulebook-0.9.3/tests/sources/
--rw-r--r--   0 ben        (501) staff       (20)        0 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     2025 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/file.py
--rw-r--r--   0 ben        (501) staff       (20)      375 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/hosts.py
--rw-r--r--   0 ben        (501) staff       (20)      555 2022-10-18 14:13:25.000000 ansible_rulebook-0.9.3/tests/sources/infrange.py
--rw-r--r--   0 ben        (501) staff       (20)     2253 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/log_scraper.py
--rwxr-xr-x   0 ben        (501) staff       (20)      500 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/nested.py
--rw-r--r--   0 ben        (501) staff       (20)      622 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/ping.py
--rw-r--r--   0 ben        (501) staff       (20)     1607 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/process_check.py
--rw-r--r--   0 ben        (501) staff       (20)      413 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/range.py
--rw-r--r--   0 ben        (501) staff       (20)      426 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/range2.py
--rwxr-xr-x   0 ben        (501) staff       (20)      990 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/replay.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:23:59.859356 ansible_rulebook-0.9.3/tests/sources/replays/
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/replays/01.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/replays/02.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/replays/03.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/replays/04.json
--rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/replays/05.json
--rw-r--r--   0 ben        (501) staff       (20)      636 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/sources/template.py
--rw-r--r--   0 ben        (501) staff       (20)      303 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/tick.py
--rwxr-xr-x   0 ben        (501) staff       (20)      436 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/timestamp.py
--rw-r--r--   0 ben        (501) staff       (20)     1320 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/sources/url_check.py
--rw-r--r--   0 ben        (501) staff       (20)      532 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.3/tests/test_ansible_events.py
--rw-r--r--   0 ben        (501) staff       (20)     6677 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/test_ast.py
--rw-r--r--   0 ben        (501) staff       (20)      619 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/test_collection.py
--rw-r--r--   0 ben        (501) staff       (20)     6916 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.3/tests/test_conditions.py
--rw-r--r--   0 ben        (501) staff       (20)    15703 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/test_engine.py
--rw-r--r--   0 ben        (501) staff       (20)    28166 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.3/tests/test_examples.py
--rwxr-xr-x   0 ben        (501) staff       (20)     7849 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.3/tests/test_rules.py
--rw-r--r--   0 ben        (501) staff       (20)      576 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.3/tests/test_simple.yml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.894245 ansible_rulebook-0.9.4/
+-rw-r--r--   0 ben        (501) staff       (20)     5536 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/CONTRIBUTING.rst
+-rw-r--r--   0 ben        (501) staff       (20)       89 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/HISTORY.rst
+-rw-r--r--   0 ben        (501) staff       (20)    11358 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)      295 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/MANIFEST.in
+-rw-r--r--   0 ben        (501) staff       (20)     6207 2022-10-18 14:33:50.894403 ansible_rulebook-0.9.4/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     5418 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/README.rst
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.690923 ansible_rulebook-0.9.4/ansible_rulebook/
+-rw-r--r--   0 ben        (501) staff       (20)       83 2022-10-18 14:32:48.000000 ansible_rulebook-0.9.4/ansible_rulebook/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)       46 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/__main__.py
+-rw-r--r--   0 ben        (501) staff       (20)       63 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/ansible_events.py
+-rw-r--r--   0 ben        (501) staff       (20)     4567 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/app.py
+-rw-r--r--   0 ben        (501) staff       (20)    16870 2022-10-18 14:18:43.000000 ansible_rulebook-0.9.4/ansible_rulebook/builtin.py
+-rw-r--r--   0 ben        (501) staff       (20)     3967 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/cli.py
+-rw-r--r--   0 ben        (501) staff       (20)     2696 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/collection.py
+-rw-r--r--   0 ben        (501) staff       (20)     3524 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/condition_parser.py
+-rw-r--r--   0 ben        (501) staff       (20)      689 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/condition_types.py
+-rw-r--r--   0 ben        (501) staff       (20)      124 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/conf.py
+-rw-r--r--   0 ben        (501) staff       (20)     3783 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/durability.py
+-rw-r--r--   0 ben        (501) staff       (20)    12574 2022-10-18 14:19:08.000000 ansible_rulebook-0.9.4/ansible_rulebook/engine.py
+-rw-r--r--   0 ben        (501) staff       (20)      156 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/exception.py
+-rw-r--r--   0 ben        (501) staff       (20)      668 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/inventory.py
+-rw-r--r--   0 ben        (501) staff       (20)     8641 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/json_generator.py
+-rw-r--r--   0 ben        (501) staff       (20)      960 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/key.py
+-rw-r--r--   0 ben        (501) staff       (20)       70 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/ansible_rulebook/messages.py
+-rw-r--r--   0 ben        (501) staff       (20)     9368 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/ansible_rulebook/rule_generator.py
+-rw-r--r--   0 ben        (501) staff       (20)     1449 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/ansible_rulebook/rule_types.py
+-rw-r--r--   0 ben        (501) staff       (20)     3740 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/rules_parser.py
+-rw-r--r--   0 ben        (501) staff       (20)     3142 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/ansible_rulebook/util.py
+-rw-r--r--   0 ben        (501) staff       (20)     3555 2022-10-15 18:36:10.000000 ansible_rulebook-0.9.4/ansible_rulebook/websocket.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.695021 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     6207 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     7492 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)       63 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/entry_points.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2022-10-11 23:07:19.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/not-zip-safe
+-rw-r--r--   0 ben        (501) staff       (20)      110 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       17 2022-10-18 14:33:50.000000 ansible_rulebook-0.9.4/ansible_rulebook.egg-info/top_level.txt
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.716221 ansible_rulebook-0.9.4/docs/
+-rw-r--r--   0 ben        (501) staff       (20)      617 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/Makefile
+-rw-r--r--   0 ben        (501) staff       (20)      590 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/actions.rst
+-rw-r--r--   0 ben        (501) staff       (20)       28 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/authors.rst
+-rw-r--r--   0 ben        (501) staff       (20)       39 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/collections.rst
+-rw-r--r--   0 ben        (501) staff       (20)     1202 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/conditions.rst
+-rwxr-xr-x   0 ben        (501) staff       (20)     4898 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/conf.py
+-rw-r--r--   0 ben        (501) staff       (20)       33 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/contributing.rst
+-rw-r--r--   0 ben        (501) staff       (20)       42 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/environments.rst
+-rw-r--r--   0 ben        (501) staff       (20)      342 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/filters.rst
+-rw-r--r--   0 ben        (501) staff       (20)       28 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/history.rst
+-rw-r--r--   0 ben        (501) staff       (20)      564 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/host_limit.rst
+-rw-r--r--   0 ben        (501) staff       (20)      403 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/index.rst
+-rw-r--r--   0 ben        (501) staff       (20)     1113 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/installation.rst
+-rw-r--r--   0 ben        (501) staff       (20)      778 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/docs/make.bat
+-rw-r--r--   0 ben        (501) staff       (20)     1582 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/multi_events.rst
+-rw-r--r--   0 ben        (501) staff       (20)      801 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/multi_sources.rst
+-rw-r--r--   0 ben        (501) staff       (20)       27 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/readme.rst
+-rw-r--r--   0 ben        (501) staff       (20)    19540 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/rules.rst
+-rw-r--r--   0 ben        (501) staff       (20)       24 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/docs/runner.rst
+-rw-r--r--   0 ben        (501) staff       (20)     4406 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/sources.rst
+-rw-r--r--   0 ben        (501) staff       (20)     2344 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/docs/usage.rst
+-rw-r--r--   0 ben        (501) staff       (20)      277 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/pyproject.toml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.717654 ansible_rulebook-0.9.4/schema/
+-rw-r--r--   0 ben        (501) staff       (20)     5868 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/schema/ruleset_schema.json
+-rw-r--r--   0 ben        (501) staff       (20)     1507 2022-10-18 14:33:50.895105 ansible_rulebook-0.9.4/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.733298 ansible_rulebook-0.9.4/tests/
+-rw-r--r--   0 ben        (501) staff       (20)       46 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/tests/__init__.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.793491 ansible_rulebook-0.9.4/tests/asts/
+-rw-r--r--   0 ben        (501) staff       (20)      516 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/01_noop.yml
+-rw-r--r--   0 ben        (501) staff       (20)      510 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/02_debug.yml
+-rw-r--r--   0 ben        (501) staff       (20)      522 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/03_print_event.yml
+-rw-r--r--   0 ben        (501) staff       (20)      888 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/04_set_fact.yml
+-rw-r--r--   0 ben        (501) staff       (20)      890 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/05_post_event.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1183 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/06_retract_fact.yml
+-rw-r--r--   0 ben        (501) staff       (20)      772 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/07_and.yml
+-rw-r--r--   0 ben        (501) staff       (20)      770 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/08_or.yml
+-rw-r--r--   0 ben        (501) staff       (20)      522 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/09_gt.yml
+-rw-r--r--   0 ben        (501) staff       (20)      516 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/10_lt.yml
+-rw-r--r--   0 ben        (501) staff       (20)      537 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/11_le.yml
+-rw-r--r--   0 ben        (501) staff       (20)      543 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/12_ge.yml
+-rw-r--r--   0 ben        (501) staff       (20)      662 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/13_add.yml
+-rw-r--r--   0 ben        (501) staff       (20)      670 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/14_sub.yml
+-rw-r--r--   0 ben        (501) staff       (20)      683 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/15_multiple_events_all.yml
+-rw-r--r--   0 ben        (501) staff       (20)      683 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/16_multiple_events_any.yml
+-rw-r--r--   0 ben        (501) staff       (20)      783 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/17_multiple_sources_any.yml
+-rw-r--r--   0 ben        (501) staff       (20)      787 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/18_multiple_sources_all.yml
+-rw-r--r--   0 ben        (501) staff       (20)      802 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/19_is_defined.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1100 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/20_is_not_defined.yml
+-rw-r--r--   0 ben        (501) staff       (20)      561 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/21_run_playbook.yml
+-rw-r--r--   0 ben        (501) staff       (20)      565 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/23_nested_data.yml
+-rw-r--r--   0 ben        (501) staff       (20)      563 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/24_max_attributes.yml
+-rw-r--r--   0 ben        (501) staff       (20)      604 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/25_max_attributes_nested.yml
+-rw-r--r--   0 ben        (501) staff       (20)      643 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/26_print_events.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1066 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/27_var_root.yml
+-rw-r--r--   0 ben        (501) staff       (20)      769 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/28_right_side_condition_template.yml
+-rw-r--r--   0 ben        (501) staff       (20)      621 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/29_run_module.yml
+-rw-r--r--   0 ben        (501) staff       (20)      619 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/30_run_module_missing.yml
+-rw-r--r--   0 ben        (501) staff       (20)      626 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/31_run_module_missing_args.yml
+-rw-r--r--   0 ben        (501) staff       (20)      641 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/32_run_module_fail.yml
+-rw-r--r--   0 ben        (501) staff       (20)      649 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/33_run_playbook_retry.yml
+-rw-r--r--   0 ben        (501) staff       (20)      625 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/34_run_playbook_retries.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1521 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1537 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1090 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/37_hosts_facts.yml
+-rw-r--r--   0 ben        (501) staff       (20)      534 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/asts/38_shutdown.yml
+-rw-r--r--   0 ben        (501) staff       (20)     2984 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/rules.yml
+-rw-r--r--   0 ben        (501) staff       (20)      708 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_assignment.yml
+-rw-r--r--   0 ben        (501) staff       (20)      707 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_assignment2.yml
+-rw-r--r--   0 ben        (501) staff       (20)      923 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions.yml
+-rw-r--r--   0 ben        (501) staff       (20)      924 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1440 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1601 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_time.yml
+-rw-r--r--   0 ben        (501) staff       (20)     2380 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_timestamp.yml
+-rw-r--r--   0 ben        (501) staff       (20)      915 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_with_vars.yml
+-rw-r--r--   0 ben        (501) staff       (20)      579 2022-10-17 15:19:47.000000 ansible_rulebook-0.9.4/tests/asts/rules_without_assignment.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1634 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_filters.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1958 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_host_rules.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1950 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules.yml
+-rw-r--r--   0 ben        (501) staff       (20)     2017 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts.yml
+-rw-r--r--   0 ben        (501) staff       (20)      529 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 ben        (501) staff       (20)      529 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1286 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_set_facts.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1548 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/asts/test_simple.yml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.796087 ansible_rulebook-0.9.4/tests/event_filters/
+-rw-r--r--   0 ben        (501) staff       (20)     1027 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/event_filters/dashes_to_underscores.py
+-rw-r--r--   0 ben        (501) staff       (20)     1376 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/event_filters/json_filter.py
+-rw-r--r--   0 ben        (501) staff       (20)      103 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/event_filters/noop.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.832444 ansible_rulebook-0.9.4/tests/examples/
+-rw-r--r--   0 ben        (501) staff       (20)      182 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/01_noop.yml
+-rw-r--r--   0 ben        (501) staff       (20)      176 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/02_debug.yml
+-rw-r--r--   0 ben        (501) staff       (20)      188 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/03_print_event.yml
+-rw-r--r--   0 ben        (501) staff       (20)      324 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/04_set_fact.yml
+-rw-r--r--   0 ben        (501) staff       (20)      326 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/05_post_event.yml
+-rw-r--r--   0 ben        (501) staff       (20)      458 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/06_retract_fact.yml
+-rw-r--r--   0 ben        (501) staff       (20)      210 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/07_and.yml
+-rw-r--r--   0 ben        (501) staff       (20)      208 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/08_or.yml
+-rw-r--r--   0 ben        (501) staff       (20)      165 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/09_gt.yml
+-rw-r--r--   0 ben        (501) staff       (20)      162 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/10_lt.yml
+-rw-r--r--   0 ben        (501) staff       (20)      175 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/11_le.yml
+-rw-r--r--   0 ben        (501) staff       (20)      178 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/12_ge.yml
+-rw-r--r--   0 ben        (501) staff       (20)      203 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/13_add.yml
+-rw-r--r--   0 ben        (501) staff       (20)      208 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/14_sub.yml
+-rw-r--r--   0 ben        (501) staff       (20)      259 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/15_multiple_events_all.yml
+-rw-r--r--   0 ben        (501) staff       (20)      259 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/16_multiple_events_any.yml
+-rw-r--r--   0 ben        (501) staff       (20)      258 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/17_multiple_sources_any.yml
+-rw-r--r--   0 ben        (501) staff       (20)      262 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/18_multiple_sources_all.yml
+-rw-r--r--   0 ben        (501) staff       (20)      291 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/19_is_defined.yml
+-rw-r--r--   0 ben        (501) staff       (20)      431 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/20_is_not_defined.yml
+-rw-r--r--   0 ben        (501) staff       (20)      216 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/21_run_playbook.yml
+-rw-r--r--   0 ben        (501) staff       (20)      249 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/22_run_playbook.yml
+-rw-r--r--   0 ben        (501) staff       (20)      222 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/23_nested_data.yml
+-rw-r--r--   0 ben        (501) staff       (20)      220 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/24_max_attributes.yml
+-rw-r--r--   0 ben        (501) staff       (20)      261 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/25_max_attributes_nested.yml
+-rw-r--r--   0 ben        (501) staff       (20)      240 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/26_print_events.yml
+-rw-r--r--   0 ben        (501) staff       (20)      423 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/27_var_root.yml
+-rw-r--r--   0 ben        (501) staff       (20)      349 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/28_right_side_condition_template.yml
+-rw-r--r--   0 ben        (501) staff       (20)      270 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/29_run_module.yml
+-rw-r--r--   0 ben        (501) staff       (20)      268 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/30_run_module_missing.yml
+-rw-r--r--   0 ben        (501) staff       (20)      275 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/31_run_module_missing_args.yml
+-rw-r--r--   0 ben        (501) staff       (20)      278 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/32_run_module_fail.yml
+-rw-r--r--   0 ben        (501) staff       (20)      288 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/33_run_playbook_retry.yml
+-rw-r--r--   0 ben        (501) staff       (20)      268 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/34_run_playbook_retries.yml
+-rw-r--r--   0 ben        (501) staff       (20)      575 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/35_multiple_rulesets_1_fired.yml
+-rw-r--r--   0 ben        (501) staff       (20)      591 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/36_multiple_rulesets_both_fired.yml
+-rw-r--r--   0 ben        (501) staff       (20)      402 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/37_hosts_facts.yml
+-rw-r--r--   0 ben        (501) staff       (20)      206 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/examples/38_shutdown.yml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.668601 ansible_rulebook-0.9.4/tests/examples/replays/
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.841111 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/
+-rw-r--r--   0 ben        (501) staff       (20)       73 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/00.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/01.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/02.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/03.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/04.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/05.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/06.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/07.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/08.json
+-rw-r--r--   0 ben        (501) staff       (20)       72 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/09.json
+-rwxr-xr-x   0 ben        (501) staff       (20)      245 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/23_nested_data/generate_data.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.842636 ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/
+-rw-r--r--   0 ben        (501) staff       (20)     5032 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/00.json
+-rwxr-xr-x   0 ben        (501) staff       (20)      310 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/generate_data.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.844143 ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/
+-rw-r--r--   0 ben        (501) staff       (20)     3791 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/00.json
+-rwxr-xr-x   0 ben        (501) staff       (20)      519 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/generate_data.py
+-rwxr-xr-x   0 ben        (501) staff       (20)     1108 2022-10-18 14:13:47.000000 ansible_rulebook-0.9.4/tests/generate_asts.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.851946 ansible_rulebook-0.9.4/tests/playbooks/
+-rw-r--r--   0 ben        (501) staff       (20)      616 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/check_facts_playbook.yml
+-rw-r--r--   0 ben        (501) staff       (20)      302 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/compare_value.yml
+-rw-r--r--   0 ben        (501) staff       (20)      825 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/fail_and_succeed.yml
+-rw-r--r--   0 ben        (501) staff       (20)      221 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/hello.yml
+-rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/hello_events.yml
+-rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/hello_world_set_fact.yml
+-rw-r--r--   0 ben        (501) staff       (20)       62 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/inventory.yml
+-rw-r--r--   0 ben        (501) staff       (20)      111 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/inventory1.yml
+-rw-r--r--   0 ben        (501) staff       (20)      362 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/validate_args_playbook.yml
+-rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/playbooks/vars.yml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.879335 ansible_rulebook-0.9.4/tests/rules/
+-rw-r--r--   0 ben        (501) staff       (20)     1410 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/rules.yml
+-rw-r--r--   0 ben        (501) staff       (20)      267 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_assignment.yml
+-rw-r--r--   0 ben        (501) staff       (20)      266 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_assignment2.yml
+-rw-r--r--   0 ben        (501) staff       (20)      307 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_multiple_conditions.yml
+-rw-r--r--   0 ben        (501) staff       (20)      308 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_multiple_conditions2.yml
+-rw-r--r--   0 ben        (501) staff       (20)      475 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_multiple_conditions3.yml
+-rw-r--r--   0 ben        (501) staff       (20)      741 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_time.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_timestamp.yml
+-rw-r--r--   0 ben        (501) staff       (20)      281 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_with_vars.yml
+-rw-r--r--   0 ben        (501) staff       (20)      244 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/rules_without_assignment.yml
+-rw-r--r--   0 ben        (501) staff       (20)      286 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_duplicate_rule_names.yml
+-rw-r--r--   0 ben        (501) staff       (20)      199 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_empty_rule_names.yml
+-rw-r--r--   0 ben        (501) staff       (20)      618 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_filters.yml
+-rw-r--r--   0 ben        (501) staff       (20)      754 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_host_rules.yml
+-rw-r--r--   0 ben        (501) staff       (20)     1463 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_kafka.yml
+-rw-r--r--   0 ben        (501) staff       (20)      189 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_missing_rule_names.yml
+-rw-r--r--   0 ben        (501) staff       (20)      337 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/test_multiple_sources.yml
+-rw-r--r--   0 ben        (501) staff       (20)      746 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules.yml
+-rw-r--r--   0 ben        (501) staff       (20)      461 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_expanded_conditions.yml
+-rw-r--r--   0 ben        (501) staff       (20)      813 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts.yml
+-rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts2.yml
+-rw-r--r--   0 ben        (501) staff       (20)      195 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts3.yml
+-rw-r--r--   0 ben        (501) staff       (20)      244 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/test_rules_playbooks.yml
+-rw-r--r--   0 ben        (501) staff       (20)      688 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_set_facts.yml
+-rw-r--r--   0 ben        (501) staff       (20)      587 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_simple.yml
+-rw-r--r--   0 ben        (501) staff       (20)      985 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/rules/test_states.yml
+-rw-r--r--   0 ben        (501) staff       (20)      944 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/rules/webserver_down.yml
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.891722 ansible_rulebook-0.9.4/tests/sources/
+-rw-r--r--   0 ben        (501) staff       (20)        0 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     2025 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/file.py
+-rw-r--r--   0 ben        (501) staff       (20)      375 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/hosts.py
+-rw-r--r--   0 ben        (501) staff       (20)      555 2022-10-18 14:13:25.000000 ansible_rulebook-0.9.4/tests/sources/infrange.py
+-rw-r--r--   0 ben        (501) staff       (20)     2253 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/log_scraper.py
+-rwxr-xr-x   0 ben        (501) staff       (20)      500 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/nested.py
+-rw-r--r--   0 ben        (501) staff       (20)      622 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/ping.py
+-rw-r--r--   0 ben        (501) staff       (20)     1607 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/process_check.py
+-rw-r--r--   0 ben        (501) staff       (20)      413 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/range.py
+-rw-r--r--   0 ben        (501) staff       (20)      426 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/range2.py
+-rwxr-xr-x   0 ben        (501) staff       (20)      990 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replay.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-10-18 14:33:50.893830 ansible_rulebook-0.9.4/tests/sources/replays/
+-rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/01.json
+-rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/02.json
+-rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/03.json
+-rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/04.json
+-rw-r--r--   0 ben        (501) staff       (20)        9 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/replays/05.json
+-rw-r--r--   0 ben        (501) staff       (20)      636 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/sources/template.py
+-rw-r--r--   0 ben        (501) staff       (20)      303 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/tick.py
+-rwxr-xr-x   0 ben        (501) staff       (20)      436 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/timestamp.py
+-rw-r--r--   0 ben        (501) staff       (20)     1320 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/sources/url_check.py
+-rw-r--r--   0 ben        (501) staff       (20)      532 2022-10-14 16:16:19.000000 ansible_rulebook-0.9.4/tests/test_ansible_events.py
+-rw-r--r--   0 ben        (501) staff       (20)     6677 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_ast.py
+-rw-r--r--   0 ben        (501) staff       (20)      619 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_collection.py
+-rw-r--r--   0 ben        (501) staff       (20)     6916 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/tests/test_conditions.py
+-rw-r--r--   0 ben        (501) staff       (20)    15703 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_engine.py
+-rw-r--r--   0 ben        (501) staff       (20)    28166 2022-10-18 14:11:24.000000 ansible_rulebook-0.9.4/tests/test_examples.py
+-rwxr-xr-x   0 ben        (501) staff       (20)     7849 2022-10-18 14:12:31.000000 ansible_rulebook-0.9.4/tests/test_rules.py
+-rw-r--r--   0 ben        (501) staff       (20)      576 2022-10-11 23:06:05.000000 ansible_rulebook-0.9.4/tests/test_simple.yml
```

### Comparing `ansible_rulebook-0.9.3/CONTRIBUTING.rst` & `ansible_rulebook-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/LICENSE` & `ansible_rulebook-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/PKG-INFO` & `ansible_rulebook-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ansible_rulebook
-Version: 0.9.3
+Version: 0.9.4
 Summary: Event driven automation for Ansible
 Home-page: https://github.com/ansible/ansible-rulebook
 License: Apache-2.0
 Keywords: ansible_rulebook
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 ================
 ansible-rulebook
 ================
```

### Comparing `ansible_rulebook-0.9.3/README.rst` & `ansible_rulebook-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/app.py` & `ansible_rulebook-0.9.4/ansible_rulebook/app.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/builtin.py` & `ansible_rulebook-0.9.4/ansible_rulebook/builtin.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/cli.py` & `ansible_rulebook-0.9.4/ansible_rulebook/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/collection.py` & `ansible_rulebook-0.9.4/ansible_rulebook/collection.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/condition_parser.py` & `ansible_rulebook-0.9.4/ansible_rulebook/condition_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/condition_types.py` & `ansible_rulebook-0.9.4/ansible_rulebook/condition_types.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/durability.py` & `ansible_rulebook-0.9.4/ansible_rulebook/durability.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/engine.py` & `ansible_rulebook-0.9.4/ansible_rulebook/engine.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/inventory.py` & `ansible_rulebook-0.9.4/ansible_rulebook/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/json_generator.py` & `ansible_rulebook-0.9.4/ansible_rulebook/json_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/key.py` & `ansible_rulebook-0.9.4/ansible_rulebook/key.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/rule_generator.py` & `ansible_rulebook-0.9.4/ansible_rulebook/rule_generator.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/rule_types.py` & `ansible_rulebook-0.9.4/ansible_rulebook/rule_types.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/rules_parser.py` & `ansible_rulebook-0.9.4/ansible_rulebook/rules_parser.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/util.py` & `ansible_rulebook-0.9.4/ansible_rulebook/util.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook/websocket.py` & `ansible_rulebook-0.9.4/ansible_rulebook/websocket.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook.egg-info/PKG-INFO` & `ansible_rulebook-0.9.4/ansible_rulebook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ansible-rulebook
-Version: 0.9.3
+Version: 0.9.4
 Summary: Event driven automation for Ansible
 Home-page: https://github.com/ansible/ansible-rulebook
 License: Apache-2.0
 Keywords: ansible_rulebook
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 
 ================
 ansible-rulebook
 ================
```

### Comparing `ansible_rulebook-0.9.3/ansible_rulebook.egg-info/SOURCES.txt` & `ansible_rulebook-0.9.4/ansible_rulebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/Makefile` & `ansible_rulebook-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/actions.rst` & `ansible_rulebook-0.9.4/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/conditions.rst` & `ansible_rulebook-0.9.4/docs/conditions.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/conf.py` & `ansible_rulebook-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/host_limit.rst` & `ansible_rulebook-0.9.4/docs/host_limit.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/installation.rst` & `ansible_rulebook-0.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/make.bat` & `ansible_rulebook-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/multi_events.rst` & `ansible_rulebook-0.9.4/docs/multi_events.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/multi_sources.rst` & `ansible_rulebook-0.9.4/docs/multi_sources.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/rules.rst` & `ansible_rulebook-0.9.4/docs/rules.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/sources.rst` & `ansible_rulebook-0.9.4/docs/sources.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/docs/usage.rst` & `ansible_rulebook-0.9.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/schema/ruleset_schema.json` & `ansible_rulebook-0.9.4/schema/ruleset_schema.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/setup.cfg` & `ansible_rulebook-0.9.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [bumpversion]
-current_version = 0.9.3
+current_version = 0.9.4
 commit = True
 tag = True
 
 [metadata]
 name = ansible_rulebook
-version = 0.9.3
+version = 0.9.4
 description = Event driven automation for Ansible
 url = https://github.com/ansible/ansible-rulebook
 license = Apache-2.0
 keywords = ansible_rulebook
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.8
 install_requires = 
 	asyncio
 	durable_rules
 	pyparsing >= 3.0
 	jsonschema
 	jinja2
 	redis
```

### Comparing `ansible_rulebook-0.9.3/tests/asts/01_noop.yml` & `ansible_rulebook-0.9.4/tests/asts/01_noop.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/03_print_event.yml` & `ansible_rulebook-0.9.4/tests/asts/03_print_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/04_set_fact.yml` & `ansible_rulebook-0.9.4/tests/asts/04_set_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/05_post_event.yml` & `ansible_rulebook-0.9.4/tests/asts/05_post_event.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/06_retract_fact.yml` & `ansible_rulebook-0.9.4/tests/asts/06_retract_fact.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/07_and.yml` & `ansible_rulebook-0.9.4/tests/asts/07_and.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/08_or.yml` & `ansible_rulebook-0.9.4/tests/asts/08_or.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/09_gt.yml` & `ansible_rulebook-0.9.4/tests/asts/09_gt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/10_lt.yml` & `ansible_rulebook-0.9.4/tests/asts/10_lt.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/11_le.yml` & `ansible_rulebook-0.9.4/tests/asts/11_le.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/12_ge.yml` & `ansible_rulebook-0.9.4/tests/asts/12_ge.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/13_add.yml` & `ansible_rulebook-0.9.4/tests/asts/13_add.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/14_sub.yml` & `ansible_rulebook-0.9.4/tests/asts/14_sub.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/15_multiple_events_all.yml` & `ansible_rulebook-0.9.4/tests/asts/15_multiple_events_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/16_multiple_events_any.yml` & `ansible_rulebook-0.9.4/tests/asts/16_multiple_events_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/17_multiple_sources_any.yml` & `ansible_rulebook-0.9.4/tests/asts/17_multiple_sources_any.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/18_multiple_sources_all.yml` & `ansible_rulebook-0.9.4/tests/asts/18_multiple_sources_all.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/19_is_defined.yml` & `ansible_rulebook-0.9.4/tests/asts/19_is_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/20_is_not_defined.yml` & `ansible_rulebook-0.9.4/tests/asts/20_is_not_defined.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/21_run_playbook.yml` & `ansible_rulebook-0.9.4/tests/asts/21_run_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/23_nested_data.yml` & `ansible_rulebook-0.9.4/tests/asts/23_nested_data.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/24_max_attributes.yml` & `ansible_rulebook-0.9.4/tests/asts/24_max_attributes.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/25_max_attributes_nested.yml` & `ansible_rulebook-0.9.4/tests/asts/25_max_attributes_nested.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/26_print_events.yml` & `ansible_rulebook-0.9.4/tests/asts/26_print_events.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/27_var_root.yml` & `ansible_rulebook-0.9.4/tests/asts/27_var_root.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/28_right_side_condition_template.yml` & `ansible_rulebook-0.9.4/tests/asts/28_right_side_condition_template.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/29_run_module.yml` & `ansible_rulebook-0.9.4/tests/asts/29_run_module.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/30_run_module_missing.yml` & `ansible_rulebook-0.9.4/tests/asts/30_run_module_missing.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/31_run_module_missing_args.yml` & `ansible_rulebook-0.9.4/tests/asts/31_run_module_missing_args.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/32_run_module_fail.yml` & `ansible_rulebook-0.9.4/tests/asts/32_run_module_fail.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/33_run_playbook_retry.yml` & `ansible_rulebook-0.9.4/tests/asts/33_run_playbook_retry.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/34_run_playbook_retries.yml` & `ansible_rulebook-0.9.4/tests/asts/34_run_playbook_retries.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-0.9.4/tests/asts/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-0.9.4/tests/asts/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/37_hosts_facts.yml` & `ansible_rulebook-0.9.4/tests/asts/37_hosts_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/38_shutdown.yml` & `ansible_rulebook-0.9.4/tests/asts/38_shutdown.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules.yml` & `ansible_rulebook-0.9.4/tests/asts/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_assignment.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_assignment.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_assignment2.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_assignment2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_multiple_conditions.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_multiple_conditions2.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_multiple_conditions3.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_multiple_conditions3.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_time.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_timestamp.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_with_vars.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_with_vars.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/rules_without_assignment.yml` & `ansible_rulebook-0.9.4/tests/asts/rules_without_assignment.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_filters.yml` & `ansible_rulebook-0.9.4/tests/asts/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_host_rules.yml` & `ansible_rulebook-0.9.4/tests/asts/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_rules.yml` & `ansible_rulebook-0.9.4/tests/asts/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_rules_multiple_hosts.yml` & `ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_rules_multiple_hosts2.yml` & `ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts2.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_rules_multiple_hosts3.yml` & `ansible_rulebook-0.9.4/tests/asts/test_rules_multiple_hosts3.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_set_facts.yml` & `ansible_rulebook-0.9.4/tests/asts/test_set_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/asts/test_simple.yml` & `ansible_rulebook-0.9.4/tests/asts/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/event_filters/dashes_to_underscores.py` & `ansible_rulebook-0.9.4/tests/event_filters/dashes_to_underscores.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/event_filters/json_filter.py` & `ansible_rulebook-0.9.4/tests/event_filters/json_filter.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/examples/35_multiple_rulesets_1_fired.yml` & `ansible_rulebook-0.9.4/tests/examples/35_multiple_rulesets_1_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/examples/36_multiple_rulesets_both_fired.yml` & `ansible_rulebook-0.9.4/tests/examples/36_multiple_rulesets_both_fired.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/examples/replays/24_max_attributes/00.json` & `ansible_rulebook-0.9.4/tests/examples/replays/24_max_attributes/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/examples/replays/25_max_attributes_nested/00.json` & `ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/00.json`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/examples/replays/25_max_attributes_nested/generate_data.py` & `ansible_rulebook-0.9.4/tests/examples/replays/25_max_attributes_nested/generate_data.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/generate_asts.py` & `ansible_rulebook-0.9.4/tests/generate_asts.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/playbooks/check_facts_playbook.yml` & `ansible_rulebook-0.9.4/tests/playbooks/check_facts_playbook.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/playbooks/fail_and_succeed.yml` & `ansible_rulebook-0.9.4/tests/playbooks/fail_and_succeed.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/rules.yml` & `ansible_rulebook-0.9.4/tests/rules/rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/rules_with_time.yml` & `ansible_rulebook-0.9.4/tests/rules/rules_with_time.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/rules_with_timestamp.yml` & `ansible_rulebook-0.9.4/tests/rules/rules_with_timestamp.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_filters.yml` & `ansible_rulebook-0.9.4/tests/rules/test_filters.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_host_rules.yml` & `ansible_rulebook-0.9.4/tests/rules/test_host_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_kafka.yml` & `ansible_rulebook-0.9.4/tests/rules/test_kafka.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_rules.yml` & `ansible_rulebook-0.9.4/tests/rules/test_rules.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_rules_multiple_hosts.yml` & `ansible_rulebook-0.9.4/tests/rules/test_rules_multiple_hosts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_set_facts.yml` & `ansible_rulebook-0.9.4/tests/rules/test_set_facts.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_simple.yml` & `ansible_rulebook-0.9.4/tests/rules/test_simple.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/test_states.yml` & `ansible_rulebook-0.9.4/tests/rules/test_states.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/rules/webserver_down.yml` & `ansible_rulebook-0.9.4/tests/rules/webserver_down.yml`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/file.py` & `ansible_rulebook-0.9.4/tests/sources/file.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/infrange.py` & `ansible_rulebook-0.9.4/tests/sources/infrange.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/log_scraper.py` & `ansible_rulebook-0.9.4/tests/sources/log_scraper.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/ping.py` & `ansible_rulebook-0.9.4/tests/sources/ping.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/process_check.py` & `ansible_rulebook-0.9.4/tests/sources/process_check.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/replay.py` & `ansible_rulebook-0.9.4/tests/sources/replay.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/template.py` & `ansible_rulebook-0.9.4/tests/sources/template.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/sources/url_check.py` & `ansible_rulebook-0.9.4/tests/sources/url_check.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_ansible_events.py` & `ansible_rulebook-0.9.4/tests/test_ansible_events.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_ast.py` & `ansible_rulebook-0.9.4/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_collection.py` & `ansible_rulebook-0.9.4/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_conditions.py` & `ansible_rulebook-0.9.4/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_engine.py` & `ansible_rulebook-0.9.4/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_examples.py` & `ansible_rulebook-0.9.4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_rules.py` & `ansible_rulebook-0.9.4/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `ansible_rulebook-0.9.3/tests/test_simple.yml` & `ansible_rulebook-0.9.4/tests/test_simple.yml`

 * *Files identical despite different names*

