# Comparing `tmp/talisman-tools-0.3.1.tar.gz` & `tmp/talisman-tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-tools-0.3.1.tar", last modified: Mon Mar 27 12:26:10 2023, max compression
+gzip compressed data, was "talisman-tools-0.4.0.tar", last modified: Wed Apr 12 08:26:35 2023, max compression
```

## Comparing `talisman-tools-0.3.1.tar` & `talisman-tools-0.4.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:10.002480 talisman-tools-0.3.1/
--rw-r--r--   0 root         (0) root         (0)      739 2023-03-27 12:26:10.002480 talisman-tools-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-03-27 11:25:03.000000 talisman-tools-0.3.1/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-27 12:26:10.002480 talisman-tools-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1571 2023-03-27 11:25:03.000000 talisman-tools-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/arguments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/arguments/kb.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/arguments/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/arguments/reader.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/arguments/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/analyse_ambiguity/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/analyse_ambiguity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2696 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/analyse_ambiguity/action.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/analyse_ambiguity/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/convert/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/convert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/convert/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/dataset/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/kb/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/kb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4289 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/kb/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/kb/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/model/
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/model/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/model/commands/check_performance/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/check_performance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/check_performance/action.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/check_performance/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/model/commands/configure/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/configure/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5858 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1948 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/coreference.py
--rw-rw-rw-   0 root         (0) root         (0)     5287 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/disambiguation_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     8950 2023-03-24 09:57:01.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)    15234 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/model/commands/process/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/process/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/model/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/arguments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1622 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/arguments/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/methods/load.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-03-27 11:25:03.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3564 2023-03-27 11:25:03.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/methods/process.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/methods/update.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-03-27 11:25:03.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2627 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/servers/server_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/commands/subparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/commands/train/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/commands/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-03-24 09:57:01.000000 talisman-tools-0.3.1/talisman_tools/commands/train/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2023-03-24 09:57:01.000000 talisman-tools-0.3.1/talisman_tools/commands/train/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/configure/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5290 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/configure/configure.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/configure/wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/configure/wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/configure/wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/configure/wrapper/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools/helper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-27 12:26:08.000000 talisman-tools-0.3.1/talisman_tools/helper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-03-27 10:53:03.000000 talisman-tools-0.3.1/talisman_tools/helper/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-27 10:53:03.000000 talisman-tools-0.3.1/talisman_tools/helper/env.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-03-27 10:53:03.000000 talisman-tools-0.3.1/talisman_tools/helper/multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/parser_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:10.002480 talisman-tools-0.3.1/talisman_tools/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-03-24 09:57:01.000000 talisman-tools-0.3.1/talisman_tools/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/kb.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-03-24 09:57:01.000000 talisman-tools-0.3.1/talisman_tools/plugin/reader.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/tdm.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/plugin/wrapper_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/talisman.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-03-20 09:52:48.000000 talisman-tools-0.3.1/talisman_tools/talisman_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-27 12:26:09.998480 talisman-tools-0.3.1/talisman_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      739 2023-03-27 12:26:09.000000 talisman-tools-0.3.1/talisman_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4263 2023-03-27 12:26:09.000000 talisman-tools-0.3.1/talisman_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-27 12:26:09.000000 talisman-tools-0.3.1/talisman_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-03-27 12:26:09.000000 talisman-tools-0.3.1/talisman_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      220 2023-03-27 12:26:09.000000 talisman-tools-0.3.1/talisman_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-03-27 12:26:09.000000 talisman-tools-0.3.1/talisman_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)      739 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-04-12 08:18:57.000000 talisman-tools-0.4.0/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-12 08:18:57.000000 talisman-tools-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.482123 talisman-tools-0.4.0/talisman_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/arguments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/arguments/kb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/arguments/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/arguments/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/arguments/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/analyse_ambiguity/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/analyse_ambiguity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/analyse_ambiguity/action.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/analyse_ambiguity/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/convert/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/convert/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/dataset/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/kb/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/kb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4289 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/kb/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/kb/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/model/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/model/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools/commands/model/commands/check_performance/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/check_performance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/check_performance/action.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/check_performance/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/model/commands/configure/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/configure/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5858 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/coreference.py
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/disambiguation_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     8950 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)    15234 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/model/commands/process/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/process/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/model/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/arguments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/arguments/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/methods/load.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2023-04-12 08:18:57.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.490124 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2023-04-12 08:18:57.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/methods/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/methods/update.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-12 08:18:57.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/servers/server_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      904 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/subparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/talisman_tools/commands/train/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/commands/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/train/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/commands/train/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/talisman_tools/configure/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5290 2023-04-04 13:41:47.000000 talisman-tools-0.4.0/talisman_tools/configure/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/configure/wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/talisman_tools/configure/wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/configure/wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/configure/wrapper/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/talisman_tools/helper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:30.000000 talisman-tools-0.4.0/talisman_tools/helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/helper/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/helper/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/helper/multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/parser_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.494124 talisman-tools-0.4.0/talisman_tools/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1144 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/kb.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/tdm.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/plugin/wrapper_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/talisman.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2023-04-01 17:58:03.000000 talisman-tools-0.4.0/talisman_tools/talisman_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:35.486124 talisman-tools-0.4.0/talisman_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2023-04-12 08:26:35.000000 talisman-tools-0.4.0/talisman_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-04-12 08:26:35.000000 talisman-tools-0.4.0/talisman_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 08:26:35.000000 talisman-tools-0.4.0/talisman_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-04-12 08:26:35.000000 talisman-tools-0.4.0/talisman_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-04-12 08:26:35.000000 talisman-tools-0.4.0/talisman_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-12 08:26:35.000000 talisman-tools-0.4.0/talisman_tools.egg-info/top_level.txt
```

### Comparing `talisman-tools-0.3.1/PKG-INFO` & `talisman-tools-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-tools
-Version: 0.3.1
+Version: 0.4.0
 Summary: Talisman applications
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-tools-0.3.1/setup.py` & `talisman-tools-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description_content_type="text/markdown",
     author='ISPRAS Talisman NLP team',
     author_email='modis@ispras.ru',
     maintainer='Vladimir Mayorov',
     maintainer_email='vmayorov@ispras.ru',
     packages=find_packages(include=['talisman_tools', 'talisman_tools.*']),
     install_requires=[
-        'talisman-interfaces~=0.3.2',
+        'talisman-interfaces',
         'fastapi>=0.73.0', 'python-multipart>=0.0.5', 'requests>=2.22.0', 'uvicorn>=0.13.3', 'jsonformatter>=0.3.0', 'starlette', 'anyio'
     ],
     extras_require={
         'logstash': ['python3-logstash>=0.4.80'],
         'evaluate': ['numpy', 'scipy'],
         'cuda_metrics': ['torch']
     },
```

### Comparing `talisman-tools-0.3.1/talisman_tools/arguments/kb.py` & `talisman-tools-0.4.0/talisman_tools/arguments/kb.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/arguments/processor.py` & `talisman-tools-0.4.0/talisman_tools/arguments/processor.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/arguments/reader.py` & `talisman-tools-0.4.0/talisman_tools/arguments/reader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/arguments/serializer.py` & `talisman-tools-0.4.0/talisman_tools/arguments/serializer.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/analyse_ambiguity/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/analyse_ambiguity/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/analyse_ambiguity/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/analyse_ambiguity/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/convert/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/convert/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/dataset/commands/subparsers.py` & `talisman-tools-0.4.0/talisman_tools/commands/dataset/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/dataset/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/dataset/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/kb/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/kb/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/kb/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/kb/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/check_performance/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/check_performance/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/check_performance/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/check_performance/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/configure/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/configure/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/coreference.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/coreference.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/disambiguation_quality.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/disambiguation_quality.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/evaluation.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/evaluation.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/metrics.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/evaluate/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/evaluate/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/process/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/process/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/commands/subparsers.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/model/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/model/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/arguments/server.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/arguments/server.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/methods/load.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/methods/load.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/loader/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/loader/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     app = FastAPI(title="talisman-ie REST server", description=f"talisman-ie REST server for {processor}")
 
     register_process_docs(
         app=app,
         endpoint='/',
         processor=processor,
         document_model=document_model,
-        output_future=args.future,
         logger=logger
     )
 
     if isinstance(processor, AbstractUpdatableModel):
         register_update(app, processor, processor.update_type)
 
     for endpoint, register in EndpointPlugins.flattened.items():
```

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/methods/process.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/methods/process.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import logging
 from functools import partial
 from logging import Logger
 from operator import itemgetter
 from typing import Any, List, Optional, Sequence, Tuple, Type, Union
 
 from fastapi import FastAPI, HTTPException, Request
-from tdm.abstract.datamodel import AbstractTalismanDocument as LegacyTalismanDocument
-from tdm.future.abstract.datamodel import TalismanDocument
-from tdm.future.json_schema.document import TalismanDocumentModel as FutureDocumentModel
 from tdm.json_schema import TalismanDocumentModel
 
 from talisman_tools.commands.servers.server_helper import log_debug_data
 from talisman_tools.helper.concurrency import execute_concurrently
 from tp_interfaces.abstract import AbstractDocumentProcessor, ImmutableBaseModel
 from tp_interfaces.helpers.batch import AbstractModelInput, batch_process_inputs
 from tp_interfaces.logging.context import update_log_extras
@@ -20,52 +17,36 @@
 
 
 def register_process_docs(
         app: FastAPI,
         endpoint: str,
         processor: AbstractDocumentProcessor,
         document_model: Type[TalismanDocumentModel],
-        output_future: bool = False,
         logger: Logger = _logger
 ):
     config_model = processor.config_type
 
-    if output_future:
-        def output_doc_model(doc: TalismanDocument) -> FutureDocumentModel:
-            if not isinstance(doc, TalismanDocument):
-                raise ValueError(f"inappropriate output document type")
-            return FutureDocumentModel.serialize(doc)
-
-        output_model = FutureDocumentModel
-    else:
-        def output_doc_model(doc: LegacyTalismanDocument) -> TalismanDocumentModel:
-            if not isinstance(doc, LegacyTalismanDocument):
-                raise ValueError(f"inappropriate output document type")
-            return document_model.build(doc)
-
-        output_model = document_model
-
     class ModelInput(AbstractModelInput):
         message: document_model
         config: config_model
 
         def get_message(self) -> Any:
             return self.message
 
         def get_config(self) -> Optional[ImmutableBaseModel]:
             return self.config
 
     def process_with_config(messages: Sequence[TalismanDocumentModel], config: ImmutableBaseModel) \
-            -> Tuple[output_model, ...]:
+            -> Tuple[TalismanDocumentModel, ...]:
         docs = tuple(message.to_doc() for message in messages)
         with update_log_extras(doc_id=[doc.doc_id for doc in docs]):
             output_docs = processor.process_docs(docs, config)
-            return tuple(output_doc_model(output_doc) for output_doc in output_docs)
+            return tuple(document_model.build(output_doc) for output_doc in output_docs)
 
-    @app.post(endpoint, response_model=Union[List[output_model], output_model], response_model_exclude_none=True)
+    @app.post(endpoint, response_model=Union[List[TalismanDocumentModel], TalismanDocumentModel], response_model_exclude_none=True)
     async def process(request: Request, *, messages: Union[List[ModelInput], ModelInput]):
         response_post_processor = lambda x: x
         if not isinstance(messages, list):
             messages = [messages]
             response_post_processor = itemgetter(0)
 
         with update_log_extras(doc_id=[message.message.id for message in messages]):
```

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/methods/update.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/methods/update.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/processor/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/processor/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from talisman_tools.plugin import TDMPlugins
 from talisman_tools.plugin.cli import add_extra_cli_arguments
 
 
 def configure_processor_parser(parser: ArgumentParser) -> None:
     kb_factory = get_kb_factory(parser)
     parser.add_argument('-dm', type=str, choices=set(TDMPlugins.plugins), metavar='<document model>')
-    parser.add_argument('-future', action='store_true', default=False)
     processor_factory = get_processor_factory(parser)
 
     extra_actions = add_extra_cli_arguments(parser, 'processor')
 
     def get_action() -> Callable[[Namespace], FastAPI]:
         def action_with_extra(args: Namespace) -> FastAPI:
             for action in extra_actions:
```

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/commands/subparsers.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/servers/server_helper.py` & `talisman-tools-0.4.0/talisman_tools/commands/servers/server_helper.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/subparsers.py` & `talisman-tools-0.4.0/talisman_tools/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/train/action.py` & `talisman-tools-0.4.0/talisman_tools/commands/train/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/commands/train/parser.py` & `talisman-tools-0.4.0/talisman_tools/commands/train/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/configure/configure.py` & `talisman-tools-0.4.0/talisman_tools/configure/configure.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/configure/wrapper/actions.py` & `talisman-tools-0.4.0/talisman_tools/configure/wrapper/actions.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/helper/concurrency.py` & `talisman-tools-0.4.0/talisman_tools/helper/concurrency.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/helper/env.py` & `talisman-tools-0.4.0/talisman_tools/helper/env.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/helper/multiprocessing.py` & `talisman-tools-0.4.0/talisman_tools/helper/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/__init__.py` & `talisman-tools-0.4.0/talisman_tools/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/abstract.py` & `talisman-tools-0.4.0/talisman_tools/plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/cli.py` & `talisman-tools-0.4.0/talisman_tools/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/endpoint.py` & `talisman-tools-0.4.0/talisman_tools/plugin/endpoint.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/reader.py` & `talisman-tools-0.4.0/talisman_tools/plugin/reader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/serializer.py` & `talisman-tools-0.4.0/talisman_tools/plugin/serializer.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/plugin/wrapper_actions.py` & `talisman-tools-0.4.0/talisman_tools/plugin/wrapper_actions.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/talisman.py` & `talisman-tools-0.4.0/talisman_tools/talisman.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools/talisman_logging.py` & `talisman-tools-0.4.0/talisman_tools/talisman_logging.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.3.1/talisman_tools.egg-info/PKG-INFO` & `talisman-tools-0.4.0/talisman_tools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-tools
-Version: 0.3.1
+Version: 0.4.0
 Summary: Talisman applications
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-tools-0.3.1/talisman_tools.egg-info/SOURCES.txt` & `talisman-tools-0.4.0/talisman_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

