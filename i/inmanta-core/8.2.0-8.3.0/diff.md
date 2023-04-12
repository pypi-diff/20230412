# Comparing `tmp/inmanta-core-8.2.0.tar.gz` & `tmp/inmanta-core-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmanta-core-8.2.0.tar", last modified: Thu Feb  9 10:00:27 2023, max compression
+gzip compressed data, was "inmanta-core-8.3.0.tar", last modified: Wed Apr 12 07:26:35 2023, max compression
```

## Comparing `inmanta-core-8.2.0.tar` & `inmanta-core-8.3.0.tar`

### file list

```diff
@@ -1,245 +1,252 @@
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.838055 inmanta-core-8.2.0/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/LICENSE
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      311 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/MANIFEST.in
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3182 2023-02-09 10:00:27.838055 inmanta-core-8.2.0/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2225 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/README.md
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.814053 inmanta-core-8.2.0/misc/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       31 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/extensions.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      402 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/inmanta-agent.service
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      333 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/inmanta-server.service
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7608 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/inmanta-workon-register.sh
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2906 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/inmanta.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12162 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/inmanta.lang
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1205 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/inmanta.vim
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      141 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/misc/logrotation_config
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1432 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/pyproject.toml
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      918 2023-02-09 10:00:27.839054 inmanta-core-8.2.0/setup.cfg
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3306 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/setup.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.812053 inmanta-core-8.2.0/src/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.817054 inmanta-core-8.2.0/src/inmanta/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      914 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/__init__.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.818054 inmanta-core-8.2.0/src/inmanta/agent/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      738 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    58982 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/agent.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10115 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/cache.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4634 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    42405 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/handler.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.818054 inmanta-core-8.2.0/src/inmanta/agent/io/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2815 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/io/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    19870 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/io/local.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6362 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/io/remote.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3395 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/agent/reporting.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    31738 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/app.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.819054 inmanta-core-8.2.0/src/inmanta/ast/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    30203 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7103 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/attribute.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6355 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/blocks.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.819054 inmanta-core-8.2.0/src/inmanta/ast/constraint/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/constraint/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17187 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/constraint/expression.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18701 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/entity.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2783 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/export.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.820054 inmanta-core-8.2.0/src/inmanta/ast/statements/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    22445 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/statements/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    21870 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/statements/assign.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12251 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/statements/call.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    24368 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/statements/define.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    37332 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/statements/generator.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    20697 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/type.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12047 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/ast/variables.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2985 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/command.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.820054 inmanta-core-8.2.0/src/inmanta/compiler/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    13889 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1963 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1110 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/data.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.820054 inmanta-core-8.2.0/src/inmanta/compiler/help/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/help/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8327 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/help/explainer.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.821054 inmanta-core-8.2.0/src/inmanta/compiler/help/templates/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      235 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/help/templates/index_collision.j2
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3604 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      733 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    20658 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9187 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/const.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.821054 inmanta-core-8.2.0/src/inmanta/data/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   224939 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/data/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    43652 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/data/dataview.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    21756 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/data/model.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12205 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/data/schema.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.822054 inmanta-core-8.2.0/src/inmanta/db/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5462 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/util.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.825054 inmanta-core-8.2.0/src/inmanta/db/versions/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12131 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v1.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1737 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v17.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1393 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v2.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2443 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202105170.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      915 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202106080.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1247 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202106210.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1826 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202109100.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202111260.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1581 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202203140.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2200 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202203160.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      910 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202205250.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202206290.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      948 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202208180.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1881 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202208190.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      976 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202209090.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3957 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202209130.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      861 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202209160.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2919 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202211230.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1430 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202212010.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1494 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202301100.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      924 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202301110.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      977 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202301120.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      929 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202301160.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      896 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202301170.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1313 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v202301190.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1471 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v3.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3556 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v4.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1529 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v5.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1043 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v6.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1558 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/db/versions/v7.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    16438 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/deploy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2694 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/docstring_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    56383 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/env.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.826054 inmanta-core-8.2.0/src/inmanta/execute/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/__init__.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.826054 inmanta-core-8.2.0/src/inmanta/execute/dataflow/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    41029 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/dataflow/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9488 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/dataflow/datatrace.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7405 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/dataflow/graphic.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7152 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/dataflow/root_cause.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8478 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/proxy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    46717 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/runtime.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    30085 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/scheduler.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1807 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/tracking.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1451 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/execute/util.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25455 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/export.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5488 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/file_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    24386 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/loader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    35363 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/main.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9146 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/model.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   140687 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/module.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    81102 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/moduletool.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.827054 inmanta-core-8.2.0/src/inmanta/parser/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2934 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/parser/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5591 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/parser/cache.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   505683 2023-02-09 10:00:17.000000 inmanta-core-8.2.0/src/inmanta/parser/parser.out
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    66421 2023-02-09 10:00:17.000000 inmanta-core-8.2.0/src/inmanta/parser/parsetab.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1563 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/parser/pickle.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7799 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/parser/plyInmantaLex.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    36122 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/parser/plyInmantaParser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    21187 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/plugins.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5509 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/postgresproc.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      734 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/profile_mem.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.828054 inmanta-core-8.2.0/src/inmanta/protocol/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3131 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    40283 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/common.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8549 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/decorators.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    17519 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/endpoints.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4455 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/exceptions.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    32908 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/methods.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    59046 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/methods_v2.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.829054 inmanta-core-8.2.0/src/inmanta/protocol/openapi/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/openapi/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    19132 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/openapi/converter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8343 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/openapi/model.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.829054 inmanta-core-8.2.0/src/inmanta/protocol/rest/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    21717 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/rest/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6064 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/rest/client.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    13872 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/rest/server.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2158 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/protocol/return_value_meta.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/py.typed
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6273 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/reporter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    23112 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/resources.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.830054 inmanta-core-8.2.0/src/inmanta/server/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1338 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    56391 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/agentmanager.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9731 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/bootloader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      688 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/compilerservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    10111 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7314 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/diff.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7672 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/extensions.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    27495 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/protocol.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7036 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/server.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.832054 inmanta-core-8.2.0/src/inmanta/server/services/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5702 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/codeservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    38106 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/compilerservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4850 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/databaseservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11640 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/dryrunservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    25390 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/environment_metrics_service.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    27831 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/environmentservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6242 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/fileservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4551 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/metricservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7970 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/notificationservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    48458 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/orchestrationservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    13605 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/paramservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6154 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/projectservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    43300 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/services/resourceservice.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11714 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/server/validate_filter.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      865 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/stable_api.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2927 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/types.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    24125 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/util.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6487 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta/warnings.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.833054 inmanta-core-8.2.0/src/inmanta_core.egg-info/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3182 2023-02-09 10:00:27.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6618 2023-02-09 10:00:27.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-09 10:00:27.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       76 2023-02-09 10:00:27.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-02-09 10:00:09.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      577 2023-02-09 10:00:27.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/requires.txt
--rw-rw-r--   0 jenkins    (989) jenkins    (987)       36 2023-02-09 10:00:27.000000 inmanta-core-8.2.0/src/inmanta_core.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.812053 inmanta-core-8.2.0/src/inmanta_ext/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.833054 inmanta-core-8.2.0/src/inmanta_ext/core/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta_ext/core/__init__.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2163 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta_ext/core/extension.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.812053 inmanta-core-8.2.0/src/inmanta_plugins/
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.833054 inmanta-core-8.2.0/src/inmanta_plugins/1/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/src/inmanta_plugins/1/__init__.py
-drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-02-09 10:00:27.838055 inmanta-core-8.2.0/tests/
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7790 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_2way_protocol.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     7692 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_agent.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    55229 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_agent_manager.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    16768 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_app.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12682 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_app_cli.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    12792 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_cache.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18793 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_cli.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4624 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_compilation.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4819 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_compiler_entrypoints.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11567 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_config.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1301 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_const.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)   116677 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_data.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8116 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_data_concurrency.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4378 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_data_model.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3912 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_deploy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5151 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_docs_snippets.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3047 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_docstring_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    27232 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_env.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    21255 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_export.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     9103 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_extension_loading.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2789 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_file_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6670 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_handler.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     4111 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_import_entry_points.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5982 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_influxdbreporting.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     8541 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_io.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     5352 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_jwt.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18512 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_loader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    54161 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_module_loader.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    18976 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_modules.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    29095 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_openapi.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)      988 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_param.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    62820 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_parser.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     6299 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_postgres.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     2110 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_postgres_proc.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    22771 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_project.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3346 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_projectmetadata.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    76126 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_protocol.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3038 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_proxy.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    11167 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_resource.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    53410 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_server.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     3664 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_type.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)    16966 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tests/test_util.py
--rw-rw-r--   0 jenkins    (989) jenkins    (987)     1924 2023-02-09 09:57:10.000000 inmanta-core-8.2.0/tox.ini
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.434978 inmanta-core-8.3.0/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10174 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/LICENSE
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      311 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/MANIFEST.in
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3195 2023-04-12 07:26:35.434978 inmanta-core-8.3.0/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2238 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/README.md
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.409977 inmanta-core-8.3.0/misc/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       31 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/extensions.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      402 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/inmanta-agent.service
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      333 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/inmanta-server.service
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8762 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/inmanta-workon-register.sh
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2906 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/inmanta.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12162 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/inmanta.lang
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1256 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/inmanta.vim
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      141 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/misc/logrotation_config
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1432 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/pyproject.toml
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      918 2023-04-12 07:26:35.434978 inmanta-core-8.3.0/setup.cfg
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3393 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/setup.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.407977 inmanta-core-8.3.0/src/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.412977 inmanta-core-8.3.0/src/inmanta/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      914 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/__init__.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.413977 inmanta-core-8.3.0/src/inmanta/agent/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      738 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    59551 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/agent.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10115 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/cache.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4634 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    42404 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/handler.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.413977 inmanta-core-8.3.0/src/inmanta/agent/io/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2815 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/io/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    19884 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/io/local.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6362 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/io/remote.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3395 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/agent/reporting.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    32322 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/app.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.414977 inmanta-core-8.3.0/src/inmanta/ast/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    32260 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7103 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/attribute.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6354 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/blocks.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.414977 inmanta-core-8.3.0/src/inmanta/ast/constraint/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/constraint/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17187 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/constraint/expression.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    19266 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/entity.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2783 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/export.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.415977 inmanta-core-8.3.0/src/inmanta/ast/statements/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    22464 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/statements/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    21894 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/statements/assign.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12250 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/statements/call.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    24146 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/statements/define.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    40816 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/statements/generator.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    20775 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/type.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12520 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/ast/variables.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2985 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/command.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.415977 inmanta-core-8.3.0/src/inmanta/compiler/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    14012 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1963 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1110 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/data.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.416977 inmanta-core-8.3.0/src/inmanta/compiler/help/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/help/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8327 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/help/explainer.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.416977 inmanta-core-8.3.0/src/inmanta/compiler/help/templates/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      235 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/help/templates/index_collision.j2
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3604 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      733 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    20756 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9233 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/const.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.416977 inmanta-core-8.3.0/src/inmanta/data/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   240602 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/data/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    44266 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/data/dataview.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    21310 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/data/model.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12206 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/data/schema.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.417977 inmanta-core-8.3.0/src/inmanta/db/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8702 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/util.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.421977 inmanta-core-8.3.0/src/inmanta/db/versions/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12123 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v1.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1737 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v17.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1393 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v2.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2443 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202105170.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      915 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202106080.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1247 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202106210.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1826 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202109100.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202111260.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1581 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202203140.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2200 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202203160.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      910 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202205250.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      979 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202206290.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      948 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202208180.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1881 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202208190.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      976 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202209090.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3957 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202209130.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      861 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202209160.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2919 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202211230.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1430 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202212010.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1494 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202301100.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      924 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202301110.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      977 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202301120.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      929 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202301160.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      896 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202301170.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1313 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202301190.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      860 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202302200.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1036 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202302270.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      825 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202303070.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1936 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v202303071.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1471 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v3.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3556 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v4.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1529 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v5.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1043 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v6.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1558 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/db/versions/v7.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    16471 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/deploy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2694 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/docstring_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    56412 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/env.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.421977 inmanta-core-8.3.0/src/inmanta/execute/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/__init__.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.422978 inmanta-core-8.3.0/src/inmanta/execute/dataflow/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    41029 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/dataflow/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9488 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/dataflow/datatrace.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7405 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/dataflow/graphic.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7152 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/dataflow/root_cause.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8478 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/proxy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    49389 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/runtime.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    30598 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/scheduler.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1807 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/tracking.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1451 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/execute/util.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25617 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/export.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5488 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/file_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    24386 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/loader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    35363 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/main.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9144 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/model.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   141814 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/module.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    82419 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/moduletool.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.423977 inmanta-core-8.3.0/src/inmanta/parser/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2934 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/parser/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5591 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/parser/cache.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   505683 2023-04-12 07:26:25.000000 inmanta-core-8.3.0/src/inmanta/parser/parser.out
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    66421 2023-04-12 07:26:25.000000 inmanta-core-8.3.0/src/inmanta/parser/parsetab.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1563 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/parser/pickle.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7799 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/parser/plyInmantaLex.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    36122 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/parser/plyInmantaParser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    21362 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/plugins.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5509 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/postgresproc.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      734 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/profile_mem.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.424978 inmanta-core-8.3.0/src/inmanta/protocol/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3131 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    41952 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/common.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8807 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/decorators.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17519 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/endpoints.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4455 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/exceptions.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    33273 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/methods.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    61334 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/methods_v2.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.424978 inmanta-core-8.3.0/src/inmanta/protocol/openapi/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/openapi/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    20514 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/openapi/converter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9049 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/openapi/model.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.424978 inmanta-core-8.3.0/src/inmanta/protocol/rest/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    21717 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/rest/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6064 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/rest/client.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    13836 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/rest/server.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2158 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/protocol/return_value_meta.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/py.typed
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6273 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/reporter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    23291 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/resources.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.426978 inmanta-core-8.3.0/src/inmanta/server/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1363 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    55982 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/agentmanager.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9730 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/bootloader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      688 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/compilerservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    10223 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7314 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/diff.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7672 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/extensions.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27495 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/protocol.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7036 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/server.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.427978 inmanta-core-8.3.0/src/inmanta/server/services/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5702 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/codeservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    38105 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/compilerservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4850 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/databaseservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11640 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/dryrunservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25390 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/environment_metrics_service.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27904 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/environmentservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6420 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/fileservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4551 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/metricservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7970 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/notificationservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    64468 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/orchestrationservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    13562 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/paramservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6280 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/projectservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    45518 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/resourceservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4852 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/services/userservice.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11714 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/server/validate_filter.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      865 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/stable_api.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2927 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/types.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6908 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/user_setup.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    25266 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/util.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6487 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta/warnings.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.428978 inmanta-core-8.3.0/src/inmanta_core.egg-info/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3195 2023-04-12 07:26:35.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6863 2023-04-12 07:26:35.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 07:26:35.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      129 2023-04-12 07:26:35.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/entry_points.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)        1 2023-04-12 07:26:17.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/not-zip-safe
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      589 2023-04-12 07:26:35.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/requires.txt
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)       36 2023-04-12 07:26:35.000000 inmanta-core-8.3.0/src/inmanta_core.egg-info/top_level.txt
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.407977 inmanta-core-8.3.0/src/inmanta_ext/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.428978 inmanta-core-8.3.0/src/inmanta_ext/core/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta_ext/core/__init__.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2238 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta_ext/core/extension.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.407977 inmanta-core-8.3.0/src/inmanta_plugins/
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.429978 inmanta-core-8.3.0/src/inmanta_plugins/1/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      627 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/src/inmanta_plugins/1/__init__.py
+drwxrwxr-x   0 jenkins    (989) jenkins    (987)        0 2023-04-12 07:26:35.434978 inmanta-core-8.3.0/tests/
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7790 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_2way_protocol.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7692 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_agent.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    54792 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_agent_manager.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18854 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_app.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12682 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_app_cli.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    12791 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_cache.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18791 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_cli.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4624 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_compilation.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     7682 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_compiler_entrypoints.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11564 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_config.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1300 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_const.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)   120276 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_data.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8212 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_data_concurrency.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3426 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_data_model.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3912 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_deploy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5151 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_docs_snippets.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3047 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_docstring_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    27232 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_env.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    21255 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_export.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     9102 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_extension_loading.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2789 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_file_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6670 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_handler.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     4111 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_import_entry_points.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5982 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_influxdbreporting.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     8541 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_io.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5352 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_jwt.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18512 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_loader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    54161 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_module_loader.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    18976 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_modules.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    33059 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_openapi.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)      988 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_param.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    62820 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_parser.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     6299 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_postgres.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     2110 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_postgres_proc.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    24509 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_project.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3805 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_projectmetadata.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    77912 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_protocol.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3038 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_proxy.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    11162 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_resource.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    59544 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_server.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     3664 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_type.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     5678 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_usersetup.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)    17775 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tests/test_util.py
+-rw-rw-r--   0 jenkins    (989) jenkins    (987)     1924 2023-04-12 07:23:21.000000 inmanta-core-8.3.0/tox.ini
```

### Comparing `inmanta-core-8.2.0/LICENSE` & `inmanta-core-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/PKG-INFO` & `inmanta-core-8.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-core
-Version: 8.2.0
+Version: 8.3.0
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta-core
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
@@ -49,15 +49,15 @@
    approach and the configuration model using dependencies.
 
 Currently, the Inmanta project is mainly developed and maintained by Inmanta NV.
 
 ## Links
 
 * [Documentation](https://docs.inmanta.com/community/latest/)
-* [Quickstart](https://github.com/inmanta/quickstart-docker)
+* [Quickstart](https://docs.inmanta.com/community/latest/quickstart.html)
 
 ## Install
 
 * [Install Guide](https://docs.inmanta.com/community/latest/install.html)
 
 ## Running the tests using tox
```

### Comparing `inmanta-core-8.2.0/README.md` & `inmanta-core-8.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
    approach and the configuration model using dependencies.
 
 Currently, the Inmanta project is mainly developed and maintained by Inmanta NV.
 
 ## Links
 
 * [Documentation](https://docs.inmanta.com/community/latest/)
-* [Quickstart](https://github.com/inmanta/quickstart-docker)
+* [Quickstart](https://docs.inmanta.com/community/latest/quickstart.html)
 
 ## Install
 
 * [Install Guide](https://docs.inmanta.com/community/latest/install.html)
 
 ## Running the tests using tox
```

### Comparing `inmanta-core-8.2.0/misc/inmanta-workon-register.sh` & `inmanta-core-8.3.0/misc/inmanta-workon-register.sh`

 * *Files 10% similar despite different names*

```diff
@@ -140,14 +140,20 @@
         command ls -1 "$envs_dir" 2> /dev/null
     fi
     return 0
 }
 
 
 function __inmanta_workon_activate {
+    # Check user
+    declare current_user=$(whoami)
+    if [[ "${current_user}" != "root" && "${current_user}" != ${INMANTA_USER:-inmanta} ]]; then
+        echo "WARNING: The inmanta-workon tool should be run as either root or the inmanta user to have write access (to be able to run pip install or inmanta project install)." >&2
+    fi
+
     # Activates the environment's venv and registers the deactivate function
 
     declare env_name="$1"
     declare env_id="$2"
     declare envs_dir="$3"
 
     if [ ! -d "$envs_dir/$env_id" ]; then
@@ -164,18 +170,28 @@
         return 1
     fi
 
     # if we are in an active venv, deactivate it first: restores PS1 and triggers our custom deactivate logic if it's an inmanta venv
     declare -F deactivate > /dev/null && deactivate
     # store PS1 before sourcing activate because we don't care about virtualenv's modifications
     declare OLD_PS1="$PS1"
+
+    # store INMANTA_CONFIG_ENVIRONMENT before activation
+    if [ -n "${INMANTA_CONFIG_ENVIRONMENT:-}" ] ; then
+        _OLD_INMANTA_CONFIG_ENVIRONMENT="${INMANTA_CONFIG_ENVIRONMENT:-}"
+    fi
+    export INMANTA_CONFIG_ENVIRONMENT=$env_id
+
     source "$activate"
     export PS1="($env_name) $OLD_PS1"
 
+
     eval 'inmanta () { python3 -m inmanta.app "$@"; }' # workaround for #4259
+
+    echo "WARNING: Make sure you exit the current environment by running the 'deactivate' command rather than simply exiting the shell. This ensures the proper permission checks are performed." >&2
     __inmanta_workon_register_deactivate
 }
 
 
 function __inmanta_workon_register_deactivate {
     # Registers a custom deactivate function. Modified from virtualenvwrapper's implementation
 
@@ -191,17 +207,26 @@
         declare user=${INMANTA_USER:-inmanta}
 
         # Call the original function.
         virtualenv_deactivate "$1"
         unset -f inmanta >/dev/null 2>&1
         # no need to restore PS1 because virtualenv_deactivate already does that
 
+        if [ -n "${_OLD_INMANTA_CONFIG_ENVIRONMENT:-}" ] ; then
+            # Another env was active prior to inmanta-workon call: restore INMANTA_CONFIG_ENVIRONMENT to its old value
+            INMANTA_CONFIG_ENVIRONMENT="${_OLD_INMANTA_CONFIG_ENVIRONMENT:-}"
+            export INMANTA_CONFIG_ENVIRONMENT
+            unset _OLD_INMANTA_CONFIG_ENVIRONMENT
+        else
+            unset INMANTA_CONFIG_ENVIRONMENT
+        fi
+
         ownership_issues=$(find "$inmanta_env_dir" \! -user "$user" -print -quit)
         if [ -n "$ownership_issues" ]; then
-            echo "WARNING: Some files in the environment are not owned by the $user user. To fix this, run \`find '\''$inmanta_env_dir'\'' ! -user '\''$user'\'' -exec chown '\''$user'\'':'\''$user'\'' {} \;\` as root." >&2
+            echo "WARNING: Some files in the environment are not owned by the $user user. To fix this, run \`chown -R $user:$user '\''$inmanta_env_dir'\''\` as root." >&2
         fi
 
         if [ ! "$1" = "nondestructive" ]; then
             # Remove this function
             unset -f virtualenv_deactivate >/dev/null 2>&1
             unset -f deactivate >/dev/null 2>&1
         fi
```

### Comparing `inmanta-core-8.2.0/misc/inmanta.cfg` & `inmanta-core-8.3.0/misc/inmanta.cfg`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/misc/inmanta.lang` & `inmanta-core-8.3.0/misc/inmanta.lang`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/misc/inmanta.vim` & `inmanta-core-8.3.0/misc/inmanta.vim`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 if exists("b:current_syntax")
     finish
 endif
 
 syn region Comment start="#" end="$" contains=Todo
 syn region String start="\"" skip="\\\"" end="\""
-syn region String start="\"\"\"" end="\"\"\""
+syn region String start="'" skip="\\'" end="'"
+syn region String start="\"\{3,5}" end="\"\{3,5}"
 syn region regex start="/" skip="\\/" end="/"
 syn match number "\<[0123456789]*\>'\@!"
 
 " Constant
 syn keyword Constant null
 syn keyword Boolean true false
```

### Comparing `inmanta-core-8.2.0/pyproject.toml` & `inmanta-core-8.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/setup.cfg` & `inmanta-core-8.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/setup.py` & `inmanta-core-8.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "asyncpg~=0.25,<0.28",
     "click-plugins~=1.0",
     # click has been known to publish non-backwards compatible minors in the past (removed deprecated code in 8.1.0)
     "click>=8.0,<8.2",
     "colorlog~=6.4",
     "cookiecutter>=1,<3",
     "crontab>=0.23,<2.0",
-    "cryptography>=36,<40",
+    "cryptography>=36,<41",
     # docstring-parser has been known to publish non-backwards compatible minors in the past
     "docstring-parser>=0.10,<0.16",
     "email-validator~=1.0",
     "execnet~=1.0",
     "importlib_metadata>=4,<7",
     "jinja2~=3.0",
     "more-itertools>=8,<10",
@@ -23,14 +23,15 @@
     # pip>=21.3 required for editable pyproject.toml + setup.cfg based install support
     "pip>=21.3",
     "ply~=3.0",
     # Exclude pre-release due to https://github.com/samuelcolvin/pydantic/issues/3546
     "pydantic~=1.0,!=1.9.0a1",
     "pyformance~=0.4",
     "PyJWT~=2.0",
+    "pynacl~=1.5",
     "python-dateutil~=2.0",
     "pyyaml~=6.0",
     "texttable~=1.0",
     "tornado~=6.0",
     "typing_inspect~=0.7",
     "build~=0.7",
     "ruamel.yaml~=0.17",
@@ -39,15 +40,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "8.2.0"
+version = "8.3.0"
 
 setup(
     version=version,
     python_requires=">=3.9",  # also update classifiers
     # Meta data
     name="inmanta-core",
     description="Inmanta deployment tool",
@@ -86,10 +87,11 @@
         "pytest-inmanta-extensions": [f"pytest-inmanta-extensions~={version}.0.dev"],
         "datatrace": ["graphviz"],
     },
     entry_points={
         "console_scripts": [
             "inmanta-cli = inmanta.main:main",
             "inmanta = inmanta.app:app",
+            "inmanta-initial-user-setup = inmanta.user_setup:main",
         ],
     },
 )
```

### Comparing `inmanta-core-8.2.0/src/inmanta/__init__.py` & `inmanta-core-8.3.0/src/inmanta/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 
-COMPILER_VERSION = "2023.1"
+COMPILER_VERSION = "2023.2"
 RUNNING_TESTS = False
 """
     This is enabled/disabled by the test suite when tests are run.
     This variable is used to disable certain features that shouldn't run during tests.
 """
 
 if __name__ == "__main__":
```

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/__init__.py` & `inmanta-core-8.3.0/src/inmanta/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/agent.py` & `inmanta-core-8.3.0/src/inmanta/agent/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from inmanta.agent.reporting import collect_report
 from inmanta.const import ParameterSource, ResourceState
 from inmanta.data.model import AttributeStateChange, ResourceIdStr, ResourceVersionIdStr
 from inmanta.loader import CodeLoader, ModuleSource
 from inmanta.protocol import SessionEndpoint, SyncClient, methods, methods_v2
 from inmanta.resources import Id, Resource
 from inmanta.types import Apireturn, JsonType
-from inmanta.util import IntervalSchedule, NamedLock, ScheduledTask, TaskMethod, add_future
+from inmanta.util import IntervalSchedule, NamedLock, ScheduledTask, TaskMethod, add_future, join_threadpools
 
 LOGGER = logging.getLogger(__name__)
 GET_RESOURCE_BACKOFF = 5
 
 
 class ResourceActionResult(object):
     def __init__(self, cancel: bool) -> None:
@@ -563,14 +563,24 @@
         self._enabled = False
         self._disable_time_triggers()
         self._nq.cancel()
         self._cache.close()
         self.provider_thread_pool.shutdown(wait=False)
         self.thread_pool.shutdown(wait=False)
 
+    def join(self, thread_pool_finalizer: List[ThreadPoolExecutor]) -> None:
+        """
+        Called after stop to ensure complete shutdown
+
+        :param thread_pool_finalizer: all threadpools that should be joined should be added here.
+        """
+        assert self._stopped
+        thread_pool_finalizer.append(self.provider_thread_pool)
+        thread_pool_finalizer.append(self.thread_pool)
+
     @property
     def environment(self) -> uuid.UUID:
         return self._env_id
 
     def get_client(self) -> protocol.Client:
         return self.process._client
 
@@ -1033,16 +1043,19 @@
                     if "$" in name:
                         name = name.replace("$node-name", self.node_name)
                     await self.add_end_point_name(name)
 
     async def stop(self) -> None:
         await super(Agent, self).stop()
         self.thread_pool.shutdown(wait=False)
+        threadpools_to_join = [self.thread_pool]
         for instance in self._instances.values():
             await instance.stop()
+            instance.join(threadpools_to_join)
+        await join_threadpools(threadpools_to_join)
 
     async def start_connected(self) -> None:
         """
         This method is required because:
             1) The client transport is required to retrieve the autostart_agent_map from the server.
             2) _init_endpoint_names() needs to be an async method and async calls are not possible in a constructor.
         """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/cache.py` & `inmanta-core-8.3.0/src/inmanta/agent/cache.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/config.py` & `inmanta-core-8.3.0/src/inmanta/agent/config.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/handler.py` & `inmanta-core-8.3.0/src/inmanta/agent/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,14 @@
 
     def actual(f: Callable) -> T_FUNC:
         myignore = set(ignore)
         sig = inspect.signature(f)
         myargs = list(sig.parameters.keys())[1:]
 
         def wrapper(self, *args: object, **kwds: object) -> object:
-
             kwds.update(dict(zip(myargs, args)))
 
             def bound(**kwds):
                 return f(self, **kwds)
 
             return self.cache.get_or_else(
                 f.__name__,
```

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/io/__init__.py` & `inmanta-core-8.3.0/src/inmanta/agent/io/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/io/local.py` & `inmanta-core-8.3.0/src/inmanta/agent/io/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 try:
     from grp import getgrnam
 except ImportError:
     getgrnam = None
 
 # This code needs to stay Py2 compatible without any external libs
 if False:
-    from typing import Dict, List, Optional, Tuple, Union
+    from typing import Dict, List, Optional, Tuple, Union  # noqa: F401
 
 
 class IOBase(object):
     """
     Base class for an IO module. This class is python2 compatible so IOs that work remote can load this module on python2.
     """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/io/remote.py` & `inmanta-core-8.3.0/src/inmanta/agent/io/remote.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/agent/reporting.py` & `inmanta-core-8.3.0/src/inmanta/agent/reporting.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/app.py` & `inmanta-core-8.3.0/src/inmanta/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -658,15 +658,29 @@
         conn = protocol.SyncClient("compiler")
         LOGGER.info("Triggering deploy for version %d" % version)
         tid = cfg_env.get()
         agent_trigger_method = const.AgentTriggerMethod.get_agent_trigger_method(options.full_deploy)
         conn.release_version(tid, version, True, agent_trigger_method)
 
 
-log_levels = {0: logging.ERROR, 1: logging.WARNING, 2: logging.INFO, 3: logging.DEBUG, 4: 2}
+"""
+This dictionary maps the Inmanta log levels to the corresponding Python log levels
+"""
+log_levels = {
+    "0": logging.ERROR,
+    "1": logging.WARNING,
+    "2": logging.INFO,
+    "3": logging.DEBUG,
+    "4": 2,
+    "ERROR": logging.ERROR,
+    "WARNING": logging.WARNING,
+    "INFO": logging.INFO,
+    "DEBUG": logging.DEBUG,
+    "TRACE": 2,
+}
 
 
 def cmd_parser() -> argparse.ArgumentParser:
     # create the argument compiler
     parser = argparse.ArgumentParser()
     parser.add_argument("-p", action="store_true", dest="profile", help="Profile this run of the program")
     parser.add_argument("-c", "--config", dest="config_file", help="Use this config file", default=None)
@@ -676,16 +690,16 @@
         help="The directory containing the Inmanta configuration files",
         default="/etc/inmanta/inmanta.d",
     )
     parser.add_argument("--log-file", dest="log_file", help="Path to the logfile")
     parser.add_argument(
         "--log-file-level",
         dest="log_file_level",
-        default=2,
-        type=int,
+        choices=["0", "1", "2", "3", "4", "ERROR", "WARNING", "INFO", "DEBUG", "TRACE"],
+        default="INFO",
         help="Log level for messages going to the logfile: 0=ERROR, 1=WARNING, 2=INFO, 3=DEBUG",
     )
     parser.add_argument("--timed-logs", dest="timed", help="Add timestamps to logs", action="store_true")
     parser.add_argument(
         "-v",
         "--verbose",
         action="count",
@@ -754,35 +768,41 @@
 
     return stream_handler
 
 
 def _get_watched_file_handler(options: argparse.Namespace) -> logging.handlers.WatchedFileHandler:
     if not options.log_file:
         raise Exception("No logfile was provided.")
-    level = _convert_to_log_level(options.log_file_level)
+    level = _convert_inmanta_log_level_to_python_log_level(options.log_file_level)
     formatter = logging.Formatter(fmt="%(asctime)s %(levelname)-8s %(name)-10s %(message)s")
     file_handler = logging.handlers.WatchedFileHandler(filename=options.log_file, mode="a+")
     file_handler.setFormatter(formatter)
     file_handler.setLevel(level)
 
     return file_handler
 
 
-def _convert_to_log_level(level: int) -> int:
-    if level >= len(log_levels):
-        level = len(log_levels) - 1
+def _convert_inmanta_log_level_to_python_log_level(level: str) -> int:
+    """
+    Converts the Inmanta log level to the Python log level
+    """
+    if level.isdigit() and int(level) > 4:
+        level = "4"
     return log_levels[level]
 
 
 def _convert_cli_log_level(level: int) -> int:
+    """
+    Converts the number of -v's passed on the CLI to the corresponding Inmanta log level
+    """
     if level < 1:
         # The minimal log level on the CLI is always WARNING
         return logging.WARNING
     else:
-        return _convert_to_log_level(level)
+        return _convert_inmanta_log_level_to_python_log_level(str(level))
 
 
 def _get_log_formatter_for_stream_handler(timed: bool) -> logging.Formatter:
     log_format = "%(asctime)s " if timed else ""
     if _is_on_tty():
         log_format += "%(log_color)s%(name)-25s%(levelname)-8s%(reset)s%(blue)s%(message)s"
         formatter = MultiLineFormatter(
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/__init__.py` & `inmanta-core-8.3.0/src/inmanta/ast/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 try:
     from typing import TYPE_CHECKING
 except ImportError:
     TYPE_CHECKING = False
 
 if TYPE_CHECKING:
     from inmanta.ast.attribute import Attribute  # noqa: F401
+    from inmanta.ast.entity import Entity
     from inmanta.ast.statements import Statement  # noqa: F401
     from inmanta.ast.statements.define import DefineEntity, DefineImport  # noqa: F401
     from inmanta.ast.type import NamedType, Type  # noqa: F401
     from inmanta.compiler import Compiler
     from inmanta.execute.runtime import DelayedResultVariable, ExecutionContext, Instance, ResultVariable  # noqa: F401
     from inmanta.plugins import PluginException
 
@@ -138,25 +139,52 @@
                 and self.start_char == other.start_char
                 and self.end_lnr == other.end_lnr
                 and self.end_char == other.end_char
             )
         return False
 
 
+class AnchorTarget(object):
+    """AnchorTarget is used purely at the periphery of the compiler"""
+
+    __slots__ = ("location", "docstring")
+
+    def __init__(
+        self,
+        location: Location,
+        docstring: Optional[str] = None,
+    ) -> None:
+        """
+        Create a new AnchorTarget instance.
+        :param location: the location of the target of the anchor
+        :param docstring: the docstring attached to the target
+        """
+        self.location = location
+        self.docstring = docstring
+
+
+class WithComment(object):
+    """
+    Mixin class for AST nodes that can have a comment attached to them.
+    """
+
+    comment: Optional[str] = None
+
+
 class Locatable(object):
     __slots__ = ("_location",)
 
     def __init__(self) -> None:
         self._location: Optional[Location] = None
 
     def set_location(self, location: Location) -> None:
         assert location is not None and location.lnr > 0
         self._location = location
 
-    def get_location(self) -> Location:
+    def get_location(self) -> Optional[Location]:
         assert self._location is not None
         return self._location
 
     def copy_location(self, other: "Locatable") -> None:
         """
         Copy the location of this locatable to the given locatable
         """
@@ -208,43 +236,51 @@
     def get_range(self) -> Range:
         return self.range
 
     def get_location(self) -> Range:
         return self.range
 
     @abstractmethod
-    def resolve(self) -> Location:
+    def resolve(self) -> Optional[AnchorTarget]:
         raise NotImplementedError()
 
 
 class TypeReferenceAnchor(Anchor):
     def __init__(self, namespace: "Namespace", type: LocatableString) -> None:
         Anchor.__init__(self, range=type.get_location())
         self.namespace = namespace
         self.type = type
 
-    def resolve(self) -> Location:
+    def resolve(self) -> Optional[AnchorTarget]:
         t = self.namespace.get_type(self.type)
-        return t.get_location()
+        location = t.get_location()
+        docstring = t.comment if isinstance(t, WithComment) else None
+        if not location:
+            return None
+        return AnchorTarget(location=location, docstring=docstring)
 
 
 class AttributeReferenceAnchor(Anchor):
     def __init__(self, range: Range, namespace: "Namespace", type: LocatableString, attribute: str) -> None:
         Anchor.__init__(self, range=range)
         self.namespace = namespace
         self.type = type
         self.attribute = attribute
 
-    def resolve(self) -> Location:
+    def resolve(self) -> Optional[AnchorTarget]:
         instancetype = self.namespace.get_type(self.type)
         # type check impossible atm due to import loop
         # assert isinstance(instancetype, Entity)
         entity_attribute: Optional[Attribute] = instancetype.get_attribute(self.attribute)
         assert entity_attribute is not None
-        return entity_attribute.get_location()
+        location = entity_attribute.get_location()
+        docstring = instancetype.comment if isinstance(instancetype, WithComment) else None
+        if not location:
+            return None
+        return AnchorTarget(location=location, docstring=docstring)
 
 
 class Namespaced(Locatable):
     __slots__ = ()
 
     @abstractmethod
     def get_namespace(self) -> "Namespace":
@@ -317,24 +353,24 @@
     def import_ns(self, name: str, ns: "DefineImport") -> None:
         if name in self.visible_namespaces:
             other = self.visible_namespaces[name]
             if not isinstance(other, MockImport):
                 raise DuplicateException(ns, self.visible_namespaces[name], "Two import statements have the same name")
         self.visible_namespaces[name] = ns
 
+    def lookup_namespace(self, name: str) -> Import:
+        if name not in self.visible_namespaces:
+            raise NotFoundException(None, name, f"Namespace {name} not found. Try importing it with `import {name}`")
+        return self.visible_namespaces[name]
+
     def lookup(self, name: str) -> "Union[Type, ResultVariable]":
         if "::" not in name:
             return self.get_scope().direct_lookup(name)
-
         parts = name.rsplit("::", 1)
-
-        if parts[0] not in self.visible_namespaces:
-            raise NotFoundException(None, name, "Variable %s not found" % parts[0])
-
-        return self.visible_namespaces[parts[0]].target.get_scope().direct_lookup(parts[1])
+        return self.lookup_namespace(parts[0]).target.get_scope().direct_lookup(parts[1])
 
     def get_type(self, typ: LocatableString) -> "Type":
         name: str = str(typ)
         assert self.primitives is not None
         if "::" in name:
             parts = name.rsplit("::", 1)
             if parts[0] in self.visible_namespaces:
@@ -631,14 +667,31 @@
         self.ns = ns
         self.set_location(type.get_location())
 
     def importantance(self) -> int:
         return 20
 
 
+class AmbiguousTypeException(TypeNotFoundException):
+    """Exception raised when a type is referenced that does not exist"""
+
+    def __init__(self, type: LocatableString, candidates: List["Entity"]) -> None:
+        candidates = sorted(candidates, key=lambda x: x.get_full_name())
+        RuntimeException.__init__(
+            self,
+            stmt=None,
+            msg="Could not determine namespace for type %s. %d possible candidates exists: [%s]."
+            " To resolve this, use the fully qualified name instead of the short name."
+            % (type, len(candidates), ", ".join([x.get_full_name() for x in candidates])),
+        )
+        self.candidates = candidates
+        self.type = type
+        self.set_location(type.get_location())
+
+
 def stringify_exception(exn: Exception) -> str:
     if isinstance(exn, CompilerException):
         return str(exn)
     return "%s: %s" % (exn.__class__.__name__, str(exn))
 
 
 @stable_api
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/attribute.py` & `inmanta-core-8.3.0/src/inmanta/ast/attribute.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/blocks.py` & `inmanta-core-8.3.0/src/inmanta/ast/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing import TYPE_CHECKING, Dict, FrozenSet, Iterable, Iterator, List, Optional, Sequence, Tuple
 
 from inmanta.ast import Anchor, Locatable, Namespace, RuntimeException, TypeNotFoundException, VariableShadowWarning
 from inmanta.ast.statements import DefinitionStatement, DynamicStatement, Statement, StaticEagerPromise
 from inmanta.execute.runtime import QueueScheduler, Resolver
 
 if TYPE_CHECKING:
-
     from inmanta.execute.runtime import ExecutionContext
 
 
 class BasicBlock(object):
     def __init__(self, namespace: Namespace, stmts: List[DynamicStatement] = []) -> None:
         self.__stmts = []  # type: List[DynamicStatement]
         self.__definition_stmts = []  # type: List[DefinitionStatement]
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/constraint/__init__.py` & `inmanta-core-8.3.0/src/inmanta/ast/constraint/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/constraint/expression.py` & `inmanta-core-8.3.0/src/inmanta/ast/constraint/expression.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/entity.py` & `inmanta-core-8.3.0/src/inmanta/ast/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     DuplicateException,
     Locatable,
     Location,
     Named,
     Namespace,
     NotFoundException,
     RuntimeException,
+    WithComment,
 )
 from inmanta.ast.blocks import BasicBlock
 from inmanta.ast.statements.generator import SubConstructor
 from inmanta.ast.type import NamedType, Type
 from inmanta.execute.runtime import Instance, QueueScheduler, Resolver, dataflow
 from inmanta.execute.util import AnyType
 
@@ -47,27 +48,25 @@
     from inmanta.ast.statements import ExpressionStatement, Statement  # noqa: F401
     from inmanta.ast.statements.define import DefineAttribute, DefineImport  # noqa: F401
     from inmanta.execute.runtime import ExecutionContext, ResultVariable  # noqa: F401
 
 import inmanta.ast.attribute
 
 
-class Entity(NamedType):
+class Entity(NamedType, WithComment):
     """
     This class models a defined entity in the domain model of the configuration model.
 
     Each entity can contain attributes that are either data types or
     relations and each entity can inherit from parent entities.
 
     :param name: The name of this entity. This name can not be changed
         after this object has been created
     """
 
-    comment: Optional[str]
-
     def __init__(self, name: str, namespace: Namespace, comment: Optional[str] = None) -> None:
         NamedType.__init__(self)
 
         self.__name = name  # type: str
 
         self.__namespace = namespace
 
@@ -183,23 +182,23 @@
         """
         Set a set of attributes that are defined in this entities
         """
         self._attributes = attributes
 
     attributes: "Dict[str,Attribute]" = property(get_attributes, set_attributes, None, None)
 
-    def is_parent(self, entity: "Entity") -> bool:
+    def is_parent(self, parent_candidate: "Entity") -> bool:
         """
-        Check if the given entity is a parent of this entity. Does not consider an entity its own parent.
+        Check if the given parent_candidate entity is a parent of this entity. Does not consider an entity its own parent.
         """
-        if entity in self.parent_entities:
+        if parent_candidate in self.parent_entities:
             return True
         else:
             for parent in self.parent_entities:
-                if parent.is_parent(entity):
+                if parent.is_parent(parent_candidate):
                     return True
         return False
 
     def get_all_parent_names(self) -> "List[str]":
         """
         Get a set with all parents of this entity
         """
@@ -211,14 +210,20 @@
 
     def get_all_parent_entities(self) -> "Set[Entity]":
         parents = [x for x in self.parent_entities]
         for entity in self.parent_entities:
             parents.extend(entity.get_all_parent_entities())
         return set(parents)
 
+    def get_all_child_entities(self) -> "Set[Entity]":
+        children = [x for x in self.child_entities]
+        for entity in self.child_entities:
+            children.extend(entity.get_all_child_entities())
+        return set(children)
+
     def get_all_attribute_names(self) -> "List[str]":
         """
         Return a list of all attribute names, including parents
         """
         names = list(self._attributes.keys())
 
         for parent in self.parent_entities:
@@ -293,19 +298,22 @@
         out.set_location(location)
         for k, v in attributes.items():
             out.set_attribute(k, v, location)
 
         self.add_instance(out)
         return out
 
-    def is_subclass(self, cls: "Entity") -> bool:
+    def is_subclass(self, subclass_candidate: "Entity", *, strict: bool = True) -> bool:
         """
-        Is the given class a subclass of this class. Does not consider entities a subclass of themselves.
+        Check if the given subclass_candidate entity is a subclass of this class.
+        Does not consider entities a subclass of themselves in strict mode (the default).
+
+        :param strict: Only return True for entities that are a strict subtype, i.e. not of the same type.
         """
-        return cls.is_parent(self)
+        return (not strict and subclass_candidate == self) or subclass_candidate.is_parent(self)
 
     def validate(self, value: object) -> bool:
         """
         Validate the given value
         """
         if isinstance(value, AnyType):
             return True
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/export.py` & `inmanta-core-8.3.0/src/inmanta/ast/export.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/statements/__init__.py` & `inmanta-core-8.3.0/src/inmanta/ast/statements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     DirectExecuteException,
     Location,
     Named,
     Namespace,
     Namespaced,
     OptionalValueException,
     RuntimeException,
+    WithComment,
 )
 from inmanta.execute.dataflow import DataflowGraph
 from inmanta.execute.runtime import (
     ExecutionUnit,
     Instance,
     ProgressionPromise,
     QueueScheduler,
@@ -44,15 +45,15 @@
     VariableABC,
     WrappedValueVariable,
 )
 
 if TYPE_CHECKING:
     from inmanta.ast.assign import SetAttribute  # noqa: F401
     from inmanta.ast.blocks import BasicBlock  # noqa: F401
-    from inmanta.ast.type import NamedType  # noqa: F401
+    from inmanta.ast.type import NamedType, Type  # noqa: F401
     from inmanta.ast.variables import Reference  # noqa: F401
 
 
 class Statement(Namespaced):
     """
     An abstract baseclass representing a statement in the configuration policy.
     """
@@ -201,14 +202,15 @@
             promise.fulfill()
 
 
 @dataclass(frozen=True)
 class AttributeAssignmentLHS:
     instance: "Reference"
     attribute: str
+    type_hint: Optional["Type"] = None
 
 
 class ExpressionStatement(RequiresEmitStatement):
     __slots__ = ()
 
     def normalize(self, *, lhs_attribute: Optional[AttributeAssignmentLHS] = None) -> None:
         """
@@ -568,24 +570,21 @@
     This statement defines a new entity in the configuration.
     """
 
     def __init__(self) -> None:
         Statement.__init__(self)
 
 
-class TypeDefinitionStatement(DefinitionStatement, Named):
-    comment: Optional[str]
-
+class TypeDefinitionStatement(DefinitionStatement, Named, WithComment):
     def __init__(self, namespace: Namespace, name: str) -> None:
         DefinitionStatement.__init__(self)
         self.name = name
         self.namespace = namespace
         self.fullName = namespace.get_full_name() + "::" + str(name)
         self.type = None  # type: NamedType
-        self.comment = None
 
     def register_types(self) -> Tuple[str, "NamedType"]:
         self.namespace.define_type(self.name, self.type)
         return (self.fullName, self.type)
 
     def evaluate(self) -> None:
         pass
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/statements/assign.py` & `inmanta-core-8.3.0/src/inmanta/ast/statements/assign.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,27 +286,27 @@
 
     def __init__(self, stmt: "Statement", instance: "Instance", attribute_name: str, next: ResultCollector[T]) -> None:
         self.stmt = stmt
         self.instance = instance
         self.next = next
         self.attribute_name = attribute_name
 
-    def receive_result(self, value: T, location: Location) -> None:
+    def receive_result(self, value: T, location: Location) -> bool:
         try:
             self.next.receive_result(value, location)
+            return False
         except AttributeException as e:
             e.set_statement(self.stmt, False)
             raise
         except RuntimeException as e:
             e.set_statement(self.stmt, False)
             raise AttributeException(self.stmt, self.instance, self.attribute_name, e)
 
 
 class SetAttributeHelper(ExecutionUnit):
-
     __slots__ = ("stmt", "instance", "attribute_name")
 
     def __init__(
         self,
         queue_scheduler: QueueScheduler,
         resolver: Resolver,
         result: ResultVariable,
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/statements/call.py` & `inmanta-core-8.3.0/src/inmanta/ast/statements/call.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,14 @@
             except plugins.PluginException as e:
                 raise ExplicitPluginException(self.ast_node, "PluginException in plugin %s" % self.ast_node.name, e)
             except Exception as e:
                 raise ExternalException(self.ast_node, "Exception in plugin %s" % self.ast_node.name, e)
 
 
 class FunctionUnit(Waiter):
-
     __slots__ = ("result", "base_requires", "function", "resolver")
 
     def __init__(self, queue_scheduler, resolver, result: ResultVariable, requires, function: FunctionCall) -> None:
         Waiter.__init__(self, queue_scheduler)
         self.result = result
         # requires is used to track all required RV's
         # It can grow larger as new requires are discovered
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/statements/define.py` & `inmanta-core-8.3.0/src/inmanta/ast/statements/define.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,14 @@
 
 
 class DefineEntity(TypeDefinitionStatement):
     """
     Define a new entity in the configuration
     """
 
-    comment: Optional[str]
     type: Entity
 
     def __init__(
         self,
         namespace: Namespace,
         lname: LocatableString,
         comment: Optional[LocatableString],
@@ -137,16 +136,14 @@
 
         self.anchors = [TypeReferenceAnchor(namespace, x) for x in parents]
 
         self.name = name
         self.attributes = attributes
         if comment is not None:
             self.comment = str(comment)
-        else:
-            self.comment = None
 
         self.parents = parents
 
         if len(self.parents) == 0 and not (self.name == "Entity" and self.namespace.name == "std"):
             dummy_location: Range = Range("__internal__", 1, 1, 1, 1)
             self.parents.append(LocatableString("std::Entity", dummy_location, -1, namespace))
 
@@ -250,15 +247,14 @@
 class DefineImplementation(TypeDefinitionStatement):
     """
     Define a new implementation that has a name and contains statements
 
     :param name: The name of the implementation
     """
 
-    comment: Optional[str]
     type: Implementation
 
     def __init__(
         self,
         namespace: Namespace,
         name: LocatableString,
         target_type: LocatableString,
@@ -269,15 +265,14 @@
         self.name = str(name)
         if "-" in self.name:
             raise HyphenException(name)
 
         self.block = statements
         self.entity = target_type
 
-        self.comment = None
         if comment is not None:
             self.comment = str(comment)
 
         self.location = name.get_location()
 
         self.type = Implementation(str(self.name), self.block, self.namespace, str(target_type), self.comment)
         self.type.location = name.get_location()
@@ -319,15 +314,15 @@
 
     :param entity: The name of the entity that is implemented
     :param implementations: A list of implementations
     :param select: A clause that determines when this implementation is "active"
     :param inherit: True iff the entity should inherit all implementations from its parents
     """
 
-    comment: Optional[str]
+    comment: Optional[str] = None
 
     def __init__(
         self,
         entity_name: LocatableString,
         implementations: List[LocatableString],
         select: ExpressionStatement,
         inherit: bool = False,
@@ -343,16 +338,14 @@
         self.location = entity_name.get_location()
         if inherit and (not isinstance(select, Literal) or select.value is not True):
             raise RuntimeException(self, "Conditional implementation with parents not allowed")
         self.select = select
         self.inherit: bool = inherit
         if comment is not None:
             self.comment = str(comment)
-        else:
-            self.comment = None
 
     def __repr__(self) -> str:
         """
         Returns a representation of this class
         """
         return "Implement(%s)" % (self.entity)
 
@@ -407,30 +400,28 @@
     Define a new data type in the configuration. This type is a constrained
     version of a the built-in datatypes
 
     :param name: The name of the new  type
     :param basetype: The name of the type that is "refined"
     """
 
-    comment: Optional[str]
     __expression: ExpressionStatement
     type: ConstraintType
 
     def __init__(
         self, namespace: Namespace, name: LocatableString, basetype: LocatableString, expression: ExpressionStatement
     ) -> None:
         TypeDefinitionStatement.__init__(self, namespace, str(name))
         self.set_location(name.get_location())
         self.basetype = basetype
         self.anchors.append(TypeReferenceAnchor(namespace, basetype))
         self.anchors.extend(expression.get_anchors())
         self.set_expression(expression)
         self.type = ConstraintType(self.namespace, str(name))
         self.type.location = name.get_location()
-        self.comment = None
         if self.name in TYPES:
             warnings.warn(CompilerRuntimeWarning(self, "Trying to override a built-in type: %s" % self.name))
         if "-" in self.name:
             raise HyphenException(name)
 
     def get_expression(self) -> ExpressionStatement:
         """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/statements/generator.py` & `inmanta-core-8.3.0/src/inmanta/ast/statements/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,31 @@
 
 # pylint: disable-msg=W0613,R0201
 
 import logging
 import uuid
 from collections import abc
 from itertools import chain
-from typing import Dict, Iterator, List, Optional, Set, Tuple
+from typing import Dict, Iterator, List, Optional, Tuple
 
+import inmanta.ast.entity
 import inmanta.ast.type as inmanta_type
 import inmanta.execute.dataflow as dataflow
 from inmanta.ast import (
+    AmbiguousTypeException,
     AttributeReferenceAnchor,
     DuplicateException,
     Locatable,
     LocatableString,
     Location,
     Namespace,
     NotFoundException,
     Range,
     RuntimeException,
+    TypeNotFoundException,
     TypeReferenceAnchor,
     TypingException,
 )
 from inmanta.ast.attribute import Attribute, RelationAttribute
 from inmanta.ast.blocks import BasicBlock
 from inmanta.ast.statements import (
     AttributeAssignmentLHS,
@@ -172,28 +175,29 @@
 class GradualFor(ResultCollector[object]):
     # this class might be unnecessary if receive-result is always called and exactly once
 
     def __init__(self, stmt: "For", resolver: Resolver, queue: QueueScheduler) -> None:
         self.resolver = resolver
         self.queue = queue
         self.stmt = stmt
-        self.seen = set()  # type: Set[int]
+        self.seen: set[int] = set()
 
-    def receive_result(self, value: object, location: ResultVariable) -> None:
+    def receive_result(self, value: object, location: ResultVariable) -> bool:
         if id(value) in self.seen:
-            return
+            return False
         self.seen.add(id(value))
 
         xc = ExecutionContext(self.stmt.module, self.resolver.for_namespace(self.stmt.module.namespace))
         loopvar = xc.lookup(self.stmt.loop_var)
         # this assertion is because the typing of this method is not correct
         # it should logically always hold, but we can't express this as types yet
         assert isinstance(loopvar, ResultVariable)
         loopvar.set_value(value, self.stmt.location)
         xc.emit(self.queue)
+        return False
 
 
 class For(RequiresEmitStatement):
     """
     A for loop
     """
 
@@ -467,14 +471,15 @@
     :param class_type: The type of the object that is created by this
         constructor call.
     """
 
     __slots__ = (
         "class_type",
         "__attributes",
+        "__attribute_locations",
         "__wrapped_kwarg_attributes",
         "location",
         "type",
         "_self_ref",
         "_lhs_attribute",
         "_required_dynamic_args",
         "_direct_attributes",
@@ -488,14 +493,15 @@
         wrapped_kwargs: List["WrappedKwargs"],
         location: Location,
         namespace: Namespace,
     ) -> None:
         super().__init__()
         self.class_type = class_type
         self.__attributes = {}  # type: Dict[str,ExpressionStatement]
+        self.__attribute_locations: Dict[str, LocatableString] = {}
         self.__wrapped_kwarg_attributes: List[WrappedKwargs] = wrapped_kwargs
         self.location = location
         self.namespace = namespace
         self.anchors.append(TypeReferenceAnchor(namespace, class_type))
         for a in attributes:
             self.add_attribute(a[0], a[1])
         self.type: Optional["Entity"] = None
@@ -516,24 +522,32 @@
                     ("%s=%s" % (k, v.pretty_print()) for k, v in self.attributes.items()),
                     ("**%s" % kwargs.pretty_print() for kwargs in self.wrapped_kwargs),
                 )
             ),
         )
 
     def _normalize_rhs(self, index_attributes: abc.Set[str]) -> None:
-        for (k, v) in self.__attributes.items():
+        assert self.type is not None  # Make mypy happy
+        for k, v in self.__attributes.items():
+            attr = self.type.get_attribute(k)
+            if attr is None:
+                raise TypingException(
+                    self.__attribute_locations[k], "no attribute %s on type %s" % (k, self.type.get_full_name())
+                )
+            type_hint = attr.get_type().get_base_type()
             # don't notify the rhs for index attributes because it won't be able to resolve the reference
             # (index attributes need to be resolved before the instance can be constructed)
-            v.normalize(lhs_attribute=AttributeAssignmentLHS(self._self_ref, k) if k not in index_attributes else None)
+            v.normalize(
+                lhs_attribute=AttributeAssignmentLHS(self._self_ref, k, type_hint) if k not in index_attributes else None
+            )
         for wrapped_kwargs in self.wrapped_kwargs:
             wrapped_kwargs.normalize()
 
     def normalize(self, *, lhs_attribute: Optional[AttributeAssignmentLHS] = None) -> None:
-        mytype: "Entity" = self.namespace.get_type(self.class_type)
-        self.type = mytype
+        self.type = self._resolve_type(lhs_attribute)
 
         inindex: abc.MutableSet[str] = set()
 
         all_attributes = dict(self.type.get_default_values())
         all_attributes.update(self.__attributes)
 
         # now check that all variables that have indexes on them, are already
@@ -553,27 +567,87 @@
             # lhs attribute. If this passes but the kwargs and/or lhs attribute don't in fact provide the required arguments,
             # an exception is raised during execution.
             if not self.wrapped_kwargs and (self._lhs_attribute is None or len(self._required_dynamic_args) > 1):
                 raise IndexAttributeMissingInConstructorException(self, self.type, self._required_dynamic_args)
 
         self._normalize_rhs(inindex)
 
-        for (k, v) in all_attributes.items():
+        for k, v in all_attributes.items():
             attribute = self.type.get_attribute(k)
             if attribute is None:
-                raise TypingException(self, "no attribute %s on type %s" % (k, self.type.get_full_name()))
+                raise TypingException(
+                    self.__attribute_locations[k], "no attribute %s on type %s" % (k, self.type.get_full_name())
+                )
             if k not in inindex:
                 self._indirect_attributes[k] = v
             else:
                 self._direct_attributes[k] = v
 
         self._own_eager_promises = list(
             chain.from_iterable(subconstructor.get_all_eager_promises() for subconstructor in self.type.get_sub_constructor())
         )
 
+    def _resolve_type(self, lhs_attribute: Optional[AttributeAssignmentLHS]) -> "Entity":
+        """Type hint handling"""
+
+        # First normal resolution
+        resolver_failure: Optional[TypeNotFoundException] = None
+        local_type: "Optional[Entity]" = None
+        try:
+            tp = self.namespace.get_type(self.class_type)
+            assert isinstance(
+                tp, inmanta.ast.entity.Entity
+            ), "Should not happen because all entity types start with a capital letter"
+            local_type = tp
+        except TypeNotFoundException as e:
+            resolver_failure = e
+
+        # Do we have hint context?
+        # We only work with unqualified names for hinting
+        if lhs_attribute is not None and lhs_attribute.type_hint is not None:
+            # We can do type hinting here
+            type_hint = lhs_attribute.type_hint
+            if not isinstance(type_hint, inmanta.ast.entity.Entity):
+                # This is a type error, we are a constructor for an entity but we should not be!
+                raise TypingException(
+                    self,
+                    f"Can not assign a value of type {self.class_type} "
+                    f"to a variable of type {str(lhs_attribute.type_hint)}",
+                )
+            elif local_type is not None:
+                # always prefer local type, raise an exception if it is of an incorrect type
+                if not type_hint.is_subclass(local_type, strict=False):
+                    raise TypingException(
+                        self,
+                        f"Can not assign a value of type {str(local_type)} "
+                        f"to a variable of type {str(lhs_attribute.type_hint)}",
+                    )
+                return local_type
+            elif "::" not in str(self.class_type):
+                # Consider the hint type
+                base_types = [type_hint]
+                # Find all correct types with the matching unqualified name
+                candidates = {
+                    entity
+                    for entity in chain(base_types, type_hint.get_all_child_entities())
+                    if entity.name == str(self.class_type)
+                }
+                if len(candidates) > 1:
+                    # To many options, inheritance may cause this to break a working model due to dependency update
+                    raise AmbiguousTypeException(self.class_type, list(candidates))
+                elif len(candidates) == 1:
+                    # One, nice
+                    return next(iter(candidates))
+        elif local_type is not None:
+            return local_type
+
+        # No matching types found: pretend nothing happened, reraise original exception
+        assert resolver_failure is not None  # make mypy happy
+        raise resolver_failure
+
     def get_all_eager_promises(self) -> Iterator["StaticEagerPromise"]:
         return chain(
             super().get_all_eager_promises(),
             *(subexpr.get_all_eager_promises() for subexpr in chain(self.attributes.values(), self.wrapped_kwargs)),
         )
 
     def requires(self) -> List[str]:
@@ -601,15 +675,15 @@
         )
         requires.update(direct_requires)
 
         graph: Optional[DataflowGraph] = resolver.dataflow_graph
         if graph is not None:
             node: dataflow.InstanceNodeReference = self._register_dataflow_node(graph)
             # TODO: also add wrapped_kwargs
-            for (k, v) in chain(self._direct_attributes.items(), self._indirect_attributes.items()):
+            for k, v in chain(self._direct_attributes.items(), self._indirect_attributes.items()):
                 node.assign_attribute(k, v.get_dataflow_node(graph), self, graph)
 
         return requires
 
     def _collect_required_dynamic_arguments(
         self, requires: Dict[object, object], resolver: Resolver, queue: QueueScheduler
     ) -> abc.Mapping[str, object]:
@@ -619,15 +693,15 @@
         """
         type_class = self.type
         assert type_class
 
         # kwargs
         kwarg_attrs: dict[str, object] = {}
         for kwargs in self.wrapped_kwargs:
-            for (k, v) in kwargs.execute(requires, resolver, queue):
+            for k, v in kwargs.execute(requires, resolver, queue):
                 if k in self.attributes or k in kwarg_attrs:
                     raise RuntimeException(
                         self, "The attribute %s is set twice in the constructor call of %s." % (k, self.class_type)
                     )
                 attribute = type_class.get_attribute(k)
                 if attribute is None:
                     raise TypingException(self, "no attribute %s on type %s" % (k, type_class.get_full_name()))
@@ -650,29 +724,29 @@
                         f" {lhs_attribute} on {lhs_instance}"
                     ),
                 )
             inverse: Optional[RelationAttribute] = lhs_attribute.end
             if (
                 inverse is not None
                 and inverse.name not in self._direct_attributes
-                # in case of a double set, prefer kwargs: double set will be raised when the bidirictional relation is set by
+                # in case of a double set, prefer kwargs: double set will be raised when the bidirectional relation is set by
                 # the LHS
                 and inverse.name not in kwarg_attrs
                 and inverse.name in chain.from_iterable(type_class.get_indices())
                 and (inverse.entity == type_class or type_class.is_parent(inverse.entity))
             ):
                 lhs_inverse_assignment = (inverse.name, lhs_instance)
 
         late_args = {**dict([lhs_inverse_assignment] if lhs_inverse_assignment is not None else []), **kwarg_attrs}
         missing_attrs: abc.Sequence[str] = [attr for attr in self._required_dynamic_args if attr not in late_args]
         if missing_attrs:
             raise IndexAttributeMissingInConstructorException(self, type_class, missing_attrs)
         return late_args
 
-    def execute(self, requires: Dict[object, object], resolver: Resolver, queue: QueueScheduler):
+    def execute(self, requires: Dict[object, object], resolver: Resolver, queue: QueueScheduler) -> Instance:
         """
         Evaluate this statement.
         """
         LOGGER.log(LOG_LEVEL_TRACE, "executing constructor for %s at %s", self.class_type, self.location)
         super().execute(requires, resolver, queue)
 
         # the type to construct
@@ -772,14 +846,15 @@
     def add_attribute(self, lname: LocatableString, value: ExpressionStatement) -> None:
         """
         Add an attribute to this constructor call
         """
         name = str(lname)
         if name not in self.__attributes:
             self.__attributes[name] = value
+            self.__attribute_locations[name] = lname
             self.anchors.append(AttributeReferenceAnchor(lname.get_location(), lname.namespace, self.class_type, name))
             self.anchors.extend(value.get_anchors())
         else:
             raise RuntimeException(
                 self, "The attribute %s in the constructor call of %s is already set." % (name, self.class_type)
             )
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/type.py` & `inmanta-core-8.3.0/src/inmanta/ast/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing import Callable
 from typing import List as PythonList
 from typing import Optional, Sequence
 
 from inmanta.ast import (
     DuplicateException,
     Locatable,
-    Location,
     Named,
     Namespace,
     NotFoundException,
     RuntimeException,
     TypeNotFoundException,
 )
 from inmanta.execute.util import AnyType, NoneValue, Unknown
@@ -140,14 +139,17 @@
 
 
 class NamedType(Type, Named):
     def get_double_defined_exception(self, other: "NamedType") -> "DuplicateException":
         """produce an error message for this type"""
         raise DuplicateException(self, other, "Type %s is already defined" % (self.get_full_name()))
 
+    def type_string(self) -> str:
+        return self.get_full_name()
+
 
 @stable_api
 class NullableType(Type):
     """
     Represents a nullable type in the Inmanta :term:`DSL`. For example `NullableType(Number())` represents `number?`.
     """
 
@@ -249,15 +251,15 @@
             raise RuntimeException(None, "Invalid value '%s', expected Number" % value)
 
         return True  # allow this function to be called from a lambda function
 
     def is_primitive(self) -> bool:
         return True
 
-    def get_location(self) -> Location:
+    def get_location(self) -> None:
         return None
 
     def type_string(self) -> str:
         return "number"
 
     def type_string_internal(self) -> str:
         return self.type_string()
@@ -313,15 +315,15 @@
 
     def type_string_internal(self) -> str:
         return self.type_string()
 
     def is_primitive(self) -> bool:
         return True
 
-    def get_location(self) -> Location:
+    def get_location(self) -> None:
         return None
 
 
 @stable_api
 class String(Primitive):
     """
     This class represents a string type in the configuration model.
@@ -355,15 +357,15 @@
 
     def type_string_internal(self) -> str:
         return self.type_string()
 
     def is_primitive(self) -> bool:
         return True
 
-    def get_location(self) -> Location:
+    def get_location(self) -> None:
         return None
 
 
 @stable_api
 class List(Type):
     """
     Instances of this class represent a list type containing any types of values.
@@ -383,15 +385,15 @@
             raise RuntimeException(None, "Invalid value '%s', expected %s" % (value, self.type_string()))
 
         return True
 
     def type_string_internal(self) -> str:
         return "List"
 
-    def get_location(self) -> Location:
+    def get_location(self) -> None:
         return None
 
 
 @stable_api
 class TypedList(List):
     """
     Instances of this class represent a list type containing any values of type element_type.
@@ -416,21 +418,21 @@
 
         return True
 
     def _wrap_type_string(self, string: str) -> str:
         return "%s[]" % string
 
     def type_string(self) -> Optional[str]:
-        element_type_string: Optional[str] = self.element_type.type_string()
+        element_type_string = self.element_type.type_string()
         return None if element_type_string is None else self._wrap_type_string(element_type_string)
 
     def type_string_internal(self) -> str:
         return self._wrap_type_string(self.element_type.type_string_internal())
 
-    def get_location(self) -> Location:
+    def get_location(self) -> None:
         return None
 
     def get_base_type(self) -> Type:
         return self.element_type
 
     def with_base_type(self, base_type: Type) -> Type:
         return TypedList(base_type)
@@ -491,15 +493,18 @@
             raise RuntimeException(None, "Invalid value '%s', expected dict" % value)
 
         return True
 
     def type_string_internal(self) -> str:
         return "Dict"
 
-    def get_location(self) -> Location:
+    def type_string(self) -> str:
+        return "dict"
+
+    def get_location(self) -> None:
         return None
 
 
 @stable_api
 class TypedDict(Dict):
     """
     Instances of this class represent a dict type containing only values of type element_type.
@@ -521,15 +526,15 @@
             self.element_type.validate(element)
 
         return True
 
     def type_string_internal(self) -> str:
         return "dict[%s]" % self.element_type.type_string_internal()
 
-    def get_location(self) -> Location:
+    def get_location(self) -> None:
         return None
 
 
 @stable_api
 class LiteralDict(TypedDict):
     """
     Instances of this class represent a dict type containing only :py:class:`Literal` values.
@@ -638,15 +643,15 @@
         if not self._constraint(value):
             raise RuntimeException(
                 self, "Invalid value %s, does not match constraint `%s`" % (repr(value), self.expression.pretty_print())
             )
 
         return True
 
-    def type_string(self):
+    def type_string(self) -> str:
         return "%s::%s" % (self.namespace, self.name)
 
     def type_string_internal(self) -> str:
         return self.type_string()
 
     def get_full_name(self) -> str:
         return self.namespace.get_full_name() + "::" + self.name
```

### Comparing `inmanta-core-8.2.0/src/inmanta/ast/variables.py` & `inmanta-core-8.3.0/src/inmanta/ast/variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 
 import logging
+from collections import abc
 from typing import Dict, Generic, List, Optional, TypeVar
 
 import inmanta.execute.dataflow as dataflow
 from inmanta.ast import LocatableString, Location, NotFoundException, OptionalValueException, Range, RuntimeException
 from inmanta.ast.statements import (
     AssignStatement,
     AttributeAssignmentLHS,
@@ -64,15 +65,22 @@
     def __init__(self, name: LocatableString) -> None:
         ExpressionStatement.__init__(self)
         self.locatable_name = name
         self.name = str(name)
         self.full_name = str(name)
 
     def normalize(self, *, lhs_attribute: Optional[AttributeAssignmentLHS] = None) -> None:
-        pass
+        split: abc.Sequence[str] = self.name.rsplit("::", maxsplit=1)
+        if len(split) > 1:
+            # fail-fast if namespace does not exist
+            try:
+                self.namespace.lookup_namespace(split[0])
+            except NotFoundException as e:
+                e.set_statement(self)
+                raise
 
     def requires(self) -> List[str]:
         return [self.full_name]
 
     def requires_emit(
         self, resolver: Resolver, queue: QueueScheduler, *, propagate_unset: bool = False
     ) -> Dict[object, VariableABC]:
@@ -183,20 +191,25 @@
     __slots__ = ("owner", "target")
 
     def __init__(self, owner: Statement, target: ResultVariable[bool]) -> None:
         super().__init__()
         self.owner: Statement = owner
         self.target: ResultVariable[bool] = target
 
-    def receive_result(self, value: object, location: Location) -> None:
+    def pure_gradual(self) -> bool:
+        # freezing an empty variable causes progress
+        return False
+
+    def receive_result(self, value: object, location: Location) -> bool:
         """
         Gradually receive an assignment to the referenced variable. Sets the target variable to True because to receive a single
         value implies that the variable is defined.
         """
         self.target.set_value(True, self.owner.location)
+        return True
 
     def variable_resume(
         self,
         variable: VariableABC[object],
         resolver: Resolver,
         queue_scheduler: QueueScheduler,
     ) -> None:
```

### Comparing `inmanta-core-8.2.0/src/inmanta/command.py` & `inmanta-core-8.3.0/src/inmanta/command.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/__init__.py` & `inmanta-core-8.3.0/src/inmanta/compiler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 
     Contact: code@inmanta.com
 """
 import logging
 import sys
 from collections import abc
 from itertools import chain
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Set, Tuple
+from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Set, Tuple
 
 import inmanta.ast.type as inmanta_type
 import inmanta.execute.dataflow as dataflow
 from inmanta import const, module
 from inmanta.ast import (
+    AnchorTarget,
     AttributeException,
     CompilerException,
     DoubleSetException,
     LocatableString,
     Location,
     MultiException,
     Namespace,
@@ -49,15 +50,15 @@
 
 LOGGER: logging.Logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from inmanta.ast import BasicBlock, Statement  # noqa: F401
 
 
-def do_compile(refs: Dict[Any, Any] = {}) -> Tuple[Dict[str, inmanta_type.Type], Namespace]:
+def do_compile(refs: Optional[abc.Mapping[object, object]] = None) -> tuple[dict[str, inmanta_type.Type], Namespace]:
     """
     Perform a complete compilation run for the current project (as returned by :py:meth:`inmanta.module.Project.get`)
 
     :param refs: Datastructure used to pass on mocking information to the compiler. Supported options:
                     * key="facts"; value=Dict with the following structure: {"<resource_id": {"<fact_name>": "<fact_value"}}
     """
     compiler = Compiler(refs=refs)
@@ -104,30 +105,30 @@
             chain.from_iterable(
                 tp.get_all_instances() for tp in types.values() if isinstance(tp, Entity) and tp.namespace is config_ns
             )
         ),
     )
 
 
-def anchormap(refs: Dict[Any, Any] = {}) -> Sequence[Tuple[Location, Location]]:
+def anchormap(refs: Optional[abc.Mapping[object, object]] = None) -> Sequence[Tuple[Location, AnchorTarget]]:
     """
     Return all lexical references
 
     Performs compilation up to and including the type resolution, but doesn't start executing
 
     :param refs: Datastructure used to pass on mocking information to the compiler. Supported options:
                     * key="facts"; value=Dict with the following structure: {"<resource_id": {"<fact_name>": "<fact_value"}}
     """
     compiler = Compiler(refs=refs)
 
     LOGGER.debug("Starting compile")
 
     (statements, blocks) = compiler.compile()
     sched = scheduler.Scheduler()
-    return sched.anchormap(compiler, statements, blocks)
+    return sched.get_anchormap(compiler, statements, blocks)
 
 
 def get_types_and_scopes() -> Tuple[Dict[str, inmanta_type.Type], Namespace]:
     """
     Only run the compilation steps required to extract the different types and scopes.
     """
     compiler = Compiler()
@@ -142,19 +143,19 @@
     An inmanta compiler
 
     :param cf_file: DEPRECATED
     :param refs: Datastructure used to pass on mocking information to the compiler. Supported keys:
                     * key="facts"; value=Dict with the following structure: {"<resource_id": {"<fact_name>": "<fact_value"}}
     """
 
-    def __init__(self, cf_file: str = "main.cf", refs: Dict[Any, Any] = {}) -> None:
+    def __init__(self, cf_file: str = "main.cf", refs: Optional[abc.Mapping[object, object]] = None) -> None:
         self.__root_ns: Optional[Namespace] = None
         self._data: CompileData = CompileData()
         self.plugins: Dict[str, Plugin] = {}
-        self.refs = refs
+        self.refs = refs if refs is not None else {}
 
     def get_plugins(self) -> Dict[str, Plugin]:
         return self.plugins
 
     def is_loaded(self) -> bool:
         """
         Is everything loaded and the namespace structure built?
@@ -193,15 +194,14 @@
         project.load()
         statements, blocks = project.get_complete_ast()
 
         project.log_installed_modules()
 
         # load plugins
         for name, cls in PluginMeta.get_functions().items():
-
             mod_ns = cls.__module__.split(".")
             if mod_ns[0] != const.PLUGINS_PACKAGE:
                 raise Exception(
                     "All plugin modules should be loaded in the %s package not in %s" % (const.PLUGINS_PACKAGE, cls.__module__)
                 )
 
             mod_ns = mod_ns[1:]
```

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/config.py` & `inmanta-core-8.3.0/src/inmanta/compiler/config.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/data.py` & `inmanta-core-8.3.0/src/inmanta/compiler/data.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/help/__init__.py` & `inmanta-core-8.3.0/src/inmanta/compiler/help/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/help/explainer.py` & `inmanta-core-8.3.0/src/inmanta/compiler/help/explainer.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2` & `inmanta-core-8.3.0/src/inmanta/compiler/help/templates/modified_after_freeze.j2`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2` & `inmanta-core-8.3.0/src/inmanta/compiler/help/templates/module_v2_in_v1_path.j2`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/config.py` & `inmanta-core-8.3.0/src/inmanta/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,15 @@
 
     return socket.gethostname()
 
 
 nodename = Option("config", "node-name", get_default_nodename, "Force the hostname of this machine to a specific value", is_str)
 feature_file_config = Option("config", "feature-file", None, "The loacation of the inmanta feature file.", is_str_opt)
 
+
 ###############################
 # Transport Config
 ###############################
 class TransportConfig(object):
     """
     A class to register the config options for Client classes
     """
@@ -426,14 +427,19 @@
 
     sections: Dict[str, "AuthJWTConfig"] = {}
     issuers: Dict[str, "AuthJWTConfig"] = {}
 
     validate_cert: bool
 
     @classmethod
+    def reset(cls) -> None:
+        cls.sections = {}
+        cls.issuers = {}
+
+    @classmethod
     def list(cls) -> List[str]:
         """
         Return a list of all defined auth jwt configurations. This method will load new sections if they were added
         since the last invocation.
         """
         cfg = Config._get_instance()
         prefix_len = len(AUTH_JWT_PREFIX)
```

### Comparing `inmanta-core-8.2.0/src/inmanta/const.py` & `inmanta-core-8.3.0/src/inmanta/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,22 +199,20 @@
     LogLevel.ERROR: 40,
     LogLevel.WARNING: 30,
     LogLevel.INFO: 20,
     LogLevel.DEBUG: 10,
     LogLevel.TRACE: 3,
 }
 
-
 # The following code registers the integer log levels as values
 # in the LogLevel enum.  It allows to pass them in the constructor
 # as if it was an integer enum: LogLevel(50) == LogLevel.CRITICAL
 for level, value in LOG_LEVEL_AS_INTEGER.items():
     LogLevel._value2member_map_[value] = level
 
-
 INMANTA_URN = "urn:inmanta:"
 
 
 class Compilestate(str, Enum):
     """
     Compile state, whether the compile did succeed or not
     """
@@ -238,30 +236,27 @@
 
 
 # For testing
 
 # assume we are running in a tty
 ENVIRON_FORCE_TTY = "FORCE_TTY"
 
-
 LOG_LEVEL_TRACE = 3
 
 NAME_RESOURCE_ACTION_LOGGER = "resource_action_logger"
 
-
 # Time we give the server/agent to shutdown gracefully, before we force stop the ioloop
 SHUTDOWN_GRACE_IOLOOP = 10
 # Time we give the server/agent to shutdown gracefully, before we execute sys.exit(3)
 SHUTDOWN_GRACE_HARD = 15
 # Hard shutdown exit code
 EXIT_HARD = 3
 # Startup failed exit code
 EXIT_START_FAILED = 4
 
-
 TIME_ISOFMT = "%Y-%m-%dT%H:%M:%S.%f"
 TIME_LOGFMT = "%Y-%m-%d %H:%M:%S%z"
 
 PLUGINS_PACKAGE = "inmanta_plugins"
 
 # namespace in which extensions are discovered
 EXTENSION_NAMESPACE = "inmanta_ext"
@@ -270,14 +265,17 @@
 
 # Default envelope key
 ENVELOPE_KEY = "data"
 
 # Max number of attempts when updating modules
 MAX_UPDATE_ATTEMPT = 5
 
+# Minimum password length
+MIN_PASSWORD_LENGTH = 8
+
 
 class AgentAction(str, Enum):
     pause = "pause"
     unpause = "unpause"
     keep_paused_on_resume = "keep_paused_on_resume"
     unpause_on_resume = "unpause_on_resume"
```

### Comparing `inmanta-core-8.2.0/src/inmanta/data/__init__.py` & `inmanta-core-8.3.0/src/inmanta/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 import inmanta.db.versions
 import inmanta.resources as resources
 import inmanta.util as util
 from crontab import CronTab
 from inmanta.const import DONE_STATES, UNDEPLOYABLE_NAMES, AgentStatus, LogLevel, ResourceState
 from inmanta.data import model as m
 from inmanta.data import schema
-from inmanta.data.model import PagingBoundaries, ResourceIdStr, api_boundary_datetime_normalizer
+from inmanta.data.model import AuthMethod, PagingBoundaries, ResourceIdStr, api_boundary_datetime_normalizer
 from inmanta.protocol.common import custom_json_encoder
 from inmanta.protocol.exceptions import BadRequest, NotFound
 from inmanta.server import config
 from inmanta.stable_api import stable_api
 from inmanta.types import JsonType, PrimitiveTypes
 
 LOGGER = logging.getLogger(__name__)
@@ -1550,15 +1550,19 @@
     async def insert(self, connection: Optional[asyncpg.connection.Connection] = None) -> None:
         """
         Insert a new document based on the instance passed. Validation is done based on the defined fields.
         """
         (column_names, values) = self._get_column_names_and_values()
         column_names_as_sql_string = ",".join(column_names)
         values_as_parameterize_sql_string = ",".join(["$" + str(i) for i in range(1, len(values) + 1)])
-        query = f"INSERT INTO {self.table_name()} ({column_names_as_sql_string}) VALUES ({values_as_parameterize_sql_string})"
+        query = (
+            f"INSERT INTO {self.table_name()} "
+            f"({column_names_as_sql_string}) "
+            f"VALUES ({values_as_parameterize_sql_string})"
+        )
         await self._execute_query(query, *values, connection=connection)
 
     @classmethod
     async def _fetchval(cls, query: str, *values: object, connection: Optional[asyncpg.connection.Connection] = None) -> object:
         async with cls.get_connection(connection) as con:
             return await con.fetchval(query, *values)
 
@@ -1614,15 +1618,15 @@
         for doc in documents:
             current_record = []
             for col in columns:
                 current_record.append(cls._get_value(doc.__getattribute__(col)))
             records.append(tuple(current_record))
 
         async with cls.get_connection(connection) as con:
-            await con.copy_records_to_table(table_name=cls.table_name(), columns=columns, records=records)
+            await con.copy_records_to_table(table_name=cls.table_name(), columns=columns, records=records, schema_name="public")
 
     def add_default_values_when_undefined(self, **kwargs: object) -> Dict[str, object]:
         result = dict(kwargs)
         for name, field in self._fields.items():
             if name not in kwargs:
                 default_value = field.default_value
                 result[name] = default_value
@@ -2062,15 +2066,15 @@
             )
             for i, (operator, bound) in enumerate(value)
         )
         return (filter_statement, [cls._get_value(v) for v in values])
 
     @staticmethod
     def _combine_filter_statements(statements_and_values: Iterable[Tuple[str, List[object]]]) -> Tuple[str, List[object]]:
-        statements: Tuple[str]
+        filter_statements: Tuple[str]
         values: Tuple[List[object]]
         filter_statements, values = zip(*statements_and_values)  # type: ignore
         return (
             " AND ".join(s for s in filter_statements if s != ""),
             list(chain.from_iterable(values)),
         )
 
@@ -2467,19 +2471,19 @@
             validator=convert_agent_trigger_method,
             doc="The agent trigger method to use when " + PUSH_ON_AUTO_DEPLOY + " is enabled",
             allowed_values=[opt.name for opt in const.AgentTriggerMethod],
         ),
         ENVIRONMENT_AGENT_TRIGGER_METHOD: Setting(
             name=ENVIRONMENT_AGENT_TRIGGER_METHOD,
             typ="enum",
-            default=const.AgentTriggerMethod.push_full_deploy.name,
+            default=const.AgentTriggerMethod.push_incremental_deploy.name,
             validator=convert_agent_trigger_method,
-            doc="The agent trigger method to use. "
-            f"If {PUSH_ON_AUTO_DEPLOY} is enabled, "
-            f"{AGENT_TRIGGER_METHOD_ON_AUTO_DEPLOY} overrides this setting",
+            doc="The agent trigger method to use when no specific method is specified in the API call. "
+            "This determines the behavior of the 'Promote' button. "
+            f"For auto deploy, {AGENT_TRIGGER_METHOD_ON_AUTO_DEPLOY} is used.",
             allowed_values=[opt.name for opt in const.AgentTriggerMethod],
         ),
         AUTOSTART_SPLAY: Setting(
             name=AUTOSTART_SPLAY,
             typ="int",
             default=10,
             doc="[DEPRECATED] Splay time for autostarted agents.",
@@ -2883,14 +2887,15 @@
         query = "SELECT * FROM " + cls.table_name() + " WHERE environment=$1"
         values = [cls._get_value(env_id)]
         for key, value in metadata_constraints.items():
             query_param_index = len(values) + 1
             query += " AND metadata @> $" + str(query_param_index) + "::jsonb"
             dict_value = {key: value}
             values.append(cls._get_value(dict_value))
+        query += " ORDER BY name"
         result = await cls.select_query(query, values)
         return result
 
     def as_fact(self) -> m.Fact:
         assert self.source == "fact"
         return m.Fact(
             id=self.id,
@@ -2938,14 +2943,54 @@
             source=self.source,
             resource_id=self.resource_id,
             version=new_version,
             metadata=self.metadata,
             resolved=self.resolved,
         )
 
+    @classmethod
+    async def get_unknowns_to_copy_in_partial_compile(
+        cls,
+        environment: uuid.UUID,
+        source_version: int,
+        updated_resource_sets: abc.Set[str],
+        deleted_resource_sets: abc.Set[str],
+        rids_in_partial_compile: abc.Set[ResourceIdStr],
+        *,
+        connection: Optional[asyncpg.connection.Connection] = None,
+    ) -> List["UnknownParameter"]:
+        """
+        Returns a subset of the unknowns in source_version of environment. It returns the unknowns that:
+            * Are not associated with a resource
+            * Are associated with a resource that:
+               - don't belong to the resource set updated_resource_sets and deleted_resource_sets
+               - and, don't have a resource_id in rids_in_partial_compile (An unknown might belong to a shared resource that
+                 is not exported by the partial compile)
+        """
+        query = f"""
+            SELECT u.*
+            FROM {cls.table_name()} AS u LEFT JOIN {Resource.table_name()} AS r
+                ON u.environment=r.environment AND u.version=r.model AND u.resource_id=r.resource_id
+            WHERE
+                u.environment=$1
+                AND u.version=$2
+                AND u.resolved IS FALSE
+                AND (r.resource_id IS NULL OR NOT r.resource_id=ANY($4))
+                AND (r.resource_set IS NULL OR NOT r.resource_set=ANY($3))
+        """
+        async with cls.get_connection(connection) as con:
+            result = await con.fetch(
+                query,
+                environment,
+                source_version,
+                list(updated_resource_sets | deleted_resource_sets),
+                list(rids_in_partial_compile),
+            )
+            return [cls(from_postgres=True, **uk) for uk in result]
+
 
 class AgentProcess(BaseDocument):
     """
     A process in the infrastructure that has (had) a session as an agent.
 
     :param hostname: The hostname of the device.
     :param environment: To what environment is this process bound
@@ -3118,15 +3163,14 @@
         connection: Optional[asyncpg.connection.Connection] = None,
     ) -> None:
         """
         Create new agent instances for a given session.
         """
         if not endpoints:
             return
-
         async with cls.get_connection(connection) as con:
             await con.executemany(
                 f"""
                 INSERT INTO
                 {cls.table_name()}
                 (id, tid, process, name, expired)
                 VALUES ($1, $2, $3, $4, null)
@@ -3329,15 +3373,15 @@
 
         :param env: The environment of the agent
         :param endpoints_with_new_primary: Contains a tuple (agent-name, sid) for each agent that has got a new
                                            primary agent instance. The sid in the tuple is the session id of the new
                                            primary. If the session id is None, the Agent doesn't have a primary anymore.
         :param now: Timestamp of this failover
         """
-        for (endpoint, sid) in endpoints_with_new_primary:
+        for endpoint, sid in endpoints_with_new_primary:
             # Lock mode is required because we will update in this transaction
             # Deadlocks with cleanup otherwise
             agent = await cls.get(env, endpoint, connection=connection, lock=RowLockMode.FOR_UPDATE)
             if agent is None:
                 continue
 
             if sid is None:
@@ -3354,14 +3398,39 @@
         query = f"""
                 UPDATE {cls.table_name()}
                 SET id_primary=NULL
                 WHERE id_primary IS NOT NULL
         """
         await cls._execute_query(query, connection=connection)
 
+    @classmethod
+    async def clean_up(cls, connection: Optional[asyncpg.connection.Connection] = None) -> None:
+        query = """
+DELETE FROM public.agent AS a
+WHERE (environment, name) NOT IN (
+    SELECT DISTINCT environment_id as environment, agent as name
+    FROM (
+        -- agent is in the agent map
+        SELECT e.id as environment_id, map.key as agent
+        FROM public.environment e
+        CROSS JOIN LATERAL jsonb_each(e.settings->'autostart_agent_map') AS map(key, value)
+    ) in_agent_map
+)
+-- have no primary ID set (that are down)
+AND id_primary IS NULL
+-- not used by any version
+AND NOT EXISTS (
+    SELECT 1
+    FROM public.resource AS re
+    WHERE a.environment=re.environment
+    AND a.name=re.agent
+);
+"""
+        await cls._execute_query(query, connection=connection)
+
 
 @stable_api
 class Report(BaseDocument):
     """
     A report of a substep of compilation
 
     :param started: when the substep started
@@ -4234,14 +4303,19 @@
         record["resource_version_id"] = parsed_id.resource_version_str()
         record["id"] = record["resource_version_id"]
         record["resource_type"] = parsed_id.entity_type
         if "requires" in record["attributes"]:
             record["attributes"]["requires"] = [
                 resources.Id.set_version_in_id(id, version) for id in record["attributes"]["requires"]
             ]
+        # Due to a bug, the version field has always been present in the attributes dictionary.
+        # This bug has been fixed in the database. For backwards compatibility reason we here make sure that the
+        # version field is present in the attributes dictionary served out via the API.
+        if "version" not in record["attributes"]:
+            record["attributes"]["version"] = version
         record["provides"] = [resources.Id.set_version_in_id(id, version) for id in record["provides"]]
 
     @classmethod
     async def get_last_non_deploying_state_for_dependencies(
         cls, environment: uuid.UUID, resource_version_id: "resources.Id", connection: Optional[Connection] = None
     ) -> Dict[m.ResourceVersionIdStr, ResourceState]:
         """
@@ -4523,14 +4597,36 @@
             resource_id_value=vid.attribute_value,
         )
 
         attr.update(kwargs)
 
         return cls(**attr)
 
+    def copy_for_partial_compile(self, new_version: int) -> "Resource":
+        """
+        Create a new resource dao instance from this dao instance. Only creates the object without inserting it.
+        The new instance will have the given version.
+        """
+        new_resource_state = ResourceState.undefined if self.status is ResourceState.undefined else ResourceState.available
+        return Resource(
+            environment=self.environment,
+            model=new_version,
+            resource_id=self.resource_id,
+            resource_type=self.resource_type,
+            resource_id_value=self.resource_id_value,
+            agent=self.agent,
+            last_deploy=None,
+            attributes=self.attributes.copy(),
+            attribute_hash=self.attribute_hash,
+            status=new_resource_state,
+            last_non_deploying_status=const.NonDeployingResourceState[new_resource_state.name],
+            resource_set=self.resource_set,
+            provides=self.provides,
+        )
+
     @classmethod
     async def get_deleted_resources(
         cls,
         environment: uuid.UUID,
         current_version: int,
         current_resources: Sequence[m.ResourceIdStr],
         *,
@@ -4634,16 +4730,17 @@
         THEN 'orphaned'
         ELSE resource.status::text END
         ) as status
         """
 
         query = f"""
         SELECT DISTINCT ON (resource_id) first.resource_id, cm.date as first_generated_time,
-        first.model as first_model, latest.resource_id as latest_resource_id, latest.resource_type,
-        latest.agent, latest.resource_id_value, latest.last_deploy as latest_deploy, latest.attributes, latest.status
+        first.model as first_model, latest.model AS latest_model, latest.resource_id as latest_resource_id,
+        latest.resource_type, latest.agent, latest.resource_id_value, latest.last_deploy as latest_deploy, latest.attributes,
+        latest.status
         FROM resource first
         INNER JOIN
             /* 'latest' is the latest released version of the resource */
             (SELECT distinct on (resource_id) resource_id, attribute_hash, model, last_deploy, attributes,
                 resource_type, agent, resource_id_value, {status_subquery}
                 FROM resource
                 JOIN configurationmodel cm ON resource.model = cm.version AND resource.environment = cm.environment
@@ -4661,14 +4758,19 @@
         result = await cls.select_query(query, values, no_obj=True)
 
         if not result:
             return None
         record = result[0]
         parsed_id = resources.Id.parse_id(record["latest_resource_id"])
         attributes = json.loads(record["attributes"])
+        # Due to a bug, the version field has always been present in the attributes dictionary.
+        # This bug has been fixed in the database. For backwards compatibility reason we here make sure that the
+        # version field is present in the attributes dictionary served out via the API.
+        if "version" not in attributes:
+            attributes["version"] = record["latest_model"]
         requires = [resources.Id.parse_id(req).resource_str() for req in attributes["requires"]]
 
         # fetch the status of each of the requires. This is not calculated in the database because the lack of joinable
         # fields requires to calculate the status for each resource record, before it is filtered
         status_query = f"""
         SELECT DISTINCT ON (resource_id) resource_id, {status_subquery}
         FROM resource
@@ -4724,14 +4826,103 @@
         """
         raw_results = await cls._fetch_query(query, cls._get_value(environment))
         results = {}
         for row in raw_results:
             results[row["status"]] = row["count"]
         return m.ResourceDeploySummary.create_from_db_result(results)
 
+    @classmethod
+    async def copy_resources_from_unchanged_resource_set(
+        cls,
+        environment: uuid.UUID,
+        source_version: int,
+        destination_version: int,
+        updated_resource_sets: abc.Set[str],
+        deleted_resource_sets: abc.Set[str],
+        *,
+        connection: Optional[asyncpg.connection.Connection] = None,
+    ) -> abc.Set[m.ResourceIdStr]:
+        """
+        Copy the resources that belong to an unchanged resource set of a partial compile,
+        from source_version to destination_version. This method doesn't copy shared resources.
+        """
+        query = f"""
+            INSERT INTO {cls.table_name()}(
+                environment,
+                model,
+                resource_id,
+                resource_type,
+                resource_id_value,
+                agent,
+                status,
+                attributes,
+                attribute_hash,
+                resource_set,
+                provides
+            )(
+                SELECT
+                    r.environment,
+                    $3,
+                    r.resource_id,
+                    r.resource_type,
+                    r.resource_id_value,
+                    r.agent,
+                    (
+                        CASE WHEN r.status='undefined'::resourcestate
+                        THEN 'undefined'::resourcestate
+                        ELSE 'available'::resourcestate
+                        END
+                    ) AS status,
+                    r.attributes AS attributes,
+                    r.attribute_hash,
+                    r.resource_set,
+                    r.provides
+                FROM {cls.table_name()} AS r
+                WHERE r.environment=$1 AND r.model=$2 AND r.resource_set IS NOT NULL AND NOT r.resource_set=ANY($4)
+            )
+            RETURNING resource_id
+        """
+        async with cls.get_connection(connection) as con:
+            result = await con.fetch(
+                query,
+                environment,
+                source_version,
+                destination_version,
+                updated_resource_sets | deleted_resource_sets,
+            )
+            return {record["resource_id"] for record in result}
+
+    @classmethod
+    async def get_resources_in_resource_sets(
+        cls,
+        environment: uuid.UUID,
+        version: int,
+        resource_sets: abc.Set[str],
+        include_shared_resources: bool = False,
+        *,
+        connection: Optional[asyncpg.connection.Connection] = None,
+    ) -> abc.Mapping[ResourceIdStr, "Resource"]:
+        """
+        Returns the resource in the given environment and version that belong to any of the given resource sets.
+        This method also returns the resources in the share resource set iff the include_shared_resources boolean
+        is set to True.
+        """
+        if include_shared_resources:
+            resource_set_filter_statement = "(r.resource_set IS NULL OR r.resource_set=ANY($3))"
+        else:
+            resource_set_filter_statement = "r.resource_set=ANY($3)"
+        query = f"""
+            SELECT *
+            FROM {cls.table_name()} AS r
+            WHERE r.environment=$1 AND r.model=$2 AND {resource_set_filter_statement}
+        """
+        async with cls.get_connection(connection) as con:
+            result = await con.fetch(query, environment, version, resource_sets)
+            return {record["resource_id"]: cls(from_postgres=True, **record) for record in result}
+
     async def insert(self, connection: Optional[asyncpg.connection.Connection] = None) -> None:
         self.make_hash()
         await super(Resource, self).insert(connection=connection)
 
     @classmethod
     async def insert_many(
         cls, documents: Sequence["Resource"], *, connection: Optional[asyncpg.connection.Connection] = None
@@ -4744,27 +4935,41 @@
         self.make_hash()
         await super(Resource, self).update(connection=connection, **kwargs)
 
     async def update_fields(self, connection: Optional[asyncpg.connection.Connection] = None, **kwargs: Any) -> None:
         self.make_hash()
         await super(Resource, self).update_fields(connection=connection, **kwargs)
 
+    def get_requires(self) -> abc.Sequence[ResourceIdStr]:
+        """
+        Returns the content of the requires field in the attributes.
+        """
+        if "requires" not in self.attributes:
+            return []
+        return list(self.attributes["requires"])
+
     def to_dict(self) -> Dict[str, Any]:
         self.make_hash()
         dct = super(Resource, self).to_dict()
         self.__mangle_dict(dct)
         return dct
 
     def to_dto(self) -> m.Resource:
         attributes = self.attributes.copy()
 
         if "requires" in self.attributes:
             version = self.model
             attributes["requires"] = [resources.Id.set_version_in_id(id, version) for id in self.attributes["requires"]]
 
+        # Due to a bug, the version field has always been present in the attributes dictionary.
+        # This bug has been fixed in the database. For backwards compatibility reason we here make sure that the
+        # version field is present in the attributes dictionary served out via the API.
+        if "version" not in self.attributes:
+            attributes["version"] = self.model
+
         return m.Resource(
             environment=self.environment,
             model=self.model,
             resource_id=self.resource_id,
             resource_type=self.resource_type,
             resource_version_id=resources.Id.set_version_in_id(self.resource_id, self.model),
             agent=self.agent,
@@ -4786,27 +4991,31 @@
     :param date: The date this configuration model was created
     :param partial_base: If this version was calculated from a partial export, the version the partial was applied on.
     :param released: Is this model released and available for deployment?
     :param deployed: Is this model deployed?
     :param result: The result of the deployment. Success or error.
     :param version_info: Version metadata
     :param total: The total number of resources
+    :param is_suitable_for_partial_compiles: This boolean indicates whether the model can later on be updated using a
+                                             partial compile. In other words, the value is True iff no cross resource set
+                                             dependencies exist between the resources.
     """
 
     __primary_key__ = ("version", "environment")
 
     version: int
     environment: uuid.UUID
     date: Optional[datetime.datetime] = None
     partial_base: Optional[int] = None
 
     released: bool = False
     deployed: bool = False
     result: const.VersionState = const.VersionState.pending
     version_info: Optional[Dict[str, Any]] = None
+    is_suitable_for_partial_compiles: bool
 
     total: int = 0
 
     # cached state for release
     undeployable: List[m.ResourceIdStr] = []
     skipped_for_undeployable: List[m.ResourceIdStr] = []
 
@@ -4824,14 +5033,137 @@
         # Keep resources which are deployed in done, even when a repair operation
         # changes its state to deploying again.
         if self.deployed:
             return self.total
         return self._done
 
     @classmethod
+    async def create_for_partial_compile(
+        cls,
+        env_id: uuid.UUID,
+        version: int,
+        total: int,
+        version_info: Optional[JsonType],
+        undeployable: abc.Sequence[ResourceIdStr],
+        skipped_for_undeployable: abc.Sequence[ResourceIdStr],
+        partial_base: int,
+        rids_in_partial_compile: abc.Set[ResourceIdStr],
+        connection: Optional[Connection] = None,
+    ) -> "ConfigurationModel":
+        """
+        Create and insert a new configurationmodel that is the result of a partial compile. The new ConfigururationModel will
+        contain all the undeployables and skipped_for_undeployables present in the partial_base version that are not part of
+        the partial compile, i.e. not present in rids_in_partial_compile.
+        """
+        query = f"""
+            WITH base_version_exists AS (
+                SELECT EXISTS(
+                    SELECT 1
+                    FROM {cls.table_name()} AS c1
+                    WHERE c1.environment=$1 AND c1.version=$8
+                ) AS base_version_found
+            ),
+            rids_undeployable_base_version AS (
+                SELECT DISTINCT unnest(c2.undeployable) AS rid
+                FROM {cls.table_name()} AS c2
+                WHERE c2.environment=$1 AND c2.version=$8
+            ),
+            rids_skipped_for_undeployable_base_version AS (
+                SELECT DISTINCT unnest(c3.skipped_for_undeployable) AS rid
+                FROM {cls.table_name()} AS c3
+                WHERE c3.environment=$1 AND c3.version=$8
+            )
+            INSERT INTO {cls.table_name()}(
+                environment,
+                version,
+                date,
+                total,
+                version_info,
+                undeployable,
+                skipped_for_undeployable,
+                partial_base,
+                is_suitable_for_partial_compiles
+            ) VALUES(
+                $1,
+                $2,
+                $3,
+                $4,
+                $5,
+                (
+                    SELECT array_agg(rid)
+                    FROM (
+                        -- Undeployables in previous version of the model that are not part of the partial compile.
+                        (
+                            SELECT rid
+                            FROM rids_undeployable_base_version AS undepl
+                            WHERE NOT undepl.rid=ANY($9)
+                        )
+                        UNION
+                        -- Undeployables part of the partial compile.
+                        (
+                            SELECT DISTINCT rid FROM unnest($6::varchar[]) AS undeploy_filtered_new(rid)
+                        )
+                    ) AS all_undeployable
+                ),
+                (
+                    SELECT array_agg(rid)
+                    FROM (
+                        -- skipped_for_undeployables in previous version of the model that are not part of the partial
+                        -- compile.
+                        (
+                            SELECT skipped.rid
+                            FROM rids_skipped_for_undeployable_base_version AS skipped
+                            WHERE NOT skipped.rid=ANY($9)
+                        )
+                        UNION
+                        -- Skipped_for_undeployables part of the partial compile.
+                        (
+                            SELECT DISTINCT rid FROM unnest($7::varchar[]) AS skipped_filtered_new(rid)
+                        )
+                    ) AS all_skipped
+                ),
+                $8,
+                True
+            )
+            RETURNING
+                (SELECT base_version_found FROM base_version_exists LIMIT 1) AS base_version_found,
+                environment,
+                version,
+                date,
+                total,
+                version_info,
+                undeployable,
+                skipped_for_undeployable,
+                partial_base,
+                released,
+                deployed,
+                result,
+                is_suitable_for_partial_compiles
+        """
+        async with cls.get_connection(connection) as con:
+            result = await con.fetchrow(
+                query,
+                env_id,
+                version,
+                datetime.datetime.now().astimezone(),
+                total,
+                cls._get_value(version_info),
+                undeployable,
+                skipped_for_undeployable,
+                partial_base,
+                list(rids_in_partial_compile),
+            )
+            # Make mypy happy
+            assert result is not None
+            if not result["base_version_found"]:
+                raise Exception(f"Model with version {partial_base} not found in environment {env_id}")
+            fields = {name: val for name, val in result.items() if name != "base_version_found"}
+            return cls(from_postgres=True, **fields)
+
+    @classmethod
     async def _get_status_field(cls, environment: uuid.UUID, values: str) -> Dict[str, str]:
         """
         This field is required to ensure backward compatibility on the API.
         """
         result = {}
         values = json.loads(values)
         for value_entry in values:
@@ -4906,15 +5238,15 @@
                 obj._status = status
                 result.append(obj)
         return result
 
     def to_dict(self) -> JsonType:
         dct = BaseDocument.to_dict(self)
         dct["status"] = dict(self._status)
-        dct["done"] = self._done
+        dct["done"] = self.done
         return dct
 
     @classmethod
     async def version_exists(cls, environment: uuid.UUID, version: int) -> bool:
         query = f"""SELECT 1
                             FROM {ConfigurationModel.table_name()}
                             WHERE environment=$1 AND version=$2"""
@@ -5118,15 +5450,15 @@
         values = [cls._get_value(environment)]
         version_records = await cls._fetch_query(query, *values)
 
         versions = [record["version"] for record in version_records]
 
         for version in versions:
             # todo in next version
-            next = []
+            next: list[abc.Mapping[str, object]] = []
 
             vresources = await Resource.get_resources_for_version_raw(environment, version, projection)
             id_to_resource = {r["resource_id"]: r for r in vresources}
 
             for res in work:
                 # not present -> increment
                 if res["resource_id"] not in id_to_resource:
@@ -5242,14 +5574,35 @@
                                         END) as status""",
             from_clause=f" FROM {cls.table_name()} as cm",
             filter_statements=[" environment = $1 "],
             values=values,
         )
         return query_builder.build()
 
+    async def recalculate_total(self, connection: Optional[asyncpg.connection.Connection] = None) -> None:
+        """
+        Make the total field of this ConfigurationModel in-line with the number
+        of resources that are associated with it.
+        """
+        query = f"""
+            UPDATE {self.table_name()} AS c_outer
+            SET total=(
+                SELECT COUNT(*)
+                FROM {self.table_name()} AS c INNER JOIN {Resource.table_name()} AS r
+                     ON c.environment = r.environment AND c.version=r.model
+                WHERE c.environment=$1 AND c.version=$2
+            )
+            WHERE c_outer.environment=$1 AND c_outer.version=$2
+            RETURNING total
+        """
+        new_total = await self._fetchval(query, self.environment, self.version, connection=connection)
+        if new_total is None:
+            raise KeyError(f"Configurationmodel {self.version} in environment {self.environment} was deleted.")
+        self.total = new_total
+
 
 class Code(BaseDocument):
     """
     A code deployment
 
     :param environment: The environment this code belongs to
     :param version: The version of configuration model it belongs to
@@ -5503,14 +5856,35 @@
     timestamp: datetime.datetime
     count: int
     value: float
 
     __primary_key__ = ("environment", "metric_name", "category", "timestamp")
 
 
+class User(BaseDocument):
+    """A user that can authenticate against inmanta"""
+
+    __primary_key__ = ("id",)
+
+    id: uuid.UUID
+    username: str
+    password_hash: str
+    auth_method: AuthMethod
+
+    @classmethod
+    def table_name(cls) -> str:
+        """
+        Return the name of table. we call it inmanta_user to differentiate it from the pg user table.
+        """
+        return "inmanta_user"
+
+    def to_dao(self) -> m.User:
+        return m.User(username=self.username, auth_method=self.auth_method)
+
+
 _classes = [
     Project,
     Environment,
     UnknownParameter,
     AgentProcess,
     AgentInstance,
     Agent,
@@ -5521,14 +5895,15 @@
     Parameter,
     DryRun,
     Compile,
     Report,
     Notification,
     EnvironmentMetricsGauge,
     EnvironmentMetricsTimer,
+    User,
 ]
 
 
 def set_connection_pool(pool: asyncpg.pool.Pool) -> None:
     LOGGER.debug("Connecting data classes")
     for cls in _classes:
         cls.set_connection_pool(pool)
```

### Comparing `inmanta-core-8.2.0/src/inmanta/data/dataview.py` & `inmanta-core-8.3.0/src/inmanta/data/dataview.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     DateRangeFilter,
     Filter,
     FilterValidator,
     IntRangeFilter,
     InvalidFilter,
     LogLevelFilter,
 )
-from inmanta.types import SimpleTypes
+from inmanta.types import JsonType, SimpleTypes
 from inmanta.util import datetime_utc_isoformat
 
 T_ORDER = TypeVar("T_ORDER", bound=DatabaseOrderV2)
 T_DTO = TypeVar("T_DTO", bound=BaseModel)
 
 
 class RequestedPagingBoundaries:
@@ -790,38 +790,48 @@
                       ORDER BY date
                     ) AS seqid
                   FROM resource JOIN configurationmodel cm
                     ON resource.model = cm.version AND resource.environment = cm.environment
                   WHERE resource.environment = $1 AND resource_id = $2 AND cm.released = TRUE
                 )
             """,
-            select_clause="SELECT attribute_hash, date, attributes",
+            select_clause="SELECT attribute_hash, date, attributes, model",
             from_clause="""
             FROM (SELECT
                     attribute_hash,
                     min(date) as date,
+                    min(model) as model,
                         (SELECT distinct on (attribute_hash) attributes
                             FROM resourcewithsequenceids
                             WHERE resourcewithsequenceids.attribute_hash = rs.attribute_hash
                             AND resourcewithsequenceids.seqid = rs.seqid
                             ORDER BY attribute_hash, model
                         ) as attributes
                     FROM resourcewithsequenceids rs
                     GROUP BY attribute_hash,  seqID) as sub
             """,
             values=[self.environment.id, self.rid],
         )
         return query_builder
 
     def construct_dtos(self, records: Sequence[Record]) -> Sequence[ResourceHistory]:
+        def get_attributes(record: Record) -> JsonType:
+            attributes = json.loads(record["attributes"])
+            if "version" not in attributes:
+                # Due to a bug, the version field has always been present in the attributes dictionary.
+                # This bug has been fixed in the database. For backwards compatibility reason we here make sure that the
+                # version field is present in the attributes dictionary served out via the API.
+                attributes["version"] = record["model"]
+            return attributes
+
         return [
             ResourceHistory(
                 resource_id=self.rid,
                 attribute_hash=record["attribute_hash"],
-                attributes=json.loads(record["attributes"]),
+                attributes=get_attributes(record),
                 date=record["date"],
                 requires=[Id.parse_id(rid).resource_str() for rid in json.loads(record["attributes"]).get("requires", [])],
             )
             for record in records
         ]
```

### Comparing `inmanta-core-8.2.0/src/inmanta/data/model.py` & `inmanta-core-8.3.0/src/inmanta/data/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import uuid
 from enum import Enum
 from itertools import chain
 from typing import Any, ClassVar, Dict, List, NewType, Optional, Union
 
 import pydantic
 import pydantic.schema
-from pydantic import Extra, validator
+from pydantic import Extra, root_validator, validator
 from pydantic.fields import ModelField
 
 import inmanta
 import inmanta.ast.export as ast_export
 import inmanta.data
 from inmanta import const, protocol, resources
 from inmanta.stable_api import stable_api
@@ -37,14 +37,16 @@
 old_field_type_schema = pydantic.schema.field_type_schema
 
 
 def patch_pydantic_field_type_schema() -> None:
     """
     This ugly patch fixes the serialization of models containing Optional in them.
     https://github.com/samuelcolvin/pydantic/issues/1270
+
+    The fix for this issue will be included in pydantic V2.
     """
 
     def patch_nullable(field: ModelField, **kwargs):
         f_schema, definitions, nested_models = old_field_type_schema(field, **kwargs)
         if field.allow_none:
             f_schema["nullable"] = True
         return f_schema, definitions, nested_models
@@ -321,51 +323,20 @@
     """
     Represents a resource object as it comes in over the API. Provides strictly required validation only.
     """
 
     id: ResourceVersionIdStr
 
     @classmethod
-    def create_with_version(cls, new_version: int, id: ResourceIdStr, attributes: Dict[str, object]) -> "ResourceMinimal":
-        """
-        Create a new ResourceMinimal from the given attributes, but ensure that the given version
-        is set on all the fields that hold the version number of the model.
-        """
-        if "requires" not in attributes:
-            raise ValueError("'requires' attribute is missing in kwargs")
-        new_attributes = attributes.copy()
-        new_attributes["version"] = new_version
-        new_attributes["id"] = resources.Id.set_version_in_id(id, new_version)
-        new_attributes["requires"] = [
-            resources.Id.set_version_in_id(r, new_version=new_version) for r in attributes["requires"]
-        ]
-        return cls(**new_attributes)
-
-    def copy_with_new_version(self, new_version: int) -> "ResourceMinimal":
-        """
-        Create a new ResourceMinimal by cloning this ResourceMinimal. The returned object
-        will have the given new_version set on all the fields that hold the version number
-        of the mode.
-        """
-        return self.create_with_version(
-            new_version=new_version,
-            id=resources.Id.parse_id(self.id).resource_str(),
-            attributes={k: v for k, v in self.dict().items() if k != "id"},
-        )
-
-    @classmethod
     @validator("id")
     def id_is_resource_version_id(cls, v):
         if resources.Id.is_resource_version_id(v):
             return v
         raise ValueError(f"id {v} is not of type ResourceVersionIdStr")
 
-    def get_resource_id_str(self) -> ResourceIdStr:
-        return resources.Id.parse_id(self.id).resource_str()
-
     class Config:
         extra = Extra.allow
 
 
 class Resource(BaseModel):
     environment: uuid.UUID
     model: int
@@ -517,14 +488,24 @@
     :param resource_version_id: The id of the resource
     :param version: The version of the resource
     """
 
     resource_version_id: ResourceVersionIdStr
     version: int
 
+    @root_validator
+    @classmethod
+    def ensure_version_field_set_in_attributes(cls, v: JsonType) -> JsonType:
+        # Due to a bug, the version field has always been present in the attributes dictionary.
+        # This bug has been fixed in the database. For backwards compatibility reason we here make sure that the
+        # version field is present in the attributes dictionary served out via the API.
+        if "version" not in v["attributes"]:
+            v["attributes"]["version"] = v["version"]
+        return v
+
 
 class ReleasedResourceDetails(ResourceDetails):
     """The details of a released resource
     :param last_deploy: The value of the last_deploy on the latest released version of the resource
     :param first_generated_time: The first time this resource was generated
     :param first_generated_version: The first model version this resource was in
     :param status: The current status of the resource
@@ -718,7 +699,31 @@
                     for that specific time window.
     """
 
     start: datetime.datetime
     end: datetime.datetime
     timestamps: List[datetime.datetime]
     metrics: Dict[str, List[Optional[Union[float, Dict[str, float]]]]]
+
+
+class AuthMethod(str, Enum):
+    database = "database"
+    oidc = "oidc"
+
+
+class User(BaseModel):
+    """A user"""
+
+    username: str
+    auth_method: AuthMethod
+
+
+class LoginReturn(BaseModel):
+    """
+    Login information
+
+    :param token: A token representing the user's authentication session
+    :param user: The user object for which the token was created
+    """
+
+    token: str
+    user: User
```

### Comparing `inmanta-core-8.2.0/src/inmanta/data/schema.py` & `inmanta-core-8.3.0/src/inmanta/data/schema.py`

 * *Files identical despite different names*

```diff
@@ -128,14 +128,15 @@
                     FROM information_schema.columns
                     WHERE table_name=$1 AND column_name=$2
                 )
                 """,
                 SCHEMA_VERSION_TABLE,
                 "current_version",
             )
+
             if legacy_column is None:
                 raise Exception("Failed to query existence of legacy column, this should not happen.")
             if legacy_column["exists"]:
                 self.logger.info("Migrating legacy schema version table")
                 await self.connection.execute(
                     f"""
                     ALTER TABLE {SCHEMA_VERSION_TABLE}
```

### Comparing `inmanta-core-8.2.0/src/inmanta/db/__init__.py` & `inmanta-core-8.3.0/src/inmanta/db/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/__init__.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v1.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     FOREIGN KEY (environment, version) REFERENCES configurationmodel (environment, version) ON DELETE CASCADE
 );
 
 -- Used in:
 --      * server.get_version()
 CREATE INDEX unknownparameter_env_version_index ON unknownparameter (environment, version);
 -- Used in:
---      * server.renew_expired_facts()
+--      * server.renew_facts()
 CREATE INDEX unknownparameter_resolved_index ON unknownparameter (resolved);
 
 -- Table: public.agentprocess
 CREATE TABLE IF NOT EXISTS public.agentprocess (
     hostname varchar NOT NULL,
     environment uuid NOT NULL REFERENCES environment(id) ON DELETE CASCADE,
     first_seen timestamp,
```

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v17.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v17.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v2.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v2.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202105170.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202105170.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202106080.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202106080.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202106210.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202106210.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202109100.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202109100.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202111260.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202111260.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202203140.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202203140.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202203160.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202203160.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202205250.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202205250.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202206290.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202206290.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202208180.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202208180.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202208190.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202208190.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202209090.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202209090.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202209130.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202209130.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202209160.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202209160.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202211230.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202211230.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202212010.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202212010.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202301100.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202301100.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202301110.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202301110.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202301120.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202301120.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202301160.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202301160.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202301170.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202301170.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v202301190.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v202301190.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v3.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v3.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v4.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v4.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v5.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v5.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v6.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v6.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/db/versions/v7.py` & `inmanta-core-8.3.0/src/inmanta/db/versions/v7.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/deploy.py` & `inmanta-core-8.3.0/src/inmanta/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,16 @@
             fd.write(config_file)
 
         log_file = os.path.join(log_dir, "inmanta.log")
         args = [
             sys.executable,
             "-m",
             "inmanta.app",
-            "-vvv",
+            "--log-file-level",
+            "DEBUG",
             "-c",
             server_config,
             "--config-dir",
             Config._config_dir if Config._config_dir is not None else "",
             "--log-file",
             log_file,
             "server",
```

### Comparing `inmanta-core-8.2.0/src/inmanta/docstring_parser.py` & `inmanta-core-8.3.0/src/inmanta/docstring_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/env.py` & `inmanta-core-8.3.0/src/inmanta/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,14 @@
     Can be used in two ways:
     - if we don't know the exact conflicts (detected by e.g. pip), the messages is used
     - if we have detailed conflict info, the message is derived from it
 
     """
 
     def __init__(self, message: str, conflicts: Optional[Set[VersionConflict]] = None):
-
         CompilerException.__init__(self, msg=message)
         self.conflicts = conflicts
 
     def get_message(self) -> str:
         # The message has three potential parts
         # First the advices, derived from the conflicts, if present
         # Then the message, if present
@@ -1004,19 +1003,19 @@
             packages meet the given constraints. All listed packages are expected to be installed.
         :return: True iff the check succeeds.
         """
         constraint_violations_non_strict, constraint_violations_strict = cls.get_constraint_violations_for_check(
             in_scope, constraints
         )
 
-        dist_info: DistInfoDistribution
+        working_set: abc.Iterable[DistInfoDistribution] = pkg_resources.working_set
         # add all requirements of all in scope packages installed in this environment
         all_constraints: Set[Requirement] = set(constraints if constraints is not None else []).union(
             requirement
-            for dist_info in pkg_resources.working_set
+            for dist_info in working_set
             if in_scope.fullmatch(dist_info.key)
             for requirement in dist_info.requires()
         )
 
         installed_versions: Dict[str, version.Version] = PythonWorkingSet.get_packages_in_working_set()
         constraint_violations: Set[VersionConflict] = set(
             VersionConflict(constraint, installed_versions.get(constraint.key, None))
```

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/__init__.py` & `inmanta-core-8.3.0/src/inmanta/execute/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/dataflow/__init__.py` & `inmanta-core-8.3.0/src/inmanta/execute/dataflow/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/dataflow/datatrace.py` & `inmanta-core-8.3.0/src/inmanta/execute/dataflow/datatrace.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/dataflow/graphic.py` & `inmanta-core-8.3.0/src/inmanta/execute/dataflow/graphic.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/dataflow/root_cause.py` & `inmanta-core-8.3.0/src/inmanta/execute/dataflow/root_cause.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/proxy.py` & `inmanta-core-8.3.0/src/inmanta/execute/proxy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/runtime.py` & `inmanta-core-8.3.0/src/inmanta/execute/runtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     limitations under the License.
 
     Contact: code@inmanta.com
 """
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Deque, Dict, Generic, Hashable, List, Optional, Set, TypeVar, Union, cast
 
-import inmanta.ast.attribute  # noqa: F401 (pep8 does not recognize partially qualified access ast.attribute)
+import inmanta.ast.attribute  # noqa: F401 (pyflakes does not recognize partially qualified access ast.attribute)
 from inmanta import ast
 from inmanta.ast import (
     AttributeException,
     CompilerException,
     DoubleSetException,
     Locatable,
     Location,
@@ -47,22 +47,36 @@
 
 
 T = TypeVar("T")
 
 
 class ResultCollector(Generic[T]):
     """
-    Helper interface for gradual execution
+    Helper interface for gradual execution. Should be attached as a listener to a ResultVariable, which will then call
+    receive_result whenever it receives a new value.
     """
 
     __slots__ = ()
 
-    def receive_result(self, value: T, location: Location) -> None:
+    def pure_gradual(self) -> bool:
         """
-        receive a possibly partial result
+        Returns true iff this result collector represents pure gradual execution, i.e. all progress comes from new values and
+        no progress is expected as a result of the variable being frozen.
+
+        This is a static property of a result collector, i.e. this method will always have the same result at any point within
+        the lifetime of the instance.
+        """
+        return True
+
+    def receive_result(self, value: T, location: Location) -> bool:
+        """
+        Receive a single value for gradual execution. Called once for each value that is part of the result.
+
+        :return: Whether this collector is complete, i.e. it does not need to receive any further results and its associated
+            waiter will no longer cause progress. Once this is signalled, this instance should get no further results.
         """
         raise NotImplementedError()
 
 
 class IPromise:
     """
     A promise to the owner to provide a value or progression towards a value in some way, either directly or indirectly.
@@ -127,14 +141,20 @@
         """
         raise NotImplementedError()
 
     def listener(self, resultcollector: ResultCollector[T], location: Location) -> None:
         """
         Add a listener to report new values to. If the variable already has a value, this is reported immediately. Explicit
         assignments of `null` will not be reported.
+
+        Each listener is expected to register one associated waiter to track completeness. The progress potential implementation
+        is based on this invariant.
+
+        :param resultcollector: The collector for the values of this variable.
+        :param location: The location associated with this listener.
         """
         raise NotImplementedError()
 
     def waitfor(self, waiter: "Waiter") -> None:
         """
         Informs this variable that a waiter waits on its value. Once the variable receives a value, it should inform the waiter.
         """
@@ -262,16 +282,16 @@
 
     def can_get(self) -> bool:
         return self.hasValue
 
     def freeze(self) -> None:
         pass
 
-    def receive_result(self, value: T, location: Location) -> None:
-        pass
+    def receive_result(self, value: T, location: Location) -> bool:
+        return True
 
     def listener(self, resultcollector: ResultCollector[T], location: Location) -> None:
         """
         Add a listener to report new values to, only for lists. Explicit assignments of `null` will not be reported.
         """
         pass
 
@@ -421,15 +441,15 @@
     DelayedResultVariable are queued with the scheduler at the point at which they might be complete.
     The scheduler can decide when to freeze them. A DelayedResultVariable  can be complete when
       - it contains enough elements
       - there are no providers which still have to provide some values (tracked inexactly)
         (a queue variable can be dequeued by the scheduler when a provider is added)
     """
 
-    __slots__ = ("queued", "queues", "listeners", "promises", "done_promises")
+    __slots__ = ("queued", "queues", "promises", "done_promises")
 
     def __init__(self, queue: "QueueScheduler", value: Optional[T] = None) -> None:
         ResultVariable.__init__(self, value)
         self.promises: Optional[List[IPromise]] = []
         self.done_promises: Optional[Set[IPromise]] = set()
         self.queued = False
         self.queues = queue
@@ -463,15 +483,14 @@
             return
         self.queued = True
         self.hasValue = True
         for waiter in self.waiters:
             waiter.ready(self)
         # prevent memory leaks
         self.waiters = None
-        self.listeners = None
         self.queues = None
         self.promises = None
         self.done_promises = None
 
     def queue(self) -> None:
         if self.queued:
             return
@@ -490,32 +509,38 @@
         assert self.done_promises is not None
         out = len(self.promises) - len(self.done_promises)
         if out < 0:
             raise Exception("SEVERE: COMPILER STATE CORRUPT: provide count negative")
         return out
 
     def get_progress_potential(self) -> int:
-        """How many are actually waiting for us"""
-        raise NotImplementedError()
+        """
+        Returns the number of blocked waiters, meaning any waiters that may progress when this variable is frozen.
+        """
+        return len(self.waiters)
 
 
 ListValue = Union["Instance", List["Instance"]]
 
 
 class BaseListVariable(DelayedResultVariable[ListValue]):
     """
     List variable, but only the part that is independent of an instance
     """
 
     value: "List[Instance]"
 
-    __slots__ = ()
+    __slots__ = ("_listeners", "_nb_gradual_waiters")
 
     def __init__(self, queue: "QueueScheduler") -> None:
-        self.listeners: List[ResultCollector[ListValue]] = []
+        # use dict for easy lookup with reliable ordering
+        self._listeners: Optional[dict[ResultCollector[ListValue], None]] = {}
+        # Cache count for waiters without progress potential. Meaning waiters associated with either a purely gradual
+        # listener or with a listener that indicated it is done.
+        self._nb_gradual_waiters: int = 0
         super().__init__(queue, [])
 
     def _set_value(self, value: ListValue, location: Location, recur: bool = True) -> bool:
         """
         First half of set_value, returns True if second half should run
         """
         if self.hasValue:
@@ -557,60 +582,86 @@
         if value in self.value:
             # any set_value may fulfill a promise, allowing this object to be queued
             if self.can_get():
                 self.queue()
             return False
 
         self.value.append(value)
-
-        for listener in self.listeners:
-            listener.receive_result(value, location)
+        self._notify_listeners(value, location)
 
         return True
 
+    def _notify_listeners(self, value: ListValue, location: Location) -> None:
+        """
+        Notifies all listeners about a new value. Deregisters any listeners that indicate they no longer wish to receive
+        results.
+        """
+        assert self._listeners is not None
+        for listener in list(self._listeners.keys()):
+            done: bool = listener.receive_result(value, location)
+            if done:
+                if not listener.pure_gradual():
+                    # listener used to have progress potential but not anymore
+                    self._nb_gradual_waiters += 1
+                # keep memory footprint minimal
+                del self._listeners[listener]
+
     def set_value(self, value: ListValue, location: Location, recur: bool = True) -> None:
         if not self._set_value(value, location, recur):
             return
         if self.can_get():
             self.queue()
 
     def can_get(self) -> bool:
         return self.get_waiting_providers() == 0
 
-    def receive_result(self, value: ListValue, location: Location) -> None:
+    def receive_result(self, value: ListValue, location: Location) -> bool:
         self.set_value(value, location)
+        return False
 
     def listener(self, resultcollector: ResultCollector, location: Location) -> None:
         for value in self.value:
             resultcollector.receive_result(value, location)
         if not self.hasValue:
-            self.listeners.append(resultcollector)
+            assert self._listeners is not None
+            if resultcollector in self._listeners:
+                # may happen in case of a duplicate assignment, e.g. `x.a = [y.a, y.a]`
+                # consider the new one to have no progress potential because we don't track it separately
+                self._nb_gradual_waiters += 1
+                return
+            self._listeners[resultcollector] = None
+            if resultcollector.pure_gradual():
+                self._nb_gradual_waiters += 1
 
     def is_multi(self) -> bool:
         return True
 
+    def get_progress_potential(self) -> int:
+        # purely gradual waiters aren't blocked on this variable being frozen
+        return len(self.waiters) - self._nb_gradual_waiters
+
+    def freeze(self) -> None:
+        super().freeze()
+        # prevent memory leaks
+        self._listeners = None
+
     def __str__(self) -> str:
         return "BaseListVariable %s" % (self.value)
 
 
 # known issue: typed as ResultVariable[ListValue] but is actually ResultVariable[object]
 class ListLiteral(BaseListVariable):
     """
     Transient variable to represent a list (of either constants or instances) literal (not a variable).
     Requires all providers to acquire a promise before the first gets fulfilled and in return provides accurate promise
     tracking and freezing. Instances of this class should never require forceful freezing.
     """
 
     __slots__ = ()
 
-    def get_progress_potential(self) -> int:
-        """How many are actually waiting for us"""
-        # A ListLiteral is never associated with an Entity, so it cannot have a relation precedence rule.
-        return len(self.waiters) - len(self.listeners)
-
     def fulfill(self, promise: IPromise) -> None:
         """
         Fulfill a promise with 100% accurate promise tracking. Because of this class' invariant that all promises are
         acquired before the first is fulfilled, the list can safely be frozen once all registered promises have been fulfilled.
         """
         super().fulfill(promise)
         # 100% accurate promisse tracking
@@ -677,18 +728,17 @@
     def can_get(self) -> bool:
         return len(self.value) >= self.attribute.low and self.get_waiting_providers() == 0
 
     def __str__(self) -> str:
         return "ListVariable %s %s = %s" % (self.myself, self.attribute, self.value)
 
     def get_progress_potential(self) -> int:
-        """How many are actually waiting for us"""
         # Ensure that relationships with a relation precedence rule cannot end up in the zerowaiters queue
         # of the scheduler. We know the order in which those types can be frozen safely.
-        return len(self.waiters) - len(self.listeners) + int(self.attribute.has_relation_precedence_rules())
+        return super().get_progress_potential() + int(self.attribute.has_relation_precedence_rules())
 
 
 class OptionVariable(DelayedResultVariable["Instance"], RelationAttributeVariable):
     """
     Variable to hold the value for an optional relation (arity [0:1])
     """
 
@@ -749,16 +799,15 @@
             raise OptionalValueException(self.myself, self.attribute)
         return result
 
     def __str__(self) -> str:
         return "OptionVariable %s %s = %s" % (self.myself, self.attribute, self.value)
 
     def get_progress_potential(self) -> int:
-        """How many are actually waiting for us"""
-        return len(self.waiters) + int(self.attribute.has_relation_precedence_rules())
+        return super().get_progress_potential() + int(self.attribute.has_relation_precedence_rules())
 
 
 class QueueScheduler(object):
     """
     Object representing the compiler to the AST nodes. It provides access to the queueing mechanism and the type system.
 
     MUTABLE!
@@ -1011,15 +1060,14 @@
 
 """
 
 Typeorvalue = Union[Type, ResultVariable]
 
 
 class Resolver(object):
-
     __slots__ = ("namespace", "dataflow_graph")
 
     def __init__(self, namespace: Namespace, enable_dataflow_graph: bool = False) -> None:
         self.namespace = namespace
         self.dataflow_graph: Optional[DataflowGraph] = DataflowGraph(self) if enable_dataflow_graph else None
 
     def lookup(self, name: str, root: Optional[Namespace] = None) -> Typeorvalue:
@@ -1076,15 +1124,14 @@
         return self.parent.lookup(name, root)
 
     def get_root_resolver(self) -> "Resolver":
         return self.parent.get_root_resolver()
 
 
 class NamespaceResolver(Resolver):
-
     __slots__ = ("parent", "root")
 
     def __init__(self, parent: Resolver, lecial_root: Namespace) -> None:
         self.parent = parent
         self.root = lecial_root
         self.dataflow_graph: Optional[DataflowGraph] = None
         if parent.dataflow_graph is not None:
@@ -1099,15 +1146,14 @@
         return NamespaceResolver(self, namespace)
 
     def get_root_resolver(self) -> "Resolver":
         return self.parent.get_root_resolver()
 
 
 class ExecutionContext(Resolver):
-
     __slots__ = ("block", "slots", "resolver")
 
     def __init__(self, block: "BasicBlock", resolver: Resolver):
         self.block = block
         self.slots: Dict[str, ResultVariable] = {n: ResultVariable() for n in block.get_variables()}
         self.resolver = resolver
         self.dataflow_graph: Optional[DataflowGraph] = None
@@ -1142,15 +1188,15 @@
 
 # also extends locatable
 class Instance(ExecutionContext):
     def set_location(self, location: Location) -> None:
         Locatable.set_location(self, location)
         self.locations.append(location)
 
-    def get_location(self) -> Location:
+    def get_location(self) -> Optional[Location]:
         return Locatable.get_location(self)
 
     location = property(get_location, set_location)
 
     __slots__ = (
         "_location",
         "resolver",
@@ -1271,17 +1317,16 @@
                             )
                         )
 
     def dump(self) -> None:
         print("------------ ")
         print(str(self))
         print("------------ ")
-        for (n, v) in self.slots.items():
+        for n, v in self.slots.items():
             if v.can_get():
-
                 value = v.value
                 print("%s\t\t%s" % (n, value))
             else:
                 print("BAD: %s\t\t%s" % (n, ", ".join(repr(prom) for prom in v.promises)))
 
     def verify_done(self) -> bool:
         for v in self.slots.values():
```

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/scheduler.py` & `inmanta-core-8.3.0/src/inmanta/execute/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 import os
 import time
 from collections import deque
 from typing import TYPE_CHECKING, Any, Deque, Dict, Iterable, Iterator, List, Optional, Sequence, Set, Tuple
 
 from inmanta import plugins
-from inmanta.ast import Anchor, CompilerException, CycleException, Location, MultiException, RuntimeException
+from inmanta.ast import Anchor, AnchorTarget, CompilerException, CycleException, Location, MultiException, RuntimeException
 from inmanta.ast.attribute import RelationAttribute
 from inmanta.ast.entity import Entity, Implementation
 from inmanta.ast.statements import DefinitionStatement, TypeDefinitionStatement
 from inmanta.ast.statements.define import DefineEntity, DefineImplement, DefineIndex, DefineRelation, DefineTypeConstraint
 from inmanta.ast.type import TYPES, Type
 from inmanta.const import LOG_LEVEL_TRACE
 from inmanta.execute.proxy import UnsetException
@@ -208,15 +208,15 @@
         compiler.get_ns().set_primitives(TYPES)
 
         # all stmts contributing types and impls
         newtypes: List[Tuple[str, NamedType]] = [
             k for k in [t.register_types() for t in definitions if isinstance(t, TypeDefinitionStatement)] if k is not None
         ]
 
-        for (name, type_symbol) in newtypes:
+        for name, type_symbol in newtypes:
             types_and_impl[name] = type_symbol
 
         # now that we have objects for all types, populate them
         implements = [t for t in definitions if isinstance(t, DefineImplement)]
         other_definitions = [t for t in definitions if not isinstance(t, DefineImplement)]
         entities: Dict[str, DefineEntity] = {t.fullName: t for t in other_definitions if isinstance(t, DefineEntity)}
         type_constraints = [t for t in other_definitions if isinstance(t, DefineTypeConstraint)]
@@ -258,17 +258,17 @@
 
         # normalize root blocks
         for block in blocks:
             block.normalize()
 
         self.types = {k: v for k, v in types_and_impl.items() if isinstance(v, Type)}
 
-    def anchormap(
+    def get_anchormap(
         self, compiler: "Compiler", statements: Sequence["Statement"], blocks: Sequence["BasicBlock"]
-    ) -> Sequence[Tuple[Location, Location]]:
+    ) -> Sequence[Tuple[Location, AnchorTarget]]:
         prev = time.time()
 
         # first evaluate all definitions, this should be done in one iteration
         self.define_types(compiler, statements, blocks)
 
         # relations are also in blocks
         not_relation_statements: Iterator[Statement] = (s for s in statements if not isinstance(s, DefineRelation))
@@ -276,21 +276,32 @@
         anchors: Iterator[Anchor] = (
             anchor
             for container in itertools.chain(not_relation_statements, blocks)  # container: Union[Statement, BasicBlock]
             for anchor in container.get_anchors()
             if anchor is not None
         )
 
-        rangetorange = [(anchor.get_location(), anchor.resolve()) for anchor in anchors]
-        rangetorange = [(f, t) for f, t in rangetorange if t is not None]
+        range_to_anchor_target = [(anchor.get_location(), anchor.resolve()) for anchor in anchors]
+        range_to_anchor_target = [(f, t) for f, t in range_to_anchor_target if t is not None]
 
         now = time.time()
         LOGGER.debug("Anchormap took %f seconds", now - prev)
 
-        return rangetorange
+        return range_to_anchor_target
+
+    def anchormap(
+        self, compiler: "Compiler", statements: Sequence["Statement"], blocks: Sequence["BasicBlock"]
+    ) -> Sequence[Tuple[Location, Location]]:
+        """
+        This methode exists for backward compatibility with inmantals
+        """
+        range_to_anchor_target = self.get_anchormap(compiler, statements, blocks)
+        range_to_range = [(f, t.location) for f, t in range_to_anchor_target]
+
+        return range_to_range
 
     def find_wait_cycle(self, attributes_with_precedence_rule: List[RelationAttribute], allwaiters: Set[Waiter]) -> bool:
         """
         Preconditions: no progress is made anymore
 
         This means that all DelayedResultVariable that have not been frozen either have
         no progress potential or have outstanding promises.
```

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/tracking.py` & `inmanta-core-8.3.0/src/inmanta/execute/tracking.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/execute/util.py` & `inmanta-core-8.3.0/src/inmanta/execute/util.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/export.py` & `inmanta-core-8.3.0/src/inmanta/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         self.types = types
         self.scopes = scopes
 
         self._version = self.get_version(no_commit, partial_compile)
 
         if types is not None:
             # then process the configuration model to submit it to the mgmt server
-            # This is the actuel export : convert entities to resources.
+            # This is the actual export : convert entities to resources.
             self._load_resources(types)
             resource_sets_to_remove_all += self._empty_resource_sets
             # call dependency managers
             self._call_dep_manager(types)
             metadata[const.META_DATA_COMPILE_STATE] = const.Compilestate.success
             self.failed = False
         else:
@@ -526,16 +526,18 @@
                 LOGGER.debug("Uploaded file with hash %s" % hash_id)
 
         # Collecting version information
         version_info = {const.EXPORT_META_DATA: metadata}
 
         # TODO: start transaction
         LOGGER.info("Sending resource updates to server")
-        for res in resources:
-            LOGGER.debug("  %s", res["id"])
+        if LOGGER.isEnabledFor(logging.DEBUG):
+            for res in resources:
+                rid = res["id"]
+                LOGGER.debug("  %s in resource set %s", rid, self._resource_sets.get(Id.parse_id(rid).resource_str(), ""))
 
         if partial_compile:
             result = conn.put_partial(
                 tid=tid,
                 resources=resources,
                 resource_sets=self._resource_sets,
                 unknowns=unknown_parameters,
```

### Comparing `inmanta-core-8.2.0/src/inmanta/file_parser.py` & `inmanta-core-8.3.0/src/inmanta/file_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/loader.py` & `inmanta-core-8.3.0/src/inmanta/loader.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/main.py` & `inmanta-core-8.3.0/src/inmanta/main.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/model.py` & `inmanta-core-8.3.0/src/inmanta/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
             "nullable": self.nullable,
             "comment": self.comment,
             "location": self.location.to_dict(),
         }
 
     @staticmethod
     def from_dict(ctx: JsonType) -> None:
-
         return Attribute(
             mytype=ctx["type"],
             nullable=ctx["nullable"],
             multi=ctx["multi"],
             comment=ctx["comment"],
             location=Location.from_dict(ctx["location"]),
         )
@@ -159,15 +158,14 @@
     """
     A reference to an instance of an entity.
 
     :param str reference: the handle for the entity this value refers to
     """
 
     def __init__(self, reference):
-
         self.reference = reference
 
     def to_dict(self) -> JsonType:
         """
         Convert to serialized form:
 
         .. code-block:: python
```

### Comparing `inmanta-core-8.2.0/src/inmanta/module.py` & `inmanta-core-8.3.0/src/inmanta/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 """
 
 import configparser
 import enum
 import glob
 import importlib
 import logging
+import operator
 import os
 import re
 import subprocess
 import sys
 import tempfile
 import textwrap
 import traceback
 import types
 import warnings
 from abc import ABC, abstractmethod
 from collections import abc, defaultdict
 from configparser import ConfigParser
 from dataclasses import dataclass
+from functools import reduce
 from importlib.abc import Loader
 from io import BytesIO, TextIOBase
 from itertools import chain
 from subprocess import CalledProcessError
 from tarfile import TarFile
 from time import time
 from typing import (
@@ -952,14 +954,22 @@
     def clone(self, name: str, dest: str) -> bool:
         raise NotImplementedError("Abstract method")
 
     def path_for(self, name: str) -> Optional[str]:
         # same class is used for search path and remote repos, perhaps not optimal
         raise NotImplementedError("Abstract method")
 
+    def is_empty(self) -> bool:
+        """
+        Return true if this repo will never produce any repo.
+
+        Used to distinguish an empty compose repo from a non-empty one
+        """
+        return False
+
 
 class CompositeModuleRepo(ModuleRepo):
     def __init__(self, children: List[ModuleRepo]) -> None:
         self.children = children
 
     def clone(self, name: str, dest: str) -> bool:
         for child in self.children:
@@ -970,14 +980,17 @@
     def path_for(self, name: str) -> Optional[str]:
         for child in self.children:
             result = child.path_for(name)
             if result is not None:
                 return result
         return None
 
+    def is_empty(self) -> bool:
+        return reduce(operator.and_, (child.is_empty() for child in self.children), True)
+
 
 class LocalFileRepo(ModuleRepo):
     def __init__(self, root: str, parent_root: Optional[str] = None) -> None:
         if parent_root is None:
             self.root = os.path.abspath(root)
         else:
             self.root = os.path.join(parent_root, root)
@@ -992,14 +1005,18 @@
 
     def path_for(self, name: str) -> Optional[str]:
         path = os.path.join(self.root, name)
         if os.path.exists(path):
             return path
         return None
 
+    def is_empty(self) -> bool:
+        # May have or receive items
+        return False
+
 
 class RemoteRepo(ModuleRepo):
     def __init__(self, baseurl: str) -> None:
         self.baseurl = baseurl
 
     def clone(self, name: str, dest: str) -> bool:
         url, nbr_substitutions = re.subn(r"{}", name, self.baseurl)
@@ -1013,14 +1030,18 @@
         except Exception:
             LOGGER.debug("could not clone repo", exc_info=True)
             return False
 
     def path_for(self, name: str) -> Optional[str]:
         raise NotImplementedError("Should only be called on local repos")
 
+    def is_empty(self) -> bool:
+        # May have or receive items
+        return False
+
 
 def make_repo(path: str, root: Optional[str] = None) -> Union[LocalFileRepo, RemoteRepo]:
     """
     Returns the appropriate `ModuleRepo` instance (v1) for the given path.
     """
     # check that the second char is not a colon (windows)
     if ":" in path and path[1] != ":":
@@ -1526,15 +1547,18 @@
         can have the following values:
 
         * git: When the type is set to git, the url field should contain a template of the Git repo URL. Inmanta creates the
           git repo url by formatting {} or {0} with the name of the module. If no formatter is present it appends the name
           of the module to the URL.
         * package: When the type is set to package, the URL field should contain the URL of the Python package repository.
           The repository should be `PEP 503 <https://www.python.org/dev/peps/pep-0503/>`_ (the simple repository API)
-          compliant.
+          compliant. If more than one package url is configured, they will all be passed to pip. This is generally only
+          recommended if all configured indexes are under full control of the end user to protect against dependency
+          confusion attacks. See the `pip install documentation <https://pip.pypa.io/en/stable/cli/pip_install/>`_ and
+          `PEP 708 (draft) <https://peps.python.org/pep-0708/>`_ for more information.
 
         The old syntax, which only defines a Git URL per list entry is maintained for backward compatibility.
     :param requires: (Optional) This key can contain a list (a yaml list) of version constraints for modules used in this
         project. Similar to the module, version constraints are defined using
         `PEP440 syntax <https://www.python.org/dev/peps/pep-0440/#version-specifiers>`_.
     :param freeze_recursive: (Optional) This key determined if the freeze command will behave recursively or not. If
         freeze_recursive is set to false or not set, the current version of all modules imported directly in the main.cf file
@@ -1548,15 +1572,15 @@
         place, the compiler will first freeze `first-type.relation-name` and only then `then-type.relation-name`.
     :param strict_deps_check: Determines whether the compiler or inmanta tools that install/update module dependencies,
         should check the virtual environment for version conflicts in a strict way or not.
         A strict check means that all transitive dependencies will be checked for version conflicts and that any violation will
         result in an error.
         When a non-strict check is done, only version conflicts in a direct dependency will result in an error.
         All other violations will only result in a warning message.
-    :param agent_install_dependency_modules: [EXPERIMENTAL FEATURE] If true, when a module declares Python dependencies on
+    :param agent_install_dependency_modules: [EXPERT FEATURE] If true, when a module declares Python dependencies on
         other (v2) modules, the agent will install these dependency modules with pip. This option should only be enabled
         if the agent is configured with the appropriate pip related environment variables. The option allows to an extent
         for inter-module dependencies within handler code, even if the dependency module doesn't have any handlers that
         would otherwise be considered relevant for this agent.
 
         Care should still be taken when you use inter-module imports. The current code loading mechanism does not explicitly
         order reloads. A general guideline is to use qualified imports where you can (import the module rather than objects
@@ -1893,21 +1917,23 @@
         self.module_source_v1: ModuleV1Source = ModuleV1Source(
             local_repo=CompositeModuleRepo([make_repo(x) for x in self.modulepath]),
             remote_repo=CompositeModuleRepo(
                 [make_repo(repo.url, root=path) for repo in self._metadata.repo if repo.type == ModuleRepoType.git]
             ),
         )
 
-        if self._metadata.downloadpath is not None:
-            self._metadata.downloadpath = os.path.abspath(os.path.join(path, self._metadata.downloadpath))
-            if self._metadata.downloadpath not in self._metadata.modulepath:
-                LOGGER.warning("Downloadpath is not in module path! Module install will not work as expected")
+        if not self.module_source_v1.remote_repo.is_empty():
+            # This is only relevant if we have a V1 module source
+            if self._metadata.downloadpath is not None:
+                self._metadata.downloadpath = os.path.abspath(os.path.join(path, self._metadata.downloadpath))
+                if self._metadata.downloadpath not in self._metadata.modulepath:
+                    LOGGER.warning("Downloadpath is not in module path! Module install will not work as expected")
 
-            if not os.path.exists(self._metadata.downloadpath):
-                os.mkdir(self._metadata.downloadpath)
+                if not os.path.exists(self._metadata.downloadpath):
+                    os.mkdir(self._metadata.downloadpath)
 
         self.virtualenv: env.ActiveEnv
         if venv_path is None:
             self.virtualenv = env.process_env
         else:
             if isinstance(venv_path, env.VirtualEnv):
                 self.virtualenv = venv_path
```

### Comparing `inmanta-core-8.2.0/src/inmanta/moduletool.py` & `inmanta-core-8.3.0/src/inmanta/moduletool.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Contact: code@inmanta.com
 """
 import argparse
 import configparser
 import datetime
 import enum
 import inspect
+import itertools
 import logging
 import os
 import py_compile
 import re
 import shutil
 import subprocess
 import sys
@@ -34,14 +35,15 @@
 from collections import abc
 from configparser import ConfigParser
 from functools import total_ordering
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Pattern, Sequence, Set, Type
 
 import click
+import more_itertools
 import texttable
 import yaml
 from cookiecutter.main import cookiecutter
 from pkg_resources import parse_version
 
 import build
 import build.env
@@ -78,15 +80,14 @@
 if TYPE_CHECKING:
     from pkg_resources import Requirement  # noqa: F401
 
     from packaging.requirements import InvalidRequirement
 else:
     from pkg_resources.extern.packaging.requirements import InvalidRequirement
 
-
 LOGGER = logging.getLogger(__name__)
 
 
 class ModuleVersionException(CLIException):
     def __init__(self, msg: str) -> None:
         super().__init__(msg, exitcode=5)
 
@@ -100,25 +101,29 @@
     Add the --no-strict-deps-check and --strict-deps-check options to the given parser.
     """
     parser.add_argument(
         "--no-strict-deps-check",
         dest="no_strict_deps_check",
         action="store_true",
         default=False,
-        help="When this option is enabled, only version conflicts in the direct dependencies will result in an error. "
-        "All other version conflicts will result in a warning. This option is mutually exclusive with the "
-        "--strict-deps-check option.",
+        help=(
+            "When this option is enabled, only version conflicts in the direct dependencies will result in an error. "
+            "All other version conflicts will result in a warning. This option is mutually exclusive with the "
+            "--strict-deps-check option."
+        ),
     )
     parser.add_argument(
         "--strict-deps-check",
         dest="strict_deps_check",
         action="store_true",
         default=False,
-        help="When this option is enabled, a version conflict in any (transitive) dependency will results in an error. "
-        "This option is mutually exclusive with the --no-strict-deps-check option.",
+        help=(
+            "When this option is enabled, a version conflict in any (transitive) dependency will results in an error. "
+            "This option is mutually exclusive with the --no-strict-deps-check option."
+        ),
     )
 
 
 def get_strict_deps_check(no_strict_deps_check: bool, strict_deps_check: bool) -> Optional[bool]:
     """
     Perform input validation on the --no-strict-deps-check and --strict-deps-check options and
     return True iff strict dependency checking should be used.
@@ -189,15 +194,17 @@
                 if len(opts) == 0:
                     LOGGER.error("One of the following options is required: --major, --minor or --patch")
                     return None
                 elif len(opts) > 1:
                     LOGGER.error("You can use only one of the following options: --major, --minor or --patch")
                     return None
 
-                change_type: Optional[ChangeType] = ChangeType.parse_from_bools(patch, minor, major)
+                # We do not support revision for deprecated methods
+                revision = False
+                change_type: Optional[ChangeType] = ChangeType.parse_from_bools(revision, patch, minor, major)
                 if change_type:
                     outversion = str(VersionOperation.bump_version(change_type, old_version, version_tag=""))
                 else:
                     outversion = str(VersionOperation.set_version_tag(old_version, version_tag=""))
 
             if dev:
                 outversion = "%s.dev%d" % (outversion, time.time())
@@ -212,60 +219,58 @@
 
 @total_ordering
 @enum.unique
 class ChangeType(enum.Enum):
     MAJOR: str = "major"
     MINOR: str = "minor"
     PATCH: str = "patch"
-
-    def less(self) -> Optional["ChangeType"]:
-        """
-        Returns the change type that is one less than this one.
-        """
-        if self == ChangeType.MAJOR:
-            return ChangeType.MINOR
-        if self == ChangeType.MINOR:
-            return ChangeType.PATCH
-        return None
+    REVISION: str = "revision"
 
     def __lt__(self, other: "ChangeType") -> bool:
-        order: List[ChangeType] = [ChangeType.PATCH, ChangeType.MINOR, ChangeType.MAJOR]
+        order: List[ChangeType] = [ChangeType.REVISION, ChangeType.PATCH, ChangeType.MINOR, ChangeType.MAJOR]
         if other not in order:
             return NotImplemented
         return order.index(self) < order.index(other)
 
     @classmethod
     def diff(cls, *, low: Version, high: Version) -> Optional["ChangeType"]:
         """
         Returns the order of magnitude of the change type diff between two versions.
-        Return None if the versions are less than a patch separated from each other.
+        Return None if the versions are less than a patch / a revision (if 4 digit version number) separated from each other.
         For example, a dev release and a post release for the same version number are less
         than a patch separated from each other.
         """
         if low > high:
             raise ValueError(f"Expected low <= high, got {low} > {high}")
         if Version(low.base_version) == Version(high.base_version):
             return None
         if high.major > low.major:
             return cls.MAJOR
         if high.minor > low.minor:
             return cls.MINOR
         if high.micro > low.micro:
             return cls.PATCH
+        if len(high.base_version.split(".")) >= 4:
+            high_revision = int(high.base_version.split(".")[3])
+            # We are switching from 3 digits to 4
+            if len(low.base_version.split(".")) < 4 or high_revision > int(low.base_version.split(".")[3]):
+                return cls.REVISION
         raise Exception("Couldn't determine version change type diff: this state should be unreachable")
 
     @classmethod
-    def parse_from_bools(cls, patch: bool, minor: bool, major: bool) -> Optional["ChangeType"]:
+    def parse_from_bools(cls, revision: bool, patch: bool, minor: bool, major: bool) -> Optional["ChangeType"]:
         """
         Create a ChangeType for the type of which the boolean is set to True. If none
         of the boolean arguments is set to True, None is returned. If more
         than one boolean argument is set to True, a ValueError is raised.
         """
-        if sum([patch, minor, major]) > 1:
-            raise ValueError("Only one argument of patch, minor or major can be set to True at the same time.")
+        if sum([revision, patch, minor, major]) > 1:
+            raise ValueError("Only one argument of revision, patch, minor or major can be set to True at the same time.")
+        if revision:
+            return ChangeType.REVISION
         if patch:
             return ChangeType.PATCH
         if minor:
             return ChangeType.MINOR
         if major:
             return ChangeType.MAJOR
         return None
@@ -274,29 +279,42 @@
 class VersionOperation:
     @classmethod
     def bump_version(cls, change_type: ChangeType, version: Version, version_tag: str) -> Version:
         """
         Bump the release part of the given version with this ChangeType and apply the given version_tag to it.
         If the given version has a different version tag set, it will be ignored.
         """
-        parts = [int(x) for x in version.base_version.split(".")]
-        while len(parts) < 3:
-            parts.append(0)
-        if change_type is ChangeType.PATCH:
-            parts[2] += 1
-        if change_type is ChangeType.MINOR:
-            parts[1] += 1
-            parts[2] = 0
-        if change_type is ChangeType.MAJOR:
-            parts[0] += 1
-            parts[1] = 0
-            parts[2] = 0
-        # Reset remaining digits to zero
-        if len(parts) > 3:
-            parts[3:] = [0 for _ in range(len(parts) - 3)]
+        bump_index: int
+        if change_type is ChangeType.REVISION:
+            bump_index = 3
+        elif change_type is ChangeType.PATCH:
+            bump_index = 2
+        elif change_type is ChangeType.MINOR:
+            bump_index = 1
+        elif change_type is ChangeType.MAJOR:
+            bump_index = 0
+        else:
+            raise RuntimeError(f"Unsupported change type: {change_type}!")
+
+        base_parts = [int(x) for x in version.base_version.split(".")]
+        # use 4th digit only if it already existed or if it is being bumped
+        nb_digits: int = max(bump_index + 1, 3, len(base_parts))
+        parts = list(
+            more_itertools.take(
+                nb_digits,
+                itertools.chain(
+                    base_parts[: bump_index + 1],
+                    itertools.repeat(0),
+                ),
+            )
+        )
+        parts[bump_index] += 1
+
+        while len(parts) > 3 and parts[-1] == 0:
+            parts.pop()
 
         return cls._to_version(parts, version_tag)
 
     @classmethod
     def set_version_tag(cls, version: Version, version_tag: str) -> Version:
         """
         Return a new version that is a copy of the given version where the version_tag
@@ -679,18 +697,18 @@
 When a stable release is done, this command:
 * Does a commit that changes the current version to a stable version.
 * Adds Git release tag.
 * Does a commit that changes the current version to a development version that is one patch increment ahead of the released
   version.
 When a development release is done using the --dev option, this command:
 * Does a commit that updates the current version of the module to a development version that is a patch, minor or major version
-  ahead of the previous stable release. The size of the increment is determined by the --patch, --minor or --major argument
-  (--patch is the default). When a CHANGELOG.md file is present in the root of the module directory then the version number in
-  the changelog is also updated accordingly. The changelog file is always populated with the associated stable version and
-  not a development version.
+  ahead of the previous stable release. The size of the increment is determined by the --revision, --patch, --minor or
+  --major argument (--patch is the default). When a CHANGELOG.md file is present in the root of the module
+  directory then the version number in the changelog is also updated accordingly. The changelog file is always populated with
+  the associated stable version and not a development version.
             """.strip(),
             formatter_class=RawTextHelpFormatter,
         )
         release.add_argument(
             "--dev",
             dest="dev",
             help="Create a development version. The new version number will have the .dev0 build tag.",
@@ -711,21 +729,28 @@
         )
         release.add_argument(
             "--patch",
             dest="patch",
             help="Do a patch version bump compared to the previous stable release.",
             action="store_true",
         )
+        release.add_argument(
+            "--revision",
+            dest="revision",
+            help="Do a revision version bump compared to the previous stable release (only with 4 digits version).",
+            action="store_true",
+        )
         release.add_argument("-m", "--message", help="Commit message")
         release.add_argument(
             "-c",
             "--changelog-message",
             help="This changelog message will be written to the changelog file. If the -m option is not provided, "
             "this message will also be used as the commit message.",
         )
+        release.add_argument("-a", "--all", dest="commit_all", help="Use commit -a", action="store_true")
 
     def add(self, module_req: str, v1: bool = False, v2: bool = False, override: bool = False) -> None:
         """
         Add a module dependency to an Inmanta module or project.
 
         :param module_req: The module to add, optionally with a version constraint.
         :param v1: Whether the given module should be added as a V1 module or not.
@@ -908,15 +933,14 @@
 
         project = Project.get()
         project.get_complete_ast()
 
         names: Sequence[str] = sorted(project.modules.keys())
         specs: Dict[str, List[InmantaModuleRequirement]] = project.collect_imported_requirements()
         for name in names:
-
             mod: Module = Project.get().modules[name]
             version = str(mod.version)
             if name not in specs:
                 specs[name] = []
 
             generation: str = str(mod.GENERATION.name).lower()
 
@@ -1171,27 +1195,29 @@
 
         return new_version
 
     def release(
         self,
         dev: bool,
         message: Optional[str] = None,
+        revision: bool = False,
         patch: bool = False,
         minor: bool = False,
         major: bool = False,
+        commit_all: bool = False,
         changelog_message: Optional[str] = None,
     ) -> None:
         """
         Execute the release command.
         """
 
         # Validate patch, minor, major
-        nb_version_bump_arguments_set = sum([patch, minor, major])
+        nb_version_bump_arguments_set = sum([revision, patch, minor, major])
         if nb_version_bump_arguments_set > 1:
-            raise click.UsageError("Only one of --patch, --minor and --major can be set at the same time.")
+            raise click.UsageError("Only one of --revision, --patch, --minor and --major can be set at the same time.")
 
         # Make module
         module_dir = os.path.abspath(os.getcwd())
         module: Module[ModuleMetadata] = self.construct_module(project=DummyProject(), path=module_dir)
         if not gitprovider.is_git_repository(repo=module_dir):
             raise click.ClickException(f"Directory {module_dir} is not a git repository.")
 
@@ -1205,15 +1231,15 @@
         stable_releases: list[Version] = gitprovider.get_version_tags(module_dir, only_return_stable_versions=True)
 
         path_changelog_file = os.path.join(module_dir, const.MODULE_CHANGELOG_FILE)
         changelog: Optional[ModuleChangelog] = (
             ModuleChangelog(path_changelog_file) if os.path.exists(path_changelog_file) else None
         )
 
-        requested_version_bump: Optional[ChangeType] = ChangeType.parse_from_bools(patch, minor, major)
+        requested_version_bump: Optional[ChangeType] = ChangeType.parse_from_bools(revision, patch, minor, major)
         if not requested_version_bump and dev:
             # Dev always bumps
             requested_version_bump = ChangeType.PATCH
 
         if requested_version_bump:
             new_version: Version = self._get_dev_version_with_minimal_distance_to_previous_stable_release(
                 current_version, stable_releases, requested_version_bump
@@ -1238,30 +1264,30 @@
             assert new_version.dev is not None and new_version.dev == 0
             new_base_version_str, version_tag = str(new_version).rsplit(".", maxsplit=1)
             module.rewrite_version(new_version=new_base_version_str, version_tag=version_tag)
             # If no changes, commit will not happen
             gitprovider.commit(
                 repo=module_dir,
                 message=changelog_message if changelog_message else message if message else f"Bump version to {new_version}",
-                commit_all=True,
-                add=[module.get_metadata_file_path()] + [changelog.get_path()] if changelog else [],
+                commit_all=commit_all,
+                add=[module.get_metadata_file_path()] + ([changelog.get_path()] if changelog else []),
                 raise_exc_when_nothing_to_commit=False,
             )
         else:
             release_tag: Version = VersionOperation.set_version_tag(new_version, version_tag="")
             if release_tag in stable_releases:
                 raise click.ClickException(f"A Git version tag already exists for version {release_tag}")
             module.rewrite_version(new_version=str(release_tag), version_tag="")
             if changelog:
                 changelog.set_release_date_for_version(release_tag)
             gitprovider.commit(
                 repo=module_dir,
                 message=message if message else f"Release version {module.metadata.get_full_version()}",
-                commit_all=True,
-                add=[module.get_metadata_file_path()] + [changelog.get_path()] if changelog else [],
+                commit_all=commit_all,
+                add=[module.get_metadata_file_path()] + ([changelog.get_path()] if changelog else []),
                 raise_exc_when_nothing_to_commit=False,
             )
             gitprovider.tag(repo=module_dir, tag=str(release_tag))
             # bump to the next dev version
             self.release(dev=True, message="Bump version to next development version", patch=True)
 
 
@@ -1519,15 +1545,14 @@
         """
         if self._isolated_env:
             super(IsolatedEnvBuilderCached, self).__exit__(None, None, None)
             self._isolated_env = None
 
 
 class V2ModuleBuilder:
-
     DISABLE_ISOLATED_ENV_BUILDER_CACHE: bool = False
 
     def __init__(self, module_path: str) -> None:
         """
         :raises InvalidModuleException: The given module_path doesn't reference a valid module.
         :raises ModuleBuildFailedError: Module build was unsuccessful.
         """
@@ -1664,15 +1689,15 @@
 
         def should_ignore(name: str) -> bool:
             return ignore is not None and ignore.fullmatch(name) is not None
 
         if not os.path.isdir(directory):
             raise Exception(f"{directory} is not a directory")
         result: Set[str] = set()
-        for (dirpath, dirnames, filenames) in os.walk(directory):
+        for dirpath, dirnames, filenames in os.walk(directory):
             if should_ignore(os.path.basename(dirpath)):
                 # ignore whole subdirectory
                 continue
             relative_paths_to_filenames = set(
                 os.path.relpath(os.path.join(dirpath, f), directory) for f in filenames if not should_ignore(f)
             )
             result = result | relative_paths_to_filenames
```

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/__init__.py` & `inmanta-core-8.3.0/src/inmanta/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/cache.py` & `inmanta-core-8.3.0/src/inmanta/parser/cache.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/parser.out` & `inmanta-core-8.3.0/src/inmanta/parser/parser.out`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/parsetab.py` & `inmanta-core-8.3.0/src/inmanta/parser/parsetab.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/pickle.py` & `inmanta-core-8.3.0/src/inmanta/parser/pickle.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/plyInmantaLex.py` & `inmanta-core-8.3.0/src/inmanta/parser/plyInmantaLex.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/parser/plyInmantaParser.py` & `inmanta-core-8.3.0/src/inmanta/parser/plyInmantaParser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/plugins.py` & `inmanta-core-8.3.0/src/inmanta/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,24 @@
 import warnings
 from collections import abc
 from functools import reduce
 from typing import TYPE_CHECKING, Any, Callable, Dict, FrozenSet, List, Optional, Tuple, Type, TypeVar
 
 import inmanta.ast.type as inmanta_type
 from inmanta import const, protocol
-from inmanta.ast import CompilerException, LocatableString, Location, Namespace, Range, RuntimeException, TypeNotFoundException
+from inmanta.ast import (
+    CompilerException,
+    LocatableString,
+    Location,
+    Namespace,
+    Range,
+    RuntimeException,
+    TypeNotFoundException,
+    WithComment,
+)
 from inmanta.ast.type import NamedType
 from inmanta.config import Config
 from inmanta.execute.proxy import DynamicProxy
 from inmanta.execute.runtime import QueueScheduler, Resolver, ResultVariable
 from inmanta.execute.util import Unknown
 from inmanta.stable_api import stable_api
 from inmanta.warnings import InmantaWarning
@@ -177,15 +186,15 @@
                 for fq_name, plugin_class in cls.__functions.items()
                 if plugin_class.__module__ != top_level and not plugin_class.__module__.startswith(f"{top_level}.")
             }
         else:
             cls.__functions = {}
 
 
-class Plugin(NamedType, metaclass=PluginMeta):
+class Plugin(NamedType, WithComment, metaclass=PluginMeta):
     """
     This class models a plugin that can be called from the language.
     """
 
     deprecated: bool = False
     replaced_by: Optional[str] = None
 
@@ -208,14 +217,17 @@
         assert filename is not None
         try:
             line: int = inspect.getsourcelines(self.__class__.__function__)[1] + 1
         except OSError:
             # In case of bytecompiled code there is no source line
             line = 1
 
+        if self.__class__.__function__.__doc__:
+            self.comment = self.__class__.__function__.__doc__
+
         self.location = Location(filename, line)
 
     def normalize(self) -> None:
         self.resolver = self.namespace
         self.argtypes = [self.to_type(x[1], self.namespace) for x in self.arguments]
         self.returntype = self.to_type(self._return, self.namespace)
```

### Comparing `inmanta-core-8.2.0/src/inmanta/postgresproc.py` & `inmanta-core-8.3.0/src/inmanta/postgresproc.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/profile_mem.py` & `inmanta-core-8.3.0/src/inmanta/profile_mem.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/__init__.py` & `inmanta-core-8.3.0/src/inmanta/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/common.py` & `inmanta-core-8.3.0/src/inmanta/protocol/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 from pydantic.main import create_model
 from tornado import web
 
 from inmanta import config as inmanta_config
 from inmanta import const, execute, types, util
 from inmanta.data.model import BaseModel, validator_timezone_aware_timestamps
 from inmanta.protocol.exceptions import BadRequest, BaseHttpException
+from inmanta.protocol.openapi import model as openapi_model
 from inmanta.stable_api import stable_api
 from inmanta.types import ArgumentTypes, HandlerType, JsonType, MethodType, ReturnTypes, StrictNonIntBool
 
 from . import exceptions
 
 if TYPE_CHECKING:
     from .endpoints import CallTarget
@@ -243,15 +244,15 @@
     def __repr__(self) -> str:
         return f"ReturnValue<code={self.status_code} headers=<{self.headers}> response=<{self._response}>>"
 
     def __str__(self) -> str:
         return repr(self)
 
 
-class Response(object):
+class Response:
     """
     A response object of a call
     """
 
     @classmethod
     def create(
         cls,
@@ -323,25 +324,30 @@
         """Generate a path that uses regex named groups for tornado"""
         path = self._path
         for var in self._vars:
             path = path.replace(f"<{var}>", f"(?P<{var}>[^/]+)")
 
         return path
 
+    def has_path_variable(self, var_name: str) -> bool:
+        """
+        Return True iff the given var_name is a path parameter of this UrlPath.
+        """
+        return var_name in self._vars
+
 
 class InvalidMethodDefinition(Exception):
     """This exception is raised when the definition of a method is invalid."""
 
 
 VALID_URL_ARG_TYPES = (Enum, uuid.UUID, str, float, int, bool, datetime)
 VALID_SIMPLE_ARG_TYPES = (BaseModel, Enum, uuid.UUID, str, float, int, StrictNonIntBool, datetime, bytes)
 
 
 class MethodArgumentsBaseModel(pydantic.BaseModel):
-
     _normalize_timestamps: ClassVar[classmethod] = pydantic.validator("*", allow_reuse=True)(
         validator_timezone_aware_timestamps
     )
 
 
 class MethodProperties(object):
     """
@@ -377,14 +383,15 @@
         client_types: List[const.ClientType],
         api_version: int,
         api_prefix: str,
         envelope: bool,
         typed: bool = False,
         envelope_key: str = const.ENVELOPE_KEY,
         strict_typing: bool = True,
+        enforce_auth: bool = True,
         varkw: bool = False,
     ) -> None:
         """
         Decorator to identify a method as a RPC call. The arguments of the decorator are used by each transport to build
         and model the protocol.
 
         :param path: The path in the url
@@ -399,14 +406,16 @@
                             to which the options apply.
         :param api_version: The version of the api this method belongs to
         :param api_prefix: The prefix of the method: /<prefix>/v<version>/<method_name>
         :param envelope: Put the response of the call under an envelope key.
         :param typed: Is the method definition typed or not
         :param envelope_key: The envelope key to use
         :param strict_typing: If true, does not allow `Any` when validating argument types
+        :param enforce_auth: When set to true authentication is enforced on this endpoint. When set to false, authentication is
+                             not enforced, even if auth is enabled.
         :param varkw: If true, additional arguments are allowed and will be dispatched to the handler. The handler is
                       responsible for the validation.
         """
         if api is None:
             api = not server_agent and not agent_server
 
         if validate_sid is None:
@@ -423,14 +432,15 @@
         self._validate_sid: bool = validate_sid
         self._client_types = client_types
         self._api_version = api_version
         self._api_prefix = api_prefix
         self._envelope = envelope
         self._envelope_key = envelope_key
         self._strict_typing = strict_typing
+        self._enforce_auth = enforce_auth
         self.function = function
         self._varkw: bool = varkw
         self._varkw_name: Optional[str] = None
 
         self._parsed_docstring = docstring_parser.parse(text=function.__doc__, style=docstring_parser.DocstringStyle.REST)
         self._docstring_parameter_map = {p.arg_name: p.description for p in self._parsed_docstring.params}
 
@@ -443,14 +453,18 @@
         self.argument_validator = self.arguments_to_pydantic()
 
     @property
     def varkw(self) -> bool:
         """Does the method allow for a variable number of key/value arguments."""
         return self._varkw
 
+    @property
+    def enforce_auth(self) -> bool:
+        return self._enforce_auth
+
     def validate_arguments(self, values: Dict[str, Any]) -> Dict[str, Any]:
         """
         Validate methods arguments. Values is a dict with key/value pairs for the arguments (similar to kwargs). This method
         validates and converts types if required (e.g. str to int). The returns value has the correct typing to dispatch
         to method handlers.
         """
         try:
@@ -671,20 +685,20 @@
             )
 
     @property
     def operation(self) -> str:
         return self._operation
 
     @property
+    @stable_api
     def arg_options(self) -> Dict[str, ArgOption]:
         return self._arg_options
 
     @property
     def timeout(self) -> Optional[int]:
-
         return self._timeout
 
     @property
     def validate_sid(self) -> bool:
         return self._validate_sid
 
     @property
@@ -711,20 +725,22 @@
     def strict_typing(self) -> bool:
         return self._strict_typing
 
     @property
     def api_version(self) -> int:
         return self._api_version
 
+    @stable_api
     def get_long_method_description(self) -> Optional[str]:
         """
         Return the full description present in the docstring of the method, excluding the first paragraph.
         """
         return self._parsed_docstring.long_description
 
+    @stable_api
     def get_short_method_description(self) -> Optional[str]:
         """
         Return the first paragraph of the description present in the docstring of the method.
         """
         return self._parsed_docstring.short_description
 
     def get_description_for_param(self, param_name: str) -> Optional[str]:
@@ -778,15 +794,15 @@
         else:
             result[200] = ""
 
         # Get descriptions for raises statements
         for raise_statement in self._parsed_docstring.raises:
             exception_name = raise_statement.type_name
             status_code = self._get_http_status_code_for_exception(exception_name)
-            result[status_code] = raise_statement.description
+            result[status_code] = raise_statement.description if raise_statement.description is not None else ""
 
         return result
 
     def get_call_headers(self) -> Set[str]:
         """
         Returns the set of headers required to create call
         """
@@ -868,14 +884,29 @@
     def _encode_dict_for_get(
         self, query_param_name: str, query_param_value: Dict[str, Union[Any, List[Any]]]
     ) -> Dict[str, str]:
         """Dicts are encoded in the following manner: param = {'ab': 1, 'cd': 2} to param.abc=1&param.cd=2"""
         sub_dict = {f"{query_param_name}.{key}": value for key, value in query_param_value.items()}
         return sub_dict
 
+    @stable_api
+    def get_openapi_parameter_type_for(self, param_name: str) -> Optional[openapi_model.ParameterType]:
+        """
+        Return the openapi ParameterType for the parameter with the given param_name or None when the parameter
+        with the given name is not an OpenAPI parameter (but a RequestBodyParameter for example).
+        """
+        if param_name in self.arg_options and self.arg_options[param_name].header:
+            return openapi_model.ParameterType.header
+        elif self._path.has_path_variable(param_name):
+            return openapi_model.ParameterType.path
+        elif self.arguments_in_url():
+            return openapi_model.ParameterType.query
+        else:
+            return None
+
 
 class UrlMethod(object):
     """
     This class holds the method definition together with the API (url, method) information
 
     :param properties: The properties of this method
     :param endpoint: The object on which this method is defined
@@ -974,14 +1005,20 @@
 def encode_token(
     client_types: List[str], environment: Optional[str] = None, idempotent: bool = False, expire: Optional[float] = None
 ) -> str:
     cfg = inmanta_config.AuthJWTConfig.get_sign_config()
     if cfg is None:
         raise Exception("No JWT signing configuration available.")
 
+    for ct in client_types:
+        if ct not in cfg.client_types:
+            raise Exception(
+                f"The signing config does not support the requested client type {ct}. Only {cfg.client_types} are allowed."
+            )
+
     payload: Dict[str, Any] = {"iss": cfg.issuer, "aud": [cfg.audience], const.INMANTA_URN + "ct": ",".join(client_types)}
 
     if not idempotent:
         payload["iat"] = int(time.time())
 
         if cfg.expire > 0:
             payload["exp"] = int(time.time() + cfg.expire)
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/decorators.py` & `inmanta-core-8.3.0/src/inmanta/protocol/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
     agent_server: bool = False,
     validate_sid: Optional[bool] = None,
     client_types: List[const.ClientType] = [const.ClientType.api],
     api_version: int = 1,
     api_prefix: str = "api",
     envelope_key: str = const.ENVELOPE_KEY,
     strict_typing: bool = True,
+    enforce_auth: bool = True,
     varkw: bool = False,
 ) -> Callable[..., Callable]:
     """
     Decorator to identify a method as a RPC call. The arguments of the decorator are used by each transport to build
     and model the protocol.
 
     :param path: The url path to use for this call. This path can contain parameter names of the function. These names
@@ -166,14 +167,16 @@
                     type of the argument. This method can raise an HTTPException to return a 404 for example.
     :param api_version: The version of the api this method belongs to
     :param api_prefix: The prefix of the method: /<prefix>/v<version>/<method_name>
     :param envelope_key: The envelope key to use.
     :param strict_typing: If true, does not allow `Any`. Setting this option to False is heavily discouraged except for some
         few very specific cases where the type system does not allow the strict type to be specified, for example in case of
         infinite recursion.
+    :param enforce_auth: When set to true authentication is enforced on this endpoint. When set to false, authentication is not
+                         enforced, even if auth is enabled.
     :param varkw: If true, additional arguments are allowed and will be dispatched to the handler. The handler is
                   responsible for the validation.
     """
 
     def wrapper(func: MethodT) -> MethodT:
         properties = common.MethodProperties(
             func,
@@ -189,13 +192,14 @@
             client_types,
             api_version,
             api_prefix,
             True,
             True,
             envelope_key,
             strict_typing=strict_typing,
+            enforce_auth=enforce_auth,
             varkw=varkw,
         )
         common.MethodProperties.register_method(properties)
         return func
 
     return wrapper
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/endpoints.py` & `inmanta-core-8.3.0/src/inmanta/protocol/endpoints.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/exceptions.py` & `inmanta-core-8.3.0/src/inmanta/protocol/exceptions.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/methods.py` & `inmanta-core-8.3.0/src/inmanta/protocol/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     Delete the given project and all related data
     """
 
 
 @method(path="/project", operation="GET", client_types=[const.ClientType.api])
 def list_projects():
     """
-    Create a list of projects
+    Returns a list of projects ordered alphabetically by name. The environments within each project are also sorted by name.
     """
 
 
 @method(path="/project/<id>", operation="GET", client_types=[const.ClientType.api])
 def get_project(id: uuid.UUID):
     """
     Get a project and a list of the ids of all environments
@@ -144,15 +144,15 @@
     :raises Forbidden: The given environment is protected.
     """
 
 
 @method(path="/environment", operation="GET", client_types=[const.ClientType.api])
 def list_environments():
     """
-    Create a list of environments
+    Returns a list of environments. The results are sorted by (project id, environment name, environment id).
     """
 
 
 @method(
     path="/environment/<id>",
     operation="GET",
     client_types=[const.ClientType.api],
@@ -178,15 +178,15 @@
     arg_options=ENV_OPTS,
     api=True,
     agent_server=True,
     client_types=[const.ClientType.api, const.ClientType.agent, const.ClientType.compiler],
 )
 def list_settings(tid: uuid.UUID):
     """
-    List the settings in the current environment
+    List the settings in the current environment ordered by name alphabetically.
     """
 
 
 @method(
     path="/environment_settings/<id>",
     operation="POST",
     arg_options=ENV_OPTS,
@@ -588,15 +588,15 @@
     :param id: The version of the CM to deploy
     """
 
 
 @method(path="/dryrun", operation="GET", arg_options=ENV_OPTS, client_types=[const.ClientType.api])
 def dryrun_list(tid: uuid.UUID, version: int = None):
     """
-    Create a list of dry runs
+    Get the list of dry runs for an environment. The results are sorted by dry run id.
 
     :param tid: The id of the environment
     :param version: Only for this version
     """
 
 
 @method(path="/dryrun/<id>", operation="GET", arg_options=ENV_OPTS, client_types=[const.ClientType.api])
@@ -747,15 +747,15 @@
 
 
 @method(
     path="/parameter", operation="POST", arg_options=ENV_OPTS, client_types=[const.ClientType.api, const.ClientType.compiler]
 )
 def list_params(tid: uuid.UUID, query: dict = {}):
     """
-    List/query parameters in this environment
+    List/query parameters in this environment. The results are ordered alphabetically by parameter name.
 
     :param tid: The id of the environment
     :param query: A query to match against metadata
     """
 
 
 #  Get and set parameters on the server
@@ -989,9 +989,9 @@
     arg_options=ENV_OPTS,
     client_types=[const.ClientType.api],
     api_version=1,
     envelope_key="queue",
 )
 def get_compile_queue(tid: uuid.UUID) -> List[model.CompileRun]:
     """
-    Get the current compiler queue on the server
+    Get the current compiler queue on the server, ordered by increasing `requested` timestamp.
     """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/methods_v2.py` & `inmanta-core-8.3.0/src/inmanta/protocol/methods_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     Delete the given project and all related data
     """
 
 
 @typedmethod(path="/project", operation="GET", client_types=[ClientType.api], api_version=2)
 def project_list(environment_details: bool = False) -> List[model.Project]:
     """
-    Returns a list of projects
+    Returns a list of projects ordered alphabetically by name. The environments within each project are also sorted by name.
     :param environment_details: Whether to include the icon and description of the environments in the results
     """
 
 
 @typedmethod(path="/project/<id>", operation="GET", client_types=[ClientType.api], api_version=2)
 def project_get(id: uuid.UUID, environment_details: bool = False) -> model.Project:
     """
@@ -314,15 +314,15 @@
     api=True,
     agent_server=True,
     client_types=[ClientType.api, ClientType.agent, ClientType.compiler],
     api_version=2,
 )
 def environment_settings_list(tid: uuid.UUID) -> model.EnvironmentSettingsReponse:
     """
-    List the settings in the current environment
+    List the settings in the current environment ordered by name alphabetically.
     """
 
 
 @typedmethod(
     path="/environment_settings/<id>",
     operation="POST",
     arg_options=methods.ENV_OPTS,
@@ -814,15 +814,15 @@
 
 
 @typedmethod(
     path="/resource/<rid>/facts", operation="GET", arg_options=methods.ENV_OPTS, client_types=[ClientType.api], api_version=2
 )
 def get_facts(tid: uuid.UUID, rid: model.ResourceIdStr) -> List[model.Fact]:
     """
-    Get the facts related to a specific resource
+    Get the facts related to a specific resource. The results are sorted alphabetically by name.
     :param tid: The id of the environment
     :param rid: Id of the resource
     :return: The facts related to this resource
     :raise NotFound: This status code is returned when the referenced environment is not found
     """
 
 
@@ -1324,7 +1324,56 @@
 
     :param tid: The id of the environment for which the metrics have to be collected.
     :param metrics: List of names of metrics that have to be returned.
     :param start_interval: The start of the time window for which the metrics should be returned.
     :param end_interval: The end of the time window for which the metrics should be returned.
     :param nb_datapoints: The amount of datapoint that will be returned within the given time interval for each metric.
     """
+
+
+@typedmethod(path="/login", operation="POST", client_types=[ClientType.api], enforce_auth=False, api_version=2)
+def login(username: str, password: str) -> ReturnValue[model.LoginReturn]:
+    """Login a user. When the login succeeds an authentication header is returned with the Bearer token set.
+
+    :param username: The user to login
+    :param password: The password of this user
+    :raises UnauthorizedException: Raised when the login failed or if server authentication is not enabled
+    """
+
+
+@typedmethod(path="/user", operation="GET", client_types=[ClientType.api], api_version=2)
+def list_users() -> List[model.User]:
+    """List all users
+
+    :return: A list of all users"""
+
+
+@typedmethod(path="/user/<username>", operation="DELETE", client_types=[ClientType.api], api_version=2)
+def delete_user(username: str) -> None:
+    """Delete a user from the system with given username.
+
+    :param username: The username to delete
+    :raises NotFound: Raised when the user does not exist
+    :raises BadRequest: Raised when server authentication is not enabled
+    """
+
+
+@typedmethod(path="/user", operation="POST", client_types=[ClientType.api], api_version=2)
+def add_user(username: str, password: str) -> model.User:
+    """Add a new user to the system
+
+    :param username: The username of the new user. The username cannot be an empty string.
+    :param password: The password of this new user. The password should be at least 8 characters long.
+    :raises Conflict: Raised when there is already a user with this user_name
+    :raises BadRequest: Raised when server authentication is not enabled
+    """
+
+
+@typedmethod(path="/user/<username>/password", operation="PATCH", client_types=[ClientType.api], api_version=2)
+def set_password(username: str, password: str) -> None:
+    """Change the password of a user
+
+    :param username: The username of the user
+    :param password: The password of this new user. The password should be at least 8 characters long.
+    :raises NotFound: Raised when the user does not exist
+    :raises BadRequest: Raised when server authentication is not enabled
+    """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/openapi/__init__.py` & `inmanta-core-8.3.0/src/inmanta/protocol/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/openapi/converter.py` & `inmanta-core-8.3.0/src/inmanta/protocol/openapi/converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from inmanta.protocol.common import ArgOption, MethodProperties, ReturnValue, UrlMethod
 from inmanta.protocol.openapi.model import (
     Components,
     Header,
     Info,
     MediaType,
     OpenAPI,
+    OpenApiDataTypes,
     Operation,
     Parameter,
     ParameterType,
     PathItem,
     Reference,
     RequestBody,
     Response,
@@ -157,29 +158,50 @@
         self.ref_prefix = "#/components/schemas/"
         self.ref_regex = re.compile(self.ref_prefix + r"(.*)")
 
         # Applying some monkey patching to pydantic
         patch_pydantic_field_type_schema()
 
     def get_openapi_type_of_parameter(self, parameter_type: inspect.Parameter) -> Schema:
-        type_annotation = parameter_type.annotation
-        return self.get_openapi_type(type_annotation)
+        schema = self.get_openapi_type(parameter_type.annotation)
+        if parameter_type.default is not inspect.Parameter.empty:
+            schema.default = parameter_type.default
+        return schema
 
     def _handle_pydantic_model(self, type_annotation: Type, by_alias: bool = True) -> Schema:
         # JsonSchema stores the model (and sub-model) definitions at #/definitions,
         # but OpenAPI requires them to be placed at "#/components/schemas/"
         # The ref_prefix changes the references, but the actual schemas are still at #/definitions
         schema = model_schema(type_annotation, by_alias=by_alias, ref_prefix=self.ref_prefix)
         if "definitions" in schema.keys():
             definitions: Dict[str, Dict[str, object]] = schema.pop("definitions")
             if self.components.schemas is not None:
                 for key, definition in definitions.items():
+                    definition = self._add_type_field_to_enum_value(definition)
                     self.components.schemas[key] = Schema(**definition)
         return Schema(**schema)
 
+    def _add_type_field_to_enum_value(self, definition: Dict[str, object]) -> Dict[str, object]:
+        """
+        When pydantic converts a Python Enum type to its corresponding json schema, it doesn't
+        populate the type field. This way the rendered API documentation doesn't include all possible
+        enum values. This method makes sure that the type attribute of an enum is always populated.
+        """
+        if definition.get("enum") is not None and not definition.get("type"):
+            # Convert Python type to a type known by OpenAPI
+            if all(isinstance(e, bool) for e in definition["enum"]):
+                definition["type"] = OpenApiDataTypes.BOOLEAN.value
+            elif all(isinstance(e, int) for e in definition["enum"]):
+                definition["type"] = OpenApiDataTypes.INTEGER.value
+            elif all(isinstance(e, float) or isinstance(e, int) for e in definition["enum"]):
+                definition["type"] = OpenApiDataTypes.NUMBER.value
+            else:
+                definition["type"] = OpenApiDataTypes.STRING.value
+        return definition
+
     def get_openapi_type(self, type_annotation: Type) -> Schema:
         class Sub(BaseModel):
             the_field: type_annotation
 
             class Config:
                 arbitrary_types_allowed = True
 
@@ -226,15 +248,17 @@
 
     def extract_response_headers_from_arg_options(
         self, arg_options: Dict[str, ArgOption]
     ) -> Optional[Dict[str, Union[Header, Reference]]]:
         headers: Dict[str, Union[Header, Reference]] = {}
         for option_name, option in arg_options.items():
             if option.header and option.reply_header:
-                headers[option.header] = Header(description=option.header, schema=Schema(type="string"))
+                headers[option.header] = Header(
+                    description=f"The value of the request header {option.header}", schema=Schema(type="string")
+                )
         return headers if headers else None
 
 
 class FunctionParameterHandler:
     """
     Creates OpenAPI Parameters and RequestBody items based on the handler function parameters
     """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/openapi/model.py` & `inmanta-core-8.3.0/src/inmanta/protocol/openapi/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     format: Optional[str] = None
     default: Optional[Any] = None
     nullable: Optional[bool] = None
     readOnly: Optional[bool] = None
     example: Optional[Any] = None
     deprecated: Optional[bool] = None
     anyOf: Optional[Sequence["Schema"]] = None
+    allOf: Optional[Sequence["Schema"]] = None
+    oneOf: Optional[Sequence["Schema"]] = None
     enum: Optional[List[str]] = None
 
     def resolve(self, ref_prefix: str, known_schemas: Dict[str, "Schema"]) -> "Schema":
         """
         Returns this object or the one this object is refering to.
 
         :param ref_prefix: The prefix this object ref should have if it is only a reference
@@ -108,18 +110,26 @@
 
         # We only do a deepcopy if the parameter says so AND this object has not been newly built
         deep = deep and schema is not self
 
         # Duplicate the schema, and update some of its values
         duplicate = schema.copy(update=update, deep=deep)
 
-        # We copy and resolve the list of schema
+        # We copy and resolve the anyOf if we have any
         if duplicate.anyOf is not None:
             duplicate.anyOf = [s.recursive_resolve(ref_prefix, known_schemas, update, deep=False) for s in duplicate.anyOf]
 
+        # We copy and resolve the allOf if we have any
+        if duplicate.allOf is not None:
+            duplicate.allOf = [s.recursive_resolve(ref_prefix, known_schemas, update, deep=False) for s in duplicate.allOf]
+
+        # We copy and resolve the oneOf if we have any
+        if duplicate.oneOf is not None:
+            duplicate.oneOf = [s.recursive_resolve(ref_prefix, known_schemas, update, deep=False) for s in duplicate.oneOf]
+
         # We copy and resolve the items if we have any
         if duplicate.items is not None:
             duplicate.items = duplicate.items.recursive_resolve(ref_prefix, known_schemas, update, deep=False)
 
         # We copy and resolve the properties if we have any
         if duplicate.properties is not None:
             duplicate.properties = {
@@ -237,7 +247,16 @@
 
 class OpenAPI(BaseModel):
     openapi: str
     info: Info
     servers: Optional[List[Server]] = None
     paths: Dict[str, PathItem]
     components: Optional[Components] = None
+
+
+class OpenApiDataTypes(Enum):
+    STRING = "string"
+    NUMBER = "number"
+    INTEGER = "integer"
+    BOOLEAN = "boolean"
+    ARRAY = "array"
+    OBJECT = "object"
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/rest/__init__.py` & `inmanta-core-8.3.0/src/inmanta/protocol/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/rest/client.py` & `inmanta-core-8.3.0/src/inmanta/protocol/rest/client.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/rest/server.py` & `inmanta-core-8.3.0/src/inmanta/protocol/rest/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         """
         Get the auth token provided by the caller. The token is provided as a bearer token.
         """
         if "Authorization" not in headers:
             return None
 
         parts = headers["Authorization"].split(" ")
-        if len(parts) == 0 or parts[0].lower() != "bearer" or len(parts) > 2 or len(parts) == 1:
+        if len(parts) != 2 or parts[0].lower() != "bearer":
             LOGGER.warning(
                 "Invalid authentication header, Inmanta expects a bearer token. (%s was provided)", headers["Authorization"]
             )
             return None
 
         return common.decode_token(parts[1])
 
@@ -136,21 +136,21 @@
                     else:
                         message[key] = [v.decode("latin-1") for v in value]
 
                 request_headers = self.request.headers
                 auth_token = self.get_auth_token(request_headers)
 
                 auth_enabled = server_enable_auth.get()
-                if not auth_enabled or auth_token is not None:
+                if not auth_enabled or auth_token is not None or not call_config.properties.enforce_auth:
                     result = await self._transport._execute_call(
                         kwargs, http_method, call_config, message, request_headers, auth_token
                     )
                     self.respond(result.body, result.headers, result.status_code)
                 else:
-                    raise exceptions.UnauthorizedException("Access to this resource is unauthorized.")
+                    raise exceptions.UnauthorizedException()
 
             except JSONDecodeError as e:
                 error_message = f"The request body couldn't be decoded as a JSON: {e}"
                 LOGGER.info(error_message, exc_info=True)
                 self.respond({"message": error_message}, {}, 400)
 
             except ValueError:
```

### Comparing `inmanta-core-8.2.0/src/inmanta/protocol/return_value_meta.py` & `inmanta-core-8.3.0/src/inmanta/protocol/return_value_meta.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/reporter.py` & `inmanta-core-8.3.0/src/inmanta/reporter.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/resources.py` & `inmanta-core-8.3.0/src/inmanta/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -595,29 +595,32 @@
     def parse_resource_version_id(cls, resource_id: ResourceVersionIdStr) -> "Id":
         id: Id = Id.parse_id(resource_id)
         if id.version == 0:
             raise ValueError(f"Version is missing from resource id: {resource_id}")
         return id
 
     @classmethod
-    def parse_id(cls, resource_id: Union[ResourceVersionIdStr, ResourceIdStr]) -> "Id":
+    def parse_id(cls, resource_id: Union[ResourceVersionIdStr, ResourceIdStr], version: Optional[int] = None) -> "Id":
         """
         Parse the resource id and return the type, the hostname and the
         resource identifier.
+
+        :param version: If provided, the version field of the returned Id will be set to this version.
         """
         result = PARSE_ID_REGEX.search(resource_id)
 
         if result is None:
             raise ValueError("Invalid id for resource %s" % resource_id)
 
-        version_match: str = result.group("version")
+        if version is None:
+            version_match: str = result.group("version")
 
-        version = 0
-        if version_match is not None:
-            version = int(version_match)
+            version = 0
+            if version_match is not None:
+                version = int(version_match)
 
         id_obj = Id(result.group("type"), result.group("hostname"), result.group("attr"), result.group("value"), version)
         return id_obj
 
     @classmethod
     def is_resource_version_id(cls, value: str) -> bool:
         """
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/__init__.py` & `inmanta-core-8.3.0/src/inmanta/server/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,7 +33,8 @@
 SLICE_METRICS = "core.metrics"
 SLICE_PARAM = "core.parameters"
 SLICE_RESOURCE = "core.resource"
 SLICE_ORCHESTRATION = "core.orchestration"
 SLICE_DRYRUN = "core.dryrun"
 SLICE_NOTIFICATION = "core.notification"
 SLICE_ENVIRONMENT_METRICS = "core.environment-metrics"
+SLICE_USER = "core.user"
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/agentmanager.py` & `inmanta-core-8.3.0/src/inmanta/server/agentmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
                 return await self._create_default_agent(env, nodename, connection=connection)
 
     async def _create_default_agent(
         self, env: data.Environment, nodename: str, *, connection: Optional[asyncpg.connection.Connection] = None
     ) -> data.Agent:
         """
         This method creates a new agent (agent in the model) in the database.
-        If an active agent instance exists for the given agent, it is marked as a the
+        If an active agent instance exists for the given agent, it is marked as the
         primary instance for that agent in the database.
 
         Note: This method must be called under session lock
         """
         saved = data.Agent(environment=env.id, name=nodename, paused=False)
         await saved.insert(connection=connection)
 
@@ -837,15 +837,14 @@
 
             # only request facts of a resource every _fact_resource_block time
             now = time.time()
             if (
                 resource_id not in self._fact_resource_block_set
                 or (self._fact_resource_block_set[resource_id] + self._fact_resource_block) < now
             ):
-
                 agents = await data.ConfigurationModel.get_agents(env.id, version)
                 await self._autostarted_agent_manager._ensure_agents(env, agents)
 
                 client = self.get_agent_client(env_id, res.agent)
                 if client is not None:
                     self.add_background_task(client.get_parameter(str(env_id), res.agent, res.to_dict()))
 
@@ -1010,25 +1009,18 @@
         :param env: The environment to start the agents for
         :param agents: A list of agent names that possibly should be started in this environment.
         :param restart: Restart all agents even if the list of agents is up to date.
         """
         if self._stopping:
             raise ShutdownInProgress()
 
-        agent_map: Dict[str, str]
-        agent_map = cast(
+        agent_map: Dict[str, str] = cast(
             Dict[str, str], await env.get(data.AUTOSTART_AGENT_MAP, connection=connection)
         )  # we know the type of this map
 
-        # The internal agent should always be present in the autostart_agent_map. If it's not, this autostart_agent_map was
-        # set in a previous version of the orchestrator which didn't have this constraint. This code fixes the inconsistency.
-        if "internal" not in agent_map:
-            agent_map["internal"] = "local:"
-            await env.set(data.AUTOSTART_AGENT_MAP, dict(agent_map), connection=connection)
-
         agents = [agent for agent in agents if agent in agent_map]
         needsstart = restart
         if len(agents) == 0:
             return False
 
         async def is_start_agent_required() -> bool:
             if needsstart:
@@ -1076,15 +1068,16 @@
 
         agent_log = os.path.join(self._server_storage["logs"], "agent-%s.log" % env.id)
 
         proc: Optional[subprocess.Process] = None
         try:
             proc = await self._fork_inmanta(
                 [
-                    "-vvvv",
+                    "--log-file-level",
+                    "DEBUG",
                     "--timed-logs",
                     "--config",
                     config_path,
                     "--config-dir",
                     Config._config_dir if Config._config_dir is not None else "",
                     "--log-file",
                     agent_log,
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/bootloader.py` & `inmanta-core-8.3.0/src/inmanta/server/bootloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     # returned name an absolute name instead of a relative one. This allows
     # import_module to work without having to do additional modification to
     # the name.
     return pkgutil.iter_modules(ns_pkg.__path__, ns_pkg.__name__ + ".")
 
 
 class PluginLoadFailed(Exception):
-
     pass
 
 
 class ConstrainedApplicationContext(ApplicationContext):
     def __init__(self, parent: ApplicationContext, namespace: str) -> None:
         super().__init__()
         self.parent = parent
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/compilerservice.py` & `inmanta-core-8.3.0/src/inmanta/server/compilerservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/config.py` & `inmanta-core-8.3.0/src/inmanta/server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,24 +116,25 @@
             "The server_rest_transport.port config option is deprecated in favour of the server.bind-port option.",
             category=DeprecationWarning,
         )
         return Config.get("server_rest_transport", "port", 8888)
 
 
 server_enable_auth = Option("server", "auth", False, "Enable authentication on the server API", is_bool)
+server_auth_method = Option("server", "auth_method", None, "The authentication method to use: oidc or database", is_str_opt)
 
 server_ssl_key = Option(
     "server", "ssl_key_file", None, "Server private key to use for this server Leave blank to disable SSL", is_str_opt
 )
 
 server_ssl_cert = Option(
     "server", "ssl_cert_file", None, "SSL certificate file for the server key. Leave blank to disable SSL", is_str_opt
 )
 
-server_ssl_ca_cert: Option[str] = Option(
+server_ssl_ca_cert = Option(
     "server",
     "ssl_ca_cert_file",
     None,
     "The CA cert file required to validate the server ssl cert. This setting is used by the server"
     "to correctly configure the compiler and agents that the server starts itself. If not set and "
     "SSL is enabled, the server cert should be verifiable with the CAs installed in the OS.",
     is_str_opt,
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/diff.py` & `inmanta-core-8.3.0/src/inmanta/server/diff.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/extensions.py` & `inmanta-core-8.3.0/src/inmanta/server/extensions.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/protocol.py` & `inmanta-core-8.3.0/src/inmanta/server/protocol.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/server.py` & `inmanta-core-8.3.0/src/inmanta/server/server.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/__init__.py` & `inmanta-core-8.3.0/src/inmanta/server/services/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/codeservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/codeservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/compilerservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/compilerservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,15 +866,14 @@
         first_id: Optional[uuid.UUID] = None,
         last_id: Optional[uuid.UUID] = None,
         start: Optional[datetime.datetime] = None,
         end: Optional[datetime.datetime] = None,
         filter: Optional[Dict[str, List[str]]] = None,
         sort: str = "requested.desc",
     ) -> ReturnValue[Sequence[model.CompileReport]]:
-
         try:
             handler = CompileReportView(env, limit, filter, sort, first_id, last_id, start, end)
             return await handler.execute()
         except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
             raise BadRequest(e.message) from e
 
     @protocol.handle(methods_v2.compile_details, env="tid")
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/databaseservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/databaseservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/dryrunservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/dryrunservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             model = await data.ConfigurationModel.get_version(environment=env.id, version=version)
             if model is None:
                 raise NotFound("The request version does not exist.")
 
             query_args["model"] = version
 
         dryruns = await data.DryRun.get_list(
-            order_by_column=None, order=None, limit=None, offset=None, no_obj=None, lock=None, connection=None, **query_args
+            order_by_column="id", order=None, limit=None, offset=None, no_obj=None, lock=None, connection=None, **query_args
         )
 
         return (
             200,
             {"dryruns": [{"id": x.id, "version": x.model, "date": x.date, "total": x.total, "todo": x.todo} for x in dryruns]},
         )
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/environment_metrics_service.py` & `inmanta-core-8.3.0/src/inmanta/server/services/environment_metrics_service.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/environmentservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/environmentservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,16 +302,16 @@
         """
         Create a new auth token for this environment
         """
         return 200, {"token": await self.environment_create_token(env, client_types, idempotent)}
 
     @handle(methods.list_settings, env="tid")
     async def list_settings(self, env: data.Environment) -> Apireturn:
-        settings = {k: env.settings[k] for k in env.settings.keys() if k in data.Environment._settings.keys()}
-        return 200, {"settings": settings, "metadata": data.Environment._settings}
+        settings = {k: env.settings[k] for k in sorted(env.settings.keys()) if k in data.Environment._settings.keys()}
+        return 200, {"settings": settings, "metadata": dict(sorted(data.Environment._settings.items()))}
 
     @handle(methods.set_setting, env="tid", key="id")
     async def set_setting(self, env: data.Environment, key: str, value: model.EnvSettingType) -> Apireturn:
         try:
             original_env = env.to_dto()
             await env.set(key, value)
             warnings = await self._setting_change(env, key)
@@ -528,15 +528,16 @@
         if not config.Config.getboolean("server", "auth", False):
             raise BadRequest("Authentication is disabled, generating a token is not allowed")
         return encode_token(client_types, str(env.id), idempotent)
 
     @handle(methods_v2.environment_settings_list, env="tid")
     async def environment_settings_list(self, env: data.Environment) -> model.EnvironmentSettingsReponse:
         return model.EnvironmentSettingsReponse(
-            settings=env.settings, definition={k: v.to_dto() for k, v in data.Environment._settings.items()}
+            settings=dict(sorted(env.settings.items())),
+            definition={k: v.to_dto() for k, v in sorted(data.Environment._settings.items())},
         )
 
     @handle(methods_v2.environment_settings_set, env="tid", key="id")
     async def environment_settings_set(self, env: data.Environment, key: str, value: model.EnvSettingType) -> ReturnValue[None]:
         try:
             original_env = env.to_dto()
             await env.set(key, value)
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/fileservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/fileservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,21 +127,24 @@
         """
         return 200, {"files": self.stat_file_internal(files)}
 
     def stat_file_internal(self, files: Iterable[str]) -> List[str]:
         """
         Return which files in the list don't exist on the server
         """
-        response: List[str] = []
+        # A dict is used here instead of a set to have efficient set-like behaviour while preserving insertion order. Only its
+        # keys are relevant.
+        response: dict[str, object] = {}
+
         for f in files:
             f_path = os.path.join(self.server_slice._server_storage["files"], f)
             if not os.path.exists(f_path):
-                response.append(f)
+                response[f] = None
 
-        return response
+        return list(response.keys())
 
     @handle(methods.diff)
     async def file_diff(self, a: str, b: str) -> Apireturn:
         """
         Diff the two files identified with the two hashes
         """
         if a == "" or a == "0":
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/metricservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/metricservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/notificationservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/notificationservice.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/orchestrationservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/resourceservice.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,1081 +11,1030 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
-import dataclasses
+import asyncio
 import datetime
 import logging
+import os
 import uuid
 from collections import abc, defaultdict
-from typing import Dict, List, Literal, Mapping, Optional, Sequence, Set, cast
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union, cast
 
-import asyncpg
-import asyncpg.connection
-import pydantic
-
-from inmanta import const, data
-from inmanta.const import ResourceState
-from inmanta.data import APILIMIT, AVAILABLE_VERSIONS_TO_KEEP, ENVIRONMENT_AGENT_TRIGGER_METHOD, PURGE_ON_DELETE, InvalidSort
-from inmanta.data.dataview import DesiredStateVersionView
+from asyncpg.connection import Connection
+from asyncpg.exceptions import UniqueViolationError
+from tornado.httputil import url_concat
+
+from inmanta import const, data, util
+from inmanta.const import STATE_UPDATE, TERMINAL_STATES, TRANSIENT_STATES, VALID_STATES_ON_STATE_UPDATE, Change, ResourceState
+from inmanta.data import APILIMIT, InvalidSort
+from inmanta.data.dataview import ResourceHistoryView, ResourceLogsView, ResourcesInVersionView, ResourceView
 from inmanta.data.model import (
-    DesiredStateVersion,
-    PromoteTriggerMethod,
-    ResourceDiff,
+    AttributeStateChange,
+    LatestReleasedResource,
+    LogLine,
+    ReleasedResourceDetails,
+    Resource,
+    ResourceAction,
+    ResourceHistory,
     ResourceIdStr,
-    ResourceMinimal,
+    ResourceLog,
+    ResourceType,
     ResourceVersionIdStr,
+    VersionedResource,
+    VersionedResourceDetails,
 )
 from inmanta.protocol import handle, methods, methods_v2
-from inmanta.protocol.common import ReturnValue, attach_warnings
-from inmanta.protocol.exceptions import BadRequest, BaseHttpException, NotFound, ServerError
+from inmanta.protocol.common import ReturnValue
+from inmanta.protocol.exceptions import BadRequest, Conflict, NotFound
+from inmanta.protocol.return_value_meta import ReturnValueWithMeta
 from inmanta.resources import Id
-from inmanta.server import (
-    SLICE_AGENT_MANAGER,
-    SLICE_AUTOSTARTED_AGENT_MANAGER,
-    SLICE_DATABASE,
-    SLICE_ORCHESTRATION,
-    SLICE_RESOURCE,
-    SLICE_TRANSPORT,
-)
+from inmanta.server import SLICE_AGENT_MANAGER, SLICE_DATABASE, SLICE_RESOURCE, SLICE_TRANSPORT
 from inmanta.server import config as opt
-from inmanta.server import diff, protocol
-from inmanta.server.agentmanager import AgentManager, AutostartedAgentManager
-from inmanta.server.services.resourceservice import ResourceService
+from inmanta.server import protocol
+from inmanta.server.agentmanager import AgentManager
 from inmanta.server.validate_filter import InvalidFilter
-from inmanta.types import Apireturn, JsonType, PrimitiveTypes
+from inmanta.types import Apireturn, PrimitiveTypes
 
 LOGGER = logging.getLogger(__name__)
 
-PERFORM_CLEANUP: bool = True
-# Kill switch for cleanup, for use when working with historical data
-
-
-class ResourceWithResourceSet:
-    def __init__(
-        self,
-        resource: ResourceMinimal,
-        resource_set: Optional[str],
-        resource_state: const.ResourceState,
-    ) -> None:
-        self.resource = resource
-        self.resource_set = resource_set
-        self.resource_state = resource_state
-
-    def get_resource_id_str(self) -> ResourceIdStr:
-        return self.resource.get_resource_id_str()
-
-    def get_resource_state_for_new_resource(self) -> Literal[ResourceState.undefined, ResourceState.available]:
-        """
-        Return the resource state as expected by the `resource_state` argument of the `OrchestrationService._put_version()`
-        method. This method should set the resource state of a resource to undefined when it directly depends on an unknown or
-        available when it doesn't.
-        """
-        if self.resource_state is ResourceState.undefined:
-            return ResourceState.undefined
-        else:
-            return ResourceState.available
 
-    def is_shared_resource(self) -> bool:
-        return self.resource_set is None
-
-    def is_update(self, other: "ResourceWithResourceSet") -> bool:
-        """
-        return true if the ResourceWithResourceSet is an update of other: other exists but is different from self
-        """
-        if other is None:
-            return False
-        new_resource_dict = self.resource.dict()
-        old_resource_dict = other.resource.dict()
-        attr_names_new_resource = set(new_resource_dict.keys()).difference("id")
-        attr_names_old_resource = set(old_resource_dict.keys()).difference("id")
-        return attr_names_new_resource != attr_names_old_resource or any(
-            new_resource_dict[k] != old_resource_dict[k] for k in attr_names_new_resource
-        )
-
-
-class PairedResource:
+def error_and_log(message: str, **context: Any) -> None:
     """
-    Pairs an old and a new ResourceWithResourceSet for the same id. Offers methods to inspect the difference.
+    :param message: message to return both to logger and to remote caller
+    :param context: additional context to attach to log
     """
-
-    def __init__(
-        self,
-        new_resource: ResourceWithResourceSet,
-        old_resource: Optional[ResourceWithResourceSet],
-    ) -> None:
-        self.new_resource = new_resource
-        self.old_resource = old_resource
-
-    def is_update(self) -> bool:
-        """
-        return true if new_resource is an update of old_resource: old_resource exists but is different form new_resource.
-        """
-        return self.new_resource.is_update(self.old_resource)
-
-    def is_new_resource(self) -> bool:
-        """
-        return true if old_resource doesn't exist
-        """
-        return self.old_resource is None
-
-    def resource_changed_resource_set(self) -> bool:
-        """
-        return true if the resource_set in new_resource and old_resource are not the same
-        """
-        assert self.old_resource is not None
-        return self.new_resource.resource_set != self.old_resource.resource_set
-
-
-@dataclasses.dataclass(frozen=True)
-class MergedModel:
-    """
-    A class containing the result of merging an old version of a configuration model with a partial model.
-    """
-
-    resources: list[dict[str, object]]
-    resource_states: dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]]
-    resource_sets: dict[ResourceIdStr, Optional[str]]
-    unknowns: List[data.UnknownParameter]
-
-
-class PartialUpdateMerger:
-    """
-    This class is used to merge the result of a partial compile with previous resources and resource_sets. Takes a partial spec
-    that should be applied on a given base version to form the given new version.
-
-    Any resource version ids this class works with (e.g. within resource objects) already represent the new version. It is the
-    caller's responsibility to ensure this invariant is met for any resource version ids in input objects.
-    """
-
-    def __init__(
-        self,
-        env: data.Environment,
-        base_version: int,
-        new_version: int,
-        partial_updates: Sequence[ResourceMinimal],
-        resource_states: Mapping[ResourceIdStr, ResourceState],
-        resource_sets: Mapping[ResourceIdStr, Optional[str]],
-        removed_resource_sets: Sequence[str],
-        unknowns: Sequence[data.UnknownParameter],
-    ) -> None:
-        """
-        :param env: The environment in which the partial compile happens.
-        :param base_version: The version number of the old configuration model from which the resources are merged
-                             together with the resources from the partial compile.
-        :param new_version: The version number of the newly generated configuration model.
-        :param partial_updates: The resources part of the partial compile
-        :param resource_states: The resource states of the resources in the partial compile.
-        :param resource_sets: The resource sets of the resources in the partial compile.
-        :param removed_resource_sets: The resources in these resource sets should be present in the new configuration model.
-        :param unknowns: The unknowns that belong to the partial model.
-        """
-        self.partial_updates = partial_updates
-        self.resource_states = resource_states
-        self.resource_sets = resource_sets
-        self.removed_resource_sets = removed_resource_sets
-        self.base_version: int = base_version
-        self.new_version: int = new_version
-        self.env = env
-        self.unknowns = unknowns
-
-    def pair_resources_partial_update_to_old_version(
-        self, old_resources: Dict[ResourceIdStr, ResourceWithResourceSet]
-    ) -> List[PairedResource]:
-        """
-        returns a list of paired resources
-
-        :param old_resources: A dict with as Key an ResourceIdStr and as value a resource and its resource_set.
-        """
-        paired_resources: List[PairedResource] = []
-        for partial_update in self.partial_updates:
-            key = Id.parse_id(partial_update.id).resource_str()
-            resource_set = self.resource_sets.get(key)
-            resource_state = self.resource_states.get(key, const.ResourceState.available)
-            pair: PairedResource = PairedResource(
-                new_resource=ResourceWithResourceSet(partial_update, resource_set, resource_state),
-                old_resource=old_resources.get(key),
-            )
-            paired_resources.append(pair)
-        return paired_resources
-
-    async def _get_base_resources(
-        self, *, connection: asyncpg.connection.Connection
-    ) -> dict[ResourceIdStr, ResourceWithResourceSet]:
-        """
-        Makes a call to the DB to get the resources for this instance's base version in the environment and return a dict
-        where the keys are the Ids of the resources and the values are ResourceWithResourceSet.
-        Sets the resource objects' version to the new version for the partial export.
-        """
-        old_data = await data.Resource.get_resources_for_version(
-            environment=self.env.id, version=self.base_version, connection=connection
-        )
-        old_resources: Dict[ResourceIdStr, ResourceWithResourceSet] = {}
-        for res in old_data:
-            resource: ResourceMinimal = ResourceMinimal.create_with_version(
-                new_version=self.new_version, id=res.resource_id, attributes=res.attributes
-            )
-            old_resources[resource.get_resource_id_str()] = ResourceWithResourceSet(
-                resource=resource, resource_set=res.resource_set, resource_state=res.status
-            )
-        return old_resources
-
-    def _merge_resources(
-        self,
-        old_resources: Dict[ResourceIdStr, ResourceWithResourceSet],
-        paired_resources_partial: List[PairedResource],
-        updated_resource_sets: Set[str],
-    ) -> dict[ResourceIdStr, ResourceWithResourceSet]:
-        """
-        Merges the resources of the partial compile with the old resources. To do so it keeps the old resources that are not in
-        the removed_resource_sets, that are in the shared resource_set and that are not being updated. It then adds the
-        resources coming form the partial compile if they don't break any rule:
-        - cannot move a resource to another resource set
-        - cannot update resources without a resource set.
-
-        :param old_resources: The resources to use as base for the merge. The version for each resource is expected to already
-            be set to the new version for this partial export.
-        """
-        to_keep: Sequence[ResourceWithResourceSet] = [
-            r
-            for r in old_resources.values()
-            if r.resource_set not in self.removed_resource_sets
-            and (r.is_shared_resource() or r.resource_set not in updated_resource_sets)
-        ]
-
-        merged_resources: Dict[ResourceIdStr, ResourceWithResourceSet] = {r.get_resource_id_str(): r for r in to_keep}
-
-        for paired_resource in paired_resources_partial:
-            new_resource = paired_resource.new_resource
-            old_resource = paired_resource.old_resource
-            assert (
-                old_resource is None
-                or Id.parse_id(old_resource.resource.id).resource_str() == Id.parse_id(new_resource.resource.id).resource_str()
-            )
-            if paired_resource.is_new_resource():
-                merged_resources[new_resource.get_resource_id_str()] = new_resource
-            else:
-                if paired_resource.resource_changed_resource_set():
-                    raise BadRequest(
-                        f"A partial compile cannot migrate resource {new_resource.resource.id} to another resource set"
-                    )
-                if new_resource.is_shared_resource() and paired_resource.is_update():
-                    raise BadRequest(
-                        f"Resource ({new_resource.resource.id}) without a resource set cannot"
-                        " be updated via a partial compile"
-                    )
-                else:
-                    merged_resources[new_resource.get_resource_id_str()] = new_resource
-        return merged_resources
-
-    def _merge_resource_sets(
-        self, old_resource_sets: Dict[ResourceIdStr, Optional[str]], updated_resource_sets: Set[str]
-    ) -> Dict[ResourceIdStr, Optional[str]]:
-        changed_resource_sets: Set[str] = updated_resource_sets.union(self.removed_resource_sets)
-        unchanged_resource_sets: Dict[ResourceIdStr, Optional[str]] = {
-            k: v for k, v in old_resource_sets.items() if v not in changed_resource_sets
-        }
-        return {**unchanged_resource_sets, **self.resource_sets}
-
-    async def _merge_unknowns(
-        self, merged_resources: dict[ResourceIdStr, ResourceWithResourceSet]
-    ) -> List[data.UnknownParameter]:
-        """
-        Merge all relevant, unresolved unknowns from the old version of the model together with the unknowns
-        of the partial compile.
-        """
-        rids_in_partial_update = {resource_minimal.get_resource_id_str() for resource_minimal in self.partial_updates}
-        rids_not_in_partial_compile = {rid for rid in merged_resources if rid not in rids_in_partial_update}
-        old_unresolved_unknowns_to_keep = [
-            uk.copy(self.new_version)
-            for uk in await data.UnknownParameter.get_list(environment=self.env.id, version=self.base_version, resolved=False)
-            # Always keep unknowns not tied to a specific resource
-            if not uk.resource_id or uk.resource_id in rids_not_in_partial_compile
-        ]
-        return [*old_unresolved_unknowns_to_keep, *self.unknowns]
-
-    async def apply_partial(self, *, connection: asyncpg.connection.Connection) -> MergedModel:
-        """
-        Applies the partial model's resources on this instance's base version. The caller should acquire appropriate locks on
-        the database connection as defined in the put_partial method definition.
-
-        :param connection: The database connection to use to determine the latest version. Appropriate locks are assumed to be
-            acquired.
-        :return: A tuple of the resources and the resource sets. All resource version ids are set to this instance's new
-            version.
-        """
-        old_resources: dict[ResourceIdStr, ResourceWithResourceSet] = await self._get_base_resources(connection=connection)
-        old_resource_sets: Dict[ResourceIdStr, Optional[str]] = {
-            res_id: res.resource_set for res_id, res in old_resources.items()
-        }
-        paired_resources_partial = self.pair_resources_partial_update_to_old_version(old_resources)
-        updated_resource_sets: Set[str] = set(
-            res.new_resource.resource_set for res in paired_resources_partial if not res.new_resource.is_shared_resource()
+    ctx = ",".join([f"{k}: {v}" for k, v in context.items()])
+    LOGGER.error("%s %s", message, ctx)
+    raise BadRequest(message)
+
+
+class ResourceActionLogLine(logging.LogRecord):
+    """A special log record that is used to report log lines that come from the agent"""
+
+    def __init__(self, logger_name: str, level: int, msg: str, created: datetime.datetime) -> None:
+        super().__init__(
+            name=logger_name,
+            level=level,
+            pathname="(unknown file)",
+            lineno=0,
+            msg=msg,
+            args=[],
+            exc_info=None,
+            func=None,
+            sinfo=None,
         )
 
-        merged_resources: dict[ResourceIdStr, ResourceWithResourceSet] = self._merge_resources(
-            old_resources, paired_resources_partial, updated_resource_sets
-        )
-        return MergedModel(
-            resources=[r.resource.dict() for r in merged_resources.values()],
-            resource_states={rid: r.get_resource_state_for_new_resource() for rid, r in merged_resources.items()},
-            resource_sets=self._merge_resource_sets(old_resource_sets, updated_resource_sets),
-            unknowns=await self._merge_unknowns(merged_resources),
-        )
+        self.created = created.timestamp()
+        self.msecs = (self.created - int(self.created)) * 1000
+        self.relativeCreated = (self.created - logging._startTime) * 1000
 
 
-class OrchestrationService(protocol.ServerSlice):
+class ResourceService(protocol.ServerSlice):
     """Resource Manager service"""
 
     agentmanager_service: "AgentManager"
-    autostarted_agent_manager: AutostartedAgentManager
-    resource_service: ResourceService
 
     def __init__(self) -> None:
-        super(OrchestrationService, self).__init__(SLICE_ORCHESTRATION)
+        super(ResourceService, self).__init__(SLICE_RESOURCE)
+
+        self._resource_action_loggers: Dict[uuid.UUID, logging.Logger] = {}
+        self._resource_action_handlers: Dict[uuid.UUID, logging.Handler] = {}
+
+        # Dict: environment_id: (model_version, increment, negative_increment)
+        self._increment_cache: Dict[uuid.UUID, Optional[tuple[int, abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]]]] = {}
+        # lock to ensure only one inflight request
+        self._increment_cache_locks: Dict[uuid.UUID, asyncio.Lock] = defaultdict(lambda: asyncio.Lock())
 
     def get_dependencies(self) -> List[str]:
-        return [SLICE_RESOURCE, SLICE_AGENT_MANAGER, SLICE_DATABASE]
+        return [SLICE_DATABASE, SLICE_AGENT_MANAGER]
 
     def get_depended_by(self) -> List[str]:
         return [SLICE_TRANSPORT]
 
     async def prestart(self, server: protocol.Server) -> None:
         await super().prestart(server)
         self.agentmanager_service = cast("AgentManager", server.get_slice(SLICE_AGENT_MANAGER))
-        self.autostarted_agent_manager = cast(AutostartedAgentManager, server.get_slice(SLICE_AUTOSTARTED_AGENT_MANAGER))
-        self.resource_service = cast(ResourceService, server.get_slice(SLICE_RESOURCE))
 
     async def start(self) -> None:
-        if PERFORM_CLEANUP:
-            self.schedule(self._purge_versions, opt.server_purge_version_interval.get(), cancel_on_stop=False)
-            self.add_background_task(self._purge_versions())
+        self.schedule(
+            data.ResourceAction.purge_logs, opt.server_purge_resource_action_logs_interval.get(), cancel_on_stop=False
+        )
         await super().start()
 
-    async def _purge_versions(self) -> None:
-        """
-        Purge versions from the database
-        """
-        # TODO: move to data and use queries for delete
-        envs = await data.Environment.get_list()
-        for env_item in envs:
-            # get available versions
-            n_versions = await env_item.get(AVAILABLE_VERSIONS_TO_KEEP)
-            assert isinstance(n_versions, int)
-            versions = await data.ConfigurationModel.get_list(environment=env_item.id)
-            if len(versions) > n_versions:
-                LOGGER.info("Removing %s available versions from environment %s", len(versions) - n_versions, env_item.id)
-                version_dict = {x.version: x for x in versions}
-                delete_list = sorted(version_dict.keys())
-                delete_list = delete_list[:-n_versions]
-
-                for v in delete_list:
-                    await version_dict[v].delete_cascade()
-
-    @handle(methods.list_versions, env="tid")
-    async def list_version(self, env: data.Environment, start: Optional[int] = None, limit: Optional[int] = None) -> Apireturn:
-        if (start is None and limit is not None) or (limit is None and start is not None):
-            raise ServerError("Start and limit should always be set together.")
-
-        if start is None or limit is None:
-            start = 0
-            limit = data.APILIMIT
+    async def stop(self) -> None:
+        await super().stop()
+        self._close_resource_action_loggers()
 
-        if limit > APILIMIT:
-            raise BadRequest(f"limit parameter can not exceed {APILIMIT}, got {limit}.")
+    def clear_env_cache(self, env: data.Environment) -> None:
+        LOGGER.log(const.LOG_LEVEL_TRACE, "Clearing cache for %s", env.id)
+        self._increment_cache[env.id] = None
 
-        models = await data.ConfigurationModel.get_versions(env.id, start, limit)
-        count = len(models)
+    @staticmethod
+    def get_resource_action_log_file(environment: uuid.UUID) -> str:
+        """Get the correct filename for the given environment
+        :param environment: The environment id to get the file for
+        :return: The path to the logfile
+        """
+        return os.path.join(opt.log_dir.get(), opt.server_resource_action_log_prefix.get() + str(environment) + ".log")
 
-        d = {
-            "versions": models,
-            "start": start,
-            "limit": limit,
-            "count": count,
-        }
+    def get_resource_action_logger(self, environment: uuid.UUID) -> logging.Logger:
+        """Get the resource action logger for the given environment. If the logger was not created, create it.
+        :param environment: The environment to get a logger for
+        :return: The logger for the given environment.
+        """
+        if environment in self._resource_action_loggers:
+            return self._resource_action_loggers[environment]
 
-        return 200, d
+        resource_action_log = self.get_resource_action_log_file(environment)
 
-    @handle(methods.get_version, version_id="id", env="tid")
-    async def get_version(
-        self,
-        env: data.Environment,
-        version_id: int,
-        include_logs: Optional[bool] = None,
-        log_filter: Optional[str] = None,
-        limit: Optional[int] = 0,
-    ) -> Apireturn:
-        version = await data.ConfigurationModel.get_version(env.id, version_id)
-        if version is None:
-            return 404, {"message": "The given configuration model does not exist yet."}
+        file_handler = logging.handlers.WatchedFileHandler(filename=resource_action_log, mode="a+")
+        # Most logs will come from agents. We need to use their level and timestamp and their formatted message
+        file_handler.setFormatter(logging.Formatter(fmt="%(asctime)s %(levelname)-8s %(name)-10s %(message)s"))
+        file_handler.setLevel(logging.DEBUG)
 
-        resources = await data.Resource.get_resources_for_version(env.id, version_id, no_obj=True)
-        if resources is None:
-            return 404, {"message": "The given configuration model does not exist yet."}
+        resource_action_logger = logging.getLogger(const.NAME_RESOURCE_ACTION_LOGGER).getChild(str(environment))
+        resource_action_logger.setLevel(logging.DEBUG)
+        resource_action_logger.addHandler(file_handler)
 
-        if limit is None:
-            limit = APILIMIT
-        elif limit > APILIMIT:
-            raise BadRequest(
-                f"limit parameter can not exceed {APILIMIT}, got {limit}."
-                f" To retrieve more entries, use /api/v2/resource_actions"
-            )
+        self._resource_action_loggers[environment] = resource_action_logger
+        self._resource_action_handlers[environment] = file_handler
 
-        resources_out: List[JsonType] = []
-        d = {"model": version, "resources": resources_out}
-        resource_action_lookup: Dict[ResourceVersionIdStr, List[data.ResourceAction]] = {}
-
-        for res_dict in resources:
-            resources_out.append(res_dict)
-            if bool(include_logs):
-                actions: List[data.ResourceAction] = []
-                res_dict["actions"] = actions
-                resource_action_lookup[res_dict["resource_version_id"]] = actions
-
-        if include_logs:
-            # get all logs, unsorted
-            all_logs = await data.ResourceAction.get_logs_for_version(env.id, version_id, log_filter, limit)
-            for log in all_logs:
-                for resource_version_id in log.resource_version_ids:
-                    resource_action_lookup[resource_version_id].append(log)
-
-        d["unknowns"] = await data.UnknownParameter.get_list(environment=env.id, version=version_id)
-
-        return 200, d
-
-    @handle(methods.delete_version, version_id="id", env="tid")
-    async def delete_version(self, env: data.Environment, version_id: int) -> Apireturn:
-        version = await data.ConfigurationModel.get_version(env.id, version_id)
-        if version is None:
-            return 404, {"message": "The given configuration model does not exist yet."}
+        return resource_action_logger
 
-        await version.delete_cascade()
-        return 200
+    def _close_resource_action_loggers(self) -> None:
+        """Close all resource action loggers and their associated handlers"""
+        try:
+            while True:
+                env, logger = self._resource_action_loggers.popitem()
+                self.close_resource_action_logger(env, logger)
+        except KeyError:
+            pass
+
+    def close_resource_action_logger(self, env: uuid.UUID, logger: Optional[logging.Logger] = None) -> None:
+        """Close the given logger for the given env.
+        :param env: The environment to close the logger for
+        :param logger: The logger to close, if the logger is none it is retrieved
+        """
+        if logger is None:
+            if env in self._resource_action_loggers:
+                logger = self._resource_action_loggers.pop(env)
+            else:
+                return
+
+        handler = self._resource_action_handlers.pop(env)
+        logger.removeHandler(handler)
+        handler.flush()
+        handler.close()
 
-    @handle(methods_v2.reserve_version, env="tid")
-    async def reserve_version(self, env: data.Environment) -> int:
-        return await env.get_next_version()
+    def log_resource_action(
+        self, env: uuid.UUID, resource_ids: Sequence[str], log_level: int, ts: datetime.datetime, message: str
+    ) -> None:
+        """Write the given log to the correct resource action logger"""
+        logger = self.get_resource_action_logger(env)
+        if len(resource_ids) == 0:
+            message = "no resources: " + message
+        elif len(resource_ids) > 1:
+            message = "multiple resources: " + message
+        else:
+            message = resource_ids[0] + ": " + message
+        log_record = ResourceActionLogLine(logger.name, log_level, message, ts)
+        logger.handle(log_record)
 
-    async def _put_version(
+    @handle(methods.get_resource, resource_id="id", env="tid")
+    async def get_resource(
         self,
         env: data.Environment,
-        version: int,
-        resources: List[JsonType],
-        resource_state: Dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]],
-        unknowns: List[data.UnknownParameter],
-        version_info: Optional[JsonType] = None,
-        resource_sets: Optional[Dict[ResourceIdStr, Optional[str]]] = None,
-        partial_base_version: Optional[int] = None,
-        *,
-        connection: asyncpg.connection.Connection,
-    ) -> None:
-        """
-        :param resources: a list of serialized resources
-        """
+        resource_id: ResourceVersionIdStr,
+        logs: bool,
+        status: bool,
+        log_action: const.ResourceAction,
+        log_limit: int,
+    ) -> Apireturn:
+        resv = await data.Resource.get(env.id, resource_id)
+        if resv is None:
+            return 404, {"message": "The resource with the given id does not exist in the given environment"}
+
+        if status is not None and status:
+            return 200, {"status": resv.status}
+
+        actions: List[data.ResourceAction] = []
+        if bool(logs):
+            action_name = None
+            if log_action is not None:
+                action_name = log_action.name
 
-        if version > env.last_version:
-            raise BadRequest(
-                f"The version number used is {version} "
-                f"which is higher than the last outstanding reservation {env.last_version}"
+            actions = await data.ResourceAction.get_log(
+                environment=env.id, resource_version_id=resource_id, action=action_name, limit=log_limit
             )
-        if version <= 0:
-            raise BadRequest(f"The version number used ({version}) is not positive")
-
-        for r in resources:
-            resource = Id.parse_id(r["id"])
-            if resource.get_version() != version:
-                raise BadRequest(
-                    f"The resource version of resource {r['id']} does not match the version argument (version: {version})"
-                )
 
-        if not resource_sets:
-            resource_sets = {}
+        return 200, {"resource": resv, "logs": actions}
 
-        for res_set in resource_sets.keys():
-            try:
-                Id.parse_id(res_set)
-            except Exception as e:
-                raise BadRequest("Invalid resource id in resource set: %s" % str(e))
+    # This endpoint does't have a method associated yet.
+    # Intended for use by other slices
+    async def get_resources_in_latest_version(
+        self,
+        environment: data.Environment,
+        resource_type: Optional[ResourceType] = None,
+        attributes: Dict[PrimitiveTypes, PrimitiveTypes] = {},
+    ) -> List[Resource]:
+        result = await data.Resource.get_resources_in_latest_version(environment.id, resource_type, attributes)
+        return [r.to_dto() for r in result]
+
+    @handle(methods.get_resources_for_agent, env="tid")
+    async def get_resources_for_agent(
+        self, env: data.Environment, agent: str, version: int, sid: uuid.UUID, incremental_deploy: bool
+    ) -> Apireturn:
+        if not self.agentmanager_service.is_primary(env, sid, agent):
+            return 409, {"message": "This agent is not currently the primary for the endpoint %s (sid: %s)" % (agent, sid)}
+        if incremental_deploy:
+            if version is not None:
+                return 500, {"message": "Cannot request increment for a specific version"}
+            result = await self.get_resource_increment_for_agent(env, agent)
+        else:
+            result = await self.get_all_resources_for_agent(env, agent, version)
+        return result
 
+    async def get_all_resources_for_agent(self, env: data.Environment, agent: str, version: int) -> Apireturn:
         started = datetime.datetime.now().astimezone()
+        if version is None:
+            version = await data.ConfigurationModel.get_version_nr_latest_version(env.id)
+            if version is None:
+                return 404, {"message": "No version available"}
 
-        agents = set()
-        # lookup for all RV's, lookup by resource id
-        rv_dict: Dict[ResourceIdStr, data.Resource] = {}
-        # reverse dependency tree, Resource.provides [:] -- Resource.requires as resource_id
-        provides_tree: Dict[str, List[str]] = defaultdict(lambda: [])
-        # list of all resources which have a cross agent dependency, as a tuple, (dependant,requires)
-        cross_agent_dep = []
-        # list of all resources which are undeployable
-        undeployable: List[data.Resource] = []
-
-        resource_objects = []
-        resource_version_ids = []
-        for res_dict in resources:
-            res_obj = data.Resource.new(env.id, res_dict["id"])
-            if res_obj.resource_id in resource_state:
-                res_obj.status = const.ResourceState[resource_state[res_obj.resource_id]]
-                if res_obj.status in const.UNDEPLOYABLE_STATES:
-                    undeployable.append(res_obj)
-            if res_obj.resource_id in resource_sets:
-                res_obj.resource_set = resource_sets[res_obj.resource_id]
-
-            # collect all agents
-            agents.add(res_obj.agent)
-
-            attributes = {}
-            for field, value in res_dict.items():
-                if field != "id":
-                    attributes[field] = value
-
-            res_obj.attributes = attributes
-            resource_objects.append(res_obj)
-            resource_version_ids.append(res_obj.resource_version_id)
-
-            rv_dict[res_obj.resource_id] = res_obj
-
-            # find cross agent dependencies
-            agent = res_obj.agent
-            resc_id = res_obj.resource_id
-            if "requires" not in attributes:
-                LOGGER.warning("Received resource without requires attribute (%s)" % res_obj.resource_id)
-            else:
-                # Collect all requires as resource_ids instead of resource version ids
-                cleaned_requires = []
-                for req in attributes["requires"]:
-                    rid = Id.parse_id(req)
-                    provides_tree[rid.resource_str()].append(resc_id)
-                    if rid.get_agent_name() != agent:
-                        # it is a CAD
-                        cross_agent_dep.append((res_obj, rid))
-                    cleaned_requires.append(rid.resource_str())
-                attributes["requires"] = cleaned_requires
-        resource_ids = {res.resource_id for res in resource_objects}
-        superfluous_ids = set(resource_sets.keys()) - resource_ids
-        if superfluous_ids:
-            raise BadRequest(
-                "The following resource ids provided in the resource_sets parameter are not present "
-                f"in the resources list: {', '.join(superfluous_ids)}"
-            )
-        requires_ids = set(provides_tree.keys())
-        if not requires_ids.issubset(resource_ids):
-            raise BadRequest(
-                "The model should have a dependency graph that is closed and no dangling dependencies:"
-                f" {requires_ids-resource_ids}"
+        else:
+            exists = await data.ConfigurationModel.version_exists(environment=env.id, version=version)
+            if not exists:
+                return 404, {"message": "The given version does not exist"}
+
+        deploy_model = []
+
+        resources = await data.Resource.get_resources_for_version(env.id, version, agent)
+
+        resource_ids = []
+        for rv in resources:
+            deploy_model.append(rv.to_dict())
+            resource_ids.append(rv.resource_version_id)
+
+        # Don't log ResourceActions without resource_version_ids, because
+        # no API call exists to retrieve them.
+        if resource_ids:
+            now = datetime.datetime.now().astimezone()
+            log_line = data.LogLine.log(
+                logging.INFO, "Resource version pulled by client for agent %(agent)s state", agent=agent
             )
-        # hook up all CADs
-        for f, t in cross_agent_dep:
-            res_obj = rv_dict[t.resource_str()]
-            res_obj.provides.append(f.resource_id)
-
-        # detect failed compiles
-        def safe_get(input: object, key: str, default: object) -> object:
-            if not isinstance(input, dict):
-                return default
-            if key not in input:
-                return default
-            return input[key]
-
-        metadata: object = safe_get(version_info, const.EXPORT_META_DATA, {})
-        compile_state = safe_get(metadata, const.META_DATA_COMPILE_STATE, "")
-        failed = compile_state == const.Compilestate.failed
-
-        resources_to_purge: List[data.Resource] = []
-        if not failed and (await env.get(PURGE_ON_DELETE)):
-            # search for deleted resources (purge_on_delete)
-            resources_to_purge = await data.Resource.get_deleted_resources(
-                env.id, version, list(rv_dict.keys()), connection=connection
+            self.log_resource_action(env.id, resource_ids, logging.INFO, now, log_line.msg)
+            ra = data.ResourceAction(
+                environment=env.id,
+                version=version,
+                resource_version_ids=resource_ids,
+                action=const.ResourceAction.pull,
+                action_id=uuid.uuid4(),
+                started=started,
+                finished=now,
+                messages=[log_line],
             )
+            await ra.insert()
 
-            previous_requires = {}
-            for res in resources_to_purge:
-                LOGGER.warning("Purging %s, purged resource based on %s" % (res.resource_id, res.resource_version_id))
-
-                attributes = res.attributes.copy()
-                attributes["purged"] = True
-                attributes["requires"] = []
-                res_obj = data.Resource.new(
-                    env.id,
-                    resource_version_id=ResourceVersionIdStr("%s,v=%s" % (res.resource_id, version)),
-                    attributes=attributes,
-                )
-                resource_objects.append(res_obj)
+        return 200, {"environment": env.id, "agent": agent, "version": version, "resources": deploy_model}
 
-                previous_requires[res_obj.resource_id] = res.attributes["requires"]
-                resource_version_ids.append(res_obj.resource_version_id)
-                agents.add(res_obj.agent)
-                rv_dict[res_obj.resource_id] = res_obj
-
-            # invert dependencies on purges
-            for res_id, requires in previous_requires.items():
-                res_obj = rv_dict[res_id]
-                for require in requires:
-                    req_id = Id.parse_id(require)
-
-                    if req_id.resource_str() in rv_dict:
-                        req_res = rv_dict[req_id.resource_str()]
-
-                        req_res.attributes["requires"].append(res_obj.resource_version_id)
-                        res_obj.provides.append(req_res.resource_id)
-
-        undeployable_ids: List[str] = [res.resource_id for res in undeployable]
-        # get skipped for undeployable
-        work = list(undeployable_ids)
-        skippeable: Set[str] = set()
-        while len(work) > 0:
-            current = work.pop()
-            if current in skippeable:
-                continue
-            skippeable.add(current)
-            work.extend(provides_tree[current])
+    async def get_resource_increment_for_agent(self, env: data.Environment, agent: str) -> Apireturn:
+        started = datetime.datetime.now().astimezone()
 
-        skip_list = sorted(list(skippeable - set(undeployable_ids)))
+        version = await data.ConfigurationModel.get_version_nr_latest_version(env.id)
+        if version is None:
+            return 404, {"message": "No version available"}
 
-        try:
-            cm = data.ConfigurationModel(
-                environment=env.id,
-                version=version,
-                date=datetime.datetime.now().astimezone(),
-                total=len(resources),
-                version_info=version_info,
-                undeployable=undeployable_ids,
-                skipped_for_undeployable=skip_list,
-                partial_base=partial_base_version,
-            )
-            await cm.insert(connection=connection)
-        except asyncpg.exceptions.UniqueViolationError:
-            raise ServerError("The given version is already defined. Versions should be unique.")
+        increments: tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]] = await self.get_increment(env, version)
+        increment_ids, neg_increment = increments
 
-        await data.Resource.insert_many(resource_objects, connection=connection)
-        await cm.update_fields(total=cm.total + len(resources_to_purge), connection=connection)
+        now = datetime.datetime.now().astimezone()
+
+        def on_agent(res: ResourceIdStr) -> bool:
+            idr = Id.parse_id(res)
+            return idr.get_agent_name() == agent
+
+        # set already done to deployed
+        await self.mark_deployed(env, neg_increment, now, version, filter=on_agent)
+
+        resources = await data.Resource.get_resources_for_version(env.id, version, agent)
+
+        deploy_model: List[Dict[str, Any]] = []
+        resource_ids: List[str] = []
 
-        for uk in unknowns:
-            await uk.insert(connection=connection)
+        for rv in resources:
+            if rv.resource_id not in increment_ids:
+                continue
 
-        for agent in agents:
-            await self.agentmanager_service.ensure_agent_registered(env, agent, connection=connection)
+            # TODO double parsing of ID
+            def in_requires(req: ResourceIdStr) -> bool:
+                if req in increment_ids:
+                    return True
+                idr = Id.parse_id(req)
+                return idr.get_agent_name() != agent
+
+            rv.attributes["requires"] = [r for r in rv.attributes["requires"] if in_requires(r)]
+            deploy_model.append(rv.to_dict())
+            resource_ids.append(rv.resource_version_id)
 
         # Don't log ResourceActions without resource_version_ids, because
         # no API call exists to retrieve them.
-        if resource_version_ids:
-            now = datetime.datetime.now().astimezone()
-            log_line = data.LogLine.log(logging.INFO, "Successfully stored version %(version)d", version=version)
-            self.resource_service.log_resource_action(env.id, resource_version_ids, logging.INFO, now, log_line.msg)
+        if resource_ids:
             ra = data.ResourceAction(
                 environment=env.id,
                 version=version,
-                resource_version_ids=resource_version_ids,
+                resource_version_ids=resource_ids,
+                action=const.ResourceAction.pull,
                 action_id=uuid.uuid4(),
-                action=const.ResourceAction.store,
                 started=started,
                 finished=now,
-                messages=[log_line],
+                messages=[
+                    data.LogLine.log(logging.INFO, "Resource version pulled by client for agent %(agent)s state", agent=agent)
+                ],
             )
-            await ra.insert(connection=connection)
+            await ra.insert()
 
-        LOGGER.debug("Successfully stored version %d", version)
+        return 200, {"environment": env.id, "agent": agent, "version": version, "resources": deploy_model}
 
-        self.resource_service.clear_env_cache(env)
-
-    async def _trigger_auto_deploy(
+    async def mark_deployed(
         self,
         env: data.Environment,
+        resources_id: abc.Set[ResourceIdStr],
+        timestamp: datetime.datetime,
         version: int,
+        filter: Callable[[ResourceIdStr], bool] = lambda x: True,
     ) -> None:
         """
-        Triggers auto-deploy for stored resources. Must be called only after transaction that stores resources has been allowed
-        to commit. If not respected, the auto deploy might work on stale data, likely resulting in resources hanging in the
-        deploying state.
+        Set the status of the provided resources as deployed
+        :param env: Environment to consider.
+        :param resources_id: Set of resources to mark as deployed.
+        :param timestamp: Timestamp for the log message and the resource action entry.
+        :param version: Version of the resources to consider.
+        :param filter: Filter function that takes a resource id as an argument and returns True if it should be kept.
         """
-        auto_deploy = await env.get(data.AUTO_DEPLOY)
-        if auto_deploy:
-            LOGGER.debug("Auto deploying version %d", version)
-            push_on_auto_deploy = cast(bool, await env.get(data.PUSH_ON_AUTO_DEPLOY))
-            agent_trigger_method_on_autodeploy = cast(str, await env.get(data.AGENT_TRIGGER_METHOD_ON_AUTO_DEPLOY))
-            agent_trigger_method_on_autodeploy = const.AgentTriggerMethod[agent_trigger_method_on_autodeploy]
-            await self.release_version(env, version, push_on_auto_deploy, agent_trigger_method_on_autodeploy)
-
-    def _create_unknown_from_dct(
-        self, env_id: uuid.UUID, version: int, unknowns: Optional[List[Dict[str, PrimitiveTypes]]] = None
-    ) -> List[data.UnknownParameter]:
-        if not unknowns:
-            return []
-        result = []
-        for uk in unknowns:
-            if "resource" not in uk:
-                uk["resource"] = ""
-            if "metadata" not in uk:
-                uk["metadata"] = {}
-            unknown_parameter = data.UnknownParameter(
-                resource_id=uk["resource"],
-                name=uk["parameter"],
-                source=uk["source"],
-                environment=env_id,
-                version=version,
-                metadata=uk["metadata"],
-            )
-            result.append(unknown_parameter)
-        return result
-
-    async def _put_version_lock(self, env: data.Environment, *, shared: bool = False, connection: asyncpg.Connection) -> None:
-        """
-        Acquires a transaction-level advisory lock for concurrency control between put_version and put_partial.
-
-        :param env: The environment to acquire the lock for.
-        :param shared: If true, doesn't conflict with other shared locks, only with non-shared once.
-        :param connection: The connection hosting the transaction for which to acquire a lock.
-        """
-        lock: str = "pg_advisory_xact_lock_shared" if shared else "pg_advisory_xact_lock"
-        await connection.execute(
-            # Advisory lock keys are only 32 bit (or a single 64 bit key), while a full uuid is 128 bit.
-            # Since locking slightly too strictly at extremely low odds is acceptable, we only use a 32 bit subvalue
-            # of the uuid. For uuid4, time_low is (despite the name) randomly generated. Since it is an unsigned
-            # integer while Postgres expects a signed one, we shift it by 2**31.
-            f"SELECT {lock}({const.PG_ADVISORY_KEY_PUT_VERSION}, {env.id.time_low - 2**31})"
+        resources_version_ids: list[ResourceVersionIdStr] = [
+            ResourceVersionIdStr(f"{res_id},v={version}") for res_id in resources_id if filter(res_id)
+        ]
+        logline = {
+            "level": "INFO",
+            "msg": "Setting deployed due to known good status",
+            "timestamp": util.datetime_utc_isoformat(timestamp),
+            "args": [],
+        }
+        await self.resource_action_update(
+            env,
+            resources_version_ids,
+            action_id=uuid.uuid4(),
+            started=timestamp,
+            finished=timestamp,
+            status=const.ResourceState.deployed,
+            # does this require a different ResourceAction?
+            action=const.ResourceAction.deploy,
+            changes={},
+            messages=[logline],
+            change=const.Change.nochange,
+            send_events=False,
+            keep_increment_cache=True,
         )
 
-    @handle(methods.put_version, env="tid")
-    async def put_version(
-        self,
-        env: data.Environment,
-        version: int,
-        resources: List[JsonType],
-        resource_state: Dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]],
-        unknowns: List[Dict[str, PrimitiveTypes]],
-        version_info: JsonType,
-        compiler_version: Optional[str] = None,
-        resource_sets: Optional[Dict[ResourceIdStr, Optional[str]]] = None,
-    ) -> Apireturn:
-        """
-        :param unknowns: dict with the following structure
-                            {
-                             "resource": ResourceIdStr,
-                             "parameter": str,
-                             "source": str
-                            }
+    async def get_increment(self, env: data.Environment, version: int) -> tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]]:
         """
-        if not compiler_version:
-            raise BadRequest("Older compiler versions are no longer supported, please update your compiler")
+        Get the increment for a given environment and a given version of the model from the _increment_cache if possible.
+        In case of cache miss, the increment calculation is performed behind a lock to make sure it is only done once per
+        version, per environment.
+
+        :param env: The environment to consider.
+        :parma version: The version of the model to consider.
+        """
+
+        def _get_cache_entry() -> Optional[tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]]]:
+            """
+            Returns a tuple (increment, negative_increment) if a cache entry exists for the given environment and version
+            or None if no such cache entry exists.
+            """
+            cache_entry = self._increment_cache.get(env.id, None)
+            if cache_entry is None:
+                # No cache entry found
+                return None
+            (version_cache_entry, incr, neg_incr) = cache_entry
+            if version_cache_entry != version:
+                # Cache entry exists for another version
+                return None
+            return incr, neg_incr
+
+        increment: Optional[tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]]] = _get_cache_entry()
+        if increment is None:
+            lock = self._increment_cache_locks[env.id]
+            async with lock:
+                increment = _get_cache_entry()
+                if increment is None:
+                    increment = await data.ConfigurationModel.get_increment(env.id, version)
+                    self._increment_cache[env.id] = (version, *increment)
+        return increment
 
-        unknown_objs = self._create_unknown_from_dct(env.id, version, unknowns)
-        async with data.Resource.get_connection() as con:
-            async with con.transaction():
-                # Acquire a lock that conflicts with the lock acquired by put_partial but not with itself
-                await self._put_version_lock(env, shared=True, connection=con)
-                await self._put_version(
-                    env, version, resources, resource_state, unknown_objs, version_info, resource_sets, connection=con
-                )
-        await self._trigger_auto_deploy(env, version)
-        return 200
-
-    @handle(methods_v2.put_partial, env="tid")
-    async def put_partial(
+    @handle(methods_v2.resource_deploy_done, env="tid", resource_id="rvid")
+    async def resource_deploy_done(
         self,
         env: data.Environment,
-        resources: object,
-        resource_state: Optional[Dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]]] = None,
-        unknowns: Optional[List[Dict[str, PrimitiveTypes]]] = None,
-        version_info: Optional[JsonType] = None,
-        resource_sets: Optional[Dict[ResourceIdStr, Optional[str]]] = None,
-        removed_resource_sets: Optional[List[str]] = None,
-    ) -> int:
-        """
-        :param unknowns: dict with the following structure
-                    {
-                     "resource": ResourceIdStr,
-                     "parameter": str,
-                     "source": str
-                    }
-        """
-        if resource_state is None:
-            resource_state = {}
-        if unknowns is None:
-            unknowns = []
-        if resource_sets is None:
-            resource_sets = {}
-        if removed_resource_sets is None:
-            removed_resource_sets = []
-        try:
-            resources = pydantic.parse_obj_as(List[ResourceMinimal], resources)
-        except pydantic.ValidationError:
-            raise BadRequest(
-                "Type validation failed for resources argument. "
-                f"Expected an argument of type List[Dict[str, Any]] but received {resources}"
+        resource_id: Id,
+        action_id: uuid.UUID,
+        status: ResourceState,
+        messages: List[LogLine] = [],
+        changes: Dict[str, AttributeStateChange] = {},
+        change: Optional[Change] = None,
+        keep_increment_cache: bool = False,
+    ) -> None:
+        resource_id_str = resource_id.resource_version_str()
+        finished = datetime.datetime.now().astimezone()
+        changes_with_rvid = {resource_id_str: {attr_name: attr_change.dict()} for attr_name, attr_change in changes.items()}
+
+        if status not in VALID_STATES_ON_STATE_UPDATE:
+            error_and_log(
+                f"Status {status} is not a valid status at the end of a deployment.",
+                resource_ids=[resource_id_str],
+                action=const.ResourceAction.deploy,
+                action_id=action_id,
             )
-
-        # validate resources before any side effects take place
-        for r in resources:
-            rid = Id.parse_id(r.id)
-            if rid.get_version() != 0:
-                raise BadRequest("Resources for partial export should not contain version information")
-
-        intersection: set[str] = set(resource_sets.values()).intersection(set(removed_resource_sets))
-        if intersection:
-            raise BadRequest(
-                "Following resource sets are present in the removed resource sets and in the resources that are exported: "
-                f"{intersection}"
+        if status in TRANSIENT_STATES:
+            error_and_log(
+                "No transient state can be used to mark a deployment as done.",
+                status=status,
+                resource_ids=[resource_id_str],
+                action=const.ResourceAction.deploy,
+                action_id=action_id,
             )
 
-        async with data.Resource.get_connection() as con:
-            async with con.transaction():
-                # Acquire a lock that conflicts with itself and with the lock acquired by put_version
-                await self._put_version_lock(env, shared=False, connection=con)
-
-                # Only request a new version once the resource lock has been acquired to ensure a monotonic version history
-                version: int = await env.get_next_version(connection=con)
+        async with data.Resource.get_connection() as connection:
+            async with connection.transaction():
+                resource = await data.Resource.get_one(
+                    connection=connection,
+                    environment=env.id,
+                    resource_id=resource_id.resource_str(),
+                    model=resource_id.version,
+                    # acquire lock on Resource before read and before lock on ResourceAction to prevent conflicts with
+                    # cascading deletes
+                    lock=data.RowLockMode.FOR_UPDATE,
+                )
+                if resource is None:
+                    raise NotFound("The resource with the given id does not exist in the given environment.")
 
-                unknown_objs = self._create_unknown_from_dct(env.id, version, unknowns)
+                # no escape from terminal
+                if resource.status != status and resource.status in TERMINAL_STATES:
+                    LOGGER.error("Attempting to set undeployable resource to deployable state")
+                    raise AssertionError("Attempting to set undeployable resource to deployable state")
+
+                resource_action = await data.ResourceAction.get(action_id=action_id, connection=connection)
+                if resource_action is None:
+                    raise NotFound(
+                        f"No resource action exists for action_id {action_id}. Ensure "
+                        f"`/resource/<resource_id>/deploy/start` is called first. "
+                    )
+                if resource_action.finished is not None:
+                    raise Conflict(
+                        f"Resource action with id {resource_id_str} was already marked as done at {resource_action.finished}."
+                    )
 
-                # set version on input resources
-                resources = [r.copy_with_new_version(new_version=version) for r in resources]
+                for log in messages:
+                    # All other data is stored in the database. The msg was already formatted at the client side.
+                    self.log_resource_action(
+                        env.id,
+                        [resource_id_str],
+                        log.level.to_int,
+                        log.timestamp,
+                        log.msg,
+                    )
 
-                current_versions: abc.Sequence[data.ConfigurationModel] = await data.ConfigurationModel.get_versions(
-                    env.id, limit=1
+                await resource_action.set_and_save(
+                    messages=[
+                        {
+                            **log.dict(),
+                            "timestamp": log.timestamp.astimezone().isoformat(timespec="microseconds"),
+                        }
+                        for log in messages
+                    ],
+                    changes=changes_with_rvid,
+                    status=status,
+                    change=change,
+                    finished=finished,
+                    connection=connection,
                 )
-                if not current_versions:
-                    raise BadRequest("A partial export requires a base model but no versions have been exported yet.")
-                base_version: int = current_versions[0].version
-
-                merger = PartialUpdateMerger(
-                    env=env,
-                    base_version=base_version,
-                    new_version=version,
-                    partial_updates=resources,
-                    resource_states=resource_state,
-                    resource_sets=resource_sets,
-                    removed_resource_sets=removed_resource_sets,
-                    unknowns=unknown_objs,
+
+                # final resource update
+                if not keep_increment_cache:
+                    self.clear_env_cache(env)
+
+                await resource.update_fields(
+                    last_deploy=finished,
+                    status=status,
+                    last_non_deploying_status=const.NonDeployingResourceState(status),
+                    connection=connection,
                 )
-                merged_model: MergedModel = await merger.apply_partial(connection=con)
-                await data.Code.copy_versions(env.id, base_version, version, connection=con)
 
-                await self._put_version(
-                    env,
-                    version,
-                    merged_model.resources,
-                    merged_model.resource_states,
-                    merged_model.unknowns,
-                    version_info,
-                    merged_model.resource_sets,
-                    partial_base_version=base_version,
-                    connection=con,
+                if "purged" in resource.attributes and resource.attributes["purged"] and status == const.ResourceState.deployed:
+                    await data.Parameter.delete_all(environment=env.id, resource_id=resource.resource_id, connection=connection)
+
+        self.add_background_task(data.ConfigurationModel.mark_done_if_done(env.id, resource.model))
+
+        waiting_agents = set([(Id.parse_id(prov).get_agent_name(), resource.resource_version_id) for prov in resource.provides])
+        for agent, resource_id in waiting_agents:
+            aclient = self.agentmanager_service.get_agent_client(env.id, agent)
+            if aclient is not None:
+                if change is None:
+                    change = const.Change.nochange
+                await aclient.resource_event(
+                    tid=env.id,
+                    id=agent,
+                    resource=resource_id,
+                    send_events=False,
+                    state=status,
+                    change=change,
+                    changes=changes_with_rvid,
                 )
-        await self._trigger_auto_deploy(env, version)
-        return version
 
-    @handle(methods.release_version, version_id="id", env="tid")
-    async def release_version(
+    @handle(methods.resource_action_update, env="tid")
+    async def resource_action_update(
         self,
         env: data.Environment,
-        version_id: int,
-        push: bool,
-        agent_trigger_method: Optional[const.AgentTriggerMethod] = None,
+        resource_ids: List[ResourceVersionIdStr],
+        action_id: uuid.UUID,
+        action: const.ResourceAction,
+        started: datetime.datetime,
+        finished: datetime.datetime,
+        status: Optional[Union[const.ResourceState, const.DeprecatedResourceState]],
+        messages: List[Dict[str, Any]],
+        changes: Dict[str, Any],
+        change: const.Change,
+        send_events: bool,
+        keep_increment_cache: bool = False,
         *,
-        connection: Optional[asyncpg.connection.Connection] = None,
+        connection: Optional[Connection] = None,
     ) -> Apireturn:
-        model = await data.ConfigurationModel.get_version(env.id, version_id, connection=connection)
-        if model is None:
-            return 404, {"message": "The request version does not exist."}
-
-        await model.update_fields(released=True, result=const.VersionState.deploying, connection=connection)
-
-        if model.total == 0:
-            await model.mark_done(connection=connection)
-            return 200, {"model": model}
+        def convert_legacy_state(
+            status: Optional[Union[const.ResourceState, const.DeprecatedResourceState]]
+        ) -> Optional[const.ResourceState]:
+            if status is None or isinstance(status, const.ResourceState):
+                return status
+            if status == const.DeprecatedResourceState.processing_events:
+                return const.ResourceState.deploying
+            else:
+                raise BadRequest(f"Unsupported deprecated resources state {status.value}")
 
-        # Already mark undeployable resources as deployed to create a better UX (change the version counters)
-        undep = await model.get_undeployable()
-        now = datetime.datetime.now().astimezone()
+        status = convert_legacy_state(status)
 
-        if undep:
-            undep_ids = [ResourceVersionIdStr(rid + ",v=%s" % version_id) for rid in undep]
-            # not checking error conditions
-            await self.resource_service.resource_action_update(
-                env,
-                undep_ids,
-                action_id=uuid.uuid4(),
-                started=now,
-                finished=now,
-                status=const.ResourceState.undefined,
-                action=const.ResourceAction.deploy,
-                changes={},
-                messages=[],
-                change=const.Change.nochange,
-                send_events=False,
-                connection=connection,
-            )
+        # can update resource state
+        is_resource_state_update = action in STATE_UPDATE
+        # this ra is finishing
+        is_resource_action_finished = finished is not None
+
+        if is_resource_state_update:
+            # if status update, status is required
+            if status is None:
+                error_and_log(
+                    "Cannot perform state update without a status.",
+                    resource_ids=resource_ids,
+                    action=action,
+                    action_id=action_id,
+                )
+            # and needs to be valid
+            if status not in VALID_STATES_ON_STATE_UPDATE:
+                error_and_log(
+                    "Status %s is not valid on action %s" % (status, action),
+                    resource_ids=resource_ids,
+                    action=action,
+                    action_id=action_id,
+                )
+            if status in TRANSIENT_STATES:
+                if not is_resource_action_finished:
+                    pass
+                else:
+                    error_and_log(
+                        "The finished field must not be set for transient states",
+                        status=status,
+                        resource_ids=resource_ids,
+                        action=action,
+                        action_id=action_id,
+                    )
+            else:
+                if is_resource_action_finished:
+                    pass
+                else:
+                    error_and_log(
+                        "The finished field must be set for none transient states",
+                        status=status,
+                        resource_ids=resource_ids,
+                        action=action,
+                        action_id=action_id,
+                    )
 
-            skippable = await model.get_skipped_for_undeployable()
-            if skippable:
-                skippable_ids = [ResourceVersionIdStr(rid + ",v=%s" % version_id) for rid in skippable]
-                # not checking error conditions
-                await self.resource_service.resource_action_update(
-                    env,
-                    skippable_ids,
-                    action_id=uuid.uuid4(),
-                    started=now,
-                    finished=now,
-                    status=const.ResourceState.skipped_for_undefined,
-                    action=const.ResourceAction.deploy,
-                    changes={},
-                    messages=[],
-                    change=const.Change.nochange,
-                    send_events=False,
+        assert all(Id.is_resource_version_id(rvid) for rvid in resource_ids)
+
+        resources: List[data.Resource]
+        async with data.Resource.get_connection(connection) as connection:
+            async with connection.transaction():
+                # validate resources
+                resources = await data.Resource.get_resources(
+                    env.id,
+                    resource_ids,
+                    # acquire lock on Resource before read and before lock on ResourceAction to prevent conflicts with
+                    # cascading deletes
+                    lock=data.RowLockMode.FOR_UPDATE,
                     connection=connection,
                 )
+                if len(resources) == 0 or (len(resources) != len(resource_ids)):
+                    return (
+                        404,
+                        {
+                            "message": "The resources with the given ids do not exist in the given environment. "
+                            "Only %s of %s resources found." % (len(resources), len(resource_ids))
+                        },
+                    )
 
-        if push:
-            # fetch all resource in this cm and create a list of distinct agents
-            agents = await data.ConfigurationModel.get_agents(env.id, version_id, connection=connection)
-            await self.autostarted_agent_manager._ensure_agents(env, agents, connection=connection)
-
-            for agent in agents:
-                client = self.agentmanager_service.get_agent_client(env.id, agent)
-                if client is not None:
-                    if not agent_trigger_method:
-                        env_agent_trigger_method = await env.get(ENVIRONMENT_AGENT_TRIGGER_METHOD, connection=connection)
-                        incremental_deploy = env_agent_trigger_method == const.AgentTriggerMethod.push_incremental_deploy
-                    else:
-                        incremental_deploy = agent_trigger_method is const.AgentTriggerMethod.push_incremental_deploy
-                    self.add_background_task(client.trigger(env.id, agent, incremental_deploy))
+                # validate transitions
+                if is_resource_state_update:
+                    # no escape from terminal
+                    if any(resource.status != status and resource.status in TERMINAL_STATES for resource in resources):
+                        LOGGER.error("Attempting to set undeployable resource to deployable state")
+                        raise AssertionError("Attempting to set undeployable resource to deployable state")
+
+                # get instance
+                resource_action = await data.ResourceAction.get(action_id=action_id, connection=connection)
+                if resource_action is None:
+                    # new
+                    if started is None:
+                        return 500, {"message": "A resource action can only be created with a start datetime."}
+
+                    version = Id.parse_id(resource_ids[0]).version
+                    resource_action = data.ResourceAction(
+                        environment=env.id,
+                        version=version,
+                        resource_version_ids=resource_ids,
+                        action_id=action_id,
+                        action=action,
+                        started=started,
+                    )
+                    await resource_action.insert(connection=connection)
                 else:
-                    LOGGER.warning("Agent %s from model %s in env %s is not available for a deploy", agent, version_id, env.id)
+                    # existing
+                    if resource_action.finished is not None:
+                        return (
+                            500,
+                            {
+                                "message": (
+                                    "An resource action can only be updated when it has not been finished yet. This action "
+                                    "finished at %s" % resource_action.finished
+                                )
+                            },
+                        )
+
+                def parse_timestamp(timestamp: str) -> datetime.datetime:
+                    try:
+                        return datetime.datetime.strptime(timestamp, const.TIME_ISOFMT + "%z")
+                    except ValueError:
+                        # interpret naive datetimes as UTC
+                        return datetime.datetime.strptime(timestamp, const.TIME_ISOFMT).replace(tzinfo=datetime.timezone.utc)
+
+                for msg in messages:
+                    # All other data is stored in the database. The msg was already formatted at the client side.
+                    self.log_resource_action(
+                        env.id,
+                        resource_ids,
+                        const.LogLevel(msg["level"]).to_int,
+                        parse_timestamp(msg["timestamp"]),
+                        msg["msg"],
+                    )
+                await resource_action.set_and_save(
+                    messages=[
+                        {
+                            **msg,
+                            "timestamp": parse_timestamp(msg["timestamp"]).isoformat(timespec="microseconds"),
+                        }
+                        for msg in messages
+                    ],
+                    changes=changes,
+                    status=status,
+                    change=change,
+                    finished=finished,
+                    connection=connection,
+                )
 
-        return 200, {"model": model}
+                async def update_fields_resource(
+                    resource: data.Resource, connection: Optional[Connection] = None, **kwargs: object
+                ) -> None:
+                    """
+                    This method ensures that the `last_non_deploying_status` field in the database
+                    is updated correctly when the `status` field of a resource is updated.
+                    """
+                    if "status" in kwargs and kwargs["status"] is not ResourceState.deploying:
+                        kwargs["last_non_deploying_status"] = const.NonDeployingResourceState(kwargs["status"])
+                    await resource.update_fields(**kwargs, connection=connection)
+
+                if is_resource_state_update:
+                    # transient resource update
+                    if not is_resource_action_finished:
+                        for res in resources:
+                            await update_fields_resource(res, status=status, connection=connection)
+                        if not keep_increment_cache:
+                            self.clear_env_cache(env)
+                        return 200
 
-    @handle(methods.deploy, env="tid")
-    async def deploy(
+                    else:
+                        # final resource update
+                        if not keep_increment_cache:
+                            self.clear_env_cache(env)
+
+                        model_version = None
+                        for res in resources:
+                            await update_fields_resource(res, last_deploy=finished, status=status, connection=connection)
+                            model_version = res.model
+
+                            if (
+                                "purged" in res.attributes
+                                and res.attributes["purged"]
+                                and status == const.ResourceState.deployed
+                            ):
+                                await data.Parameter.delete_all(
+                                    environment=env.id, resource_id=res.resource_id, connection=connection
+                                )
+
+        if is_resource_state_update and is_resource_action_finished:
+            self.add_background_task(data.ConfigurationModel.mark_done_if_done(env.id, model_version))
+            waiting_agents = set(
+                [(Id.parse_id(prov).get_agent_name(), res.resource_version_id) for res in resources for prov in res.provides]
+            )
+
+            for agent, resource_id in waiting_agents:
+                aclient = self.agentmanager_service.get_agent_client(env.id, agent)
+                if aclient is not None:
+                    if change is None:
+                        change = const.Change.nochange
+                    self.add_background_task(
+                        aclient.resource_event(env.id, agent, resource_id, send_events, status, change, changes)
+                    )
+
+        return 200
+
+    @handle(methods_v2.resource_deploy_start, env="tid", resource_id="rvid")
+    async def resource_deploy_start(
         self,
         env: data.Environment,
-        agent_trigger_method: const.AgentTriggerMethod = const.AgentTriggerMethod.push_full_deploy,
-        agents: Optional[List[str]] = None,
-    ) -> Apireturn:
-        warnings = []
-
-        # get latest version
-        version_id = await data.ConfigurationModel.get_version_nr_latest_version(env.id)
-        if version_id is None:
-            return 404, {"message": "No version available"}
+        resource_id: Id,
+        action_id: uuid.UUID,
+    ) -> Dict[ResourceVersionIdStr, const.ResourceState]:
+        resource_id_str = resource_id.resource_version_str()
+        async with data.Resource.get_connection() as connection:
+            async with connection.transaction():
+                resource = await data.Resource.get_one(
+                    connection=connection,
+                    environment=env.id,
+                    resource_id=resource_id.resource_str(),
+                    model=resource_id.version,
+                )
+                if resource is None:
+                    raise NotFound(message=f"Environment {env.id} doesn't contain a resource with id {resource_id_str}")
 
-        # filter agents
-        allagents = await data.ConfigurationModel.get_agents(env.id, version_id)
-        if agents is not None:
-            required = set(agents)
-            present = set(allagents)
-            allagents = list(required.intersection(present))
-            notfound = required - present
-            if notfound:
-                warnings.append(
-                    "Model version %d does not contain agents named [%s]" % (version_id, ",".join(sorted(list(notfound))))
+                resource_action = data.ResourceAction(
+                    environment=env.id,
+                    version=resource_id.version,
+                    resource_version_ids=[resource_id_str],
+                    action_id=action_id,
+                    action=const.ResourceAction.deploy,
+                    started=datetime.datetime.now().astimezone(),
+                    messages=[
+                        data.LogLine.log(
+                            logging.INFO,
+                            "Resource deploy started on agent %(agent)s, setting status to deploying",
+                            agent=resource_id.agent_name,
+                        )
+                    ],
+                    status=const.ResourceState.deploying,
                 )
+                try:
+                    await resource_action.insert(connection=connection)
+                except UniqueViolationError:
+                    raise Conflict(message=f"A resource action with id {action_id} already exists.")
 
-        if not allagents:
-            return attach_warnings(404, {"message": "No agent could be reached"}, warnings)
+                await resource.update_fields(connection=connection, status=const.ResourceState.deploying)
 
-        present = set()
-        absent = set()
+            self.clear_env_cache(env)
 
-        await self.autostarted_agent_manager._ensure_agents(env, allagents)
+            return await data.Resource.get_last_non_deploying_state_for_dependencies(
+                environment=env.id, resource_version_id=resource_id, connection=connection
+            )
 
-        for agent in allagents:
-            client = self.agentmanager_service.get_agent_client(env.id, agent)
-            if client is not None:
-                incremental_deploy = agent_trigger_method is const.AgentTriggerMethod.push_incremental_deploy
-                self.add_background_task(client.trigger(env.id, agent, incremental_deploy))
-                present.add(agent)
-            else:
-                absent.add(agent)
+    @handle(methods_v2.get_resource_actions, env="tid")
+    async def get_resource_actions(
+        self,
+        env: data.Environment,
+        resource_type: Optional[str] = None,
+        agent: Optional[str] = None,
+        attribute: Optional[str] = None,
+        attribute_value: Optional[str] = None,
+        log_severity: Optional[str] = None,
+        limit: Optional[int] = 0,
+        action_id: Optional[uuid.UUID] = None,
+        first_timestamp: Optional[datetime.datetime] = None,
+        last_timestamp: Optional[datetime.datetime] = None,
+    ) -> ReturnValue[List[ResourceAction]]:
+        if (attribute and not attribute_value) or (not attribute and attribute_value):
+            raise BadRequest(
+                f"Attribute and attribute_value should both be supplied to use them filtering. "
+                f"Received attribute: {attribute}, attribute_value: {attribute_value}"
+            )
+        if first_timestamp and last_timestamp:
+            raise BadRequest(
+                f"Only one of the parameters first_timestamp and last_timestamp should be used "
+                f"Received first_timestamp: {first_timestamp}, last_timestamp: {last_timestamp}"
+            )
+        if action_id and not (first_timestamp or last_timestamp):
+            raise BadRequest(
+                f"The action_id parameter should be used in combination with either the first_timestamp or the last_timestamp "
+                f"Received action_id: {action_id}, first_timestamp: {first_timestamp}, last_timestamp: {last_timestamp}"
+            )
+
+        if limit is None:
+            limit = APILIMIT
+        elif limit > APILIMIT:
+            raise BadRequest(f"limit parameter can not exceed {APILIMIT}, got {limit}.")
 
-        if absent:
-            warnings.append("Could not reach agents named [%s]" % ",".join(sorted(list(absent))))
+        resource_actions = await data.ResourceAction.query_resource_actions(
+            env.id,
+            resource_type,
+            agent,
+            attribute=attribute,
+            attribute_value=attribute_value,
+            log_severity=log_severity,
+            limit=limit,
+            action_id=action_id,
+            first_timestamp=first_timestamp,
+            last_timestamp=last_timestamp,
+        )
+        resource_action_dtos = [resource_action.to_dto() for resource_action in resource_actions]
+        links = {}
 
-        if not present:
-            return attach_warnings(404, {"message": "No agent could be reached"}, warnings)
+        def _get_query_params(
+            resource_type: Optional[str] = None,
+            agent: Optional[str] = None,
+            attribute: Optional[str] = None,
+            attribute_value: Optional[str] = None,
+            log_severity: Optional[str] = None,
+            limit: Optional[int] = 0,
+        ) -> dict:
+            query_params = {
+                "resource_type": resource_type,
+                "agent": agent,
+                "attribute": attribute,
+                "attribute_value": attribute_value,
+                "log_severity": log_severity,
+                "limit": limit,
+            }
+            query_params = {param_key: param_value for param_key, param_value in query_params.items() if param_value}
+            return query_params
+
+        if limit and resource_action_dtos:
+            base_url = "/api/v2/resource_actions"
+            common_query_params = _get_query_params(resource_type, agent, attribute, attribute_value, log_severity, limit)
+            # Next is always earlier with regards to 'started' time
+            next_params = common_query_params.copy()
+            next_params["last_timestamp"] = resource_action_dtos[-1].started
+            next_params["action_id"] = resource_action_dtos[-1].action_id
+            links["next"] = url_concat(base_url, next_params)
+            previous_params = common_query_params.copy()
+            previous_params["first_timestamp"] = resource_action_dtos[0].started
+            previous_params["action_id"] = resource_action_dtos[0].action_id
+            links["prev"] = url_concat(base_url, previous_params)
+        return_value = ReturnValue(response=resource_action_dtos, links=links if links else None)
+        return return_value
 
-        return attach_warnings(200, {"agents": sorted(list(present))}, warnings)
+    @handle(methods_v2.get_resource_events, env="tid", resource_id="rvid")
+    async def get_resource_events(
+        self,
+        env: data.Environment,
+        resource_id: Id,
+    ) -> Dict[ResourceIdStr, List[ResourceAction]]:
+        return {
+            k: [ra.to_dto() for ra in v] for k, v in (await data.ResourceAction.get_resource_events(env, resource_id)).items()
+        }
+
+    @handle(methods_v2.resource_did_dependency_change, env="tid", resource_id="rvid")
+    async def resource_did_dependency_change(
+        self,
+        env: data.Environment,
+        resource_id: Id,
+    ) -> bool:
+        # This resource has been deployed before => determine whether it should be redeployed based on events
+        return any(
+            True
+            for dependency, actions in (
+                await data.ResourceAction.get_resource_events(env, resource_id, const.Change.nochange)
+            ).items()
+            for action in actions
+        )
 
-    @handle(methods_v2.list_desired_state_versions, env="tid")
-    async def desired_state_version_list(
+    @handle(methods_v2.resource_list, env="tid")
+    async def resource_list(
         self,
         env: data.Environment,
         limit: Optional[int] = None,
-        start: Optional[int] = None,
-        end: Optional[int] = None,
+        first_id: Optional[ResourceVersionIdStr] = None,
+        last_id: Optional[ResourceVersionIdStr] = None,
+        start: Optional[str] = None,
+        end: Optional[str] = None,
         filter: Optional[Dict[str, List[str]]] = None,
-        sort: str = "version.desc",
-    ) -> ReturnValue[List[DesiredStateVersion]]:
+        sort: str = "resource_type.desc",
+        deploy_summary: bool = False,
+    ) -> ReturnValueWithMeta[Sequence[LatestReleasedResource]]:
         try:
-            return await DesiredStateVersionView(
+            handler = ResourceView(env, limit, first_id, last_id, start, end, filter, sort, deploy_summary)
+
+            out = await handler.execute()
+            if deploy_summary:
+                out.metadata["deploy_summary"] = await data.Resource.get_resource_deploy_summary(env.id)
+            return out
+
+        except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
+            raise BadRequest(e.message) from e
+
+        # TODO: optimize for no orphans
+
+    @handle(methods_v2.resource_details, env="tid")
+    async def resource_details(self, env: data.Environment, rid: ResourceIdStr) -> ReleasedResourceDetails:
+        details = await data.Resource.get_resource_details(env.id, rid)
+        if not details:
+            raise NotFound("The resource with the given id does not exist, or was not released yet in the given environment.")
+        return details
+
+    @handle(methods_v2.resource_history, env="tid")
+    async def resource_history(
+        self,
+        env: data.Environment,
+        rid: ResourceIdStr,
+        limit: Optional[int] = None,
+        first_id: Optional[str] = None,
+        last_id: Optional[str] = None,
+        start: Optional[datetime.datetime] = None,
+        end: Optional[datetime.datetime] = None,
+        sort: str = "date.desc",
+    ) -> ReturnValue[Sequence[ResourceHistory]]:
+        try:
+            handler = ResourceHistoryView(
                 environment=env,
+                rid=rid,
                 limit=limit,
-                filter=filter,
                 sort=sort,
+                first_id=first_id,
+                last_id=last_id,
                 start=start,
                 end=end,
-            ).execute()
+            )
+            out = await handler.execute()
+            return out
         except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
             raise BadRequest(e.message) from e
 
-    @handle(methods_v2.promote_desired_state_version, env="tid")
-    async def promote_desired_state_version(
+    @handle(methods_v2.resource_logs, env="tid")
+    async def resource_logs(
         self,
         env: data.Environment,
-        version: int,
-        trigger_method: Optional[PromoteTriggerMethod] = None,
-    ) -> None:
-        if trigger_method == PromoteTriggerMethod.push_incremental_deploy:
-            push = True
-            agent_trigger_method = const.AgentTriggerMethod.push_incremental_deploy
-        elif trigger_method == PromoteTriggerMethod.push_full_deploy:
-            push = True
-            agent_trigger_method = const.AgentTriggerMethod.push_full_deploy
-        elif trigger_method == PromoteTriggerMethod.no_push:
-            push = False
-            agent_trigger_method = None
-        else:
-            push = True
-            agent_trigger_method = None
-
-        status_code, result = await self.release_version(
-            env, version_id=version, push=push, agent_trigger_method=agent_trigger_method
-        )
-        if status_code != 200:
-            raise BaseHttpException(status_code, result["message"])
+        rid: ResourceIdStr,
+        limit: Optional[int] = None,
+        start: Optional[datetime.datetime] = None,
+        end: Optional[datetime.datetime] = None,
+        filter: Optional[Dict[str, List[str]]] = None,
+        sort: str = "timestamp.desc",
+    ) -> ReturnValue[Sequence[ResourceLog]]:
+        try:
+            handler = ResourceLogsView(environment=env, rid=rid, limit=limit, sort=sort, start=start, end=end, filter=filter)
+            out = await handler.execute()
+            return out
+        except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
+            raise BadRequest(e.message) from e
 
-    @handle(methods_v2.get_diff_of_versions, env="tid")
-    async def get_diff_of_versions(
+    @handle(methods_v2.get_resources_in_version, env="tid")
+    async def get_resources_in_version(
         self,
         env: data.Environment,
-        from_version: int,
-        to_version: int,
-    ) -> List[ResourceDiff]:
-        await self._validate_version_parameters(env.id, from_version, to_version)
-
-        from_version_resources = await data.Resource.get_list(environment=env.id, model=from_version)
-        to_version_resources = await data.Resource.get_list(environment=env.id, model=to_version)
-
-        from_state = diff.Version(self.convert_resources(from_version_resources))
-        to_state = diff.Version(self.convert_resources(to_version_resources))
-
-        version_diff = to_state.generate_diff(from_state)
-
-        return version_diff
-
-    def convert_resources(self, resources: List[data.Resource]) -> Dict[ResourceIdStr, diff.Resource]:
-        return {res.resource_id: diff.Resource(resource_id=res.resource_id, attributes=res.attributes) for res in resources}
-
-    async def _validate_version_parameters(self, env: uuid.UUID, first_version: int, other_version: int) -> None:
-        if first_version >= other_version:
-            raise BadRequest(
-                f"Invalid version parameters: ({first_version}, {other_version}). "
-                "The second version number should be strictly greater than the first"
-            )
-        await self._check_version_exists(env, first_version)
-        await self._check_version_exists(env, other_version)
+        version: int,
+        limit: Optional[int] = None,
+        first_id: Optional[ResourceVersionIdStr] = None,
+        last_id: Optional[ResourceVersionIdStr] = None,
+        start: Optional[str] = None,
+        end: Optional[str] = None,
+        filter: Optional[Dict[str, List[str]]] = None,
+        sort: str = "resource_type.desc",
+    ) -> ReturnValueWithMeta[Sequence[VersionedResource]]:
+        try:
+            handler = ResourcesInVersionView(env, version, limit, filter, sort, first_id, last_id, start, end)
+            return await handler.execute()
+        except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
+            raise BadRequest(e.message) from e
 
-    async def _check_version_exists(self, env: uuid.UUID, version: int) -> None:
-        version_object = await data.ConfigurationModel.get_version(env, version)
-        if not version_object:
-            raise NotFound(f"Version {version} not found")
+    @handle(methods_v2.versioned_resource_details, env="tid")
+    async def versioned_resource_details(
+        self, env: data.Environment, version: int, rid: ResourceIdStr
+    ) -> VersionedResourceDetails:
+        resource = await data.Resource.get_versioned_resource_details(environment=env.id, version=version, resource_id=rid)
+        if not resource:
+            raise NotFound("The resource with the given id does not exist")
+        return resource
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/paramservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/paramservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,29 +59,29 @@
 
     async def prestart(self, server: protocol.Server) -> None:
         await super().prestart(server)
         self.server_slice = cast(Server, server.get_slice(SLICE_SERVER))
         self.agentmanager = cast(AgentManager, server.get_slice(SLICE_AGENT_MANAGER))
 
     async def start(self) -> None:
-        self.schedule(self.renew_expired_facts, self._fact_renew, cancel_on_stop=False)
+        self.schedule(self.renew_facts, self._fact_renew, cancel_on_stop=False)
         await super().start()
 
-    async def renew_expired_facts(self) -> None:
+    async def renew_facts(self) -> None:
         """
-        Send out requests to renew expired facts
+        Send out requests to renew facts.
         """
-        LOGGER.info("Renewing expired parameters")
+        LOGGER.info("Renewing parameters")
 
-        updated_before = datetime.datetime.now().astimezone() - datetime.timedelta(0, (self._fact_expire - self._fact_renew))
-        expired_params = await data.Parameter.get_updated_before(updated_before)
+        updated_before = datetime.datetime.now().astimezone() - datetime.timedelta(0, self._fact_renew)
+        params_to_renew = await data.Parameter.get_updated_before(updated_before)
 
-        LOGGER.debug("Renewing %d expired parameters" % len(expired_params))
+        LOGGER.debug("Renewing %d parameters", len(params_to_renew))
 
-        for param in expired_params:
+        for param in params_to_renew:
             if param.environment is None:
                 LOGGER.warning(
                     "Found parameter without environment (%s for resource %s). Deleting it.", param.name, param.resource_id
                 )
                 await param.delete()
             else:
                 LOGGER.debug(
@@ -99,15 +99,15 @@
                     "Found unknown parameter without environment (%s for resource %s). Deleting it.", u.name, u.resource_id
                 )
                 await u.delete()
             else:
                 LOGGER.debug("Requesting value for unknown parameter %s of resource %s in env %s", u.name, u.resource_id, u.id)
                 await self.agentmanager.request_parameter(u.environment, u.resource_id)
 
-        LOGGER.info("Done renewing expired parameters")
+        LOGGER.info("Done renewing parameters")
 
     @handle(methods.get_param, param_id="id", env="tid")
     async def get_param(self, env: data.Environment, param_id: str, resource_id: Optional[str] = None) -> Apireturn:
         if resource_id is None:
             params = await data.Parameter.get_list(environment=env.id, name=param_id)
         else:
             params = await data.Parameter.get_list(environment=env.id, name=param_id, resource_id=resource_id)
@@ -276,15 +276,15 @@
                 # Return datetime in UTC without explicit timezone offset
                 "now": util.datetime_utc_isoformat(datetime.datetime.now()),
             },
         )
 
     @handle(methods_v2.get_facts, env="tid")
     async def get_facts(self, env: data.Environment, rid: ResourceIdStr) -> List[Fact]:
-        params = await data.Parameter.get_list(environment=env.id, resource_id=rid)
+        params = await data.Parameter.get_list(environment=env.id, resource_id=rid, order_by_column="name")
         dtos = [param.as_fact() for param in params]
         return dtos
 
     @handle(methods_v2.get_fact, env="tid")
     async def get_fact(self, env: data.Environment, rid: ResourceIdStr, id: uuid.UUID) -> Fact:
         param = await data.Parameter.get_one(environment=env.id, resource_id=rid, id=id)
         if not param:
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/projectservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/projectservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,18 +129,21 @@
         except asyncpg.exceptions.UniqueViolationError:
             raise ServerError(f"A project with name {name} already exists.")
 
     @handle(methods_v2.project_list)
     async def project_list(self, environment_details: bool = False) -> List[model.Project]:
         project_list = []
 
-        for project in await data.Project.get_list():
+        for project in await data.Project.get_list(order_by_column="name", order="ASC"):
             project_model = project.to_dto()
             project_model.environments = [
-                e.to_dto() for e in await data.Environment.get_list(project=project.id, details=environment_details)
+                e.to_dto()
+                for e in await data.Environment.get_list(
+                    project=project.id, details=environment_details, order_by_column="name", order="ASC"
+                )
             ]
 
             project_list.append(project_model)
 
         return project_list
 
     @handle(methods_v2.project_get, project_id="id")
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/services/resourceservice.py` & `inmanta-core-8.3.0/src/inmanta/server/services/orchestrationservice.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    Copyright 2019 Inmanta
+    Copyright 2023 Inmanta
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         http://www.apache.org/licenses/LICENSE-2.0
 
@@ -11,989 +11,1326 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
-import asyncio
 import datetime
 import logging
-import os
 import uuid
 from collections import abc, defaultdict
-from typing import Any, Dict, List, Optional, Sequence, Union, cast
+from typing import Dict, List, Literal, Optional, Set, cast
 
-from asyncpg.connection import Connection
-from asyncpg.exceptions import UniqueViolationError
-from tornado.httputil import url_concat
-
-from inmanta import const, data, util
-from inmanta.const import STATE_UPDATE, TERMINAL_STATES, TRANSIENT_STATES, VALID_STATES_ON_STATE_UPDATE, Change, ResourceState
-from inmanta.data import APILIMIT, InvalidSort
-from inmanta.data.dataview import ResourceHistoryView, ResourceLogsView, ResourcesInVersionView, ResourceView
+import asyncpg
+import asyncpg.connection
+import asyncpg.exceptions
+import pydantic
+
+from inmanta import const, data
+from inmanta.const import ResourceState
+from inmanta.data import APILIMIT, AVAILABLE_VERSIONS_TO_KEEP, ENVIRONMENT_AGENT_TRIGGER_METHOD, PURGE_ON_DELETE, InvalidSort
+from inmanta.data.dataview import DesiredStateVersionView
 from inmanta.data.model import (
-    AttributeStateChange,
-    LatestReleasedResource,
-    LogLine,
-    ReleasedResourceDetails,
-    Resource,
-    ResourceAction,
-    ResourceHistory,
+    DesiredStateVersion,
+    PromoteTriggerMethod,
+    ResourceDiff,
     ResourceIdStr,
-    ResourceLog,
-    ResourceType,
+    ResourceMinimal,
     ResourceVersionIdStr,
-    VersionedResource,
-    VersionedResourceDetails,
 )
 from inmanta.protocol import handle, methods, methods_v2
-from inmanta.protocol.common import ReturnValue
-from inmanta.protocol.exceptions import BadRequest, Conflict, NotFound
-from inmanta.protocol.return_value_meta import ReturnValueWithMeta
+from inmanta.protocol.common import ReturnValue, attach_warnings
+from inmanta.protocol.exceptions import BadRequest, BaseHttpException, NotFound, ServerError
 from inmanta.resources import Id
-from inmanta.server import SLICE_AGENT_MANAGER, SLICE_DATABASE, SLICE_RESOURCE, SLICE_TRANSPORT
+from inmanta.server import (
+    SLICE_AGENT_MANAGER,
+    SLICE_AUTOSTARTED_AGENT_MANAGER,
+    SLICE_DATABASE,
+    SLICE_ORCHESTRATION,
+    SLICE_RESOURCE,
+    SLICE_TRANSPORT,
+)
 from inmanta.server import config as opt
-from inmanta.server import protocol
-from inmanta.server.agentmanager import AgentManager
+from inmanta.server import diff, protocol
+from inmanta.server.agentmanager import AgentManager, AutostartedAgentManager
+from inmanta.server.services.resourceservice import ResourceService
 from inmanta.server.validate_filter import InvalidFilter
-from inmanta.types import Apireturn, PrimitiveTypes
+from inmanta.types import Apireturn, JsonType, PrimitiveTypes
 
 LOGGER = logging.getLogger(__name__)
 
+PERFORM_CLEANUP: bool = True
+# Kill switch for cleanup, for use when working with historical data
+
+
+class CrossResourceSetDependencyError(Exception):
+    def __init__(self, resource_id1: ResourceIdStr, resource_id2: ResourceIdStr) -> None:
+        """
+        Raised when a cross-resource set dependency was detected between the resource with id
+        resource_id1 and resource_id2.
+        """
+        self.resource_id1 = resource_id1
+        self.resource_id2 = resource_id2
+        super().__init__(self.get_error_message())
+
+    def get_error_message(self) -> str:
+        return (
+            f"A dependency exists between resources {self.resource_id1} and {self.resource_id2}, but they belong to"
+            f" different resource sets."
+        )
+
+
+class ResourceSetValidator:
+    def __init__(self, resources: abc.Set[data.Resource]) -> None:
+        self.resources = resources
+        self.rid_to_resource_set = {res.resource_id: res.resource_set for res in self.resources}
+
+    def _is_cross_resource_set_dependency(self, res: data.Resource, rid_dependency: ResourceIdStr) -> bool:
+        """
+        Return True iff the dependency between resource res and the resource with id rid_dependency is a cross-resource set
+        dependency.
+        """
+        if res.resource_set is None:
+            # Resource is in shared resource set.
+            return False
+        if rid_dependency not in self.rid_to_resource_set:
+            # A partial compile was done and we have a dependency on a resource in another resource set
+            # that is not part of the partial compile.
+            return True
+        resource_set_dep = self.rid_to_resource_set[rid_dependency]
+        if resource_set_dep is None:
+            # Dependency towards shared resource set.
+            return False
+        return res.resource_set != resource_set_dep
+
+    def ensure_no_cross_resource_set_dependencies(self) -> None:
+        """
+        This method raises a CrossResourceSetDependencyError when a resource in self.resources that belongs to a non-shared
+        resource set has a dependency (requires/provides) on another resource that belongs to a different non-shared resource
+        set.
+        """
+        for res in self.resources:
+            # It's sufficient to only check the requires relationship. The provides
+            # relationship is always a subset of the reverse relationship (provides relationship).
+            # The provides relationship only contains the cross-agent dependencies.
+            for req in res.get_requires():
+                if self._is_cross_resource_set_dependency(res, req):
+                    raise CrossResourceSetDependencyError(res.resource_id, req)
+
+    def has_cross_resource_set_dependency(self) -> bool:
+        """
+        Return True iff a cross resource set dependency exists between the resources in self.resources.
+        """
+        try:
+            self.ensure_no_cross_resource_set_dependencies()
+        except CrossResourceSetDependencyError:
+            return True
+        else:
+            return False
+
 
-def error_and_log(message: str, **context: Any) -> None:
+class PartialUpdateMerger:
     """
-    :param message: message to return both to logger and to remote caller
-    :param context: additional context to attach to log
+    Class that contains the functionality to merge the shared resources and resources, present in a resource set that is updated
+    by the partial compile, together with the resources from the corresponding resources sets in the old version of the model.
     """
-    ctx = ",".join([f"{k}: {v}" for k, v in context.items()])
-    LOGGER.error("%s %s", message, ctx)
-    raise BadRequest(message)
-
-
-class ResourceActionLogLine(logging.LogRecord):
-    """A special log record that is used to report log lines that come from the agent"""
-
-    def __init__(self, logger_name: str, level: int, msg: str, created: datetime.datetime) -> None:
-        super().__init__(
-            name=logger_name,
-            level=level,
-            pathname="(unknown file)",
-            lineno=0,
-            msg=msg,
-            args=[],
-            exc_info=None,
-            func=None,
-            sinfo=None,
+
+    def __init__(
+        self,
+        env_id: uuid.UUID,
+        base_version: int,
+        version: int,
+        rids_in_partial_compile: abc.Set[ResourceIdStr],
+        updated_resource_sets: abc.Set[str],
+        deleted_resource_sets: abc.Set[str],
+        updated_and_shared_resources_old: abc.Mapping[ResourceIdStr, data.Resource],
+        rids_deleted_resource_sets: abc.Set[ResourceIdStr],
+    ) -> None:
+        """
+        :param env_id: The id of the environment for which a partial compile is being done.
+        :param base_version: The source version on which the partial compile in based.
+        :param version: The version of the new configuration model created by this partial compile.
+        :param rids_in_partial_compile: The ids of the resource that are part of the partial compile.
+        :param updated_resource_sets: The names of the resource sets that are updated by the partial compile.
+        :param deleted_resource_sets: The names of the resource sets that are deleted by the partial compile.
+        :param updated_and_shared_resources_old: A dictionary that contains all the resources in base_version that belong
+                                                 to a resource set in updated_resource_sets or to the shared resource set.
+        :param rids_deleted_resource_sets: The ids of the resources that are in the base_version and that are deleted by this
+                                           partial compile.
+        """
+        self.env_id = env_id
+        self.base_version = base_version
+        self.version = version
+        self.rids_in_partial_compile = rids_in_partial_compile
+        self.updated_resource_sets = updated_resource_sets
+        self.deleted_resource_sets = deleted_resource_sets
+        self.updated_and_shared_resources_old = updated_and_shared_resources_old
+        self.non_shared_resources_in_partial_update_old: abc.Mapping[ResourceIdStr, data.Resource] = {
+            rid: r for rid, r in self.updated_and_shared_resources_old.items() if r.resource_set is not None
+        }
+        self.shared_resources_old: abc.Mapping[ResourceIdStr, data.Resource] = {
+            rid: r for rid, r in self.updated_and_shared_resources_old.items() if r.resource_set is None
+        }
+        self.rids_deleted_resource_sets = rids_deleted_resource_sets
+
+    @classmethod
+    async def create(
+        cls,
+        env_id: uuid.UUID,
+        base_version: int,
+        version: int,
+        rids_in_partial_compile: abc.Set[ResourceIdStr],
+        updated_resource_sets: abc.Set[str],
+        deleted_resource_sets: abc.Set[str],
+        connection: Optional[asyncpg.connection.Connection] = None,
+    ) -> "PartialUpdateMerger":
+        """
+        A replacement constructor method for this class. This method is used to work around the limitation that no async
+        calls can be done in a constructor. See docstring real constructor for meaning of arguments.
+        """
+        updated_and_shared_resources_old: abc.Mapping[
+            ResourceIdStr, data.Resource
+        ] = await data.Resource.get_resources_in_resource_sets(
+            environment=env_id,
+            version=base_version,
+            resource_sets=updated_resource_sets,
+            include_shared_resources=True,
+            connection=connection,
+        )
+        rids_deleted_resource_sets: abc.Set[ResourceIdStr] = set(
+            rid
+            for rid in (
+                await data.Resource.get_resources_in_resource_sets(
+                    environment=env_id,
+                    version=base_version,
+                    resource_sets=deleted_resource_sets,
+                    connection=connection,
+                )
+            ).keys()
         )
+        return PartialUpdateMerger(
+            env_id,
+            base_version,
+            version,
+            rids_in_partial_compile,
+            updated_resource_sets,
+            deleted_resource_sets,
+            updated_and_shared_resources_old,
+            rids_deleted_resource_sets,
+        )
+
+    def merge_updated_and_shared_resources(
+        self, updated_and_shared_resources: abc.Sequence[data.Resource]
+    ) -> Dict[ResourceIdStr, data.Resource]:
+        """
+         Separates named resource sets from the shared resource set and expands the shared set with the shared resources in
+         the previous model version.
+
+        :param updated_and_shared_resources: The resources that are part of the partial compile.
+        :returns: The subset of resources in the new version of the configuration model that belong to the shared resource set
+                  or a resource set that is updated by this partial compile.
+        """
+        shared_resources = {r.resource_id: r for r in updated_and_shared_resources if r.resource_set is None}
+        updated_resources = {r.resource_id: r for r in updated_and_shared_resources if r.resource_set is not None}
+        shared_resources_merged = {r.resource_id: r for r in self._merge_shared_resources(shared_resources)}
+        result = {**updated_resources, **shared_resources_merged}
+        self._validate_constraints(result)
+        return result
+
+    def _validate_constraints(self, new_updated_and_shared_resources: abc.Mapping[ResourceIdStr, data.Resource]) -> None:
+        """
+        Validate whether the new updated and shared resources that results from the merging the old version of the model
+        with resources of the partial compile, are compliant with the constraints of a partial compile.
+
+        :param new_updated_and_shared_resources: The resources that have to be validated.
+        """
+        for res_id, res in new_updated_and_shared_resources.items():
+            if res.resource_id not in self.updated_and_shared_resources_old:
+                continue
+            matching_resource_old_model = self.updated_and_shared_resources_old[res.resource_id]
+
+            if res.resource_set != matching_resource_old_model.resource_set:
+                raise BadRequest(
+                    f"A partial compile cannot migrate resources: trying to move {res.resource_id} from resource set"
+                    f" {matching_resource_old_model.resource_set} to {res.resource_set}."
+                )
+
+            if res.resource_set is None and res.attribute_hash != matching_resource_old_model.attribute_hash:
+                raise BadRequest(f"Resource ({res.resource_id}) without a resource set cannot be updated via a partial compile")
+
+            resource_set_validator = ResourceSetValidator(set(new_updated_and_shared_resources.values()))
+            try:
+                resource_set_validator.ensure_no_cross_resource_set_dependencies()
+            except CrossResourceSetDependencyError as e:
+                raise BadRequest(e.get_error_message())
+
+    def _merge_shared_resources(self, shared_resources_new: Dict[ResourceIdStr, data.Resource]) -> abc.Sequence[data.Resource]:
+        """
+        Merge the set of shared resources present in the old version of the model together with the set of shared resources
+        present in the partial compile.
+
+        :param shared_resources_new: The set of shared resources present in the partial compile.
+        :returns: The set of shared resources that should be present in the new version of the model.
+        """
+        all_rids_shared_resources = set(self.shared_resources_old.keys()) | set(shared_resources_new.keys())
+        result = []
+        for rid_shared_resource in all_rids_shared_resources:
+            if rid_shared_resource in shared_resources_new and rid_shared_resource in self.shared_resources_old:
+                # Merge requires/provides shared resource
+                old_shared_resource = self.shared_resources_old[rid_shared_resource]
+                new_shared_resource = shared_resources_new[rid_shared_resource]
+                res = self._merge_requires_and_provides_of_shared_resource(old_shared_resource, new_shared_resource)
+            elif rid_shared_resource in shared_resources_new:
+                # New shared resource in partial compile
+                res = shared_resources_new[rid_shared_resource]
+            else:
+                # Old shared resource not referenced by partial compile
+                res_old = self.shared_resources_old[rid_shared_resource]
+                res = res_old.copy_for_partial_compile(new_version=self.version)
+                res = self._clean_requires_provides_old_shared_resource(res)
+            result.append(res)
+        return result
+
+    def _should_keep_dependency_old_shared_resources(self, rid_dependency: ResourceIdStr) -> bool:
+        """
+        Return True iff the given dependency present in a shared resource from the base version should be retained
+        in the new version of the model.
+        """
+        if rid_dependency in self.rids_deleted_resource_sets:
+            # Resource belongs to a deleted resource set
+            return False
+        if rid_dependency in self.non_shared_resources_in_partial_update_old:
+            # If this dependency is still present in the new version of the model, this dependency
+            # will be present in the resources that are part of the partial compile.
+            return False
+        return True
+
+    def _clean_requires_provides_old_shared_resource(self, resource: data.Resource) -> data.Resource:
+        """
+        Cleanup the requires/provides relationship for shared resources that are not present in the partial compile
+        and that were copied from the old version of the model.
+        """
+        resource.attributes["requires"] = [
+            rid for rid in resource.attributes["requires"] if self._should_keep_dependency_old_shared_resources(rid)
+        ]
+        resource.provides = [rid for rid in resource.provides if self._should_keep_dependency_old_shared_resources(rid)]
+        return resource
+
+    def _merge_requires_and_provides_of_shared_resource(self, old: data.Resource, new: data.Resource) -> data.Resource:
+        """
+        Update the requires and provides relationship of `new` to make it consistent with the new version of the model.
+
+        :param old: The shared resource present in the old version of the model.
+        :param new: The shared resource part of the incremental compile.
+        """
+        new.provides = list(self._merge_dependencies_shared_resource(old.provides, new.provides))
+        new.attributes["requires"] = self._merge_dependencies_shared_resource(old.get_requires(), new.get_requires())
+        return new
+
+    def _merge_dependencies_shared_resource(
+        self, old_deps: abc.Sequence[ResourceIdStr], new_deps: abc.Sequence[ResourceIdStr]
+    ) -> abc.Sequence[ResourceIdStr]:
+        """
+        Merge the dependencies for a certain shared resource together to make it consistent with the new version of the model.
+
+        :param old_deps: The set of dependencies present in the old version of the shared resource.
+        :param new_deps: The set of dependencies present in the shared resource that is part of the partial compile.
+        """
+        old_deps_cleaned: abc.Set[ResourceIdStr] = {
+            dep for dep in old_deps if self._should_keep_dependency_old_shared_resources(dep)
+        }
+        return list(old_deps_cleaned | set(new_deps))
 
-        self.created = created.timestamp()
-        self.msecs = (self.created - int(self.created)) * 1000
-        self.relativeCreated = (self.created - logging._startTime) * 1000
+    async def merge_unknowns(
+        self, unknowns_in_partial_compile: abc.Sequence[data.UnknownParameter]
+    ) -> abc.Sequence[data.UnknownParameter]:
+        """
+        Merge all relevant, unresolved unknowns from the old version of the model together with the unknowns
+        of the partial compile.
+        """
+        old_unresolved_unknowns_to_keep = [
+            uk.copy(self.version)
+            for uk in await data.UnknownParameter.get_unknowns_to_copy_in_partial_compile(
+                environment=self.env_id,
+                source_version=self.base_version,
+                updated_resource_sets=self.updated_resource_sets,
+                deleted_resource_sets=self.deleted_resource_sets,
+                rids_in_partial_compile=self.rids_in_partial_compile,
+            )
+        ]
+        return [*old_unresolved_unknowns_to_keep, *unknowns_in_partial_compile]
 
 
-class ResourceService(protocol.ServerSlice):
+class OrchestrationService(protocol.ServerSlice):
     """Resource Manager service"""
 
     agentmanager_service: "AgentManager"
+    autostarted_agent_manager: AutostartedAgentManager
+    resource_service: ResourceService
 
     def __init__(self) -> None:
-        super(ResourceService, self).__init__(SLICE_RESOURCE)
-
-        self._resource_action_loggers: Dict[uuid.UUID, logging.Logger] = {}
-        self._resource_action_handlers: Dict[uuid.UUID, logging.Handler] = {}
-
-        self._increment_cache: Dict[uuid.UUID, Optional[tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]]]] = {}
-        # lock to ensure only one inflight request
-        self._increment_cache_locks: Dict[uuid.UUID, asyncio.Lock] = defaultdict(lambda: asyncio.Lock())
+        super(OrchestrationService, self).__init__(SLICE_ORCHESTRATION)
 
     def get_dependencies(self) -> List[str]:
-        return [SLICE_DATABASE, SLICE_AGENT_MANAGER]
+        return [SLICE_RESOURCE, SLICE_AGENT_MANAGER, SLICE_DATABASE]
 
     def get_depended_by(self) -> List[str]:
         return [SLICE_TRANSPORT]
 
     async def prestart(self, server: protocol.Server) -> None:
         await super().prestart(server)
         self.agentmanager_service = cast("AgentManager", server.get_slice(SLICE_AGENT_MANAGER))
+        self.autostarted_agent_manager = cast(AutostartedAgentManager, server.get_slice(SLICE_AUTOSTARTED_AGENT_MANAGER))
+        self.resource_service = cast(ResourceService, server.get_slice(SLICE_RESOURCE))
 
     async def start(self) -> None:
-        self.schedule(
-            data.ResourceAction.purge_logs, opt.server_purge_resource_action_logs_interval.get(), cancel_on_stop=False
-        )
+        if PERFORM_CLEANUP:
+            self.schedule(self._purge_versions, opt.server_purge_version_interval.get(), cancel_on_stop=False)
+            self.add_background_task(self._purge_versions())
         await super().start()
 
-    async def stop(self) -> None:
-        await super().stop()
-        self._close_resource_action_loggers()
-
-    def clear_env_cache(self, env: data.Environment) -> None:
-        LOGGER.log(const.LOG_LEVEL_TRACE, "Clearing cache for %s", env.id)
-        self._increment_cache[env.id] = None
-        # ??? del self._increment_cache[env.id]
-
-    @staticmethod
-    def get_resource_action_log_file(environment: uuid.UUID) -> str:
-        """Get the correct filename for the given environment
-        :param environment: The environment id to get the file for
-        :return: The path to the logfile
+    async def _purge_versions(self) -> None:
         """
-        return os.path.join(opt.log_dir.get(), opt.server_resource_action_log_prefix.get() + str(environment) + ".log")
-
-    def get_resource_action_logger(self, environment: uuid.UUID) -> logging.Logger:
-        """Get the resource action logger for the given environment. If the logger was not created, create it.
-        :param environment: The environment to get a logger for
-        :return: The logger for the given environment.
+        Purge versions from the database
         """
-        if environment in self._resource_action_loggers:
-            return self._resource_action_loggers[environment]
-
-        resource_action_log = self.get_resource_action_log_file(environment)
-
-        file_handler = logging.handlers.WatchedFileHandler(filename=resource_action_log, mode="a+")
-        # Most logs will come from agents. We need to use their level and timestamp and their formatted message
-        file_handler.setFormatter(logging.Formatter(fmt="%(asctime)s %(levelname)-8s %(name)-10s %(message)s"))
-        file_handler.setLevel(logging.DEBUG)
-
-        resource_action_logger = logging.getLogger(const.NAME_RESOURCE_ACTION_LOGGER).getChild(str(environment))
-        resource_action_logger.setLevel(logging.DEBUG)
-        resource_action_logger.addHandler(file_handler)
+        # TODO: move to data and use queries for delete
+        envs = await data.Environment.get_list()
+        for env_item in envs:
+            # get available versions
+            n_versions = await env_item.get(AVAILABLE_VERSIONS_TO_KEEP)
+            assert isinstance(n_versions, int)
+            versions = await data.ConfigurationModel.get_list(environment=env_item.id)
+            if len(versions) > n_versions:
+                LOGGER.info("Removing %s available versions from environment %s", len(versions) - n_versions, env_item.id)
+                version_dict = {x.version: x for x in versions}
+                delete_list = sorted(version_dict.keys())
+                delete_list = delete_list[:-n_versions]
+
+                for v in delete_list:
+                    await version_dict[v].delete_cascade()
+
+        # Cleanup old agents from agent table in db
+        await data.Agent.clean_up()
+
+    @handle(methods.list_versions, env="tid")
+    async def list_version(self, env: data.Environment, start: Optional[int] = None, limit: Optional[int] = None) -> Apireturn:
+        if (start is None and limit is not None) or (limit is None and start is not None):
+            raise ServerError("Start and limit should always be set together.")
+
+        if start is None or limit is None:
+            start = 0
+            limit = data.APILIMIT
 
-        self._resource_action_loggers[environment] = resource_action_logger
-        self._resource_action_handlers[environment] = file_handler
+        if limit > APILIMIT:
+            raise BadRequest(f"limit parameter can not exceed {APILIMIT}, got {limit}.")
 
-        return resource_action_logger
+        models = await data.ConfigurationModel.get_versions(env.id, start, limit)
+        count = len(models)
 
-    def _close_resource_action_loggers(self) -> None:
-        """Close all resource action loggers and their associated handlers"""
-        try:
-            while True:
-                env, logger = self._resource_action_loggers.popitem()
-                self.close_resource_action_logger(env, logger)
-        except KeyError:
-            pass
-
-    def close_resource_action_logger(self, env: uuid.UUID, logger: Optional[logging.Logger] = None) -> None:
-        """Close the given logger for the given env.
-        :param env: The environment to close the logger for
-        :param logger: The logger to close, if the logger is none it is retrieved
-        """
-        if logger is None:
-            if env in self._resource_action_loggers:
-                logger = self._resource_action_loggers.pop(env)
-            else:
-                return
+        d = {
+            "versions": models,
+            "start": start,
+            "limit": limit,
+            "count": count,
+        }
 
-        handler = self._resource_action_handlers.pop(env)
-        logger.removeHandler(handler)
-        handler.flush()
-        handler.close()
+        return 200, d
 
-    def log_resource_action(
-        self, env: uuid.UUID, resource_ids: Sequence[str], log_level: int, ts: datetime.datetime, message: str
-    ) -> None:
-        """Write the given log to the correct resource action logger"""
-        logger = self.get_resource_action_logger(env)
-        if len(resource_ids) == 0:
-            message = "no resources: " + message
-        elif len(resource_ids) > 1:
-            message = "multiple resources: " + message
-        else:
-            message = resource_ids[0] + ": " + message
-        log_record = ResourceActionLogLine(logger.name, log_level, message, ts)
-        logger.handle(log_record)
-
-    @handle(methods.get_resource, resource_id="id", env="tid")
-    async def get_resource(
+    @handle(methods.get_version, version_id="id", env="tid")
+    async def get_version(
         self,
         env: data.Environment,
-        resource_id: ResourceVersionIdStr,
-        logs: bool,
-        status: bool,
-        log_action: const.ResourceAction,
-        log_limit: int,
-    ) -> Apireturn:
-        resv = await data.Resource.get(env.id, resource_id)
-        if resv is None:
-            return 404, {"message": "The resource with the given id does not exist in the given environment"}
-
-        if status is not None and status:
-            return 200, {"status": resv.status}
-
-        actions: List[data.ResourceAction] = []
-        if bool(logs):
-            action_name = None
-            if log_action is not None:
-                action_name = log_action.name
-
-            actions = await data.ResourceAction.get_log(
-                environment=env.id, resource_version_id=resource_id, action=action_name, limit=log_limit
-            )
-
-        return 200, {"resource": resv, "logs": actions}
-
-    # This endpoint does't have a method associated yet.
-    # Intended for use by other slices
-    async def get_resources_in_latest_version(
-        self,
-        environment: data.Environment,
-        resource_type: Optional[ResourceType] = None,
-        attributes: Dict[PrimitiveTypes, PrimitiveTypes] = {},
-    ) -> List[Resource]:
-        result = await data.Resource.get_resources_in_latest_version(environment.id, resource_type, attributes)
-        return [r.to_dto() for r in result]
-
-    @handle(methods.get_resources_for_agent, env="tid")
-    async def get_resources_for_agent(
-        self, env: data.Environment, agent: str, version: int, sid: uuid.UUID, incremental_deploy: bool
+        version_id: int,
+        include_logs: Optional[bool] = None,
+        log_filter: Optional[str] = None,
+        limit: Optional[int] = 0,
     ) -> Apireturn:
-        if not self.agentmanager_service.is_primary(env, sid, agent):
-            return 409, {"message": "This agent is not currently the primary for the endpoint %s (sid: %s)" % (agent, sid)}
-        if incremental_deploy:
-            if version is not None:
-                return 500, {"message": "Cannot request increment for a specific version"}
-            result = await self.get_resource_increment_for_agent(env, agent)
-        else:
-            result = await self.get_all_resources_for_agent(env, agent, version)
-        return result
-
-    async def get_all_resources_for_agent(self, env: data.Environment, agent: str, version: int) -> Apireturn:
-        started = datetime.datetime.now().astimezone()
+        version = await data.ConfigurationModel.get_version(env.id, version_id)
         if version is None:
-            version = await data.ConfigurationModel.get_version_nr_latest_version(env.id)
-            if version is None:
-                return 404, {"message": "No version available"}
-
-        else:
-            exists = await data.ConfigurationModel.version_exists(environment=env.id, version=version)
-            if not exists:
-                return 404, {"message": "The given version does not exist"}
-
-        deploy_model = []
-
-        resources = await data.Resource.get_resources_for_version(env.id, version, agent)
-
-        resource_ids = []
-        for rv in resources:
-            deploy_model.append(rv.to_dict())
-            resource_ids.append(rv.resource_version_id)
-
-        # Don't log ResourceActions without resource_version_ids, because
-        # no API call exists to retrieve them.
-        if resource_ids:
-            now = datetime.datetime.now().astimezone()
-            log_line = data.LogLine.log(
-                logging.INFO, "Resource version pulled by client for agent %(agent)s state", agent=agent
-            )
-            self.log_resource_action(env.id, resource_ids, logging.INFO, now, log_line.msg)
-            ra = data.ResourceAction(
-                environment=env.id,
-                version=version,
-                resource_version_ids=resource_ids,
-                action=const.ResourceAction.pull,
-                action_id=uuid.uuid4(),
-                started=started,
-                finished=now,
-                messages=[log_line],
-            )
-            await ra.insert()
+            return 404, {"message": "The given configuration model does not exist yet."}
 
-        return 200, {"environment": env.id, "agent": agent, "version": version, "resources": deploy_model}
+        resources = await data.Resource.get_resources_for_version(env.id, version_id, no_obj=True)
+        if resources is None:
+            return 404, {"message": "The given configuration model does not exist yet."}
 
-    async def get_resource_increment_for_agent(self, env: data.Environment, agent: str) -> Apireturn:
-        started = datetime.datetime.now().astimezone()
+        if limit is None:
+            limit = APILIMIT
+        elif limit > APILIMIT:
+            raise BadRequest(
+                f"limit parameter can not exceed {APILIMIT}, got {limit}."
+                f" To retrieve more entries, use /api/v2/resource_actions"
+            )
 
-        version = await data.ConfigurationModel.get_version_nr_latest_version(env.id)
+        resources_out: List[JsonType] = []
+        d = {"model": version, "resources": resources_out}
+        resource_action_lookup: Dict[ResourceVersionIdStr, List[data.ResourceAction]] = {}
+
+        for res_dict in resources:
+            resources_out.append(res_dict)
+            if bool(include_logs):
+                actions: List[data.ResourceAction] = []
+                res_dict["actions"] = actions
+                resource_action_lookup[res_dict["resource_version_id"]] = actions
+
+        if include_logs:
+            # get all logs, unsorted
+            all_logs = await data.ResourceAction.get_logs_for_version(env.id, version_id, log_filter, limit)
+            for log in all_logs:
+                for resource_version_id in log.resource_version_ids:
+                    resource_action_lookup[resource_version_id].append(log)
+
+        d["unknowns"] = await data.UnknownParameter.get_list(environment=env.id, version=version_id)
+
+        return 200, d
+
+    @handle(methods.delete_version, version_id="id", env="tid")
+    async def delete_version(self, env: data.Environment, version_id: int) -> Apireturn:
+        version = await data.ConfigurationModel.get_version(env.id, version_id)
         if version is None:
-            return 404, {"message": "No version available"}
+            return 404, {"message": "The given configuration model does not exist yet."}
 
-        increment: Optional[tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]]] = self._increment_cache.get(env.id, None)
-        if increment is None:
-            lock = self._increment_cache_locks[env.id]
-            async with lock:
-                increment = self._increment_cache.get(env.id, None)
-                if increment is None:
-                    increment = await data.ConfigurationModel.get_increment(env.id, version)
-                    self._increment_cache[env.id] = increment
+        await version.delete_cascade()
+        return 200
 
-        increment_ids, neg_increment = increment
+    @handle(methods_v2.reserve_version, env="tid")
+    async def reserve_version(self, env: data.Environment) -> int:
+        return await env.get_next_version()
 
-        # set already done to deployed
-        now = datetime.datetime.now().astimezone()
+    def _create_dao_resources_from_api_resources(
+        self,
+        env_id: uuid.UUID,
+        resources: List[JsonType],
+        resource_state: Dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]],
+        resource_sets: Dict[ResourceIdStr, Optional[str]],
+        set_version: Optional[int] = None,
+    ) -> Dict[ResourceIdStr, data.Resource]:
+        """
+        This method converts the resources sent to the put_version or put_partial endpoint to dao Resource objects.
+        The resulting resource objects will have their provides set up correctly for cross agent dependencies
+        and the version field of these resources will be set to set_version if provided.
+
+        An exception will be raised when the one of the following constraints is not satisfied:
+            * A resource present in the resource_sets parameter is not present in the resources dictionary.
+            * The dependency graph of the provided resources is not closed.
+        """
+        rid_to_resource = {}
+        # The content of the requires attribute for all the resources
+        all_requires: set[ResourceIdStr] = set()
+        # list of all resources which have a cross agent dependency, as a tuple, (dependant,requires)
+        cross_agent_dep: list[tuple[data.Resource, Id]] = []
+        for res_dict in resources:
+            # Verify that the version field and the version in the resource version id field match
+            version_part_of_resource_id = Id.parse_id(res_dict["id"]).version
+            if "version" in res_dict and res_dict["version"] != version_part_of_resource_id:
+                raise BadRequest(
+                    f"Invalid resource: The version in the id field ({res_dict['id']}) doesn't match the version in the"
+                    f" version field ({res_dict['version']})."
+                )
+            res_obj = data.Resource.new(env_id, res_dict["id"])
+            # Populate status field
+            if res_obj.resource_id in resource_state:
+                res_obj.status = const.ResourceState[resource_state[res_obj.resource_id]]
+            # Populate resource_set field
+            if res_obj.resource_id in resource_sets:
+                res_obj.resource_set = resource_sets[res_obj.resource_id]
+
+            # Populate attributes field of resources
+            attributes = {}
+            for field, value in res_dict.items():
+                if field not in {"id", "version"}:
+                    attributes[field] = value
+            res_obj.attributes = attributes
+            res_obj.make_hash()
+
+            # Update the version fields
+            if set_version is not None:
+                res_obj.model = set_version
+
+            # find cross agent dependencies
+            agent = res_obj.agent
+            if "requires" not in attributes:
+                LOGGER.warning("Received resource without requires attribute (%s)", res_obj.resource_id)
+            else:
+                # Collect all requires as resource_ids instead of resource version ids
+                cleaned_requires = []
+                for req in attributes["requires"]:
+                    rid = Id.parse_id(req)
+                    all_requires.add(rid.resource_str())
+                    if rid.get_agent_name() != agent:
+                        # it is a CAD
+                        cross_agent_dep.append((res_obj, rid))
+                    cleaned_requires.append(rid.resource_str())
+                attributes["requires"] = cleaned_requires
+
+            rid_to_resource[res_obj.resource_id] = res_obj
+
+        # hook up all CADs
+        for f, t in cross_agent_dep:
+            res_obj = rid_to_resource[t.resource_str()]
+            res_obj.provides.append(f.resource_id)
+
+        rids = set(rid_to_resource.keys())
+
+        # Sanity checks
+        superfluous_ids = set(resource_sets.keys()) - rids
+        if superfluous_ids:
+            raise BadRequest(
+                "The following resource ids provided in the resource_sets parameter are not present "
+                f"in the resources list: {', '.join(superfluous_ids)}"
+            )
+        if not all_requires.issubset(rids):
+            raise BadRequest(
+                "The model should have a dependency graph that is closed and no dangling dependencies:"
+                f" {all_requires - rids}"
+            )
 
-        def on_agent(res: ResourceIdStr) -> bool:
-            idr = Id.parse_id(res)
-            return idr.get_agent_name() == agent
+        return rid_to_resource
 
-        neg_increment_version_ids: list[ResourceVersionIdStr] = [
-            ResourceVersionIdStr(f"{res_id},v={version}") for res_id in neg_increment if on_agent(res_id)
-        ]
+    def _get_skipped_for_undeployable(
+        self, resources: abc.Sequence[data.Resource], undeployable_ids: abc.Sequence[ResourceIdStr]
+    ) -> abc.Sequence[ResourceIdStr]:
+        """
+        Return the resources that are skipped_for_undeployable given the full set of resources and
+        the resource ids of the resources that are undeployable.
 
-        logline = {
-            "level": "INFO",
-            "msg": "Setting deployed due to known good status",
-            "timestamp": util.datetime_utc_isoformat(now),
-            "args": [],
-        }
-        await self.resource_action_update(
-            env,
-            neg_increment_version_ids,
-            action_id=uuid.uuid4(),
-            started=now,
-            finished=now,
-            status=const.ResourceState.deployed,
-            # does this require a different ResourceAction?
-            action=const.ResourceAction.deploy,
-            changes={},
-            messages=[logline],
-            change=const.Change.nochange,
-            send_events=False,
-            keep_increment_cache=True,
-        )
+        :param resources: All resources in the model.
+        :param undeployable_ids: The ids of the resource that are undeployable.
+        """
+        # Build up provides tree
+        provides_tree: Dict[ResourceIdStr, List[ResourceIdStr]] = defaultdict(lambda: [])
+        for r in resources:
+            if "requires" in r.attributes:
+                for req in r.attributes["requires"]:
+                    req_id = Id.parse_id(req)
+                    provides_tree[req_id.resource_str()].append(r.resource_id)
+        # Find skipped for undeployables
+        work = list(undeployable_ids)
+        skippeable: Set[ResourceIdStr] = set()
+        while len(work) > 0:
+            current = work.pop()
+            if current in skippeable:
+                continue
+            skippeable.add(current)
+            work.extend(provides_tree[current])
+        return list(skippeable - set(undeployable_ids))
 
-        resources = await data.Resource.get_resources_for_version(env.id, version, agent)
+    async def _put_version(
+        self,
+        env: data.Environment,
+        version: int,
+        rid_to_resource: Dict[ResourceIdStr, data.Resource],
+        unknowns: abc.Sequence[data.UnknownParameter],
+        version_info: Optional[JsonType] = None,
+        resource_sets: Optional[Dict[ResourceIdStr, Optional[str]]] = None,
+        partial_base_version: Optional[int] = None,
+        removed_resource_sets: Optional[List[str]] = None,
+        *,
+        connection: asyncpg.connection.Connection,
+    ) -> None:
+        """
+        :param rid_to_resource: This parameter should contain all the resources when a full compile is done.
+                                When a partial compile is done, it should contain all the resources that belong to the
+                                updated resource sets or the shared resource sets. This method updates this object with
+                                purge-on-delete resources.
+        :param unknowns: This parameter should contain all the unknowns for all the resources in the new version of the model.
+                         Also the unknowns for resources that are not present in rid_to_resource.
+        :param partial_base_version: When a partial compile is done, this parameter contains the version of the
+                                     configurationmodel this partial compile was based on. Otherwise this parameter should be
+                                     None.
+        :param removed_resource_sets: When a partial compile is done, this parameter should indicate the names of the resource
+                                      sets that are removed by the partial compile. When no resource sets are removed by
+                                      a partial compile or when a full compile is done, this parameter can be set to None.
+
+        Pre-conditions:
+            * The requires and provides relationships of the resources in rid_to_resource must be set correctly. For a
+              partial compile, this means it is assumed to be valid with respect to all absolute constraints that apply to
+              partial compiles. Constraints that are relative to the base version will be verified by this method.
+            * When a partial compile was done, all resources in rid_to_resource must meet the constraints of a partial compile.
+            * The resource sets defined in the removed_resource_sets argument must not overlap with the resource sets present
+              in the resource_sets argument.
+
+        This method adds resources to the model that are no longer present in the new version of the model and had the
+        purge_on_delete flag set to true. This method makes sure that the requires and provides relationships of these
+        additional resources are set correctly. This dependency wiring is also safe for a partial compile because
+        a partial compile cannot delete shared resources and because resources that belong to a non-shared resource set cannot
+        reference resources in another non-shared resource set. That way all dependencies of the deleted resources are present
+        in the rid_to_resource parameter.
+
+        When a partial compile is done, the undeployable and skipped_for_undeployable resources of a configurationmodel are
+        copied from the old version to the new version. This operation is safe because the only resources missing from
+        rid_to_resource are resources that belong to an unchanged, non-shared resource set. Those resources can only have
+        cross resource set dependencies in a non-shared resource set and the latter resource set cannot be changed by a partial
+        compile.
+
+        Validations done by this method:
+            * In case of a full export: Checks whether this version has any requires-provides across resource sets and
+                                        sets the is_suitable_for_partial_compiles field appropriately, indicating whether
+                                        this version is eligible to be used as a base version for a future partial compile.
+            * In case of a partial export: Verifies that no resources moved resource sets.
+        """
+        is_partial_update = partial_base_version is not None
 
-        deploy_model: List[Dict[str, Any]] = []
-        resource_ids: List[str] = []
+        if resource_sets is None:
+            resource_sets = {}
 
-        for rv in resources:
-            if rv.resource_id not in increment_ids:
-                continue
+        if removed_resource_sets is None:
+            removed_resource_sets = []
 
-            # TODO double parsing of ID
-            def in_requires(req: ResourceIdStr) -> bool:
-                if req in increment_ids:
-                    return True
-                idr = Id.parse_id(req)
-                return idr.get_agent_name() != agent
-
-            rv.attributes["requires"] = [r for r in rv.attributes["requires"] if in_requires(r)]
-            deploy_model.append(rv.to_dict())
-            resource_ids.append(rv.resource_version_id)
-
-        # Don't log ResourceActions without resource_version_ids, because
-        # no API call exists to retrieve them.
-        if resource_ids:
-            ra = data.ResourceAction(
-                environment=env.id,
-                version=version,
-                resource_version_ids=resource_ids,
-                action=const.ResourceAction.pull,
-                action_id=uuid.uuid4(),
-                started=started,
-                finished=now,
-                messages=[
-                    data.LogLine.log(logging.INFO, "Resource version pulled by client for agent %(agent)s state", agent=agent)
-                ],
+        if version > env.last_version:
+            raise BadRequest(
+                f"The version number used is {version} "
+                f"which is higher than the last outstanding reservation {env.last_version}"
             )
-            await ra.insert()
+        if version <= 0:
+            raise BadRequest(f"The version number used ({version}) is not positive")
 
-        return 200, {"environment": env.id, "agent": agent, "version": version, "resources": deploy_model}
+        for r in rid_to_resource.values():
+            if r.model != version:
+                raise BadRequest(
+                    f"The resource version of resource {r.resource_version_id} does not match the version argument "
+                    f"(version: {version})"
+                )
 
-    @handle(methods_v2.resource_deploy_done, env="tid", resource_id="rvid")
-    async def resource_deploy_done(
-        self,
-        env: data.Environment,
-        resource_id: Id,
-        action_id: uuid.UUID,
-        status: ResourceState,
-        messages: List[LogLine] = [],
-        changes: Dict[str, AttributeStateChange] = {},
-        change: Optional[Change] = None,
-        keep_increment_cache: bool = False,
-    ) -> None:
-        resource_id_str = resource_id.resource_version_str()
-        finished = datetime.datetime.now().astimezone()
-        changes_with_rvid = {resource_id_str: {attr_name: attr_change.dict()} for attr_name, attr_change in changes.items()}
-
-        if status not in VALID_STATES_ON_STATE_UPDATE:
-            error_and_log(
-                f"Status {status} is not a valid status at the end of a deployment.",
-                resource_ids=[resource_id_str],
-                action=const.ResourceAction.deploy,
-                action_id=action_id,
-            )
-        if status in TRANSIENT_STATES:
-            error_and_log(
-                "No transient state can be used to mark a deployment as done.",
-                status=status,
-                resource_ids=[resource_id_str],
-                action=const.ResourceAction.deploy,
-                action_id=action_id,
-            )
+        for rid_name in resource_sets.keys():
+            try:
+                Id.parse_id(rid_name)
+            except Exception as e:
+                raise BadRequest("Invalid resource id in resource set: %s" % str(e))
 
-        async with data.Resource.get_connection() as connection:
-            async with connection.transaction():
-                resource = await data.Resource.get_one(
-                    connection=connection,
-                    environment=env.id,
-                    resource_id=resource_id.resource_str(),
-                    model=resource_id.version,
-                    # acquire lock on Resource before read and before lock on ResourceAction to prevent conflicts with
-                    # cascading deletes
-                    lock=data.RowLockMode.FOR_UPDATE,
-                )
-                if resource is None:
-                    raise NotFound("The resource with the given id does not exist in the given environment.")
-
-                # no escape from terminal
-                if resource.status != status and resource.status in TERMINAL_STATES:
-                    LOGGER.error("Attempting to set undeployable resource to deployable state")
-                    raise AssertionError("Attempting to set undeployable resource to deployable state")
-
-                resource_action = await data.ResourceAction.get(action_id=action_id, connection=connection)
-                if resource_action is None:
-                    raise NotFound(
-                        f"No resource action exists for action_id {action_id}. Ensure "
-                        f"`/resource/<resource_id>/deploy/start` is called first. "
-                    )
-                if resource_action.finished is not None:
-                    raise Conflict(
-                        f"Resource action with id {resource_id_str} was already marked as done at {resource_action.finished}."
-                    )
+        started = datetime.datetime.now().astimezone()
 
-                for log in messages:
-                    # All other data is stored in the database. The msg was already formatted at the client side.
-                    self.log_resource_action(
-                        env.id,
-                        [resource_id_str],
-                        log.level.to_int,
-                        log.timestamp,
-                        log.msg,
+        resource_set_validator = ResourceSetValidator(set(rid_to_resource.values()))
+        undeployable_ids: abc.Sequence[ResourceIdStr] = [
+            res.resource_id for res in rid_to_resource.values() if res.status in const.UNDEPLOYABLE_STATES
+        ]
+        async with connection.transaction():
+            try:
+                if is_partial_update:
+                    # Make mypy happy
+                    assert partial_base_version is not None
+                    cm = await data.ConfigurationModel.create_for_partial_compile(
+                        env_id=env.id,
+                        version=version,
+                        # When a partial compile is done, the total will be updated in cm.recalculate_total()
+                        # with all the resources that belong to a resource set that was not updated.
+                        total=len(rid_to_resource),
+                        version_info=version_info,
+                        undeployable=undeployable_ids,
+                        skipped_for_undeployable=sorted(
+                            self._get_skipped_for_undeployable(list(rid_to_resource.values()), undeployable_ids)
+                        ),
+                        partial_base=partial_base_version,
+                        rids_in_partial_compile=set(rid_to_resource.keys()),
+                        connection=connection,
                     )
-
-                await resource_action.set_and_save(
-                    messages=[
-                        {
-                            **log.dict(),
-                            "timestamp": log.timestamp.astimezone().isoformat(timespec="microseconds"),
-                        }
-                        for log in messages
-                    ],
-                    changes=changes_with_rvid,
-                    status=status,
-                    change=change,
-                    finished=finished,
+                else:
+                    cm = data.ConfigurationModel(
+                        environment=env.id,
+                        version=version,
+                        date=datetime.datetime.now().astimezone(),
+                        total=len(rid_to_resource),
+                        version_info=version_info,
+                        undeployable=undeployable_ids,
+                        skipped_for_undeployable=sorted(
+                            self._get_skipped_for_undeployable(list(rid_to_resource.values()), undeployable_ids)
+                        ),
+                        is_suitable_for_partial_compiles=not resource_set_validator.has_cross_resource_set_dependency(),
+                    )
+                    await cm.insert(connection=connection)
+            except asyncpg.exceptions.UniqueViolationError:
+                raise ServerError("The given version is already defined. Versions should be unique.")
+
+            all_ids: set[Id] = set(Id.parse_id(rid, version) for rid in rid_to_resource.keys())
+            if is_partial_update:
+                # Make mypy happy
+                assert partial_base_version is not None
+                rids_unchanged_resource_sets: abc.Set[
+                    ResourceIdStr
+                ] = await data.Resource.copy_resources_from_unchanged_resource_set(
+                    environment=env.id,
+                    source_version=partial_base_version,
+                    destination_version=version,
+                    updated_resource_sets=set(sr for sr in resource_sets.values() if sr is not None),
+                    deleted_resource_sets=set(removed_resource_sets),
                     connection=connection,
                 )
+                resources_that_moved_resource_sets = rids_unchanged_resource_sets & set(rid_to_resource.keys())
+                if resources_that_moved_resource_sets:
+                    raise BadRequest(
+                        f"A partial compile cannot migrate resources {list(resources_that_moved_resource_sets)} to another"
+                        " resource set"
+                    )
+                all_ids |= {Id.parse_id(rid, version) for rid in rids_unchanged_resource_sets}
 
-                # final resource update
-                if not keep_increment_cache:
-                    self.clear_env_cache(env)
-
-                await resource.update_fields(
-                    last_deploy=finished,
-                    status=status,
-                    last_non_deploying_status=const.NonDeployingResourceState(status),
-                    connection=connection,
-                )
+            purge_on_delete_resources: Dict[ResourceIdStr, data.Resource] = await self._get_resources_for_purge_on_delete(
+                env=env,
+                version=version,
+                rid_to_resource=rid_to_resource,
+                all_resource_ids=[i.resource_str() for i in all_ids],
+                version_info=version_info,
+                connection=connection,
+            )
+            rid_to_resource.update(purge_on_delete_resources)
+            all_ids |= {Id.parse_id(rid, version) for rid in purge_on_delete_resources.keys()}
 
-                if "purged" in resource.attributes and resource.attributes["purged"] and status == const.ResourceState.deployed:
-                    await data.Parameter.delete_all(environment=env.id, resource_id=resource.resource_id, connection=connection)
+            await data.Resource.insert_many(list(rid_to_resource.values()), connection=connection)
+            await cm.recalculate_total(connection=connection)
 
-        self.add_background_task(data.ConfigurationModel.mark_done_if_done(env.id, resource.model))
+            await data.UnknownParameter.insert_many(unknowns, connection=connection)
 
-        waiting_agents = set([(Id.parse_id(prov).get_agent_name(), resource.resource_version_id) for prov in resource.provides])
-        for agent, resource_id in waiting_agents:
-            aclient = self.agentmanager_service.get_agent_client(env.id, agent)
-            if aclient is not None:
-                if change is None:
-                    change = const.Change.nochange
-                await aclient.resource_event(
-                    tid=env.id,
-                    id=agent,
-                    resource=resource_id,
-                    send_events=False,
-                    state=status,
-                    change=change,
-                    changes=changes_with_rvid,
-                )
-
-    @handle(methods.resource_action_update, env="tid")
-    async def resource_action_update(
-        self,
-        env: data.Environment,
-        resource_ids: List[ResourceVersionIdStr],
-        action_id: uuid.UUID,
-        action: const.ResourceAction,
-        started: datetime.datetime,
-        finished: datetime.datetime,
-        status: Optional[Union[const.ResourceState, const.DeprecatedResourceState]],
-        messages: List[Dict[str, Any]],
-        changes: Dict[str, Any],
-        change: const.Change,
-        send_events: bool,
-        keep_increment_cache: bool = False,
-        *,
-        connection: Optional[Connection] = None,
-    ) -> Apireturn:
-        def convert_legacy_state(
-            status: Optional[Union[const.ResourceState, const.DeprecatedResourceState]]
-        ) -> Optional[const.ResourceState]:
-            if status is None or isinstance(status, const.ResourceState):
-                return status
-            if status == const.DeprecatedResourceState.processing_events:
-                return const.ResourceState.deploying
-            else:
-                raise BadRequest(f"Unsupported deprecated resources state {status.value}")
+            all_agents: abc.Set[str] = {res.agent for res in rid_to_resource.values()}
+            for agent in all_agents:
+                await self.agentmanager_service.ensure_agent_registered(env, agent, connection=connection)
+
+            # Don't log ResourceActions without resource_version_ids, because
+            # no API call exists to retrieve them.
+            all_rvids = [i.resource_version_str() for i in all_ids]
+            if all_rvids:
+                now = datetime.datetime.now().astimezone()
+                log_line = data.LogLine.log(logging.INFO, "Successfully stored version %(version)d", version=version)
+                self.resource_service.log_resource_action(env.id, list(all_rvids), logging.INFO, now, log_line.msg)
+                ra = data.ResourceAction(
+                    environment=env.id,
+                    version=version,
+                    resource_version_ids=all_rvids,
+                    action_id=uuid.uuid4(),
+                    action=const.ResourceAction.store,
+                    started=started,
+                    finished=now,
+                    messages=[log_line],
+                )
+                await ra.insert(connection=connection)
 
-        status = convert_legacy_state(status)
+        LOGGER.debug("Successfully stored version %d", version)
 
-        # can update resource state
-        is_resource_state_update = action in STATE_UPDATE
-        # this ra is finishing
-        is_resource_action_finished = finished is not None
-
-        if is_resource_state_update:
-            # if status update, status is required
-            if status is None:
-                error_and_log(
-                    "Cannot perform state update without a status.",
-                    resource_ids=resource_ids,
-                    action=action,
-                    action_id=action_id,
-                )
-            # and needs to be valid
-            if status not in VALID_STATES_ON_STATE_UPDATE:
-                error_and_log(
-                    "Status %s is not valid on action %s" % (status, action),
-                    resource_ids=resource_ids,
-                    action=action,
-                    action_id=action_id,
-                )
-            if status in TRANSIENT_STATES:
-                if not is_resource_action_finished:
-                    pass
-                else:
-                    error_and_log(
-                        "The finished field must not be set for transient states",
-                        status=status,
-                        resource_ids=resource_ids,
-                        action=action,
-                        action_id=action_id,
-                    )
-            else:
-                if is_resource_action_finished:
-                    pass
-                else:
-                    error_and_log(
-                        "The finished field must be set for none transient states",
-                        status=status,
-                        resource_ids=resource_ids,
-                        action=action,
-                        action_id=action_id,
-                    )
+    async def _get_resources_for_purge_on_delete(
+        self,
+        env: data.Environment,
+        version: int,
+        rid_to_resource: abc.Mapping[ResourceIdStr, data.Resource],
+        all_resource_ids: abc.Sequence[ResourceIdStr],
+        version_info: Optional[JsonType] = None,
+        *,
+        connection: asyncpg.connection.Connection,
+    ) -> dict[ResourceIdStr, data.Resource]:
+        """
+        Return a dictionary of resources that were present in the old version of the model but that no longer exist in this
+        version (in rid_to_resource) and had the purge_on_delete flag set to true. The returned resources will have the purged
+        attribute set to True and their requires/provides relationships inverted.
+
+        :param env: The environment we are discovering purged resources for.
+        :param version: The new version of the configuration model in which the purge_on_delete resources should be added.
+        :param rid_to_resource: When a full compile is done, this dictionary contains an entry for all resources that are
+                                part of the full compile. When a partial compile is done, this dictionary contains an entry
+                                for each resource in the new version of the model that belongs to an updated or shared
+                                resource set.
+        :param all_resource_ids: All the resource ids of all the resources present in the new version of the model. When
+                                 a partial compile is done, this sequence also includes the resource ids of resources that were
+                                 not updated by the partial compile.
+        """
 
-        assert all(Id.is_resource_version_id(rvid) for rvid in resource_ids)
+        def safe_get(input: object, key: str, default: object) -> object:
+            if not isinstance(input, dict):
+                return default
+            if key not in input:
+                return default
+            return input[key]
+
+        rid_to_resource = dict(rid_to_resource)
+
+        # detect failed compiles
+        metadata: object = safe_get(version_info, const.EXPORT_META_DATA, {})
+        compile_state = safe_get(metadata, const.META_DATA_COMPILE_STATE, "")
+        failed = compile_state == const.Compilestate.failed
+
+        result = {}
+        if not failed and (await env.get(PURGE_ON_DELETE)):
+            # search for deleted resources (purge_on_delete)
+            resources_to_purge: List[data.Resource] = await data.Resource.get_deleted_resources(
+                env.id, version, all_resource_ids, connection=connection
+            )
 
-        resources: List[data.Resource]
-        async with data.Resource.get_connection(connection) as connection:
-            async with connection.transaction():
-                # validate resources
-                resources = await data.Resource.get_resources(
+            previous_requires = {}
+            for res in resources_to_purge:
+                LOGGER.warning("Purging %s, purged resource based on %s", res.resource_id, res.resource_version_id)
+
+                attributes = res.attributes.copy()
+                attributes["purged"] = True
+                attributes["requires"] = []
+                res_obj = data.Resource.new(
                     env.id,
-                    resource_ids,
-                    # acquire lock on Resource before read and before lock on ResourceAction to prevent conflicts with
-                    # cascading deletes
-                    lock=data.RowLockMode.FOR_UPDATE,
-                    connection=connection,
+                    resource_version_id=ResourceVersionIdStr("%s,v=%s" % (res.resource_id, version)),
+                    attributes=attributes,
                 )
-                if len(resources) == 0 or (len(resources) != len(resource_ids)):
-                    return (
-                        404,
-                        {
-                            "message": "The resources with the given ids do not exist in the given environment. "
-                            "Only %s of %s resources found." % (len(resources), len(resource_ids))
-                        },
-                    )
 
-                # validate transitions
-                if is_resource_state_update:
-                    # no escape from terminal
-                    if any(resource.status != status and resource.status in TERMINAL_STATES for resource in resources):
-                        LOGGER.error("Attempting to set undeployable resource to deployable state")
-                        raise AssertionError("Attempting to set undeployable resource to deployable state")
-
-                # get instance
-                resource_action = await data.ResourceAction.get(action_id=action_id, connection=connection)
-                if resource_action is None:
-                    # new
-                    if started is None:
-                        return 500, {"message": "A resource action can only be created with a start datetime."}
+                previous_requires[res_obj.resource_id] = res.attributes["requires"]
+                rid_to_resource[res_obj.resource_id] = res_obj
+                result[res_obj.resource_id] = res_obj
+
+            # invert dependencies on purges
+            for res_id, requires in previous_requires.items():
+                res_obj = rid_to_resource[res_id]
+                for require in requires:
+                    req_id = Id.parse_id(require)
+
+                    if req_id.resource_str() in rid_to_resource:
+                        req_res = rid_to_resource[req_id.resource_str()]
+                        req_res.attributes["requires"].append(res_obj.resource_id)
+                        if res_obj.agent != req_res.agent:
+                            res_obj.provides.append(req_res.resource_id)
+        return result
 
-                    version = Id.parse_id(resource_ids[0]).version
-                    resource_action = data.ResourceAction(
-                        environment=env.id,
-                        version=version,
-                        resource_version_ids=resource_ids,
-                        action_id=action_id,
-                        action=action,
-                        started=started,
-                    )
-                    await resource_action.insert(connection=connection)
-                else:
-                    # existing
-                    if resource_action.finished is not None:
-                        return (
-                            500,
-                            {
-                                "message": (
-                                    "An resource action can only be updated when it has not been finished yet. This action "
-                                    "finished at %s" % resource_action.finished
-                                )
-                            },
-                        )
+    async def _trigger_auto_deploy(
+        self,
+        env: data.Environment,
+        version: int,
+    ) -> None:
+        """
+        Triggers auto-deploy for stored resources. Must be called only after transaction that stores resources has been allowed
+        to commit. If not respected, the auto deploy might work on stale data, likely resulting in resources hanging in the
+        deploying state.
+        """
+        auto_deploy = await env.get(data.AUTO_DEPLOY)
+        if auto_deploy:
+            LOGGER.debug("Auto deploying version %d", version)
+            push_on_auto_deploy = cast(bool, await env.get(data.PUSH_ON_AUTO_DEPLOY))
+            agent_trigger_method_on_autodeploy = cast(str, await env.get(data.AGENT_TRIGGER_METHOD_ON_AUTO_DEPLOY))
+            agent_trigger_method_on_autodeploy = const.AgentTriggerMethod[agent_trigger_method_on_autodeploy]
+            await self.release_version(env, version, push_on_auto_deploy, agent_trigger_method_on_autodeploy)
+
+    def _create_unknown_parameter_daos_from_api_unknowns(
+        self, env_id: uuid.UUID, version: int, unknowns: Optional[List[Dict[str, PrimitiveTypes]]] = None
+    ) -> List[data.UnknownParameter]:
+        """
+        Create UnknownParameter dao's from the unknowns dictionaries passed through the put_version() and put_partial API
+        endpoint.
+        """
+        if not unknowns:
+            return []
+        result = []
+        for uk in unknowns:
+            if "resource" not in uk:
+                uk["resource"] = ""
+            if "metadata" not in uk:
+                uk["metadata"] = {}
+            unknown_parameter = data.UnknownParameter(
+                resource_id=uk["resource"],
+                name=uk["parameter"],
+                source=uk["source"],
+                environment=env_id,
+                version=version,
+                metadata=uk["metadata"],
+            )
+            result.append(unknown_parameter)
+        return result
 
-                def parse_timestamp(timestamp: str) -> datetime.datetime:
-                    try:
-                        return datetime.datetime.strptime(timestamp, const.TIME_ISOFMT + "%z")
-                    except ValueError:
-                        # interpret naive datetimes as UTC
-                        return datetime.datetime.strptime(timestamp, const.TIME_ISOFMT).replace(tzinfo=datetime.timezone.utc)
-
-                for msg in messages:
-                    # All other data is stored in the database. The msg was already formatted at the client side.
-                    self.log_resource_action(
-                        env.id,
-                        resource_ids,
-                        const.LogLevel(msg["level"]).to_int,
-                        parse_timestamp(msg["timestamp"]),
-                        msg["msg"],
-                    )
-                await resource_action.set_and_save(
-                    messages=[
-                        {
-                            **msg,
-                            "timestamp": parse_timestamp(msg["timestamp"]).isoformat(timespec="microseconds"),
-                        }
-                        for msg in messages
-                    ],
-                    changes=changes,
-                    status=status,
-                    change=change,
-                    finished=finished,
-                    connection=connection,
-                )
+    async def _put_version_lock(self, env: data.Environment, *, shared: bool = False, connection: asyncpg.Connection) -> None:
+        """
+        Acquires a transaction-level advisory lock for concurrency control between put_version and put_partial.
 
-                async def update_fields_resource(
-                    resource: data.Resource, connection: Optional[Connection] = None, **kwargs: object
-                ) -> None:
-                    """
-                    This method ensures that the `last_non_deploying_status` field in the database
-                    is updated correctly when the `status` field of a resource is updated.
-                    """
-                    if "status" in kwargs and kwargs["status"] is not ResourceState.deploying:
-                        kwargs["last_non_deploying_status"] = const.NonDeployingResourceState(kwargs["status"])
-                    await resource.update_fields(**kwargs, connection=connection)
-
-                if is_resource_state_update:
-                    # transient resource update
-                    if not is_resource_action_finished:
-                        for res in resources:
-                            await update_fields_resource(res, status=status, connection=connection)
-                        if not keep_increment_cache:
-                            self.clear_env_cache(env)
-                        return 200
+        :param env: The environment to acquire the lock for.
+        :param shared: If true, doesn't conflict with other shared locks, only with non-shared once.
+        :param connection: The connection hosting the transaction for which to acquire a lock.
+        """
+        lock: str = "pg_advisory_xact_lock_shared" if shared else "pg_advisory_xact_lock"
+        await connection.execute(
+            # Advisory lock keys are only 32 bit (or a single 64 bit key), while a full uuid is 128 bit.
+            # Since locking slightly too strictly at extremely low odds is acceptable, we only use a 32 bit subvalue
+            # of the uuid. For uuid4, time_low is (despite the name) randomly generated. Since it is an unsigned
+            # integer while Postgres expects a signed one, we shift it by 2**31.
+            f"SELECT {lock}({const.PG_ADVISORY_KEY_PUT_VERSION}, {env.id.time_low - 2**31})"
+        )
 
-                    else:
-                        # final resource update
-                        if not keep_increment_cache:
-                            self.clear_env_cache(env)
-
-                        model_version = None
-                        for res in resources:
-                            await update_fields_resource(res, last_deploy=finished, status=status, connection=connection)
-                            model_version = res.model
-
-                            if (
-                                "purged" in res.attributes
-                                and res.attributes["purged"]
-                                and status == const.ResourceState.deployed
-                            ):
-                                await data.Parameter.delete_all(
-                                    environment=env.id, resource_id=res.resource_id, connection=connection
-                                )
-
-        if is_resource_state_update and is_resource_action_finished:
-            self.add_background_task(data.ConfigurationModel.mark_done_if_done(env.id, model_version))
-            waiting_agents = set(
-                [(Id.parse_id(prov).get_agent_name(), res.resource_version_id) for res in resources for prov in res.provides]
-            )
-
-            for agent, resource_id in waiting_agents:
-                aclient = self.agentmanager_service.get_agent_client(env.id, agent)
-                if aclient is not None:
-                    if change is None:
-                        change = const.Change.nochange
-                    self.add_background_task(
-                        aclient.resource_event(env.id, agent, resource_id, send_events, status, change, changes)
-                    )
+    @handle(methods.put_version, env="tid")
+    async def put_version(
+        self,
+        env: data.Environment,
+        version: int,
+        resources: List[JsonType],
+        resource_state: Dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]],
+        unknowns: List[Dict[str, PrimitiveTypes]],
+        version_info: JsonType,
+        compiler_version: Optional[str] = None,
+        resource_sets: Optional[Dict[ResourceIdStr, Optional[str]]] = None,
+    ) -> Apireturn:
+        """
+        :param unknowns: dict with the following structure
+                            {
+                             "resource": ResourceIdStr,
+                             "parameter": str,
+                             "source": str
+                            }
+        """
+        if resource_sets is None:
+            resource_sets = {}
 
+        if not compiler_version:
+            raise BadRequest("Older compiler versions are no longer supported, please update your compiler")
+
+        unknowns_objs = self._create_unknown_parameter_daos_from_api_unknowns(env.id, version, unknowns)
+        rid_to_resource = self._create_dao_resources_from_api_resources(
+            env_id=env.id,
+            resources=resources,
+            resource_state=resource_state,
+            resource_sets=resource_sets,
+        )
+        async with data.Resource.get_connection() as con:
+            async with con.transaction():
+                # Acquire a lock that conflicts with the lock acquired by put_partial but not with itself
+                await self._put_version_lock(env, shared=True, connection=con)
+                await self._put_version(
+                    env, version, rid_to_resource, unknowns_objs, version_info, resource_sets, connection=con
+                )
+        await self._trigger_auto_deploy(env, version)
         return 200
 
-    @handle(methods_v2.resource_deploy_start, env="tid", resource_id="rvid")
-    async def resource_deploy_start(
+    @handle(methods_v2.put_partial, env="tid")
+    async def put_partial(
         self,
         env: data.Environment,
-        resource_id: Id,
-        action_id: uuid.UUID,
-    ) -> Dict[ResourceVersionIdStr, const.ResourceState]:
-        resource_id_str = resource_id.resource_version_str()
-        async with data.Resource.get_connection() as connection:
-            async with connection.transaction():
-                resource = await data.Resource.get_one(
-                    connection=connection,
-                    environment=env.id,
-                    resource_id=resource_id.resource_str(),
-                    model=resource_id.version,
+        resources: object,
+        resource_state: Optional[Dict[ResourceIdStr, Literal[ResourceState.available, ResourceState.undefined]]] = None,
+        unknowns: Optional[List[Dict[str, PrimitiveTypes]]] = None,
+        version_info: Optional[JsonType] = None,
+        resource_sets: Optional[Dict[ResourceIdStr, Optional[str]]] = None,
+        removed_resource_sets: Optional[List[str]] = None,
+    ) -> int:
+        """
+        :param unknowns: dict with the following structure
+                    {
+                     "resource": ResourceIdStr,
+                     "parameter": str,
+                     "source": str
+                    }
+        """
+        if resource_state is None:
+            resource_state = {}
+        if unknowns is None:
+            unknowns = []
+        if resource_sets is None:
+            resource_sets = {}
+        if removed_resource_sets is None:
+            removed_resource_sets = []
+
+        try:
+            pydantic.parse_obj_as(List[ResourceMinimal], resources)
+        except pydantic.ValidationError:
+            raise BadRequest(
+                "Type validation failed for resources argument. "
+                f"Expected an argument of type List[Dict[str, Any]] but received {resources}"
+            )
+        else:
+            # Make mypy happy
+            resources = cast(List[JsonType], resources)
+
+        # validate resources before any side effects take place
+        for r in resources:
+            rid = Id.parse_id(r["id"])
+            if rid.get_version() != 0:
+                raise BadRequest("Resources for partial export should not contain version information")
+
+        intersection: set[str] = set(resource_sets.values()).intersection(set(removed_resource_sets))
+        if intersection:
+            raise BadRequest(
+                "Following resource sets are present in the removed resource sets and in the resources that are exported: "
+                f"{intersection}"
+            )
+
+        async with data.Resource.get_connection() as con:
+            async with con.transaction():
+                # Acquire a lock that conflicts with itself and with the lock acquired by put_version
+                await self._put_version_lock(env, shared=False, connection=con)
+
+                # Only request a new version once the resource lock has been acquired to ensure a monotonic version history
+                version: int = await env.get_next_version(connection=con)
+
+                current_versions: abc.Sequence[data.ConfigurationModel] = await data.ConfigurationModel.get_versions(
+                    env.id, limit=1
                 )
-                if resource is None:
-                    raise NotFound(message=f"Environment {env.id} doesn't contain a resource with id {resource_id_str}")
+                if not current_versions:
+                    raise BadRequest("A partial export requires a base model but no versions have been exported yet.")
 
-                resource_action = data.ResourceAction(
-                    environment=env.id,
-                    version=resource_id.version,
-                    resource_version_ids=[resource_id_str],
-                    action_id=action_id,
-                    action=const.ResourceAction.deploy,
-                    started=datetime.datetime.now().astimezone(),
-                    messages=[
-                        data.LogLine.log(
-                            logging.INFO,
-                            "Resource deploy started on agent %(agent)s, setting status to deploying",
-                            agent=resource_id.agent_name,
+                base_model = current_versions[0]
+                base_version: int = base_model.version
+                if not base_model.is_suitable_for_partial_compiles:
+                    resources_in_base_version = await data.Resource.get_resources_for_version(env.id, base_version)
+                    resource_set_validator = ResourceSetValidator(set(resources_in_base_version))
+                    try:
+                        resource_set_validator.ensure_no_cross_resource_set_dependencies()
+                    except CrossResourceSetDependencyError as e:
+                        raise BadRequest(
+                            f"Base version {base_version} is not suitable for a partial compile. {e.get_error_message()}"
+                        )
+                    else:
+                        # This should never happen
+                        LOGGER.warning(
+                            "Base version %d was marked as not suitable for partial compiles, but no cross resource set"
+                            " dependencies were found.",
+                            base_version,
                         )
-                    ],
-                    status=const.ResourceState.deploying,
+
+                rid_to_resource: Dict[ResourceIdStr, data.Resource] = self._create_dao_resources_from_api_resources(
+                    env_id=env.id,
+                    resources=resources,
+                    resource_state=resource_state,
+                    resource_sets=resource_sets,
+                    set_version=version,
                 )
-                try:
-                    await resource_action.insert(connection=connection)
-                except UniqueViolationError:
-                    raise Conflict(message=f"A resource action with id {action_id} already exists.")
 
-                await resource.update_fields(connection=connection, status=const.ResourceState.deploying)
+                updated_resource_sets: abc.Set[str] = set(sr_name for sr_name in resource_sets.values() if sr_name is not None)
+                partial_update_merger = await PartialUpdateMerger.create(
+                    env_id=env.id,
+                    base_version=base_version,
+                    version=version,
+                    rids_in_partial_compile=set(rid_to_resource.keys()),
+                    updated_resource_sets=updated_resource_sets,
+                    deleted_resource_sets=set(removed_resource_sets),
+                    connection=con,
+                )
 
-            self.clear_env_cache(env)
+                # add shared resources
+                merged_resources = partial_update_merger.merge_updated_and_shared_resources(list(rid_to_resource.values()))
 
-            return await data.Resource.get_last_non_deploying_state_for_dependencies(
-                environment=env.id, resource_version_id=resource_id, connection=connection
-            )
+                await data.Code.copy_versions(env.id, base_version, version, connection=con)
+
+                merged_unknowns = await partial_update_merger.merge_unknowns(
+                    unknowns_in_partial_compile=self._create_unknown_parameter_daos_from_api_unknowns(env.id, version, unknowns)
+                )
 
-    @handle(methods_v2.get_resource_actions, env="tid")
-    async def get_resource_actions(
+                await self._put_version(
+                    env,
+                    version,
+                    merged_resources,
+                    merged_unknowns,
+                    version_info,
+                    resource_sets,
+                    partial_base_version=base_version,
+                    removed_resource_sets=removed_resource_sets,
+                    connection=con,
+                )
+        await self._trigger_auto_deploy(env, version)
+        return version
+
+    @handle(methods.release_version, version_id="id", env="tid")
+    async def release_version(
         self,
         env: data.Environment,
-        resource_type: Optional[str] = None,
-        agent: Optional[str] = None,
-        attribute: Optional[str] = None,
-        attribute_value: Optional[str] = None,
-        log_severity: Optional[str] = None,
-        limit: Optional[int] = 0,
-        action_id: Optional[uuid.UUID] = None,
-        first_timestamp: Optional[datetime.datetime] = None,
-        last_timestamp: Optional[datetime.datetime] = None,
-    ) -> ReturnValue[List[ResourceAction]]:
-        if (attribute and not attribute_value) or (not attribute and attribute_value):
-            raise BadRequest(
-                f"Attribute and attribute_value should both be supplied to use them filtering. "
-                f"Received attribute: {attribute}, attribute_value: {attribute_value}"
-            )
-        if first_timestamp and last_timestamp:
-            raise BadRequest(
-                f"Only one of the parameters first_timestamp and last_timestamp should be used "
-                f"Received first_timestamp: {first_timestamp}, last_timestamp: {last_timestamp}"
-            )
-        if action_id and not (first_timestamp or last_timestamp):
-            raise BadRequest(
-                f"The action_id parameter should be used in combination with either the first_timestamp or the last_timestamp "
-                f"Received action_id: {action_id}, first_timestamp: {first_timestamp}, last_timestamp: {last_timestamp}"
+        version_id: int,
+        push: bool,
+        agent_trigger_method: Optional[const.AgentTriggerMethod] = None,
+        *,
+        connection: Optional[asyncpg.connection.Connection] = None,
+    ) -> Apireturn:
+        model = await data.ConfigurationModel.get_version(env.id, version_id, connection=connection)
+        if model is None:
+            return 404, {"message": "The request version does not exist."}
+
+        # Already mark undeployable resources as deployed to create a better UX (change the version counters)
+        undep = await model.get_undeployable()
+        now = datetime.datetime.now().astimezone()
+
+        if undep:
+            undep_ids = [ResourceVersionIdStr(rid + ",v=%s" % version_id) for rid in undep]
+            # not checking error conditions
+            await self.resource_service.resource_action_update(
+                env,
+                undep_ids,
+                action_id=uuid.uuid4(),
+                started=now,
+                finished=now,
+                status=const.ResourceState.undefined,
+                action=const.ResourceAction.deploy,
+                changes={},
+                messages=[],
+                change=const.Change.nochange,
+                send_events=False,
+                connection=connection,
             )
 
-        if limit is None:
-            limit = APILIMIT
-        elif limit > APILIMIT:
-            raise BadRequest(f"limit parameter can not exceed {APILIMIT}, got {limit}.")
+            skippable = await model.get_skipped_for_undeployable()
+            if skippable:
+                skippable_ids = [ResourceVersionIdStr(rid + ",v=%s" % version_id) for rid in skippable]
+                # not checking error conditions
+                await self.resource_service.resource_action_update(
+                    env,
+                    skippable_ids,
+                    action_id=uuid.uuid4(),
+                    started=now,
+                    finished=now,
+                    status=const.ResourceState.skipped_for_undefined,
+                    action=const.ResourceAction.deploy,
+                    changes={},
+                    messages=[],
+                    change=const.Change.nochange,
+                    send_events=False,
+                    connection=connection,
+                )
 
-        resource_actions = await data.ResourceAction.query_resource_actions(
-            env.id,
-            resource_type,
-            agent,
-            attribute=attribute,
-            attribute_value=attribute_value,
-            log_severity=log_severity,
-            limit=limit,
-            action_id=action_id,
-            first_timestamp=first_timestamp,
-            last_timestamp=last_timestamp,
+        increments: tuple[abc.Set[ResourceIdStr], abc.Set[ResourceIdStr]] = await self.resource_service.get_increment(
+            env, version_id
         )
-        resource_action_dtos = [resource_action.to_dto() for resource_action in resource_actions]
-        links = {}
 
-        def _get_query_params(
-            resource_type: Optional[str] = None,
-            agent: Optional[str] = None,
-            attribute: Optional[str] = None,
-            attribute_value: Optional[str] = None,
-            log_severity: Optional[str] = None,
-            limit: Optional[int] = 0,
-        ) -> dict:
-            query_params = {
-                "resource_type": resource_type,
-                "agent": agent,
-                "attribute": attribute,
-                "attribute_value": attribute_value,
-                "log_severity": log_severity,
-                "limit": limit,
-            }
-            query_params = {param_key: param_value for param_key, param_value in query_params.items() if param_value}
-            return query_params
-
-        if limit and resource_action_dtos:
-            base_url = "/api/v2/resource_actions"
-            common_query_params = _get_query_params(resource_type, agent, attribute, attribute_value, log_severity, limit)
-            # Next is always earlier with regards to 'started' time
-            next_params = common_query_params.copy()
-            next_params["last_timestamp"] = resource_action_dtos[-1].started
-            next_params["action_id"] = resource_action_dtos[-1].action_id
-            links["next"] = url_concat(base_url, next_params)
-            previous_params = common_query_params.copy()
-            previous_params["first_timestamp"] = resource_action_dtos[0].started
-            previous_params["action_id"] = resource_action_dtos[0].action_id
-            links["prev"] = url_concat(base_url, previous_params)
-        return_value = ReturnValue(response=resource_action_dtos, links=links if links else None)
-        return return_value
-
-    @handle(methods_v2.get_resource_events, env="tid", resource_id="rvid")
-    async def get_resource_events(
-        self,
-        env: data.Environment,
-        resource_id: Id,
-    ) -> Dict[ResourceIdStr, List[ResourceAction]]:
-        return {
-            k: [ra.to_dto() for ra in v] for k, v in (await data.ResourceAction.get_resource_events(env, resource_id)).items()
-        }
+        increment_ids, neg_increment = increments
+        await self.resource_service.mark_deployed(env, neg_increment, now, version_id)
 
-    @handle(methods_v2.resource_did_dependency_change, env="tid", resource_id="rvid")
-    async def resource_did_dependency_change(
-        self,
-        env: data.Environment,
-        resource_id: Id,
-    ) -> bool:
-        # This resource has been deployed before => determine whether it should be redeployed based on events
-        return any(
-            True
-            for dependency, actions in (
-                await data.ResourceAction.get_resource_events(env, resource_id, const.Change.nochange)
-            ).items()
-            for action in actions
-        )
+        # Setting the model's released field to True is the trigger for the agents to start pulling in the resources.
+        # This has to be done after the resources outside of the increment have been marked as deployed.
+        await model.update_fields(released=True, result=const.VersionState.deploying, connection=connection)
+
+        if model.total == 0:
+            await model.mark_done(connection=connection)
+            return 200, {"model": model}
+
+        if push:
+            # fetch all resource in this cm and create a list of distinct agents
+            agents = await data.ConfigurationModel.get_agents(env.id, version_id, connection=connection)
+            await self.autostarted_agent_manager._ensure_agents(env, agents, connection=connection)
+
+            for agent in agents:
+                client = self.agentmanager_service.get_agent_client(env.id, agent)
+                if client is not None:
+                    if not agent_trigger_method:
+                        env_agent_trigger_method = await env.get(ENVIRONMENT_AGENT_TRIGGER_METHOD, connection=connection)
+                        incremental_deploy = env_agent_trigger_method == const.AgentTriggerMethod.push_incremental_deploy
+                    else:
+                        incremental_deploy = agent_trigger_method is const.AgentTriggerMethod.push_incremental_deploy
+                    self.add_background_task(client.trigger(env.id, agent, incremental_deploy))
+                else:
+                    LOGGER.warning("Agent %s from model %s in env %s is not available for a deploy", agent, version_id, env.id)
 
-    @handle(methods_v2.resource_list, env="tid")
-    async def resource_list(
+        return 200, {"model": model}
+
+    @handle(methods.deploy, env="tid")
+    async def deploy(
         self,
         env: data.Environment,
-        limit: Optional[int] = None,
-        first_id: Optional[ResourceVersionIdStr] = None,
-        last_id: Optional[ResourceVersionIdStr] = None,
-        start: Optional[str] = None,
-        end: Optional[str] = None,
-        filter: Optional[Dict[str, List[str]]] = None,
-        sort: str = "resource_type.desc",
-        deploy_summary: bool = False,
-    ) -> ReturnValueWithMeta[Sequence[LatestReleasedResource]]:
+        agent_trigger_method: const.AgentTriggerMethod = const.AgentTriggerMethod.push_full_deploy,
+        agents: Optional[List[str]] = None,
+    ) -> Apireturn:
+        warnings = []
 
-        try:
-            handler = ResourceView(env, limit, first_id, last_id, start, end, filter, sort, deploy_summary)
+        # get latest version
+        version_id = await data.ConfigurationModel.get_version_nr_latest_version(env.id)
+        if version_id is None:
+            return 404, {"message": "No version available"}
 
-            out = await handler.execute()
-            if deploy_summary:
-                out.metadata["deploy_summary"] = await data.Resource.get_resource_deploy_summary(env.id)
-            return out
+        # filter agents
+        allagents = await data.ConfigurationModel.get_agents(env.id, version_id)
+        if agents is not None:
+            required = set(agents)
+            present = set(allagents)
+            allagents = list(required.intersection(present))
+            notfound = required - present
+            if notfound:
+                warnings.append(
+                    "Model version %d does not contain agents named [%s]" % (version_id, ",".join(sorted(list(notfound))))
+                )
 
-        except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
-            raise BadRequest(e.message) from e
+        if not allagents:
+            return attach_warnings(404, {"message": "No agent could be reached"}, warnings)
+
+        present = set()
+        absent = set()
 
-        # TODO: optimize for no orphans
+        await self.autostarted_agent_manager._ensure_agents(env, allagents)
 
-    @handle(methods_v2.resource_details, env="tid")
-    async def resource_details(self, env: data.Environment, rid: ResourceIdStr) -> ReleasedResourceDetails:
+        for agent in allagents:
+            client = self.agentmanager_service.get_agent_client(env.id, agent)
+            if client is not None:
+                incremental_deploy = agent_trigger_method is const.AgentTriggerMethod.push_incremental_deploy
+                self.add_background_task(client.trigger(env.id, agent, incremental_deploy))
+                present.add(agent)
+            else:
+                absent.add(agent)
+
+        if absent:
+            warnings.append("Could not reach agents named [%s]" % ",".join(sorted(list(absent))))
+
+        if not present:
+            return attach_warnings(404, {"message": "No agent could be reached"}, warnings)
 
-        details = await data.Resource.get_resource_details(env.id, rid)
-        if not details:
-            raise NotFound("The resource with the given id does not exist, or was not released yet in the given environment.")
-        return details
+        return attach_warnings(200, {"agents": sorted(list(present))}, warnings)
 
-    @handle(methods_v2.resource_history, env="tid")
-    async def resource_history(
+    @handle(methods_v2.list_desired_state_versions, env="tid")
+    async def desired_state_version_list(
         self,
         env: data.Environment,
-        rid: ResourceIdStr,
         limit: Optional[int] = None,
-        first_id: Optional[str] = None,
-        last_id: Optional[str] = None,
-        start: Optional[datetime.datetime] = None,
-        end: Optional[datetime.datetime] = None,
-        sort: str = "date.desc",
-    ) -> ReturnValue[Sequence[ResourceHistory]]:
+        start: Optional[int] = None,
+        end: Optional[int] = None,
+        filter: Optional[Dict[str, List[str]]] = None,
+        sort: str = "version.desc",
+    ) -> ReturnValue[List[DesiredStateVersion]]:
         try:
-            handler = ResourceHistoryView(
+            return await DesiredStateVersionView(
                 environment=env,
-                rid=rid,
                 limit=limit,
+                filter=filter,
                 sort=sort,
-                first_id=first_id,
-                last_id=last_id,
                 start=start,
                 end=end,
-            )
-            out = await handler.execute()
-            return out
+            ).execute()
         except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
             raise BadRequest(e.message) from e
 
-    @handle(methods_v2.resource_logs, env="tid")
-    async def resource_logs(
+    @handle(methods_v2.promote_desired_state_version, env="tid")
+    async def promote_desired_state_version(
         self,
         env: data.Environment,
-        rid: ResourceIdStr,
-        limit: Optional[int] = None,
-        start: Optional[datetime.datetime] = None,
-        end: Optional[datetime.datetime] = None,
-        filter: Optional[Dict[str, List[str]]] = None,
-        sort: str = "timestamp.desc",
-    ) -> ReturnValue[Sequence[ResourceLog]]:
-        try:
-            handler = ResourceLogsView(environment=env, rid=rid, limit=limit, sort=sort, start=start, end=end, filter=filter)
-            out = await handler.execute()
-            return out
-        except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
-            raise BadRequest(e.message) from e
+        version: int,
+        trigger_method: Optional[PromoteTriggerMethod] = None,
+    ) -> None:
+        if trigger_method == PromoteTriggerMethod.push_incremental_deploy:
+            push = True
+            agent_trigger_method = const.AgentTriggerMethod.push_incremental_deploy
+        elif trigger_method == PromoteTriggerMethod.push_full_deploy:
+            push = True
+            agent_trigger_method = const.AgentTriggerMethod.push_full_deploy
+        elif trigger_method == PromoteTriggerMethod.no_push:
+            push = False
+            agent_trigger_method = None
+        else:
+            push = True
+            agent_trigger_method = None
+
+        status_code, result = await self.release_version(
+            env, version_id=version, push=push, agent_trigger_method=agent_trigger_method
+        )
+        if status_code != 200:
+            raise BaseHttpException(status_code, result["message"])
 
-    @handle(methods_v2.get_resources_in_version, env="tid")
-    async def get_resources_in_version(
+    @handle(methods_v2.get_diff_of_versions, env="tid")
+    async def get_diff_of_versions(
         self,
         env: data.Environment,
-        version: int,
-        limit: Optional[int] = None,
-        first_id: Optional[ResourceVersionIdStr] = None,
-        last_id: Optional[ResourceVersionIdStr] = None,
-        start: Optional[str] = None,
-        end: Optional[str] = None,
-        filter: Optional[Dict[str, List[str]]] = None,
-        sort: str = "resource_type.desc",
-    ) -> ReturnValueWithMeta[Sequence[VersionedResource]]:
+        from_version: int,
+        to_version: int,
+    ) -> List[ResourceDiff]:
+        await self._validate_version_parameters(env.id, from_version, to_version)
 
-        try:
-            handler = ResourcesInVersionView(env, version, limit, filter, sort, first_id, last_id, start, end)
-            return await handler.execute()
-        except (InvalidFilter, InvalidSort, data.InvalidQueryParameter, data.InvalidFieldNameException) as e:
-            raise BadRequest(e.message) from e
+        from_version_resources = await data.Resource.get_list(environment=env.id, model=from_version)
+        to_version_resources = await data.Resource.get_list(environment=env.id, model=to_version)
 
-    @handle(methods_v2.versioned_resource_details, env="tid")
-    async def versioned_resource_details(
-        self, env: data.Environment, version: int, rid: ResourceIdStr
-    ) -> VersionedResourceDetails:
-        resource = await data.Resource.get_versioned_resource_details(environment=env.id, version=version, resource_id=rid)
-        if not resource:
-            raise NotFound("The resource with the given id does not exist")
-        return resource
+        from_state = diff.Version(self.convert_resources(from_version_resources))
+        to_state = diff.Version(self.convert_resources(to_version_resources))
+
+        version_diff = to_state.generate_diff(from_state)
+
+        return version_diff
+
+    def convert_resources(self, resources: List[data.Resource]) -> Dict[ResourceIdStr, diff.Resource]:
+        return {res.resource_id: diff.Resource(resource_id=res.resource_id, attributes=res.attributes) for res in resources}
+
+    async def _validate_version_parameters(self, env: uuid.UUID, first_version: int, other_version: int) -> None:
+        if first_version >= other_version:
+            raise BadRequest(
+                f"Invalid version parameters: ({first_version}, {other_version}). "
+                "The second version number should be strictly greater than the first"
+            )
+        await self._check_version_exists(env, first_version)
+        await self._check_version_exists(env, other_version)
+
+    async def _check_version_exists(self, env: uuid.UUID, version: int) -> None:
+        version_object = await data.ConfigurationModel.get_version(env, version)
+        if not version_object:
+            raise NotFound(f"Version {version} not found")
```

### Comparing `inmanta-core-8.2.0/src/inmanta/server/validate_filter.py` & `inmanta-core-8.3.0/src/inmanta/server/validate_filter.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/stable_api.py` & `inmanta-core-8.3.0/src/inmanta/stable_api.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/types.py` & `inmanta-core-8.3.0/src/inmanta/types.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta/util.py` & `inmanta-core-8.3.0/src/inmanta/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,22 @@
 import functools
 import hashlib
 import inspect
 import itertools
 import logging
 import os
 import socket
+import threading
 import time
 import uuid
 import warnings
 from abc import ABC, abstractmethod
 from asyncio import CancelledError, Future, Lock, Task, ensure_future, gather
 from collections import abc, defaultdict
+from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass
 from logging import Logger
 from types import TracebackType
 from typing import Awaitable, BinaryIO, Callable, Coroutine, Dict, Iterator, List, Optional, Set, Tuple, Type, TypeVar, Union
 
 from tornado import gen
 from tornado.ioloop import IOLoop
@@ -695,7 +697,39 @@
     """
 
     async def __aenter__(self) -> T:
         return self.enter_result
 
     async def __aexit__(self, *excinfo: object) -> None:
         pass
+
+
+async def join_threadpools(threadpools: List[ThreadPoolExecutor]) -> None:
+    """
+    Asynchronously join a set of threadpools
+
+    idea borrowed from BaseEventLoop.shutdown_default_executor
+
+    We implemented this method because:
+    1. ThreadPoolExecutor.shutdown(wait=True)` is a blocking call, blocking the ioloop.
+       This doesn't work because we often have back-and-forth between the ioloop and the thread
+       due to our `ResourceHandler.run_sync` method.
+    2.The python sdk has no support for async awaiting threadpool shutdown (except for the default pool)
+    """
+
+    loop = asyncio.get_event_loop()
+    future = loop.create_future()
+
+    def join() -> None:
+        for threadpool in threadpools:
+            try:
+                threadpool.shutdown(wait=True)
+            except Exception:
+                LOGGER.exception("Exception during threadpool shutdown")
+        loop.call_soon_threadsafe(future.set_result, None)
+
+    thread = threading.Thread(target=join)
+    thread.start()
+    try:
+        await future
+    finally:
+        thread.join()
```

### Comparing `inmanta-core-8.2.0/src/inmanta/warnings.py` & `inmanta-core-8.3.0/src/inmanta/warnings.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta_core.egg-info/PKG-INFO` & `inmanta-core-8.3.0/src/inmanta_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmanta-core
-Version: 8.2.0
+Version: 8.3.0
 Summary: Inmanta deployment tool
 Home-page: https://github.com/inmanta/inmanta-core
 Author: Inmanta
 Author-email: code@inmanta.com
 License: Apache Software License 2
 Project-URL: Bug Tracker, https://github.com/inmanta/inmanta-core/issues
 Project-URL: Documentation, https://docs.inmanta.com/community/latest/
@@ -49,15 +49,15 @@
    approach and the configuration model using dependencies.
 
 Currently, the Inmanta project is mainly developed and maintained by Inmanta NV.
 
 ## Links
 
 * [Documentation](https://docs.inmanta.com/community/latest/)
-* [Quickstart](https://github.com/inmanta/quickstart-docker)
+* [Quickstart](https://docs.inmanta.com/community/latest/quickstart.html)
 
 ## Install
 
 * [Install Guide](https://docs.inmanta.com/community/latest/install.html)
 
 ## Running the tests using tox
```

### Comparing `inmanta-core-8.2.0/src/inmanta_core.egg-info/SOURCES.txt` & `inmanta-core-8.3.0/src/inmanta_core.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/inmanta/postgresproc.py
 src/inmanta/profile_mem.py
 src/inmanta/py.typed
 src/inmanta/reporter.py
 src/inmanta/resources.py
 src/inmanta/stable_api.py
 src/inmanta/types.py
+src/inmanta/user_setup.py
 src/inmanta/util.py
 src/inmanta/warnings.py
 src/inmanta/agent/__init__.py
 src/inmanta/agent/agent.py
 src/inmanta/agent/cache.py
 src/inmanta/agent/config.py
 src/inmanta/agent/handler.py
@@ -97,14 +98,18 @@
 src/inmanta/db/versions/v202212010.py
 src/inmanta/db/versions/v202301100.py
 src/inmanta/db/versions/v202301110.py
 src/inmanta/db/versions/v202301120.py
 src/inmanta/db/versions/v202301160.py
 src/inmanta/db/versions/v202301170.py
 src/inmanta/db/versions/v202301190.py
+src/inmanta/db/versions/v202302200.py
+src/inmanta/db/versions/v202302270.py
+src/inmanta/db/versions/v202303070.py
+src/inmanta/db/versions/v202303071.py
 src/inmanta/db/versions/v3.py
 src/inmanta/db/versions/v4.py
 src/inmanta/db/versions/v5.py
 src/inmanta/db/versions/v6.py
 src/inmanta/db/versions/v7.py
 src/inmanta/execute/__init__.py
 src/inmanta/execute/proxy.py
@@ -157,14 +162,15 @@
 src/inmanta/server/services/fileservice.py
 src/inmanta/server/services/metricservice.py
 src/inmanta/server/services/notificationservice.py
 src/inmanta/server/services/orchestrationservice.py
 src/inmanta/server/services/paramservice.py
 src/inmanta/server/services/projectservice.py
 src/inmanta/server/services/resourceservice.py
+src/inmanta/server/services/userservice.py
 src/inmanta_core.egg-info/PKG-INFO
 src/inmanta_core.egg-info/SOURCES.txt
 src/inmanta_core.egg-info/dependency_links.txt
 src/inmanta_core.egg-info/entry_points.txt
 src/inmanta_core.egg-info/not-zip-safe
 src/inmanta_core.egg-info/requires.txt
 src/inmanta_core.egg-info/top_level.txt
@@ -208,8 +214,9 @@
 tests/test_project.py
 tests/test_projectmetadata.py
 tests/test_protocol.py
 tests/test_proxy.py
 tests/test_resource.py
 tests/test_server.py
 tests/test_type.py
+tests/test_usersetup.py
 tests/test_util.py
```

### Comparing `inmanta-core-8.2.0/src/inmanta_core.egg-info/requires.txt` & `inmanta-core-8.3.0/src/inmanta_core.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 asyncpg<0.28,~=0.25
 click-plugins~=1.0
 click<8.2,>=8.0
 colorlog~=6.4
 cookiecutter<3,>=1
 crontab<2.0,>=0.23
-cryptography<40,>=36
+cryptography<41,>=36
 docstring-parser<0.16,>=0.10
 email-validator~=1.0
 execnet~=1.0
 importlib_metadata<7,>=4
 jinja2~=3.0
 more-itertools<10,>=8
 netifaces~=0.11
 packaging>=21.3
 pip>=21.3
 ply~=3.0
 pydantic!=1.9.0a1,~=1.0
 pyformance~=0.4
 PyJWT~=2.0
+pynacl~=1.5
 python-dateutil~=2.0
 pyyaml~=6.0
 texttable~=1.0
 tornado~=6.0
 typing_inspect~=0.7
 build~=0.7
 ruamel.yaml~=0.17
@@ -30,8 +31,8 @@
 [datatrace]
 graphviz
 
 [debug]
 rpdb
 
 [pytest-inmanta-extensions]
-pytest-inmanta-extensions~=8.2.0.0.dev
+pytest-inmanta-extensions~=8.3.0.0.dev
```

### Comparing `inmanta-core-8.2.0/src/inmanta_ext/core/__init__.py` & `inmanta-core-8.3.0/src/inmanta_ext/core/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/src/inmanta_ext/core/extension.py` & `inmanta-core-8.3.0/src/inmanta_ext/core/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     fileservice,
     metricservice,
     notificationservice,
     orchestrationservice,
     paramservice,
     projectservice,
     resourceservice,
+    userservice,
 )
 
 
 def setup(application: ApplicationContext) -> None:
     application.register_slice(server.Server())
     application.register_slice(agentmanager.AgentManager())
     application.register_slice(agentmanager.AutostartedAgentManager())
@@ -47,8 +48,9 @@
     application.register_slice(codeservice.CodeService())
     application.register_slice(metricservice.MetricsService())
     application.register_slice(paramservice.ParameterService())
     application.register_slice(resourceservice.ResourceService())
     application.register_slice(orchestrationservice.OrchestrationService())
     application.register_slice(dryrunservice.DyrunService())
     application.register_slice(notificationservice.NotificationService())
+    application.register_slice(userservice.UserService())
     application.register_slice(environment_metrics_service.EnvironmentMetricsService())
```

### Comparing `inmanta-core-8.2.0/src/inmanta_plugins/1/__init__.py` & `inmanta-core-8.3.0/src/inmanta_plugins/1/__init__.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_2way_protocol.py` & `inmanta-core-8.3.0/tests/test_2way_protocol.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_agent.py` & `inmanta-core-8.3.0/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_agent_manager.py` & `inmanta-core-8.3.0/tests/test_agent_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from uuid import UUID, uuid4
 
 import pytest
 
 from inmanta import config, data
 from inmanta.agent import Agent, agent
 from inmanta.agent import config as agent_config
+from inmanta.config import Config
 from inmanta.const import AgentAction, AgentStatus
 from inmanta.protocol import Result
 from inmanta.server import SLICE_AGENT_MANAGER, SLICE_AUTOSTARTED_AGENT_MANAGER
 from inmanta.server.agentmanager import AgentManager, AutostartedAgentManager, SessionAction, SessionManager
 from inmanta.server.protocol import Session
 from utils import UNKWN, assert_equal_ish, retry_limited
 
@@ -1176,43 +1177,14 @@
     await retry_limited(lambda: len(agentmanager.sessions) == 1 and len(agentmanager.tid_endpoint_to_session) == 0, timeout=10)
 
     # One agent has a session to the server, none of them is primary. The agent is paused
     assert len(agentmanager.sessions) == 1
     assert len(agentmanager.tid_endpoint_to_session) == 0
 
 
-async def test_add_internal_agent_when_missing_in_agent_map(server, environment, postgresql_client):
-    """
-    The internal agent should always be present in the autostart_agent_map. If it is not present, it is added when to
-    auto-started agent is started. This test case verifies this behavior.
-    """
-    # Ensure agent1
-    agentmanager = server.get_slice(SLICE_AGENT_MANAGER)
-    env = await data.Environment.get_by_id(UUID(environment))
-    await agentmanager.ensure_agent_registered(env=env, nodename="agent1")
-
-    # Remove the internal agent from the autostart_agent_map
-    query = "UPDATE public.environment SET settings=jsonb_set(settings, $1::text[], to_jsonb($2::jsonb), TRUE)"
-    await postgresql_client.execute(query, [data.AUTOSTART_AGENT_MAP], "{}")
-
-    # Assert internal agent not in autostart_agent_map
-    env = await data.Environment.get_by_id(UUID(environment))
-    autostart_agent_map = await env.get(data.AUTOSTART_AGENT_MAP)
-    assert "internal" not in autostart_agent_map
-
-    # Start autostarted agent1
-    autostarted_agent_manager = server.get_slice(SLICE_AUTOSTARTED_AGENT_MANAGER)
-    await autostarted_agent_manager._ensure_agents(env=env, agents=["agent1"])
-
-    # Verify patch on autostart_agent_map
-    env = await data.Environment.get_by_id(UUID(environment))
-    autostart_agent_map = await env.get(data.AUTOSTART_AGENT_MAP)
-    assert "internal" in autostart_agent_map
-
-
 async def test_error_handling_agent_fork(server, environment, monkeypatch):
     """
     Verifies resolution of issue: inmanta/inmanta-core#2777
     """
     exception_message = "The start of the agent failed"
 
     async def _dummy_fork_inmanta(
@@ -1297,7 +1269,31 @@
     # Execute _ensure_agents() again and verify that no restart is triggered
     caplog.clear()
     await autostarted_agent_manager._ensure_agents(env=env, agents=[agent_name])
     assert len(autostarted_agent_manager._agent_procs) == 1
     assert "Started new agent with PID" not in caplog.text
     # Ensure no timeout happened
     assert "took too long to start" not in caplog.text
+
+
+async def test_auto_started_agent_log_in_debug_mode(server, environment):
+    """
+    Test the logging of an autostarted agent
+    """
+    env = await data.Environment.get_by_id(uuid.UUID(environment))
+    await env.set(data.AUTOSTART_AGENT_MAP, {"internal": "", "test1": ""})
+
+    agentmanager = server.get_slice(SLICE_AGENT_MANAGER)
+    autostarted_agentmanager = server.get_slice(SLICE_AUTOSTARTED_AGENT_MANAGER)
+
+    await agentmanager.ensure_agent_registered(env, "test1")
+    await autostarted_agentmanager._ensure_agents(env, ["test1"])
+
+    logdir = Config.get("config", "log-dir")
+    log_file_path = f"{logdir}/agent-{environment}.log"  # Path to the log file
+
+    def log_contains_debug_line():
+        with open(log_file_path, mode="r") as f:
+            log_content = f.read()
+        return "DEBUG    inmanta.protocol.endpoints Start transport for client agent" in log_content
+
+    await retry_limited(log_contains_debug_line, 10)
```

### Comparing `inmanta-core-8.2.0/tests/test_app.py` & `inmanta-core-8.3.0/tests/test_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -246,32 +246,47 @@
     log_file = "server.log"
     assert log_file not in os.listdir(log_dir)
     assert len(stdout) != 0
     check_logs(stdout, regexes_required_lines, regexes_forbidden_lines, timed)
 
 
 @pytest.mark.parametrize_any(
-    "log_level, with_tty, regexes_required_lines, regexes_forbidden_lines",
+    "log_level,with_tty, regexes_required_lines, regexes_forbidden_lines",
     [
         (
             3,
             False,
             [
                 r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
                 r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
             ],
             [],
         ),
         (
+            "DEBUG",
+            False,
+            [
+                r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
+                r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
+            ],
+            [],
+        ),
+        (
             2,
             False,
             [r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint"],
             [r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint"],
         ),
         (
+            "INFO",
+            False,
+            [r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint"],
+            [r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint"],
+        ),
+        (
             3,
             True,
             [
                 r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
                 r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
             ],
             [],
@@ -286,28 +301,77 @@
 )
 @pytest.mark.timeout(60)
 def test_log_file_set(tmpdir, log_level, with_tty, regexes_required_lines, regexes_forbidden_lines):
     if is_colorama_package_available() and with_tty:
         pytest.skip("Colorama is present")
 
     log_file = "server.log"
-    (args, log_dir) = get_command(tmpdir, stdout_log_level=log_level, log_file=log_file, log_level_log_file=log_level)
+    (args, log_dir) = get_command(tmpdir, log_file=log_file, log_level_log_file=log_level)
     if with_tty:
         (stdout, _, _) = run_with_tty(args)
     else:
         (stdout, _, _) = run_without_tty(args)
     assert log_file in os.listdir(log_dir)
     log_file = os.path.join(log_dir, log_file)
     with open(log_file, "r") as f:
         log_lines = f.readlines()
     check_logs(log_lines, regexes_required_lines, regexes_forbidden_lines, timed=True)
     check_logs(stdout, [], regexes_required_lines, timed=True)
     check_logs(stdout, [], regexes_required_lines, timed=False)
 
 
+@pytest.mark.parametrize_any(
+    "log_level, regexes_required_lines, regexes_forbidden_lines",
+    [
+        (
+            5,
+            [
+                r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
+                r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
+            ],
+            [],
+        ),
+        (
+            4,
+            [
+                r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
+                r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
+            ],
+            [],
+        ),
+        (
+            3,
+            [
+                r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
+                r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
+            ],
+            [],
+        ),
+        (
+            2,
+            [r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint"],
+            [r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint"],
+        ),
+        (
+            1,
+            [],
+            [
+                r"[a-z.]*[ ]*DEBUG[\s]+[a-x\.A-Z]*[\s]Starting Server Rest Endpoint",
+                r"[a-z.]*[ ]*INFO[\s]+[a-x\.A-Z]*[\s]Starting server endpoint",
+            ],
+        ),
+    ],
+)
+@pytest.mark.timeout(60)
+def test_log_stdout_log_level(tmpdir, log_level, regexes_required_lines, regexes_forbidden_lines):
+    (args, log_dir) = get_command(tmpdir, stdout_log_level=log_level)
+    (stdout, _, _) = run_without_tty(args)
+    check_logs(stdout, regexes_required_lines, regexes_forbidden_lines, timed=False)
+
+
 def check_logs(log_lines, regexes_required_lines, regexes_forbidden_lines, timed):
     compiled_regexes_requires_lines = get_compiled_regexes(regexes_required_lines, timed)
     compiled_regexes_forbidden_lines = get_compiled_regexes(regexes_forbidden_lines, timed)
     for line in log_lines:
         print(line)
     for regex in compiled_regexes_requires_lines:
         if not any(regex.match(line) for line in log_lines):
```

### Comparing `inmanta-core-8.2.0/tests/test_app_cli.py` & `inmanta-core-8.3.0/tests/test_app_cli.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_cache.py` & `inmanta-core-8.3.0/tests/test_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,15 +261,14 @@
     assert value == cache.find("test", resource=resource, version=version)
 
 
 def test_get_or_else(my_resource):
     called = []
 
     def creator(param, resource, version):
-
         called.append("x")
         return param
 
     cache = AgentCache()
     value = "test too"
     value2 = "test too x"
     resource = Id("test::Resource", "test", "key", "test", 100).get_instance()
```

### Comparing `inmanta-core-8.2.0/tests/test_cli.py` & `inmanta-core-8.3.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     await data.Agent(environment=env2.id, name="agent3", paused=False).insert()
 
     async def assert_agent_paused(env_id: uuid.UUID, expected_records: Dict[str, bool]) -> None:
         result = await cli.run("agent", "list", "-e", str(env_id))
         assert result.exit_code == 0
         output = result.stdout.replace(" ", "")
         assert "Agent|Environment|Paused" in output
-        for (agent_name, paused) in expected_records.items():
+        for agent_name, paused in expected_records.items():
             assert f"{agent_name}|{env_id}|{paused}" in output
 
     await assert_agent_paused(env_id=env1.id, expected_records=dict(agent1=False, agent2=False))
     await assert_agent_paused(env_id=env2.id, expected_records=dict(agent3=False))
 
     # Pause
     result = await cli.run("agent", "pause", "-e", str(env1.id), "--agent", "agent1")
```

### Comparing `inmanta-core-8.2.0/tests/test_compilation.py` & `inmanta-core-8.3.0/tests/test_compilation.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_compiler_entrypoints.py` & `inmanta-core-8.3.0/tests/test_compiler_entrypoints.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import os
 from collections import defaultdict
 
 import more_itertools
 
 from inmanta import compiler
 from inmanta.ast import Range
+from inmanta.compiler import Compiler
+from inmanta.execute import scheduler
 
 
 def test_anchors_basic(snippetcompiler):
     snippetcompiler.setup_for_snippet(
         """
 entity Test:
     string a = "a"
@@ -52,14 +54,72 @@
 """,
         autostd=False,
     )
     anchormap = compiler.anchormap()
 
     assert len(anchormap) == 9
 
+    checkmap = {(r.lnr, r.start_char, r.end_char): t.location.lnr for r, t in anchormap}
+
+    def verify_anchor(flnr, s, e, tolnr):
+        assert checkmap[(flnr, s, e)] == tolnr
+
+    for f, t in sorted(anchormap, key=lambda x: x[0].lnr):
+        print("%s:%d -> %s" % (f, f.end_char, t))
+    verify_anchor(7, 22, 26, 2)
+    verify_anchor(8, 5, 8, 13)
+    verify_anchor(11, 1, 5, 2)
+    verify_anchor(11, 24, 29, 7)
+    verify_anchor(15, 5, 9, 2)
+    verify_anchor(15, 10, 11, 4)
+    verify_anchor(19, 22, 26, 2)
+    verify_anchor(23, 11, 15, 2)
+    verify_anchor(23, 22, 23, 19)
+
+
+def test_anchors_basic_old(snippetcompiler):
+    """
+    this test verify that the old path to generate the Anchormap still works. This ensure that we remain
+    backward compatible with old Language servers.
+    """
+    snippetcompiler.setup_for_snippet(
+        """
+entity Test:
+    string a = "a"
+    string b
+end
+
+entity Test2 extends Test:
+    foo c
+end
+
+Test.relation [0:1] -- Test2.reverse [0:]
+
+typedef foo as string matching /^a+$/
+
+a = Test(b="xx")
+z = a.relation
+u = a.b
+
+implementation a for Test:
+
+end
+
+implement Test using a
+""",
+        autostd=False,
+    )
+    compiler = Compiler()
+    (statements, blocks) = compiler.compile()
+    sched = scheduler.Scheduler()
+    anchormap = sched.anchormap(compiler, statements, blocks)
+
+    assert len(anchormap) == 9
+    assert all(isinstance(item[0], Range) and isinstance(item[1], Range) for item in anchormap)
+
     checkmap = {(r.lnr, r.start_char, r.end_char): t.lnr for r, t in anchormap}
 
     def verify_anchor(flnr, s, e, tolnr):
         assert checkmap[(flnr, s, e)] == tolnr
 
     for f, t in sorted(anchormap, key=lambda x: x[0].lnr):
         print("%s:%d -> %s" % (f, f.end_char, t))
@@ -94,15 +154,15 @@
 """,
         autostd=False,
     )
     anchormap = compiler.anchormap()
 
     assert len(anchormap) == 5
 
-    checkmap = {(r.lnr, r.start_char, r.end_char): t.lnr for r, t in anchormap}
+    checkmap = {(r.lnr, r.start_char, r.end_char): t.location.lnr for r, t in anchormap}
 
     def verify_anchor(flnr, s, e, tolnr):
         assert checkmap[(flnr, s, e)] == tolnr
 
     for f, t in anchormap:
         print("%s:%d -> %s" % (f, f.end_char, t))
     verify_anchor(7, 5, 9, 2)
@@ -128,16 +188,16 @@
         for location, resolves_to in anchormap
         if location.file == os.path.join(snippetcompiler.project_dir, "main.cf")
     )
     assert location.lnr == 4
     assert location.start_char == 5
     assert location.end_lnr == 4
     assert location.end_char == 18
-    assert resolves_to.file == os.path.join(snippetcompiler.modules_dir, "tests", "plugins", "__init__.py")
-    assert resolves_to.lnr == 13
+    assert resolves_to.location.file == os.path.join(snippetcompiler.modules_dir, "tests", "plugins", "__init__.py")
+    assert resolves_to.location.lnr == 13
 
 
 def test_get_types_and_scopes(snippetcompiler):
     """
     Test the get_types_and_scopes() entrypoint of the compiler.
     """
     snippetcompiler.setup_for_snippet(
@@ -193,7 +253,59 @@
     types_in_std_ns = namespace_to_type_name["std"]
     assert len(types_in_std_ns) > 1
     assert "std::Entity" in types_in_std_ns
 
     # Verify scopes
     assert scopes.get_name() == "__root__"
     assert sorted([scope.get_name() for scope in scopes.children()]) == sorted(["__config__", "std"])
+
+
+def test_anchors_with_docs(snippetcompiler):
+    snippetcompiler.setup_for_snippet(
+        """
+import tests
+
+l = tests::length("Hello World!") # has a docstring
+m = tests::empty("Hello World!") # has no docstring
+
+entity Test:
+    \"\"\"this is a test entity\"\"\"
+end
+
+entity Test_no_doc:
+end
+
+a = Test()
+b = Test_no_doc()
+
+implementation a for Test:
+end
+
+implementation b for Test_no_doc:
+end
+
+implement Test using a
+implement Test_no_doc using b
+""",
+        autostd=False,
+    )
+    anchormap = compiler.anchormap()
+
+    assert len(anchormap) == 10
+
+    checkmap = {(r.lnr, r.start_char, r.end_char): t.docstring for r, t in anchormap}
+
+    def verify_anchor(flnr, s, e, docs):
+        assert checkmap[(flnr, s, e)] == docs
+
+    for f, t in sorted(anchormap, key=lambda x: x[0].lnr):
+        print("%s:%d -> %s docstring: %s" % (f, f.end_char, t, t.docstring))
+    verify_anchor(4, 5, 18, "returns the length of the string")
+    verify_anchor(5, 5, 17, None)
+    verify_anchor(14, 5, 9, "this is a test entity")
+    verify_anchor(15, 5, 16, None)
+    verify_anchor(17, 22, 26, "this is a test entity")
+    verify_anchor(20, 22, 33, None)
+    verify_anchor(23, 22, 23, None)
+    verify_anchor(23, 11, 15, "this is a test entity")
+    verify_anchor(24, 29, 30, None)
+    verify_anchor(24, 11, 22, None)
```

### Comparing `inmanta-core-8.2.0/tests/test_config.py` & `inmanta-core-8.3.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,18 @@
 from inmanta.config import Config, Option, option_as_default
 from inmanta.const import ClientType
 from inmanta.server.protocol import Server, ServerSlice
 from utils import LogSequence
 
 
 def test_environment_deprecated_options(caplog):
-    for (deprecated_option, new_option) in [
+    for deprecated_option, new_option in [
         (cfg.agent_interval, cfg.agent_deploy_interval),
         (cfg.agent_splay, cfg.agent_deploy_splay_time),
     ]:
-
         Config.set(deprecated_option.section, deprecated_option.name, "22")
         caplog.clear()
         assert new_option.get() == 22
         assert "Config option %s is deprecated. Use %s instead." % (deprecated_option.name, new_option.name) in caplog.text
 
         Config.set(new_option.section, new_option.name, "23")
         caplog.clear()
```

### Comparing `inmanta-core-8.2.0/tests/test_const.py` & `inmanta-core-8.3.0/tests/test_const.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     TRANSIENT_STATES,
     UNDEPLOYABLE_STATES,
     VALID_STATES_ON_STATE_UPDATE,
 )
 
 
 def test_action_set_consistency():
-
     undep = set(UNDEPLOYABLE_STATES)
     transient = set(TRANSIENT_STATES)
     not_done = set(NOT_DONE_STATES)
     done = set(DONE_STATES)
 
     initial = set(INITIAL_STATES)
     on_deploy = set(VALID_STATES_ON_STATE_UPDATE)
```

### Comparing `inmanta-core-8.2.0/tests/test_data.py` & `inmanta-core-8.3.0/tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
         agent = data.Agent(
             environment=env.id, name="agi1", last_failover=datetime.datetime.now(), paused=False, id_primary=agi1.id
         )
         await agent.insert()
 
         version = int(time.time())
-        cm = data.ConfigurationModel(version=version, environment=env.id)
+        cm = data.ConfigurationModel(version=version, environment=env.id, is_suitable_for_partial_compiles=False)
         await cm.insert()
 
         resource_ids = []
         for i in range(5):
             path = "/etc/file" + str(i)
             key = "std::File[agent1,path=" + path + "]"
             res1 = data.Resource.new(environment=env.id, resource_version_id=key + ",v=%d" % version, attributes={"path": path})
@@ -218,15 +218,15 @@
 
         assert func(await data.Project.get_by_id(project.id))
         assert func(await data.Environment.get_by_id(env.id))
         assert func(await data.AgentProcess.get_one(sid=agent_proc.sid))
         assert func(await data.AgentInstance.get_by_id(agent_instances[0].id))
         assert func(await data.AgentInstance.get_by_id(agent_instances[1].id))
         assert func(await data.Agent.get_one(environment=agent.environment, name=agent.name))
-        for (environment, resource_version_id) in resource_ids:
+        for environment, resource_version_id in resource_ids:
             id = Id.parse_id(resource_version_id)
             assert func(await data.Resource.get_one(environment=environment, resource_id=id.resource_str(), model=id.version))
         assert func(await data.Code.get_one(environment=code.environment, resource=code.resource, version=code.version))
         assert func(await data.UnknownParameter.get_by_id(unknown_parameter.id))
 
     # Setup two environments
     full_env_1 = await create_full_environment("proj1", "env1")
@@ -296,15 +296,15 @@
     agi2 = data.AgentInstance(process=agent_proc.sid, name="agi2", tid=env.id)
     await agi2.insert()
 
     agent = data.Agent(environment=env.id, name="agi1", last_failover=datetime.datetime.now(), paused=False, id_primary=agi1.id)
     await agent.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(version=version, environment=env.id)
+    cm = data.ConfigurationModel(version=version, environment=env.id, is_suitable_for_partial_compiles=False)
     await cm.insert()
 
     resource_ids = []
     for i in range(5):
         path = "/etc/file" + str(i)
         key = "std::File[agent1,path=" + path + "]"
         res1 = data.Resource.new(environment=env.id, resource_version_id=key + ",v=%d" % version, attributes={"path": path})
@@ -387,15 +387,15 @@
 async def test_environment_deprecated_setting(init_dataclasses_and_load_schema, caplog):
     project = data.Project(name="proj")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
-    for (deprecated_option, new_option) in [
+    for deprecated_option, new_option in [
         (data.AUTOSTART_AGENT_INTERVAL, data.AUTOSTART_AGENT_DEPLOY_INTERVAL),
         (data.AUTOSTART_SPLAY, data.AUTOSTART_AGENT_DEPLOY_SPLAY_TIME),
     ]:
         await env.set(deprecated_option, 22)
         caplog.clear()
         assert (await env.get(new_option)) == 22
         assert "Config option %s is deprecated. Use %s instead." % (deprecated_option, new_option) in caplog.text
@@ -721,15 +721,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     # create resources
     key = "std::File[agent1,path=/etc/motd]"
     res1 = data.Resource.new(environment=env.id, resource_version_id=key + ",v=%d" % version, attributes={"path": "/etc/motd"})
     await res1.insert()
 
@@ -743,15 +750,20 @@
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     for version in range(1, 20):
         cm = data.ConfigurationModel(
-            environment=env.id, version=version, date=datetime.datetime.now(), total=0, version_info={}
+            environment=env.id,
+            version=version,
+            date=datetime.datetime.now(),
+            total=0,
+            version_info={},
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
 
     versions = await data.ConfigurationModel.get_versions(env.id, 0, 1)
     assert len(versions) == 1
     assert versions[0].version == 19
 
@@ -776,15 +788,20 @@
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     cms = []
     for version in range(1, 5):
         cm = data.ConfigurationModel(
-            environment=env.id, version=version, date=datetime.datetime.now(), total=0, version_info={}
+            environment=env.id,
+            version=version,
+            date=datetime.datetime.now(),
+            total=0,
+            version_info={},
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
         cms.append(cm)
 
     latest_version = await data.ConfigurationModel.get_latest_version(env.id)
     assert latest_version is None
 
@@ -801,15 +818,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     assert cm.done == 0
 
     path = "/etc/file"
     key = "std::File[agent1,path=" + path + "]"
     resource = data.Resource.new(environment=env.id, resource_version_id=key + ",v=%d" % version, attributes={"path": path})
@@ -839,15 +863,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     assert cm.done == 0
 
     path = "/etc/file"
     key = "std::File[agent1,path=" + path + "]"
     resource = data.Resource.new(environment=env.id, resource_version_id=key + ",v=%d" % version, attributes={"path": path})
@@ -879,15 +910,22 @@
     env1 = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env1.insert()
     env2 = data.Environment(name="prod", project=project.id, repo_url="", repo_branch="")
     await env2.insert()
 
     for env in [env1, env2]:
         for i in range(2):
-            cm = data.ConfigurationModel(environment=env.id, version=i, date=datetime.datetime.now(), total=0, version_info={})
+            cm = data.ConfigurationModel(
+                environment=env.id,
+                version=i,
+                date=datetime.datetime.now(),
+                total=0,
+                version_info={},
+                is_suitable_for_partial_compiles=False,
+            )
             await cm.insert()
 
             for r in range(3):
                 if r % 2 == 0:
                     res = data.Resource.new(
                         environment=env.id,
                         status=const.ResourceState.deployed,
@@ -920,15 +958,17 @@
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
     now = datetime.datetime.now().astimezone()
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=now, total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id, version=version, date=now, total=1, version_info={}, is_suitable_for_partial_compiles=False
+    )
     await cm.insert()
 
     assert cm.done == 0
 
     path = "/etc/file"
     key = "std::File[agent1,path=" + path + "]"
     resource = data.Resource.new(
@@ -957,15 +997,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=0, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=0,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     path = "/etc/file"
     key = "std::File[agent1,path=" + path + "]"
     resource = data.Resource.new(environment=env.id, resource_version_id=key + ",v=%d" % version, attributes={"path": path})
     await resource.insert()
 
@@ -992,20 +1039,30 @@
 
     env_dev = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env_dev.insert()
     env_prod = data.Environment(name="prod", project=project.id, repo_url="", repo_branch="")
     await env_prod.insert()
 
     now = datetime.datetime.now()
-    await data.ConfigurationModel(environment=env_dev.id, version=4, total=0, date=now, released=True).insert()
-    await data.ConfigurationModel(environment=env_dev.id, version=7, total=0, date=now, released=True).insert()
-    await data.ConfigurationModel(environment=env_dev.id, version=9, total=0, date=now, released=False).insert()
+    await data.ConfigurationModel(
+        environment=env_dev.id, version=4, total=0, date=now, released=True, is_suitable_for_partial_compiles=False
+    ).insert()
+    await data.ConfigurationModel(
+        environment=env_dev.id, version=7, total=0, date=now, released=True, is_suitable_for_partial_compiles=False
+    ).insert()
+    await data.ConfigurationModel(
+        environment=env_dev.id, version=9, total=0, date=now, released=False, is_suitable_for_partial_compiles=False
+    ).insert()
 
-    await data.ConfigurationModel(environment=env_prod.id, version=15, total=0, date=now, released=False).insert()
-    await data.ConfigurationModel(environment=env_prod.id, version=11, total=0, date=now, released=False).insert()
+    await data.ConfigurationModel(
+        environment=env_prod.id, version=15, total=0, date=now, released=False, is_suitable_for_partial_compiles=False
+    ).insert()
+    await data.ConfigurationModel(
+        environment=env_prod.id, version=11, total=0, date=now, released=False, is_suitable_for_partial_compiles=False
+    ).insert()
 
     assert await data.ConfigurationModel.get_version_nr_latest_version(env_dev.id) == 7
     assert await data.ConfigurationModel.get_version_nr_latest_version(env_prod.id) is None
     assert await data.ConfigurationModel.get_version_nr_latest_version(uuid.uuid4()) is None
 
 
 @pytest.mark.parametrize(
@@ -1023,15 +1080,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=2, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=2,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     assert cm.done == 0
 
     path1 = "/etc/file1"
     key1 = "std::File[agent1,path=" + path1 + "]"
     resource1 = data.Resource.new(
@@ -1099,14 +1163,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=2,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm1.insert()
 
     res11 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % version,
         status=const.ResourceState.deployed,
@@ -1129,28 +1194,36 @@
             environment=env.id,
             version=version,
             date=datetime.datetime.now(),
             total=1,
             version_info={},
             released=False,
             deployed=False,
+            is_suitable_for_partial_compiles=False,
         )
         await cm2.insert()
 
         res21 = data.Resource.new(
             environment=env.id,
             resource_version_id="std::File[agent5,path=/etc/motd],v=%s" % version,
             status=const.ResourceState.available,
             attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
         )
         await res21.insert()
 
     # model 3
     version += 1
-    cm3 = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=0, version_info={})
+    cm3 = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=0,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm3.insert()
 
     to_purge = await data.Resource.get_deleted_resources(env.id, version, set())
 
     assert len(to_purge) == 1
     assert to_purge[0].model == 1
     assert to_purge[0].resource_id == "std::File[agent1,path=/etc/motd]"
@@ -1169,14 +1242,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm1.insert()
 
     res11 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % version,
         status=const.ResourceState.deployed,
@@ -1190,28 +1264,36 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=False,
         deployed=False,
+        is_suitable_for_partial_compiles=False,
     )
     await cm2.insert()
 
     res21 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % version,
         status=const.ResourceState.available,
         attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
     )
     await res21.insert()
 
     # model 3
     version += 1
-    cm3 = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=0, version_info={})
+    cm3 = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=0,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm3.insert()
 
     to_purge = await data.Resource.get_deleted_resources(env.id, version, set())
 
     assert len(to_purge) == 1
     assert to_purge[0].model == 1
     assert to_purge[0].resource_id == "std::File[agent1,path=/etc/motd]"
@@ -1232,14 +1314,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=False,
         deployed=False,
+        is_suitable_for_partial_compiles=False,
     )
     await cm2.insert()
     res11 = data.Resource.new(
         environment=env.id,
         resource_version_id=key + ",v=%d" % version,
         status=const.ResourceState.deployed,
         attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": False},
@@ -1251,14 +1334,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=False,
         deployed=False,
+        is_suitable_for_partial_compiles=False,
     )
     await cm2.insert()
     res12 = data.Resource.new(
         environment=env.id,
         resource_version_id=key + ",v=%d" % version,
         status=const.ResourceState.deployed,
         attributes={"path": "/etc/motd", "purge_on_delete": True, "purged": True},
@@ -1292,14 +1376,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm1.insert()
 
     resource_ids = []
     for i in range(1, 11):
         res = data.Resource.new(
             environment=env.id,
@@ -1334,14 +1419,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
     for i in range(1, 11):
         res = data.Resource.new(
             environment=env.id,
             resource_version_id="std::File[agent1,path=/tmp/file%d],v=%d" % (i, version),
             status=const.ResourceState.deployed,
@@ -1356,14 +1442,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
     for i in range(11, 21):
         res = data.Resource.new(
             environment=env.id,
             resource_version_id="std::File[agent2,path=/tmp/file%d],v=%d" % (i, version),
             status=const.ResourceState.deployed,
@@ -1377,14 +1464,15 @@
             environment=env.id,
             version=version,
             date=datetime.datetime.now(),
             total=1,
             version_info={},
             released=True,
             deployed=True,
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
 
     async def make_with_status(i, status):
         res = data.Resource.new(
             environment=env.id,
             resource_version_id="std::File[agent3,path=/tmp/file%d],v=3" % i,
@@ -1426,14 +1514,15 @@
             environment=env.id,
             version=version,
             date=datetime.datetime.now(),
             total=2,
             version_info={},
             released=True,
             deployed=True,
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
         for i in range(1, 3):
             res = data.Resource.new(
                 environment=env.id,
                 resource_version_id="std::File[agent1,path=/tmp/file%d],v=%d" % (i, version),
                 status=status,
@@ -1458,14 +1547,15 @@
         environment=env.id,
         version=3,
         date=datetime.datetime.now(),
         total=2,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
     resources = await data.Resource.get_resources_in_latest_version(
         env.id, "std::File", {"path": "/etc/motd1", "purge_on_delete": True}
     )
     assert len(resources) == 0
 
@@ -1474,43 +1564,53 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=3, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=3,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     async def insert_resource(env_id, version, agent_name, path, status):
         resource_version_id = f"std::File[{agent_name},path={path}],v={version}"
         resource = data.Resource.new(
-            environment=env_id, resource_version_id=resource_version_id, attributes={"path": path}, status=status
+            environment=env_id,
+            resource_version_id=resource_version_id,
+            attributes={"path": path, "version": version},
+            status=status,
         )
         await resource.insert()
 
     await insert_resource(env.id, version, "agent1", "path1", const.ResourceState.deployed)
     await insert_resource(env.id, version, "agent2", "path2", const.ResourceState.available)
     await insert_resource(env.id, version, "agent1", "path3", const.ResourceState.undefined)
 
     result = await data.Resource.get_resources_for_version(env.id, version)
     assert len(result) == 3
     assert sorted([r.agent for r in result]) == ["agent1", "agent1", "agent2"]
     for r in result:
-        assert len(r.attributes) == 1
+        assert len(r.attributes) == 2
 
     result = await data.Resource.get_resources_for_version(env.id, version, agent="agent2")
     assert len(result) == 1
     assert result[0].agent == "agent2"
 
     result = await data.Resource.get_resources_for_version(env.id, version, no_obj=True)
     assert len(result) == 3
     assert sorted([r["agent"] for r in result]) == ["agent1", "agent1", "agent2"]
     for r in result:
-        assert len(r["attributes"]) == 1
+        assert len(r["attributes"]) == 2
 
 
 async def test_escaped_resources(init_dataclasses_and_load_schema):
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
@@ -1521,14 +1621,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm1.insert()
 
     routes = {"8.0.0.0/8": "1.2.3.4", "0.0.0.0/0": "127.0.0.1"}
     res = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,name=router],v=%d" % version,
@@ -1556,14 +1657,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm1.insert()
 
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=%d" % version,
         status=const.ResourceState.deployed,
@@ -1606,14 +1708,15 @@
             environment=env.id,
             version=version,
             date=datetime.datetime.now(),
             total=1,
             version_info={},
             released=True,
             deployed=True,
+            is_suitable_for_partial_compiles=False,
         )
         await cm1.insert()
 
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=1",
         status=const.ResourceState.deployed,
@@ -1668,14 +1771,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm1.insert()
 
     res11 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=%s" % version,
         status=const.ResourceState.deployed,
@@ -1698,14 +1802,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=False,
         deployed=False,
+        is_suitable_for_partial_compiles=False,
     )
     await cm2.insert()
     res21 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=%s" % version,
         status=const.ResourceState.available,
         attributes={"path": "/etc/file1"},
@@ -1725,14 +1830,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm3.insert()
 
     res31 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file2],v=%s" % version,
         status=const.ResourceState.deployed,
@@ -1786,14 +1892,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=1",
         status=const.ResourceState.deployed,
@@ -1864,15 +1971,20 @@
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
     cm = data.ConfigurationModel(
-        environment=env.id, version=version, date=datetime.datetime.now().astimezone(), total=1, version_info={}
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now().astimezone(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     rv_id = f"std::File[agent1,path=/etc/motd],v={version}"
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id=rv_id,
@@ -1952,15 +2064,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = 1
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=1",
         status=const.ResourceState.deployed,
         last_deploy=datetime.datetime(2018, 7, 14, 14, 30),
@@ -1986,34 +2105,48 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     code1 = data.Code(environment=env.id, resource="std::File", version=version, source_refs={"ref": "ref"})
     await code1.insert()
 
     code2 = data.Code(environment=env.id, resource="std::Directory", version=version, source_refs={})
     await code2.insert()
 
     version2 = version + 1
-    cm2 = data.ConfigurationModel(environment=env.id, version=version2, date=datetime.datetime.now(), total=1, version_info={})
+    cm2 = data.ConfigurationModel(
+        environment=env.id,
+        version=version2,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm2.insert()
 
     code3 = data.Code(environment=env.id, resource="std::Directory", version=version2, source_refs={})
     await code3.insert()
 
     # Test behavior of copy_versions. Create second environment to verify the method is restricted to the first one
     env2 = data.Environment(name="dev2", project=project.id, repo_url="", repo_branch="")
     await env2.insert()
-    await data.ConfigurationModel(environment=env2.id, version=code3.version).insert()
+    await data.ConfigurationModel(environment=env2.id, version=code3.version, is_suitable_for_partial_compiles=False).insert()
     await data.Code(environment=env2.id, resource="std::File", version=code3.version, source_refs={}).insert()
     await data.Code.copy_versions(env.id, code3.version, code3.version + 1)
 
     def assert_match_code(code1, code2):
         assert code1 is not None
         assert code2 is not None
         assert code1.environment == code1.environment
@@ -2128,15 +2261,22 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = 1
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     dryrun = await data.DryRun.create(env.id, version, 10, 5)
 
     resource_version_id = "std::File[agent1,path=/etc/motd],v=%s" % version
     dryrun_data = {"id": resource_version_id, "changes": {}}
     await data.DryRun.update_resource(dryrun.id, resource_version_id, dryrun_data)
@@ -2331,14 +2471,17 @@
     )
     table_names_in_database = [x["table_name"] for x in table_names]
     table_names_in_classes_list = [x.__name__.lower() for x in data._classes]
     # Schema management table is not in classes list
     # Join tables on resource and resource action is not in the classes list
     assert len(table_names_in_classes_list) + 2 == len(table_names_in_database)
     for item in table_names_in_classes_list:
+        # The DB table name for the User class is named inmanta_user
+        if item == "user":
+            item = "inmanta_user"
         assert item in table_names_in_database
 
 
 async def test_purgelog_test(init_dataclasses_and_load_schema):
     project = data.Project(name="test")
     await project.insert()
 
@@ -2350,14 +2493,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=1",
         status=const.ResourceState.deployed,
@@ -2438,14 +2582,15 @@
         environment=env.id,
         version=version,
         date=datetime.datetime.now(),
         total=1,
         version_info={},
         released=True,
         deployed=True,
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     res1 = data.Resource.new(
         environment=env.id,
         resource_version_id="std::File[agent1,path=/etc/file1],v=%s" % version,
         status=const.ResourceState.deployed,
@@ -2485,25 +2630,33 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
 
     # Add multiple versions of model
     for i in range(1, 11):
         cm = data.ConfigurationModel(
             environment=env.id,
             version=i,
             date=datetime.datetime.now() + datetime.timedelta(minutes=i),
             total=1,
             version_info={},
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
 
     # Add resource action for motd
     motd_first_start_time = datetime.datetime.now()
 
     async def make_file_resourceaction(version, offset=0, path="/etc/motd", log_level=logging.INFO):
@@ -2671,24 +2824,32 @@
     project = data.Project(name="test")
     await project.insert()
 
     env = data.Environment(name="dev", project=project.id, repo_url="", repo_branch="")
     await env.insert()
 
     version = int(time.time())
-    cm = data.ConfigurationModel(environment=env.id, version=version, date=datetime.datetime.now(), total=1, version_info={})
+    cm = data.ConfigurationModel(
+        environment=env.id,
+        version=version,
+        date=datetime.datetime.now(),
+        total=1,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    )
     await cm.insert()
     # Add multiple versions of model
     for i in range(1, 12):
         cm = data.ConfigurationModel(
             environment=env.id,
             version=i,
             date=datetime.datetime.now(),
             total=1,
             version_info={},
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
 
     for i in range(1, 12):
         res1 = data.Resource.new(
             environment=env.id,
             resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % str(i),
@@ -2825,15 +2986,15 @@
     ) -> None:
         rvid_to_resource_state = await data.Resource.get_last_non_deploying_state_for_dependencies(
             environment=environment, resource_version_id=Id.parse_id(resource_version_id)
         )
         assert expected_states == rvid_to_resource_state
 
     # V1
-    cm = data.ConfigurationModel(version=1, environment=env.id)
+    cm = data.ConfigurationModel(version=1, environment=env.id, is_suitable_for_partial_compiles=False)
     await cm.insert()
 
     rid_r1_v1 = "std::File[agent1,path=/etc/file1]"
     rid_r2_v1 = "std::File[agent1,path=/etc/file2]"
     rid_r3_v1 = "std::File[agent1,path=/etc/file3]"
     rid_r4_v1 = "std::File[agent1,path=/etc/file4]"
 
@@ -2878,15 +3039,15 @@
     }
     await assert_last_non_deploying_state(env.id, rvid_r1_v1, expected_states=expected_states)
     await assert_last_non_deploying_state(env.id, rvid_r2_v1, expected_states={})
     await assert_last_non_deploying_state(env.id, rvid_r3_v1, expected_states={})
     await assert_last_non_deploying_state(env.id, rvid_r4_v1, expected_states={})
 
     # V2
-    cm = data.ConfigurationModel(version=2, environment=env.id)
+    cm = data.ConfigurationModel(version=2, environment=env.id, is_suitable_for_partial_compiles=False)
     await cm.insert()
 
     rid_r2_v2 = "std::File[agent1,path=/etc/file2]"
     rid_r3_v2 = "std::File[agent1,path=/etc/file3]"
 
     rvid_r1_v2 = cast(ResourceVersionIdStr, "std::File[agent1,path=/etc/file1],v=2")
     rvid_r2_v2 = cast(ResourceVersionIdStr, "std::File[agent1,path=/etc/file2],v=2")
```

### Comparing `inmanta-core-8.2.0/tests/test_data_concurrency.py` & `inmanta-core-8.3.0/tests/test_data_concurrency.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     version: int = 1
     await data.ConfigurationModel(
         environment=env_id,
         version=version,
         date=datetime.datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     ).insert()
 
     resource = model.ResourceVersionIdStr(f"std::File[agent1,path=/etc/file1],v={version}")
     await data.Resource.new(
         environment=env_id,
         status=const.ResourceState.available,
         resource_version_id=resource,
@@ -187,14 +188,15 @@
     version: int = 1
     confmodel: data.ConfigurationModel = data.ConfigurationModel(
         environment=env_id,
         version=version,
         date=datetime.datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await confmodel.insert()
 
     resource = model.ResourceVersionIdStr(f"mymod::myresource[myagent,id=1],v={version}")
     await data.Resource.new(
         environment=env_id,
         status=const.ResourceState.available,
```

### Comparing `inmanta-core-8.2.0/tests/test_data_model.py` & `inmanta-core-8.3.0/tests/test_data_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 import sys
 import typing
 from enum import Enum
 
 import pydantic
 import pytest
 
-from inmanta import const, resources, types
-from inmanta.data.model import BaseModel, LogLine, ResourceMinimal
+from inmanta import const, types
+from inmanta.data.model import BaseModel, LogLine
 from inmanta.protocol.common import json_encode
 
 
 def test_model_inheritance():
     """Test if config classes inheritance"""
 
     class Choices(str, Enum):
@@ -105,32 +105,7 @@
     class Test(BaseModel):
         timestamp: datetime.datetime
 
     timestamp = datetime.datetime.now()
     assert timestamp.tzinfo is None
     test = Test(timestamp=timestamp)
     assert test.timestamp.tzinfo is not None
-
-
-def test_resource_minimal_create_from_version():
-    """
-    Test whether the `ResourceMinimal.create_with_version()` works correctly.
-    """
-    res_id_str = "res::Resource[agent1,id_attr=val],v=11"
-    initial_attributes = {
-        "id": res_id_str,
-        "attr1": "val",
-        "version": 11,
-        "requires": ["res::Resource[agent1,id_attr=dep1],v=11", "res::Resource[agent1,id_attr=dep2],v=11"],
-    }
-    resource_minimal = ResourceMinimal.create_with_version(
-        new_version=12,
-        id=resources.Id.parse_id(res_id_str).resource_version_str(),
-        attributes=initial_attributes,
-    )
-    expected_serialization = {
-        "id": "res::Resource[agent1,id_attr=val],v=12",
-        "attr1": "val",
-        "version": 12,
-        "requires": ["res::Resource[agent1,id_attr=dep1],v=12", "res::Resource[agent1,id_attr=dep2],v=12"],
-    }
-    assert resource_minimal.dict() == expected_serialization
```

### Comparing `inmanta-core-8.2.0/tests/test_deploy.py` & `inmanta-core-8.3.0/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_docs_snippets.py` & `inmanta-core-8.3.0/tests/test_docs_snippets.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_docstring_parser.py` & `inmanta-core-8.3.0/tests/test_docstring_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_env.py` & `inmanta-core-8.3.0/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_export.py` & `inmanta-core-8.3.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_extension_loading.py` & `inmanta-core-8.3.0/tests/test_extension_loading.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     finally:
         sys.path = oldpath
         importlib.reload(inmanta_ext)
 
 
 def test_discover_and_load():
     with splice_extension_in("test_module_path"):
-
         config.server_enabled_extensions.set("testplugin")
 
         ibl = InmantaBootloader()
         print("plugins: ", ibl._discover_plugin_packages())
 
         assert "inmanta_ext.testplugin" in ibl._discover_plugin_packages()
```

### Comparing `inmanta-core-8.2.0/tests/test_file_parser.py` & `inmanta-core-8.3.0/tests/test_file_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_handler.py` & `inmanta-core-8.3.0/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_import_entry_points.py` & `inmanta-core-8.3.0/tests/test_import_entry_points.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_influxdbreporting.py` & `inmanta-core-8.3.0/tests/test_influxdbreporting.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_io.py` & `inmanta-core-8.3.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_jwt.py` & `inmanta-core-8.3.0/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_loader.py` & `inmanta-core-8.3.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_module_loader.py` & `inmanta-core-8.3.0/tests/test_module_loader.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_modules.py` & `inmanta-core-8.3.0/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_openapi.py` & `inmanta-core-8.3.0/tests/test_openapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,37 +11,38 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+import enum
 import inspect
 import json
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 from uuid import UUID
 
 import pytest
 from openapi_spec_validator import openapi_v30_spec_validator
 from pydantic.networks import AnyHttpUrl, AnyUrl, PostgresDsn
 
-from inmanta.const import ResourceAction
+from inmanta.const import ClientType, ResourceAction
 from inmanta.data import model
 from inmanta.data.model import EnvironmentSetting
 from inmanta.protocol import method
 from inmanta.protocol.common import ArgOption, BaseHttpException, MethodProperties, UrlMethod
 from inmanta.protocol.openapi.converter import (
     ArgOptionHandler,
     FunctionParameterHandler,
     OpenApiConverter,
     OpenApiTypeConverter,
     OperationHandler,
 )
-from inmanta.protocol.openapi.model import MediaType, Schema
+from inmanta.protocol.openapi.model import MediaType, OpenApiDataTypes, ParameterType, Schema
 from inmanta.server import SLICE_SERVER
 from inmanta.server.extensions import FeatureManager
 from inmanta.server.protocol import Server
 
 
 class DummyException(BaseHttpException):
     def __init__(self):
@@ -51,28 +52,28 @@
 @pytest.fixture
 def feature_manager(server: Server) -> FeatureManager:
     return server.get_slice(SLICE_SERVER).feature_manager
 
 
 @pytest.fixture(scope="function")
 def api_methods_fixture(clean_reset):
-    @method(path="/simpleoperation", client_types=["api", "agent"], envelope=True)
+    @method(path="/simpleoperation", client_types=[ClientType.api, ClientType.agent], envelope=True)
     def post_method() -> str:
         return ""
 
-    @method(path="/simpleoperation", client_types=["agent"], operation="GET")
+    @method(path="/simpleoperation", client_types=[ClientType.agent], operation="GET")
     def get_method():
         pass
 
     arg_options = {
         "header": ArgOption(header="header-val", reply_header=True, getter=lambda x, y: "test"),
         "non_header": ArgOption(getter=lambda x, y: "test"),
     }
 
-    @method(path="/operation/<id>", client_types=["api", "agent"], envelope=True, arg_options=arg_options)
+    @method(path="/operation/<id>", client_types=[ClientType.api, ClientType.agent], envelope=True, arg_options=arg_options)
     def dummy_post_with_parameters(header: str, non_header: str, param: int, id: UUID) -> str:
         """
         This is a brief description.
 
         This is a more in depth description of the method.
 
         :param header: A header value.
@@ -82,15 +83,21 @@
         :return: A return value.
         :raises OSError: Something went wrong
         :raises NotFound: Resource was not found.
         :raises test_openapi.DummyException: A dummy exception
         """
         return ""
 
-    @method(path="/operation/<id>", client_types=["api", "agent"], envelope=True, arg_options=arg_options, operation="GET")
+    @method(
+        path="/operation/<id>",
+        client_types=[ClientType.api, ClientType.agent],
+        envelope=True,
+        arg_options=arg_options,
+        operation="GET",
+    )
     def dummy_get_with_parameters(header: str, non_header: str, param: int, id: UUID) -> str:
         """
         This is a brief description.
 
         This is a more in depth description of the method.
 
         :param header: A header value.
@@ -100,30 +107,36 @@
         :return: A return value.
         :raises OSError: Something went wrong
         :raises NotFound: Resource was not found.
         :raises test_openapi.DummyException: A dummy exception
         """
         return ""
 
-    @method(path="/operation/<id>", client_types=["api", "agent"], envelope=True, arg_options=arg_options)
+    @method(path="/operation/<id>", client_types=[ClientType.api, ClientType.agent], envelope=True, arg_options=arg_options)
     def dummy_post_with_parameters_no_docstring(header: str, non_header: str, param: int, id: UUID) -> str:
         return ""
 
-    @method(path="/operation/<id>", client_types=["api", "agent"], envelope=True, arg_options=arg_options, operation="GET")
+    @method(
+        path="/operation/<id>",
+        client_types=[ClientType.api, ClientType.agent],
+        envelope=True,
+        arg_options=arg_options,
+        operation="GET",
+    )
     def dummy_get_with_parameters_no_docstring(header: str, non_header: str, param: int, id: UUID) -> str:
         return ""
 
     arg_options_partial_doc = {
         "tid_doc": ArgOption(header="header-doc", reply_header=True, getter=lambda x, y: "test"),
         "tid_no_doc": ArgOption(header="header-no-doc", reply_header=True, getter=lambda x, y: "test"),
     }
 
     @method(
         path="/operation/<id_doc>/<id_no_doc>",
-        client_types=["api", "agent"],
+        client_types=[ClientType.api, ClientType.agent],
         envelope=True,
         arg_options=arg_options_partial_doc,
     )
     def dummy_post_with_parameters_partial_documentation(
         tid_doc: UUID, tid_no_doc: UUID, param_doc: int, param_no_doc: int, id_doc: UUID, id_no_doc: UUID
     ) -> str:
         """
@@ -133,15 +146,15 @@
         :param param_doc: A parameter.
         :param id_doc: The id of the resource.
         """
         return ""
 
     @method(
         path="/operation/<id_doc>/<id_no_doc>",
-        client_types=["api", "agent"],
+        client_types=[ClientType.api, ClientType.agent],
         envelope=True,
         arg_options=arg_options_partial_doc,
         operation="GET",
     )
     def dummy_get_with_parameters_partial_documentation(
         tid_doc: UUID, tid_no_doc: UUID, param_doc: int, param_no_doc: int, id_doc: UUID, id_no_doc: UUID
     ) -> str:
@@ -150,14 +163,25 @@
 
         :param tid_doc: The inmanta environment id.
         :param param_doc: A parameter.
         :param id_doc: The id of the resource.
         """
         return ""
 
+    @method(
+        path="/default/<id>",
+        client_types=[ClientType.api],
+        envelope=True,
+        operation="GET",
+    )
+    def dummy_get_with_default_values(
+        no_def: int, id: int = 5, param: str = "test", fl: float = 0.1, opt: Optional[str] = None
+    ) -> str:
+        return ""
+
 
 async def test_generate_openapi_definition(server: Server, feature_manager: FeatureManager):
     global_url_map = server._transport.get_global_url_map(server.get_slices().values())
     openapi = OpenApiConverter(global_url_map, feature_manager)
     openapi_json = openapi.generate_openapi_json()
     assert openapi_json
     openapi_parsed = json.loads(openapi_json)
@@ -718,7 +742,81 @@
     assert Schema(**{"$ref": ref_prefix + "address"}).resolve(ref_prefix, schemas) == schemas["address"]
 
     person_schema = schemas["person"].copy(deep=True)
 
     assert not Schema(**{"$ref": ref_prefix + "person"}).recursive_resolve(ref_prefix, schemas, update={}) == person_schema
     person_schema.properties["address"] = schemas["address"]
     assert Schema(**{"$ref": ref_prefix + "person"}).recursive_resolve(ref_prefix, schemas, update={}) == person_schema
+
+
+def test_get_openapi_parameter_type_for(api_methods_fixture: None) -> None:
+    """
+    Verify whether the MethodProperties.get_openapi_parameter_type_for() method works as expected.
+    """
+    assert len(MethodProperties.methods["dummy_post_with_parameters_no_docstring"]) == 1
+    method_properties = MethodProperties.methods["dummy_post_with_parameters_no_docstring"][0]
+    assert method_properties.get_openapi_parameter_type_for("id") is ParameterType.path
+    assert method_properties.get_openapi_parameter_type_for("header") is ParameterType.header
+    assert method_properties.get_openapi_parameter_type_for("non_header") is None
+    assert method_properties.get_openapi_parameter_type_for("param") is None
+
+    assert len(MethodProperties.methods["dummy_get_with_parameters_no_docstring"]) == 1
+    method_properties = MethodProperties.methods["dummy_get_with_parameters_no_docstring"][0]
+    assert method_properties.get_openapi_parameter_type_for("id") is ParameterType.path
+    assert method_properties.get_openapi_parameter_type_for("header") is ParameterType.header
+    assert method_properties.get_openapi_parameter_type_for("non_header") is ParameterType.query
+    assert method_properties.get_openapi_parameter_type_for("param") is ParameterType.query
+
+
+def test_get_openapi_type_of_parameter(api_methods_fixture: None) -> None:
+    """
+    Verify whether the OpenApiTypeConverter.get_openapi_type_of_parameter() method works as expected.
+    """
+    type_converter = OpenApiTypeConverter()
+    assert len(MethodProperties.methods["dummy_get_with_default_values"]) == 1
+    method_properties = MethodProperties.methods["dummy_get_with_default_values"][0]
+    param_dct = inspect.signature(method_properties.function).parameters
+    for param_name, data_type, default_value, nullable in [
+        ("no_def", OpenApiDataTypes.INTEGER.value, None, False),
+        ("id", OpenApiDataTypes.INTEGER.value, 5, False),
+        ("param", OpenApiDataTypes.STRING.value, "test", False),
+        ("fl", OpenApiDataTypes.NUMBER.value, 0.1, False),
+        ("opt", OpenApiDataTypes.STRING.value, None, True),
+    ]:
+        schema = type_converter.get_openapi_type_of_parameter(param_dct[param_name])
+        assert schema.type == data_type
+        assert schema.default == default_value
+        assert schema.nullable if nullable else not schema.nullable
+
+
+def test_get_openapi_type_for_on_enum() -> None:
+    """
+    Ensure that the type field is populated correctly when OpenApiTypeConverter.get_openapi_type() is called on an Enum.
+    """
+
+    class StrValEnum(enum.Enum):
+        A = "a"
+        B = "b"
+
+    class IntValEnum(enum.Enum):
+        A = 1
+        B = 2
+
+    class FloatValEnum(enum.Enum):
+        A = 1
+        B = 2.0
+
+    class BoolValEnum(enum.Enum):
+        A = True
+        B = False
+
+    openapi_type_converter = OpenApiTypeConverter()
+
+    for python_type, openapi_type in [
+        (StrValEnum, OpenApiDataTypes.STRING.value),
+        (IntValEnum, OpenApiDataTypes.INTEGER.value),
+        (FloatValEnum, OpenApiDataTypes.NUMBER.value),
+        (BoolValEnum, OpenApiDataTypes.BOOLEAN.value),
+    ]:
+        schema = openapi_type_converter.get_openapi_type(python_type)
+        resolved_schema = schema.resolve(openapi_type_converter.ref_prefix, openapi_type_converter.components.schemas)
+        assert resolved_schema.type == openapi_type
```

### Comparing `inmanta-core-8.2.0/tests/test_param.py` & `inmanta-core-8.3.0/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_parser.py` & `inmanta-core-8.3.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_postgres.py` & `inmanta-core-8.3.0/tests/test_postgres.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_postgres_proc.py` & `inmanta-core-8.3.0/tests/test_postgres_proc.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_project.py` & `inmanta-core-8.3.0/tests/test_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
     Contact: code@inmanta.com
 """
 import base64
 import logging
 import os
 import uuid
+from collections import defaultdict
 from pathlib import Path
-from typing import Dict, cast
+from typing import Dict, List, cast
 
 import pytest
 
 from inmanta.data import model
 from inmanta.module import ModuleLoadingException, Project
 from inmanta.server import SLICE_ENVIRONMENT
 from inmanta.server.services.environmentservice import EnvironmentAction, EnvironmentListener, EnvironmentService
@@ -76,14 +77,54 @@
     assert len(result.result["projects"]) == 0
 
     # get non existing environment
     response = await client.get_environment(uuid.uuid4())
     assert response.code == 404
 
 
+async def test_project_api_v2_project_list_ordering(client_v2):
+    """
+    Creates a few projects with several environments each.
+    Check that they are ordered by ascending (project_name, environment_name)
+    """
+
+    project_environments_map: Dict[str, List[str]] = defaultdict(lambda: [])
+
+    for project_n in range(3):
+        project_name: str = f"test-project-{project_n}"
+        result = await client_v2.project_create(project_name)
+        assert result.code == 200
+        assert "data" in result.result
+        assert "id" in result.result["data"]
+
+        project_id: uuid.UUID = result.result["data"]["id"]
+        project_environments_map[project_name] = []
+
+        for environment_n in range(3):
+            env_name: str = f"test-env-{environment_n}"
+            result = await client_v2.environment_create(project_id=project_id, name=env_name)
+            assert result.code == 200
+            project_environments_map[project_name].append(env_name)
+
+    result = await client_v2.project_list()
+    assert result.code == 200
+    assert "data" in result.result
+    assert len(result.result["data"]) == 3
+    for i in range(3):
+        assert len(result.result["data"][i]["environments"]) == 3
+
+    # Make sure results are sorted according to project name...
+    assert sorted(project_environments_map.keys()) == [result.result["data"][i]["name"] for i in range(3)]
+
+    # ... and according to env name within each project
+    for project_n, key_value_pair in enumerate(sorted(project_environments_map.items())):
+        project_id, env_id_list = key_value_pair
+        assert sorted(env_id_list) == [env["name"] for env in result.result["data"][project_n]["environments"]]
+
+
 async def test_project_api_v2(client_v2):
     result = await client_v2.project_create("project-test")
     assert result.code == 200
     assert "data" in result.result
     assert "id" in result.result["data"]
 
     project_id = result.result["data"]["id"]
```

### Comparing `inmanta-core-8.2.0/tests/test_projectmetadata.py` & `inmanta-core-8.3.0/tests/test_projectmetadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,19 +11,21 @@
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
     See the License for the specific language governing permissions and
     limitations under the License.
 
     Contact: code@inmanta.com
 """
+import logging
 from typing import List, Optional
 
 import pytest
 
-from inmanta.module import ModuleRepoType, ProjectMetadata, RelationPrecedenceRule
+from inmanta.module import ModuleRepoType, Project, ProjectMetadata, RelationPrecedenceRule
+from utils import assert_no_warning
 
 
 @pytest.mark.parametrize(
     "repo",
     [
         ("https://github.com/inmanta/{}.git"),
         ("git@github.com:inmanta/{}.git"),
@@ -75,7 +77,24 @@
         project_metadata = ProjectMetadata(name="test", relation_precedence_policy=[precedence_rule])
         relation_precedence_rules: List[RelationPrecedenceRule] = project_metadata.get_relation_precedence_rules()
         assert len(relation_precedence_rules) == 1
         assert relation_precedence_rules[0] == expected_precedence_rule
     else:
         with pytest.raises(ValueError):
             ProjectMetadata(name="test", relation_precedence_policy=[precedence_rule])
+
+
+def test_no_module_path(tmp_path, caplog):
+    with caplog.at_level(logging.WARNING):
+        with (tmp_path / "project.yml").open("w") as fh:
+            fh.write(
+                """
+    name: testproject
+    downloadpath: libs
+    repo:
+        - url: https://pypi.org/simple
+          type: package
+    """
+            )
+
+        Project(tmp_path, autostd=False)
+    assert_no_warning(caplog)
```

### Comparing `inmanta-core-8.2.0/tests/test_protocol.py` & `inmanta-core-8.3.0/tests/test_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         limit -= 1
 
     thread.join()
     assert len(done) > 0
 
 
 async def test_client_files_stat(client):
-
     file_names = []
     i = 0
     while i < 10:
         (hash, content, body) = make_random_file()
         if hash not in file_names:
             file_names.append(hash)
             result = await client.upload_file(id=hash, content=body)
@@ -452,15 +451,14 @@
         async def test_methodi(self, project: Project) -> ReturnValue[Project]:
             new_project = project.copy()
 
             return ReturnValue(response=new_project)
 
         @protocol.handle(test_method2)
         async def test_method2i(self, project: List[Project]) -> ReturnValue[List[Project]]:
-
             return ReturnValue(response=project)
 
     rs = Server()
     server = ProjectServer(name="projectserver")
     rs.add_slice(server)
     await rs.start()
     async_finalizer.add(server.stop)
@@ -1332,15 +1330,14 @@
     @protocol.typedmethod(path="/test", operation="GET", client_types=["api"])
     def test_method() -> ReturnValue[str]:  # NOQA
         pass
 
     class TestServer(ServerSlice):
         @protocol.handle(test_method)
         async def test_methodY(self) -> ReturnValue[str]:  # NOQA
-
             return ReturnValue(response=html_content, content_type=HTML_CONTENT_WITH_UTF8_CHARSET)
 
     rs = Server()
     server = TestServer(name="testserver")
     rs.add_slice(server)
     await rs.start()
     async_finalizer.add(server.stop)
@@ -2166,7 +2163,48 @@
     async_finalizer.add(rs.stop)
 
     client = protocol.Client("client")
     result = await client.test_method(id="test", name="test", value=True)
     assert result.code == 200
     assert result.result["data"]["name"] == "test"
     assert result.result["data"]["value"]
+
+
+async def test_get_description_foreach_http_status_code() -> None:
+    """
+    Test whether the `MethodProperties.get_description_foreach_http_status_code()` method works as expected.
+    """
+
+    class ProjectServer(ServerSlice):
+        @protocol.typedmethod(path="/test", operation="POST", client_types=[ClientType.api], varkw=True)
+        def test_method1(id: str, **kwargs: object) -> Dict[str, str]:  # NOQA
+            """
+            Create a new project
+
+            :returns: A new project
+            :raises NotFound: The id was not found.
+            :raises 500: A server error.
+            """
+
+        @protocol.typedmethod(path="/test", operation="POST", client_types=[ClientType.api], varkw=True)
+        def test_method2(id: str, **kwargs: object) -> Dict[str, str]:  # NOQA
+            """
+            Create a new project
+
+            :returns:
+            :raises NotFound:
+            :raises 500:
+            """
+
+    method_properties = protocol.common.MethodProperties.methods["test_method1"][0]
+    response_code_to_description: Dict[int, str] = method_properties.get_description_foreach_http_status_code()
+    assert len(response_code_to_description) == 3
+    assert response_code_to_description[200] == "A new project"
+    assert response_code_to_description[404] == "The id was not found."
+    assert response_code_to_description[500] == "A server error."
+
+    method_properties = protocol.common.MethodProperties.methods["test_method2"][0]
+    response_code_to_description: Dict[int, str] = method_properties.get_description_foreach_http_status_code()
+    assert len(response_code_to_description) == 3
+    assert response_code_to_description[200] == ""
+    assert response_code_to_description[404] == ""
+    assert response_code_to_description[500] == ""
```

### Comparing `inmanta-core-8.2.0/tests/test_proxy.py` & `inmanta-core-8.3.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_resource.py` & `inmanta-core-8.3.0/tests/test_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
             fields = "y"
 
         class Test(Base):
             fields = ("z",)
 
 
 def test_resource_base(snippetcompiler):
-
     import inmanta.resources
 
     @resource("__config__::XResource", agent="agent", id_attribute="key")
     class MyResource(inmanta.resources.Resource):
         """
         A file on a filesystem
         """
@@ -94,15 +93,14 @@
 
     assert myresource.key == "key"
     assert myresource.agent == "agent"
     assert myresource.value == "value"
 
 
 def test_resource_base_with_method_key(snippetcompiler):
-
     import inmanta.resources
 
     @resource("__config__::XResource", agent="agent", id_attribute="key")
     class MyResource(inmanta.resources.Resource):
         """
         A file on a filesystem
         """
@@ -131,15 +129,14 @@
         autostd=False,
     )
     with pytest.raises(ResourceException):
         snippetcompiler.do_export()
 
 
 def test_resource_with_keyword(snippetcompiler):
-
     import inmanta.resources
 
     @resource("__config__::YResource", agent="agent", id_attribute="key")
     class MyResource(inmanta.resources.Resource):
         """
         A file on a filesystem
         """
@@ -169,15 +166,14 @@
     )
 
     with pytest.raises(ResourceException):
         snippetcompiler.do_export()
 
 
 def test_resource_with_private_method(snippetcompiler):
-
     import inmanta.resources
 
     @resource("__config__::YResource", agent="agent", id_attribute="key")
     class MyResource(inmanta.resources.Resource):
         """
         A file on a filesystem
         """
@@ -229,15 +225,14 @@
         """
     )
 
     snippetcompiler.do_export()
 
 
 def test_resource_invalid_agent_name_annotation():
-
     import inmanta.resources
 
     with pytest.raises(ResourceException):
 
         @resource("__config__::XResource", agent=42, id_attribute="key")
         class MyResource(inmanta.resources.Resource):
             """
```

### Comparing `inmanta-core-8.2.0/tests/test_server.py` & `inmanta-core-8.3.0/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from dateutil import parser
 from tornado.httpclient import AsyncHTTPClient, HTTPRequest
 
 from inmanta import const, data, loader, resources
 from inmanta.agent import handler
 from inmanta.agent.agent import Agent
 from inmanta.const import ParameterSource
-from inmanta.data.model import AttributeStateChange, LogLine
+from inmanta.data.model import AttributeStateChange, LogLine, ResourceVersionIdStr
 from inmanta.export import upload_code
 from inmanta.protocol import Client
 from inmanta.server import (
     SLICE_AGENT_MANAGER,
     SLICE_AUTOSTARTED_AGENT_MANAGER,
     SLICE_ORCHESTRATION,
     SLICE_RESOURCE,
@@ -864,14 +864,15 @@
     for i in range(1, 12):
         cm = data.ConfigurationModel(
             environment=env.id,
             version=i,
             date=datetime.now(),
             total=1,
             version_info={},
+            is_suitable_for_partial_compiles=False,
         )
         await cm.insert()
         res1 = data.Resource.new(
             environment=env.id,
             resource_version_id="std::File[agent1,path=/etc/motd],v=%s" % str(i),
             status=const.ResourceState.deployed,
             last_deploy=datetime.now() + timedelta(minutes=i),
@@ -990,14 +991,15 @@
     model_version = 1
     cm = data.ConfigurationModel(
         environment=env_id,
         version=model_version,
         date=datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     model_version = 1
     rvid_r1 = "std::File[agent1,path=/etc/file1]"
     rvid_r2 = "std::File[agent1,path=/etc/file2]"
     rvid_r3 = "std::File[agent1,path=/etc/file3]"
@@ -1092,14 +1094,15 @@
     model_version = 1
     cm = data.ConfigurationModel(
         environment=env_id,
         version=model_version,
         date=datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     model_version = 1
     rvid_r1_v1 = f"std::File[agent1,path=/etc/file1],v={model_version}"
 
     await data.Resource.new(
@@ -1134,14 +1137,15 @@
     model_version = 1
     cm = data.ConfigurationModel(
         environment=env_id,
         version=model_version,
         date=datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     rvid_r1_v1 = f"std::File[agent1,path=/etc/file1],v={model_version}"
     await data.Resource.new(
         environment=env_id,
         status=const.ResourceState.available,
@@ -1297,14 +1301,15 @@
     model_version = 1
     cm = data.ConfigurationModel(
         environment=env_id,
         version=model_version,
         date=datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     rvid_r1_v1 = f"std::File[agent1,path=/etc/file1],v={model_version}"
     await data.Resource.new(
         environment=env_id,
         status=const.ResourceState.available,
@@ -1335,14 +1340,15 @@
     model_version = 1
     cm = data.ConfigurationModel(
         environment=env_id,
         version=model_version,
         date=datetime.now().astimezone(),
         total=1,
         version_info={},
+        is_suitable_for_partial_compiles=False,
     )
     await cm.insert()
 
     rvid_r1_v1 = f"std::File[agent1,path=/etc/file1],v={model_version}"
 
     # Resource doesn't exist
     result = await agent._client.resource_deploy_done(
@@ -1401,7 +1407,162 @@
     result_url = "http://localhost:%s/console%s" % (port, path)
     http_client = AsyncHTTPClient()
     request = HTTPRequest(
         url=base_url,
     )
     response = await http_client.fetch(request, raise_error=False)
     assert result_url == response.effective_url
+
+
+async def test_cleanup_old_agents(server):
+    """
+    This test is testing the functionality of cleaning up old agents in the database.
+    The test creates 2 environments and adds agents with various properties (some used in a version,
+    some in the agent map, and some with the primary ID set), and then tests that
+    the cleanup function correctly removes only the agents that meet the criteria for deletion.
+    """
+
+    project = data.Project(name="test")
+    await project.insert()
+
+    env1 = data.Environment(name="env1", project=project.id)
+    await env1.insert()
+    env2 = data.Environment(name="env2", project=project.id)
+    await env2.insert()
+
+    await env1.set(data.AUTOSTART_AGENT_MAP, {"agent3": "", "internal": ""})
+    await env2.set(data.AUTOSTART_AGENT_MAP, {"agent1": "", "internal": ""})
+
+    process_sid = uuid.uuid4()
+    await data.AgentProcess(hostname="localhost-dummy", environment=env1.id, sid=process_sid, last_seen=datetime.now()).insert()
+
+    id_primary = uuid.uuid4()
+    await data.AgentInstance(id=id_primary, process=process_sid, name="dummy-instance", tid=env1.id).insert()
+
+    version = 1
+    await data.ConfigurationModel(
+        environment=env1.id,
+        version=version,
+        date=datetime.now(),
+        total=1,
+        released=True,
+        version_info={},
+        is_suitable_for_partial_compiles=False,
+    ).insert()
+
+    path = "/etc/file1"
+    resource_id = f"std::File[agent4,path={path}]"
+
+    await data.Resource.new(
+        environment=env1.id, resource_version_id=ResourceVersionIdStr(f"{resource_id},v={version}"), attributes={"path": path}
+    ).insert()
+
+    # should get purged
+    await data.Agent(
+        environment=env1.id,
+        name="agent1",
+        paused=False,
+        id_primary=None,
+    ).insert()
+    # should not get purged as the id_primary is set -> not down
+    await data.Agent(environment=env1.id, name="agent2", paused=False, id_primary=id_primary).insert()
+    # should not get purged as it is in the agent map
+    await data.Agent(
+        environment=env1.id,
+        name="agent3",
+        paused=False,
+        id_primary=None,
+    ).insert()
+    # should not get purged as it is used in a version of the ConfigurationModel
+    await data.Agent(
+        environment=env1.id,
+        name="agent4",
+        paused=False,
+        id_primary=None,
+    ).insert()
+    # agent with "agent2" as name but in another env will get purged:
+    await data.Agent(
+        environment=env2.id,
+        name="agent2",
+        paused=False,
+        id_primary=None,
+    ).insert()
+    # agent with "agent1" as name but being present in the agent_map and in another env will not get purged:
+    await data.Agent(
+        environment=env2.id,
+        name="agent1",
+        paused=False,
+        id_primary=None,
+    ).insert()
+
+    agents_before_purge = await data.Agent.get_list()
+    assert len(agents_before_purge) == 6
+
+    await server.get_slice(SLICE_ORCHESTRATION)._purge_versions()
+    agents_after_purge = [(agent.environment, agent.name) for agent in await data.Agent.get_list()]
+    assert len(agents_after_purge) == 4
+    expected_agents_after_purge = [
+        (env1.id, "agent2"),
+        (env1.id, "agent3"),
+        (env1.id, "agent4"),
+        (env2.id, "agent1"),
+    ]
+    assert sorted(agents_after_purge) == sorted(expected_agents_after_purge)
+
+
+async def test_serialization_attributes_of_resource_to_api(client, server, environment, clienthelper) -> None:
+    """
+    Due to a bug, the version of a resource was always included in the attribute dictionary.
+    This issue has been patched in the database, but at the API boundary we still serve the version
+    field in the attributes dictionary for backwards compatibility. This test verifies that behavior.
+    """
+    version = await clienthelper.get_version()
+    resource_id = "test::Resource[agent1,key=key1]"
+    resources = [
+        {
+            "id": f"{resource_id},v={version}",
+            "att": "val",
+            "version": version,
+            "send_event": False,
+            "purged": False,
+            "requires": [],
+        }
+    ]
+    attributes_on_api = {k: v for k, v in resources[0].items() if k != "id"}
+    result = await client.put_version(
+        tid=environment,
+        version=version,
+        resources=resources,
+        unknowns=[],
+        version_info={},
+        compiler_version=get_compiler_version(),
+    )
+    assert result.code == 200
+
+    result = await client.release_version(tid=environment, id=version)
+    assert result.code == 200
+
+    # Verify that the version field is not present in the attributes dictionary in the database.
+    result = await data.Resource.get_list()
+    assert len(result) == 1
+    resource_dao = result[0]
+    assert "version" not in resource_dao.attributes
+
+    # Ensure that the serialization of the resource DAO contains the version field in the attributes dictionary
+    resource_dto = resource_dao.to_dto()
+    assert resource_dto.attributes["version"] == version
+    resource_dct = resource_dao.to_dict()
+    assert resource_dct["attributes"]["version"] == version
+
+    # Retrieve the resource via the API and ensure that the version field is present in the attributes dictionary
+    result = await client.resource_history(environment, resource_id)
+    assert result.code == 200
+    assert len(result.result["data"]) == 1
+    assert result.result["data"][0]["attributes"] == attributes_on_api
+
+    result = await client.versioned_resource_details(tid=environment, version=version, rid=resource_id)
+    assert result.code == 200
+    assert result.result["data"]["attributes"] == attributes_on_api
+
+    result = await client.resource_details(tid=environment, rid=resource_id)
+    assert result.code == 200
+    assert result.result["data"]["attributes"] == attributes_on_api
```

### Comparing `inmanta-core-8.2.0/tests/test_type.py` & `inmanta-core-8.3.0/tests/test_type.py`

 * *Files identical despite different names*

### Comparing `inmanta-core-8.2.0/tests/test_util.py` & `inmanta-core-8.3.0/tests/test_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,29 +16,33 @@
     Contact: code@inmanta.com
 """
 import asyncio
 import dataclasses
 import datetime
 import logging
 import uuid
+from concurrent.futures import ThreadPoolExecutor
 from functools import partial
+from queue import Queue
+from threading import Event
 from typing import Optional
 
 import pytest
 
 import inmanta
 from inmanta import util
 from inmanta.util import (
     CronSchedule,
     CycleException,
     IntervalSchedule,
     NamedLock,
     ScheduledTask,
     TaskSchedule,
     ensure_future_and_handle_exception,
+    join_threadpools,
     stable_depth_first,
 )
 from utils import LogSequence, get_product_meta_data, log_contains, no_error_in_logs
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -490,7 +494,39 @@
 
 
 def test_running_test_fixture():
     """
     Assert that the RUNNING_TESTS variable is set to True when we run the tests
     """
     assert inmanta.RUNNING_TESTS
+
+
+async def test_threadpool_join():
+    tp = ThreadPoolExecutor()
+
+    hanglock = Event()
+    done = Queue()
+
+    eventloop = asyncio.get_event_loop()
+
+    async def cor():
+        await asyncio.sleep(0.02)
+
+    def worker():
+        # hang on lock
+        hanglock.wait()
+        # hang on ioloop
+        block = asyncio.run_coroutine_threadsafe(cor(), loop=eventloop)
+        block.result()
+        done.put("A")
+
+    for i in range(5):
+        tp.submit(worker)
+
+    tp.shutdown(wait=False)
+    assert done.qsize() == 0
+    hanglock.set()
+    assert done.qsize() == 0
+    await join_threadpools([tp])
+    # verify we are done
+    tp.shutdown(wait=True)
+    assert done.qsize() == 5
```

### Comparing `inmanta-core-8.2.0/tox.ini` & `inmanta-core-8.3.0/tox.ini`

 * *Files identical despite different names*

