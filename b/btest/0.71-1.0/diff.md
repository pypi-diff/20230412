# Comparing `tmp/btest-0.71.tar.gz` & `tmp/btest-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btest-0.71.tar", last modified: Mon Nov  1 19:09:30 2021, max compression
+gzip compressed data, was "btest-1.0.tar", last modified: Tue Apr 11 23:52:04 2023, max compression
```

## Comparing `btest-0.71.tar` & `btest-1.0.tar`

### file list

```diff
@@ -1,312 +1,332 @@
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.254431 btest-0.71/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.243431 btest-0.71/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.247431 btest-0.71/Baseline/examples.t4/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1252 2021-01-13 20:54:37.802129 btest-0.71/Baseline/examples.t4/dots
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.247431 btest-0.71/Baseline/examples.t5/
--rw-rw-r--   0 christian  (1000) christian  (1000)        9 2021-01-13 20:54:37.802129 btest-0.71/Baseline/examples.t5/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.247431 btest-0.71/Baseline/examples.t5-2/
--rw-rw-r--   0 christian  (1000) christian  (1000)        9 2021-01-13 20:54:37.802129 btest-0.71/Baseline/examples.t5-2/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.247431 btest-0.71/Baseline/examples.t6/
--rw-rw-r--   0 christian  (1000) christian  (1000)        2 2021-01-13 20:54:37.802129 btest-0.71/Baseline/examples.t6/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.247431 btest-0.71/Baseline/examples.t7/
--rw-rw-r--   0 christian  (1000) christian  (1000)      132 2021-01-13 20:54:37.802129 btest-0.71/Baseline/examples.t7/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.247431 btest-0.71/Baseline/examples.unstable/
--rw-rw-r--   0 christian  (1000) christian  (1000)        2 2021-01-13 20:54:37.802129 btest-0.71/Baseline/examples.unstable/output
--rw-r--r--   0 christian  (1000) christian  (1000)    35835 2021-11-01 19:08:05.558512 btest-0.71/CHANGES
--rw-rw-r--   0 christian  (1000) christian  (1000)     1839 2021-01-13 20:54:37.803129 btest-0.71/COPYING
--rw-r--r--   0 christian  (1000) christian  (1000)     8102 2021-11-01 19:09:30.243431 btest-0.71/MANIFEST
--rw-rw-r--   0 christian  (1000) christian  (1000)      204 2021-01-13 20:54:37.803129 btest-0.71/MANIFEST.in
--rw-rw-r--   0 christian  (1000) christian  (1000)      627 2021-01-13 20:54:37.803129 btest-0.71/Makefile
--rw-r--r--   0 christian  (1000) christian  (1000)      647 2021-11-01 19:09:30.254431 btest-0.71/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)    51652 2021-11-01 19:08:19.347336 btest-0.71/README
--rw-r--r--   0 christian  (1000) christian  (1000)        5 2021-11-01 19:08:19.324336 btest-0.71/VERSION
--rwxr-xr-x   0 christian  (1000) christian  (1000)    92028 2021-11-01 19:08:19.334336 btest-0.71/btest
--rwxr-xr-x   0 christian  (1000) christian  (1000)     1145 2021-10-07 19:01:44.170038 btest-0.71/btest-ask-update
--rwxr-xr-x   0 christian  (1000) christian  (1000)      708 2021-10-07 19:01:44.170038 btest-0.71/btest-bg-run
--rwxr-xr-x   0 christian  (1000) christian  (1000)      455 2021-10-07 19:01:44.171038 btest-0.71/btest-bg-run-helper
--rwxr-xr-x   0 christian  (1000) christian  (1000)     3107 2021-10-07 19:01:44.171038 btest-0.71/btest-bg-wait
--rwxr-xr-x   0 christian  (1000) christian  (1000)     7698 2021-10-07 19:01:44.171038 btest-0.71/btest-diff
--rwxr-xr-x   0 christian  (1000) christian  (1000)      892 2021-11-01 19:03:08.005313 btest-0.71/btest-progress
--rwxr-xr-x   0 christian  (1000) christian  (1000)      149 2021-10-07 19:01:44.171038 btest-0.71/btest-setsid
--rw-rw-r--   0 christian  (1000) christian  (1000)      386 2021-01-13 20:54:37.804129 btest-0.71/btest.cfg.example
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/examples/
--rw-rw-r--   0 christian  (1000) christian  (1000)      124 2021-01-13 20:54:37.804129 btest-0.71/examples/alternative
--rwxrwxr-x   0 christian  (1000) christian  (1000)       57 2021-01-13 20:54:37.804129 btest-0.71/examples/my-filter
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/examples/sphinx/
--rw-rw-r--   0 christian  (1000) christian  (1000)       21 2021-01-13 20:54:37.804129 btest-0.71/examples/sphinx/.gitignore
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.244432 btest-0.71/examples/sphinx/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/examples/sphinx/Baseline/tests.sphinx.hello-world/
--rw-r--r--   0 christian  (1000) christian  (1000)       61 2021-10-07 19:01:44.171038 btest-0.71/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#1
--rw-r--r--   0 christian  (1000) christian  (1000)       75 2021-10-07 19:01:44.171038 btest-0.71/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#2
--rw-r--r--   0 christian  (1000) christian  (1000)       89 2021-10-07 19:01:44.171038 btest-0.71/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#3
--rw-rw-r--   0 christian  (1000) christian  (1000)     5620 2021-01-13 20:54:37.804129 btest-0.71/examples/sphinx/Makefile
--rw-rw-r--   0 christian  (1000) christian  (1000)      209 2021-01-13 20:54:37.804129 btest-0.71/examples/sphinx/btest.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)     8021 2021-10-07 19:01:44.171038 btest-0.71/examples/sphinx/conf.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1316 2021-10-07 19:01:44.171038 btest-0.71/examples/sphinx/index.rst
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.244432 btest-0.71/examples/sphinx/tests/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/examples/sphinx/tests/sphinx/
--rw-rw-r--   0 christian  (1000) christian  (1000)       47 2021-01-13 20:54:37.804129 btest-0.71/examples/sphinx/tests/sphinx/hello-world.btest
--rw-rw-r--   0 christian  (1000) christian  (1000)       54 2021-01-13 20:54:37.804129 btest-0.71/examples/sphinx/tests/sphinx/hello-world.btest#2
--rw-rw-r--   0 christian  (1000) christian  (1000)       61 2021-01-13 20:54:37.804129 btest-0.71/examples/sphinx/tests/sphinx/hello-world.btest#3
--rw-rw-r--   0 christian  (1000) christian  (1000)       59 2021-01-13 20:54:37.804129 btest-0.71/examples/t1
--rw-rw-r--   0 christian  (1000) christian  (1000)       70 2021-01-13 20:54:37.804129 btest-0.71/examples/t2
--rw-rw-r--   0 christian  (1000) christian  (1000)       50 2021-01-13 20:54:37.804129 btest-0.71/examples/t3.sh
--rw-rw-r--   0 christian  (1000) christian  (1000)       93 2021-01-13 20:54:37.804129 btest-0.71/examples/t4.awk
--rw-r--r--   0 christian  (1000) christian  (1000)      158 2021-10-07 19:01:44.171038 btest-0.71/examples/t5.sh
--rw-rw-r--   0 christian  (1000) christian  (1000)      166 2021-01-13 20:54:37.804129 btest-0.71/examples/t6.sh
--rw-rw-r--   0 christian  (1000) christian  (1000)       92 2021-01-13 20:54:37.804129 btest-0.71/examples/t7
--rw-rw-r--   0 christian  (1000) christian  (1000)       44 2021-01-13 20:54:37.804129 btest-0.71/examples/t7.sh#1
--rw-rw-r--   0 christian  (1000) christian  (1000)       44 2021-01-13 20:54:37.804129 btest-0.71/examples/t7.sh#2
--rw-rw-r--   0 christian  (1000) christian  (1000)       32 2021-01-13 20:54:37.804129 btest-0.71/examples/t7.sh#3
--rw-r--r--   0 christian  (1000) christian  (1000)       78 2021-10-07 19:01:44.171038 btest-0.71/examples/unstable.sh
--rw-r--r--   0 christian  (1000) christian  (1000)     1285 2021-11-01 19:08:19.351336 btest-0.71/setup.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/sphinx/
--rwxr-xr-x   0 christian  (1000) christian  (1000)      426 2021-10-07 19:01:44.171038 btest-0.71/sphinx/btest-diff-rst
--rwxr-xr-x   0 christian  (1000) christian  (1000)     3534 2021-11-01 19:03:08.006312 btest-0.71/sphinx/btest-rst-cmd
--rwxr-xr-x   0 christian  (1000) christian  (1000)      410 2021-10-07 19:01:44.171038 btest-0.71/sphinx/btest-rst-include
--rwxr-xr-x   0 christian  (1000) christian  (1000)      156 2021-10-07 19:01:44.171038 btest-0.71/sphinx/btest-rst-pipe
--rw-r--r--   0 christian  (1000) christian  (1000)     7775 2021-10-07 19:01:44.171038 btest-0.71/sphinx/btest-sphinx.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/testing/
--rw-r--r--   0 christian  (1000) christian  (1000)        0 2021-11-01 19:07:00.127348 btest-0.71/testing/.btest.failed.dat
--rw-rw-r--   0 christian  (1000) christian  (1000)       32 2021-01-13 20:54:37.804129 btest-0.71/testing/.gitignore
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.246431 btest-0.71/testing/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/testing/Baseline/tests.abort-on-failure/
--rw-rw-r--   0 christian  (1000) christian  (1000)      255 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.abort-on-failure/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/testing/Baseline/tests.abort-on-failure-with-only-known-fails/
--rw-rw-r--   0 christian  (1000) christian  (1000)      347 2021-01-13 20:54:37.804129 btest-0.71/testing/Baseline/tests.abort-on-failure-with-only-known-fails/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/testing/Baseline/tests.alternatives-environment/
--rw-rw-r--   0 christian  (1000) christian  (1000)      294 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-environment/child-output
--rw-rw-r--   0 christian  (1000) christian  (1000)      431 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-environment/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/testing/Baseline/tests.alternatives-filter/
--rw-r--r--   0 christian  (1000) christian  (1000)      523 2021-10-07 19:01:44.171038 btest-0.71/testing/Baseline/tests.alternatives-filter/child-output
--rw-rw-r--   0 christian  (1000) christian  (1000)      221 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-filter/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.248432 btest-0.71/testing/Baseline/tests.alternatives-keywords/
--rw-rw-r--   0 christian  (1000) christian  (1000)      368 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-keywords/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.alternatives-substitution/
--rw-rw-r--   0 christian  (1000) christian  (1000)      136 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-substitution/child-output
--rw-rw-r--   0 christian  (1000) christian  (1000)      233 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-substitution/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.alternatives-testbase/
--rw-rw-r--   0 christian  (1000) christian  (1000)       58 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.alternatives-testbase/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.brief/
--rw-rw-r--   0 christian  (1000) christian  (1000)      138 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.brief/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      149 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.brief/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.btest-cfg/
--rw-rw-r--   0 christian  (1000) christian  (1000)      195 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.btest-cfg/abspath
--rw-rw-r--   0 christian  (1000) christian  (1000)      276 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.btest-cfg/nopath
--rw-rw-r--   0 christian  (1000) christian  (1000)      195 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.btest-cfg/relpath
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.console/
--rw-rw-r--   0 christian  (1000) christian  (1000)      119 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.console/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.crlf-line-terminators/
--rw-r--r--   0 christian  (1000) christian  (1000)      125 2021-08-23 21:12:55.622703 btest-0.71/testing/Baseline/tests.crlf-line-terminators/crlfs.dat
--rw-r--r--   0 christian  (1000) christian  (1000)      445 2021-08-23 21:12:55.622703 btest-0.71/testing/Baseline/tests.crlf-line-terminators/input
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.diag/
--rw-rw-r--   0 christian  (1000) christian  (1000)      732 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diag/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.diag-all/
--rw-rw-r--   0 christian  (1000) christian  (1000)      264 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diag-all/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.diag-file/
--rw-rw-r--   0 christian  (1000) christian  (1000)      216 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diag-file/diag
--rw-rw-r--   0 christian  (1000) christian  (1000)      155 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diag-file/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.diff-brief/
--rw-rw-r--   0 christian  (1000) christian  (1000)      471 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diff-brief/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.diff-max-lines/
--rw-rw-r--   0 christian  (1000) christian  (1000)      604 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diff-max-lines/output1
--rw-rw-r--   0 christian  (1000) christian  (1000)      690 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.diff-max-lines/output2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.doc/
--rw-rw-r--   0 christian  (1000) christian  (1000)      864 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.doc/md
--rw-rw-r--   0 christian  (1000) christian  (1000)      998 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.doc/rst
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.environment/
--rw-rw-r--   0 christian  (1000) christian  (1000)      717 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.environment/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.exit-codes/
--rw-rw-r--   0 christian  (1000) christian  (1000)      159 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.exit-codes/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      271 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.exit-codes/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.groups/
--rw-rw-r--   0 christian  (1000) christian  (1000)      476 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.groups/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.ignore/
--rw-rw-r--   0 christian  (1000) christian  (1000)      184 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.ignore/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.known-failure/
--rw-rw-r--   0 christian  (1000) christian  (1000)      342 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.known-failure/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.known-failure-and-success/
--rw-rw-r--   0 christian  (1000) christian  (1000)      208 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.known-failure-and-success/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.known-failure-succeeds/
--rw-rw-r--   0 christian  (1000) christian  (1000)      191 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.known-failure-succeeds/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.list/
--rw-r--r--   0 christian  (1000) christian  (1000)      124 2021-08-23 21:12:55.622703 btest-0.71/testing/Baseline/tests.list/out
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.macros/
--rw-rw-r--   0 christian  (1000) christian  (1000)      152 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.macros/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.249431 btest-0.71/testing/Baseline/tests.measure-time/
--rw-rw-r--   0 christian  (1000) christian  (1000)      504 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.measure-time/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.measure-time-options/
--rw-rw-r--   0 christian  (1000) christian  (1000)      640 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.measure-time-options/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.multiple-baseline-dirs/
--rw-rw-r--   0 christian  (1000) christian  (1000)      375 2021-01-13 20:54:37.805129 btest-0.71/testing/Baseline/tests.multiple-baseline-dirs/fail.log
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts/
--rw-rw-r--   0 christian  (1000) christian  (1000)      227 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.parts/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts-error-part/
--rw-rw-r--   0 christian  (1000) christian  (1000)      196 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.parts-error-part/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts-error-start-next/
--rw-rw-r--   0 christian  (1000) christian  (1000)      180 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.parts-error-start-next/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts-glob/
--rw-rw-r--   0 christian  (1000) christian  (1000)      243 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.parts-glob/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts-initializer-finalizer/
--rw-r--r--   0 christian  (1000) christian  (1000)      363 2021-11-01 19:03:30.131030 btest-0.71/testing/Baseline/tests.parts-initializer-finalizer/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts-skipping/
--rw-rw-r--   0 christian  (1000) christian  (1000)      179 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.parts-skipping/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.parts-teardown/
--rw-r--r--   0 christian  (1000) christian  (1000)      199 2021-11-01 19:03:30.140030 btest-0.71/testing/Baseline/tests.parts-teardown/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.progress/
--rw-rw-r--   0 christian  (1000) christian  (1000)      504 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.progress/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.progress-back-to-back/
--rw-rw-r--   0 christian  (1000) christian  (1000)      608 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.progress-back-to-back/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.quiet/
--rw-rw-r--   0 christian  (1000) christian  (1000)      115 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.quiet/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      129 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.quiet/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.requires/
--rw-rw-r--   0 christian  (1000) christian  (1000)      225 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.requires/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.requires-with-start-next/
--rw-rw-r--   0 christian  (1000) christian  (1000)      229 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.requires-with-start-next/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.rerun/
--rw-rw-r--   0 christian  (1000) christian  (1000)      202 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.rerun/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.sphinx.rst-cmd/
--rw-rw-r--   0 christian  (1000) christian  (1000)      926 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.sphinx.rst-cmd/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.sphinx.run-sphinx/
--rw-r--r--   0 christian  (1000) christian  (1000)     1390 2021-10-07 19:01:44.171038 btest-0.71/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.start-file/
--rw-rw-r--   0 christian  (1000) christian  (1000)      119 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.start-file/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.start-next/
--rw-r--r--   0 christian  (1000) christian  (1000)      125 2021-10-22 16:51:41.470356 btest-0.71/testing/Baseline/tests.start-next/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.start-next-dir/
--rw-rw-r--   0 christian  (1000) christian  (1000)      196 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.start-next-dir/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.statefile/
--rw-rw-r--   0 christian  (1000) christian  (1000)      115 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.statefile/mystate1
--rw-rw-r--   0 christian  (1000) christian  (1000)      121 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.statefile/mystate2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.statefile-sorted/
--rw-r--r--   0 christian  (1000) christian  (1000)      121 2021-08-23 21:12:55.622703 btest-0.71/testing/Baseline/tests.statefile-sorted/mystate
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.teardown/
--rw-r--r--   0 christian  (1000) christian  (1000)      271 2021-11-01 19:03:30.132030 btest-0.71/testing/Baseline/tests.teardown/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.testdirs/
--rw-rw-r--   0 christian  (1000) christian  (1000)      164 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.testdirs/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      154 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.testdirs/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.threads/
--rw-rw-r--   0 christian  (1000) christian  (1000)      188 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.threads/output.j0
--rw-rw-r--   0 christian  (1000) christian  (1000)      188 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.threads/output.j1
--rw-rw-r--   0 christian  (1000) christian  (1000)      120 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.threads/output.j5
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.250431 btest-0.71/testing/Baseline/tests.tracing/
--rw-rw-r--   0 christian  (1000) christian  (1000)      166 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.tracing/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Baseline/tests.unstable/
--rw-rw-r--   0 christian  (1000) christian  (1000)      256 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.unstable/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Baseline/tests.unstable-dir/
--rw-rw-r--   0 christian  (1000) christian  (1000)      280 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.unstable-dir/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Baseline/tests.verbose/
--rw-rw-r--   0 christian  (1000) christian  (1000)      354 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.verbose/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Baseline/tests.versioning/
--rw-rw-r--   0 christian  (1000) christian  (1000)      188 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.versioning/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Baseline/tests.xml/
--rw-rw-r--   0 christian  (1000) christian  (1000)      438 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.xml/output-j2.xml
--rw-rw-r--   0 christian  (1000) christian  (1000)      438 2021-01-13 20:54:37.806129 btest-0.71/testing/Baseline/tests.xml/output.xml
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.246431 btest-0.71/testing/Files/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Files/local_alternative/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.246431 btest-0.71/testing/Files/local_alternative/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/
--rw-r--r--   0 christian  (1000) christian  (1000)      330 2021-08-23 21:12:55.623703 btest-0.71/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/
--rw-r--r--   0 christian  (1000) christian  (1000)      255 2021-08-23 21:12:55.623703 btest-0.71/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/
--rw-r--r--   0 christian  (1000) christian  (1000)       34 2021-08-23 21:12:55.623703 btest-0.71/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/output
--rw-r--r--   0 christian  (1000) christian  (1000)      389 2021-10-07 19:01:44.171038 btest-0.71/testing/Files/local_alternative/btest.tests.cfg
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Files/local_alternative/tests/
--rw-r--r--   0 christian  (1000) christian  (1000)      116 2021-10-07 19:01:44.171038 btest-0.71/testing/Files/local_alternative/tests/local-alternative-found.test
--rw-r--r--   0 christian  (1000) christian  (1000)      234 2021-10-07 19:01:44.171038 btest-0.71/testing/Files/local_alternative/tests/local-alternative-show-env.test
--rw-r--r--   0 christian  (1000) christian  (1000)      201 2021-08-23 21:12:55.623703 btest-0.71/testing/Files/local_alternative/tests/local-alternative-show-test-baseline.test
--rw-r--r--   0 christian  (1000) christian  (1000)      200 2021-08-23 21:12:55.623703 btest-0.71/testing/Files/local_alternative/tests/local-alternative-show-testbase.test
--rw-r--r--   0 christian  (1000) christian  (1000)      236 2021-11-01 19:03:08.006312 btest-0.71/testing/Makefile
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.251431 btest-0.71/testing/Scripts/
--rwxrwxr-x   0 christian  (1000) christian  (1000)      124 2021-01-13 20:54:37.807129 btest-0.71/testing/Scripts/diff-remove-abspath
--rw-rw-r--   0 christian  (1000) christian  (1000)       48 2021-01-13 20:54:37.807129 btest-0.71/testing/Scripts/dummy-script
--rwxrwxr-x   0 christian  (1000) christian  (1000)      253 2021-01-13 20:54:37.807129 btest-0.71/testing/Scripts/script-command
--rwxrwxr-x   0 christian  (1000) christian  (1000)      121 2021-01-13 20:54:37.807129 btest-0.71/testing/Scripts/strip-iso8601-date
--rwxr-xr-x   0 christian  (1000) christian  (1000)      104 2021-10-07 19:01:44.172038 btest-0.71/testing/Scripts/strip-test-base
--rwxrwxr-x   0 christian  (1000) christian  (1000)       74 2021-01-13 20:54:37.807129 btest-0.71/testing/Scripts/test-filter
--rwxr-xr-x   0 christian  (1000) christian  (1000)      849 2021-10-07 19:01:44.172038 btest-0.71/testing/Scripts/test-perf
--rw-rw-r--   0 christian  (1000) christian  (1000)      518 2021-01-13 20:54:37.807129 btest-0.71/testing/btest.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)      548 2021-10-19 20:32:21.698171 btest-0.71/testing/btest.tests.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)        0 2021-11-01 19:06:51.285461 btest-0.71/testing/diag.log
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.253431 btest-0.71/testing/tests/
--rw-r--r--   0 christian  (1000) christian  (1000)      645 2021-11-01 19:03:08.007312 btest-0.71/testing/tests/abort-on-failure-with-only-known-fails.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      495 2021-11-01 19:03:08.007312 btest-0.71/testing/tests/abort-on-failure.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      599 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/alternatives-baseline-dir.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      428 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/alternatives-environment.test
--rw-r--r--   0 christian  (1000) christian  (1000)      204 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/alternatives-filter.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      678 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/alternatives-keywords.test
--rw-r--r--   0 christian  (1000) christian  (1000)      161 2021-08-23 21:12:55.623703 btest-0.71/testing/tests/alternatives-overwrite-env.test
--rw-r--r--   0 christian  (1000) christian  (1000)      132 2021-08-23 21:12:55.624703 btest-0.71/testing/tests/alternatives-reread-config-baselinedir.test
--rw-r--r--   0 christian  (1000) christian  (1000)      122 2021-08-23 21:12:55.624703 btest-0.71/testing/tests/alternatives-reread-config.test
--rw-r--r--   0 christian  (1000) christian  (1000)      247 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/alternatives-substitution.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      116 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/alternatives-testbase.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      548 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/baseline-dir-env.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      208 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/basic-fail.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      203 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/basic-succeed.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1214 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/binary-mode.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      310 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/brief.test
--rw-r--r--   0 christian  (1000) christian  (1000)      696 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/btest-cfg.test
--rw-r--r--   0 christian  (1000) christian  (1000)      710 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/canonifier-cmdline.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1746 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/canonifier-conversion.test
--rw-r--r--   0 christian  (1000) christian  (1000)      593 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/canonifier-fail.test
--rw-r--r--   0 christian  (1000) christian  (1000)      374 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/canonifier.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1089 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/console.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      174 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/copy-file.test
--rw-r--r--   0 christian  (1000) christian  (1000)      382 2021-08-23 21:12:55.624703 btest-0.71/testing/tests/crlf-line-terminators.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      321 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/diag-all.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      170 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/diag-file.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      330 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/diag.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      519 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/diff-brief.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      799 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/diff-max-lines.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      364 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/diff.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     2134 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/doc.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1005 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/environment.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1160 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/exit-codes.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      224 2021-10-21 23:20:39.646309 btest-0.71/testing/tests/finalizer.test
--rw-r--r--   0 christian  (1000) christian  (1000)      772 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/groups.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      897 2021-01-13 20:54:37.807129 btest-0.71/testing/tests/ignore.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      234 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/initializer.test
--rw-r--r--   0 christian  (1000) christian  (1000)      175 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/known-failure-and-success.btest
--rw-rw-r--   0 christian  (1000) christian  (1000)      189 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/known-failure-succeeds.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      266 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/known-failure.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      259 2021-08-23 21:12:55.624703 btest-0.71/testing/tests/list.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      223 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/macros.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1659 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/measure-time-options.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1078 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/measure-time.tests
--rw-rw-r--   0 christian  (1000) christian  (1000)     1182 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/multiple-baseline-dirs.test
--rw-r--r--   0 christian  (1000) christian  (1000)      168 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/parts-error-part.test
--rw-r--r--   0 christian  (1000) christian  (1000)      285 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/parts-error-start-next.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      501 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/parts-glob.test
--rw-r--r--   0 christian  (1000) christian  (1000)      821 2021-11-01 19:03:30.140030 btest-0.71/testing/tests/parts-initializer-finalizer.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      355 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/parts-skipping.tests
--rw-r--r--   0 christian  (1000) christian  (1000)      801 2021-11-01 19:03:30.132030 btest-0.71/testing/tests/parts-teardown.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      468 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/parts.tests
--rw-rw-r--   0 christian  (1000) christian  (1000)      267 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/ports.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      569 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/progress-back-to-back.test
--rw-r--r--   0 christian  (1000) christian  (1000)      575 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/progress.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      310 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/quiet.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      433 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/requires-with-start-next.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      447 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/requires.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      287 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/rerun.test
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2021-11-01 19:09:30.254431 btest-0.71/testing/tests/sphinx/
--rwxr-xr-x   0 christian  (1000) christian  (1000)      450 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/sphinx/rst-cmd.sh
--rw-r--r--   0 christian  (1000) christian  (1000)      178 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/sphinx/run-sphinx
--rw-r--r--   0 christian  (1000) christian  (1000)      301 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/start-file.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      222 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/start-next-dir.test
--rw-r--r--   0 christian  (1000) christian  (1000)      388 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/start-next-naming.test
--rw-r--r--   0 christian  (1000) christian  (1000)      245 2021-10-22 16:51:41.470356 btest-0.71/testing/tests/start-next.test
--rw-r--r--   0 christian  (1000) christian  (1000)      480 2021-11-01 19:03:08.007312 btest-0.71/testing/tests/statefile-sorted.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      545 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/statefile.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1277 2021-11-01 19:03:30.132030 btest-0.71/testing/tests/teardown.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      227 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/test-base.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      383 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/testdirs.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1662 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/threads.test
--rw-r--r--   0 christian  (1000) christian  (1000)      111 2021-10-07 19:01:44.172038 btest-0.71/testing/tests/tmps.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      417 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/tracing.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      864 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/unstable-dir.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      476 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/unstable.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      291 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/verbose.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      405 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/versioning.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      709 2021-01-13 20:54:37.808129 btest-0.71/testing/tests/xml.test
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.225184 btest-1.0/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.184184 btest-1.0/Baseline/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t4/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1252 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t4/dots
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t5/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        9 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t5/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t5-2/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        9 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t5-2/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t6/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        2 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t6/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t7/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      132 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t7/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.unstable/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        2 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.unstable/output
+-rw-r--r--   0 christian  (1000) christian  (1000)    43286 2023-04-11 23:48:59.000000 btest-1.0/CHANGES
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1839 2020-10-05 17:46:07.000000 btest-1.0/COPYING
+-rw-rw-r--   0 christian  (1000) christian  (1000)      204 2020-10-05 17:46:07.000000 btest-1.0/MANIFEST.in
+-rw-r--r--   0 christian  (1000) christian  (1000)      627 2020-12-01 21:37:29.000000 btest-1.0/Makefile
+-rw-r--r--   0 christian  (1000) christian  (1000)      661 2023-04-11 23:52:04.225184 btest-1.0/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)    53701 2023-04-11 23:48:59.000000 btest-1.0/README
+-rw-r--r--   0 christian  (1000) christian  (1000)        4 2023-04-11 23:48:59.000000 btest-1.0/VERSION
+-rwxr-xr-x   0 christian  (1000) christian  (1000)   103196 2023-04-11 23:48:59.000000 btest-1.0/btest
+-rwxr-xr-x   0 christian  (1000) christian  (1000)     1145 2021-10-25 23:17:40.000000 btest-1.0/btest-ask-update
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      708 2021-10-25 23:17:40.000000 btest-1.0/btest-bg-run
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      455 2021-10-25 23:17:40.000000 btest-1.0/btest-bg-run-helper
+-rwxr-xr-x   0 christian  (1000) christian  (1000)     3107 2021-10-25 23:17:40.000000 btest-1.0/btest-bg-wait
+-rwxr-xr-x   0 christian  (1000) christian  (1000)     7836 2023-01-24 20:15:29.000000 btest-1.0/btest-diff
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      892 2021-10-25 23:17:40.000000 btest-1.0/btest-progress
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      158 2023-02-01 03:00:52.000000 btest-1.0/btest-setsid
+-rw-rw-r--   0 christian  (1000) christian  (1000)      386 2020-10-20 16:43:55.000000 btest-1.0/btest.cfg.example
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.191184 btest-1.0/examples/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      124 2020-10-05 17:46:07.000000 btest-1.0/examples/alternative
+-rwxrwxr-x   0 christian  (1000) christian  (1000)       57 2020-10-05 17:46:07.000000 btest-1.0/examples/my-filter
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.192184 btest-1.0/examples/sphinx/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       21 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/.gitignore
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.185184 btest-1.0/examples/sphinx/Baseline/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.193184 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/
+-rw-r--r--   0 christian  (1000) christian  (1000)       61 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#1
+-rw-r--r--   0 christian  (1000) christian  (1000)       75 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#2
+-rw-r--r--   0 christian  (1000) christian  (1000)       89 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#3
+-rw-rw-r--   0 christian  (1000) christian  (1000)     5620 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/Makefile
+-rw-rw-r--   0 christian  (1000) christian  (1000)      209 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/btest.cfg
+-rw-r--r--   0 christian  (1000) christian  (1000)     8021 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/conf.py
+-rw-r--r--   0 christian  (1000) christian  (1000)     1316 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/index.rst
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.185184 btest-1.0/examples/sphinx/tests/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.193184 btest-1.0/examples/sphinx/tests/sphinx/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       47 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/tests/sphinx/hello-world.btest
+-rw-rw-r--   0 christian  (1000) christian  (1000)       54 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/tests/sphinx/hello-world.btest#2
+-rw-rw-r--   0 christian  (1000) christian  (1000)       61 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/tests/sphinx/hello-world.btest#3
+-rw-rw-r--   0 christian  (1000) christian  (1000)       59 2020-10-05 17:46:07.000000 btest-1.0/examples/t1
+-rw-rw-r--   0 christian  (1000) christian  (1000)       70 2020-10-05 17:46:07.000000 btest-1.0/examples/t2
+-rw-rw-r--   0 christian  (1000) christian  (1000)       50 2020-10-05 17:46:07.000000 btest-1.0/examples/t3.sh
+-rw-rw-r--   0 christian  (1000) christian  (1000)       93 2020-10-05 17:46:07.000000 btest-1.0/examples/t4.awk
+-rw-r--r--   0 christian  (1000) christian  (1000)      158 2021-10-25 23:17:40.000000 btest-1.0/examples/t5.sh
+-rw-rw-r--   0 christian  (1000) christian  (1000)      166 2020-10-05 17:46:07.000000 btest-1.0/examples/t6.sh
+-rw-rw-r--   0 christian  (1000) christian  (1000)       92 2020-10-05 17:46:07.000000 btest-1.0/examples/t7
+-rw-rw-r--   0 christian  (1000) christian  (1000)       44 2020-10-05 17:46:07.000000 btest-1.0/examples/t7.sh#1
+-rw-rw-r--   0 christian  (1000) christian  (1000)       44 2020-10-05 17:46:07.000000 btest-1.0/examples/t7.sh#2
+-rw-rw-r--   0 christian  (1000) christian  (1000)       32 2020-10-05 17:46:07.000000 btest-1.0/examples/t7.sh#3
+-rw-r--r--   0 christian  (1000) christian  (1000)       78 2021-10-25 23:17:40.000000 btest-1.0/examples/unstable.sh
+-rw-r--r--   0 christian  (1000) christian  (1000)      120 2023-04-11 23:52:04.225184 btest-1.0/setup.cfg
+-rw-r--r--   0 christian  (1000) christian  (1000)     1555 2023-04-11 23:48:59.000000 btest-1.0/setup.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.194184 btest-1.0/sphinx/
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      426 2021-10-25 23:17:40.000000 btest-1.0/sphinx/btest-diff-rst
+-rwxr-xr-x   0 christian  (1000) christian  (1000)     3534 2022-03-07 20:08:30.000000 btest-1.0/sphinx/btest-rst-cmd
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      410 2021-10-25 23:17:40.000000 btest-1.0/sphinx/btest-rst-include
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      156 2021-10-25 23:17:40.000000 btest-1.0/sphinx/btest-rst-pipe
+-rw-r--r--   0 christian  (1000) christian  (1000)     7665 2023-02-01 03:00:52.000000 btest-1.0/sphinx/btest-sphinx.py
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/sphinx/btest.egg-info/
+-rw-r--r--   0 christian  (1000) christian  (1000)      661 2023-04-11 23:52:03.000000 btest-1.0/sphinx/btest.egg-info/PKG-INFO
+-rw-r--r--   0 christian  (1000) christian  (1000)     8675 2023-04-11 23:52:04.000000 btest-1.0/sphinx/btest.egg-info/SOURCES.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)        1 2023-04-11 23:52:03.000000 btest-1.0/sphinx/btest.egg-info/dependency_links.txt
+-rw-r--r--   0 christian  (1000) christian  (1000)       13 2023-04-11 23:52:04.000000 btest-1.0/sphinx/btest.egg-info/top_level.txt
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/testing/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       32 2020-10-05 17:46:07.000000 btest-1.0/testing/.gitignore
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.186184 btest-1.0/testing/Baseline/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/testing/Baseline/tests.abort-on-failure/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      255 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.abort-on-failure/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/testing/Baseline/tests.abort-on-failure-with-only-known-fails/
+-rw-r--r--   0 christian  (1000) christian  (1000)      347 2020-12-07 16:45:09.000000 btest-1.0/testing/Baseline/tests.abort-on-failure-with-only-known-fails/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.196184 btest-1.0/testing/Baseline/tests.alternatives-environment/
+-rw-r--r--   0 christian  (1000) christian  (1000)      321 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-environment/child-output
+-rw-r--r--   0 christian  (1000) christian  (1000)      463 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-environment/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.196184 btest-1.0/testing/Baseline/tests.alternatives-filter/
+-rw-r--r--   0 christian  (1000) christian  (1000)      523 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.alternatives-filter/child-output
+-rw-rw-r--   0 christian  (1000) christian  (1000)      221 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.alternatives-filter/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.196184 btest-1.0/testing/Baseline/tests.alternatives-keywords/
+-rw-r--r--   0 christian  (1000) christian  (1000)      289 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-keywords/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.alternatives-substitution/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      136 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.alternatives-substitution/child-output
+-rw-rw-r--   0 christian  (1000) christian  (1000)      233 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.alternatives-substitution/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.alternatives-testbase/
+-rw-rw-r--   0 christian  (1000) christian  (1000)       58 2020-10-05 17:46:07.000000 btest-1.0/testing/Baseline/tests.alternatives-testbase/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.alternatives-undefined/
+-rw-r--r--   0 christian  (1000) christian  (1000)      154 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-undefined/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.brief/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      138 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.brief/out1
+-rw-rw-r--   0 christian  (1000) christian  (1000)      149 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.brief/out2
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.198184 btest-1.0/testing/Baseline/tests.btest-cfg/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      195 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.btest-cfg/abspath
+-rw-rw-r--   0 christian  (1000) christian  (1000)      276 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.btest-cfg/nopath
+-rw-rw-r--   0 christian  (1000) christian  (1000)      195 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.btest-cfg/relpath
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.198184 btest-1.0/testing/Baseline/tests.console/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      119 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.console/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.198184 btest-1.0/testing/Baseline/tests.crlf-line-terminators/
+-rw-r--r--   0 christian  (1000) christian  (1000)      125 2021-05-10 05:01:31.000000 btest-1.0/testing/Baseline/tests.crlf-line-terminators/crlfs.dat
+-rw-r--r--   0 christian  (1000) christian  (1000)      445 2021-05-10 05:01:31.000000 btest-1.0/testing/Baseline/tests.crlf-line-terminators/input
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diag/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      732 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diag-all/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      264 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag-all/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diag-file/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      216 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag-file/diag
+-rw-rw-r--   0 christian  (1000) christian  (1000)      155 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag-file/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diff-brief/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      471 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diff-brief/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.diff-max-lines/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      604 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diff-max-lines/output1
+-rw-rw-r--   0 christian  (1000) christian  (1000)      690 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diff-max-lines/output2
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.doc/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      864 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.doc/md
+-rw-rw-r--   0 christian  (1000) christian  (1000)      998 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.doc/rst
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.environment/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      717 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.environment/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.environment-windows/
+-rw-r--r--   0 christian  (1000) christian  (1000)      845 2023-01-24 20:15:29.000000 btest-1.0/testing/Baseline/tests.environment-windows/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.exit-codes/
+-rw-r--r--   0 christian  (1000) christian  (1000)      159 2020-12-03 19:18:53.000000 btest-1.0/testing/Baseline/tests.exit-codes/out1
+-rw-r--r--   0 christian  (1000) christian  (1000)      271 2020-12-07 16:45:09.000000 btest-1.0/testing/Baseline/tests.exit-codes/out2
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.groups/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      476 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.groups/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.ignore/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      184 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.ignore/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.known-failure/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      342 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.known-failure/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.known-failure-and-success/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      208 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.known-failure-and-success/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.known-failure-succeeds/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      191 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.known-failure-succeeds/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.list/
+-rw-r--r--   0 christian  (1000) christian  (1000)      124 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.list/out
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.macros/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      152 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.macros/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.measure-time/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      504 2020-10-05 17:46:07.000000 btest-1.0/testing/Baseline/tests.measure-time/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.measure-time-options/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      640 2020-10-05 17:46:07.000000 btest-1.0/testing/Baseline/tests.measure-time-options/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.multiple-baseline-dirs/
+-rw-r--r--   0 christian  (1000) christian  (1000)      375 2020-12-01 21:37:42.000000 btest-1.0/testing/Baseline/tests.multiple-baseline-dirs/fail.log
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.parts/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      227 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.parts-error-part/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      196 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-error-part/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-error-start-next/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      180 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-error-start-next/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-glob/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      243 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-glob/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-initializer-finalizer/
+-rw-r--r--   0 christian  (1000) christian  (1000)      363 2022-03-07 20:08:30.000000 btest-1.0/testing/Baseline/tests.parts-initializer-finalizer/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-skipping/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      179 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-skipping/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-teardown/
+-rw-r--r--   0 christian  (1000) christian  (1000)      199 2022-03-07 20:08:30.000000 btest-1.0/testing/Baseline/tests.parts-teardown/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.progress/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      504 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.progress/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.progress-back-to-back/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      608 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.progress-back-to-back/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.quiet/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      115 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.quiet/out1
+-rw-rw-r--   0 christian  (1000) christian  (1000)      129 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.quiet/out2
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.requires/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      225 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.requires/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.requires-with-start-next/
+-rw-r--r--   0 christian  (1000) christian  (1000)      229 2021-05-10 05:01:31.000000 btest-1.0/testing/Baseline/tests.requires-with-start-next/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.rerun/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      202 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.rerun/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.set-key/
+-rw-r--r--   0 christian  (1000) christian  (1000)       28 2023-01-24 20:15:29.000000 btest-1.0/testing/Baseline/tests.set-key/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.sphinx.rst-cmd/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      926 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.sphinx.rst-cmd/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.sphinx.run-sphinx/
+-rw-r--r--   0 christian  (1000) christian  (1000)     1390 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.start-file/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      119 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.start-file/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.start-next/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      125 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.start-next/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.start-next-dir/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      196 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.start-next-dir/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.statefile/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      115 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.statefile/mystate1
+-rw-rw-r--   0 christian  (1000) christian  (1000)      121 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.statefile/mystate2
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.206184 btest-1.0/testing/Baseline/tests.statefile-sorted/
+-rw-r--r--   0 christian  (1000) christian  (1000)      121 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.statefile-sorted/mystate
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.206184 btest-1.0/testing/Baseline/tests.teardown/
+-rw-r--r--   0 christian  (1000) christian  (1000)      271 2022-03-07 20:08:30.000000 btest-1.0/testing/Baseline/tests.teardown/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.206184 btest-1.0/testing/Baseline/tests.testdirs/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      164 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.testdirs/out1
+-rw-rw-r--   0 christian  (1000) christian  (1000)      154 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.testdirs/out2
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.threads/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      188 2020-12-02 21:16:24.000000 btest-1.0/testing/Baseline/tests.threads/output.j0
+-rw-r--r--   0 christian  (1000) christian  (1000)      188 2020-12-07 16:45:09.000000 btest-1.0/testing/Baseline/tests.threads/output.j1
+-rw-rw-r--   0 christian  (1000) christian  (1000)      120 2020-12-02 21:16:24.000000 btest-1.0/testing/Baseline/tests.threads/output.j5
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.tracing/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      166 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.tracing/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.unstable/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      256 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.unstable/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.unstable-dir/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      280 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.unstable-dir/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.unstable-subtest/
+-rw-r--r--   0 christian  (1000) christian  (1000)      209 2023-02-01 23:09:39.000000 btest-1.0/testing/Baseline/tests.unstable-subtest/.stderr
+-rw-r--r--   0 christian  (1000) christian  (1000)      261 2023-02-01 23:09:39.000000 btest-1.0/testing/Baseline/tests.unstable-subtest/diag
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Baseline/tests.verbose/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      354 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.verbose/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Baseline/tests.versioning/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      188 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.versioning/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Baseline/tests.xml/
+-rw-rw-r--   0 christian  (1000) christian  (1000)      438 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.xml/output-j2.xml
+-rw-rw-r--   0 christian  (1000) christian  (1000)      438 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.xml/output.xml
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.186184 btest-1.0/testing/Files/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Files/local_alternative/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.186184 btest-1.0/testing/Files/local_alternative/Baseline/
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/
+-rw-r--r--   0 christian  (1000) christian  (1000)      330 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.209184 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/
+-rw-r--r--   0 christian  (1000) christian  (1000)      255 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/output
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.209184 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/
+-rw-r--r--   0 christian  (1000) christian  (1000)       34 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/output
+-rw-r--r--   0 christian  (1000) christian  (1000)      389 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/btest.tests.cfg
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.209184 btest-1.0/testing/Files/local_alternative/tests/
+-rw-r--r--   0 christian  (1000) christian  (1000)      116 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-found.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      234 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-show-env.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      201 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-show-test-baseline.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      200 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-show-testbase.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      236 2022-03-07 20:08:30.000000 btest-1.0/testing/Makefile
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.211184 btest-1.0/testing/Scripts/
+-rw-r--r--   0 christian  (1000) christian  (1000)      359 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/convert-path-list.sh
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      134 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/diff-remove-abspath
+-rw-rw-r--   0 christian  (1000) christian  (1000)       48 2020-10-05 17:46:07.000000 btest-1.0/testing/Scripts/dummy-script
+-rw-r--r--   0 christian  (1000) christian  (1000)      153 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/is-windows
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      438 2023-01-26 00:06:26.000000 btest-1.0/testing/Scripts/script-command
+-rwxrwxr-x   0 christian  (1000) christian  (1000)      121 2020-10-05 17:46:07.000000 btest-1.0/testing/Scripts/strip-iso8601-date
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      352 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/strip-test-base
+-rwxrwxr-x   0 christian  (1000) christian  (1000)       74 2020-10-05 17:46:07.000000 btest-1.0/testing/Scripts/test-filter
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      849 2021-10-25 23:17:40.000000 btest-1.0/testing/Scripts/test-perf
+-rw-r--r--   0 christian  (1000) christian  (1000)      548 2023-01-24 20:15:29.000000 btest-1.0/testing/btest.cfg
+-rw-r--r--   0 christian  (1000) christian  (1000)      593 2023-01-24 20:15:29.000000 btest-1.0/testing/btest.tests.cfg
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.224184 btest-1.0/testing/tests/
+-rw-r--r--   0 christian  (1000) christian  (1000)      645 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/abort-on-failure-with-only-known-fails.btest
+-rw-r--r--   0 christian  (1000) christian  (1000)      495 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/abort-on-failure.btest
+-rw-r--r--   0 christian  (1000) christian  (1000)      599 2023-01-24 23:11:59.000000 btest-1.0/testing/tests/alternatives-baseline-dir.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      428 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/alternatives-environment.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      204 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-filter.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      598 2022-12-07 22:09:21.000000 btest-1.0/testing/tests/alternatives-keywords.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      161 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-overwrite-env.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      132 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-reread-config-baselinedir.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      122 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-reread-config.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      247 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-substitution.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      116 2021-10-25 23:17:37.000000 btest-1.0/testing/tests/alternatives-testbase.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      273 2022-12-07 22:09:21.000000 btest-1.0/testing/tests/alternatives-undefined.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      548 2020-12-01 21:37:42.000000 btest-1.0/testing/tests/baseline-dir-env.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      208 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/basic-fail.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      203 2020-12-05 00:33:59.000000 btest-1.0/testing/tests/basic-succeed.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1214 2023-01-24 21:25:18.000000 btest-1.0/testing/tests/binary-mode.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      310 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/brief.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      696 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/btest-cfg.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      710 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier-cmdline.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1746 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier-conversion.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      593 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier-fail.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      374 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1089 2023-01-25 01:24:24.000000 btest-1.0/testing/tests/console.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      174 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/copy-file.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      382 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/crlf-line-terminators.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      321 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diag-all.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      170 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diag-file.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      330 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diag.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      519 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diff-brief.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      799 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diff-max-lines.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      364 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diff.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)     2134 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/doc.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      250 2022-11-28 06:30:41.000000 btest-1.0/testing/tests/duplicate-selection.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      619 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/env-var-casing.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1101 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/environment-windows.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1047 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/environment.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1160 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/exit-codes.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      224 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/finalizer.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      772 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/groups.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      897 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/ignore.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      234 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/initializer.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      175 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/known-failure-and-success.btest
+-rw-rw-r--   0 christian  (1000) christian  (1000)      189 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/known-failure-succeeds.btest
+-rw-r--r--   0 christian  (1000) christian  (1000)      266 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/known-failure.btest
+-rw-r--r--   0 christian  (1000) christian  (1000)      259 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/list.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      223 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/macros.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1659 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/measure-time-options.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1078 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/measure-time.tests
+-rw-r--r--   0 christian  (1000) christian  (1000)     1202 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/multiple-baseline-dirs.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      168 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/parts-error-part.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      285 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/parts-error-start-next.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      501 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/parts-glob.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      821 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/parts-initializer-finalizer.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      355 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/parts-skipping.tests
+-rw-r--r--   0 christian  (1000) christian  (1000)      801 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/parts-teardown.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      468 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/parts.tests
+-rw-rw-r--   0 christian  (1000) christian  (1000)      267 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/ports.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      569 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/progress-back-to-back.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      575 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/progress.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      310 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/quiet.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      433 2021-05-10 05:01:31.000000 btest-1.0/testing/tests/requires-with-start-next.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      447 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/requires.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      287 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/rerun.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      248 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/set-key.test
+drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.225184 btest-1.0/testing/tests/sphinx/
+-rwxr-xr-x   0 christian  (1000) christian  (1000)      490 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/sphinx/rst-cmd.sh
+-rw-r--r--   0 christian  (1000) christian  (1000)      220 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/sphinx/run-sphinx
+-rw-r--r--   0 christian  (1000) christian  (1000)      301 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/start-file.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      222 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/start-next-dir.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      388 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/start-next-naming.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      245 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/start-next.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      480 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/statefile-sorted.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      545 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/statefile.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1277 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/teardown.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      227 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/test-base.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      383 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/testdirs.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1662 2020-12-07 16:45:09.000000 btest-1.0/testing/tests/threads.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      111 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/tmps.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      418 2022-11-28 06:30:41.000000 btest-1.0/testing/tests/tracing.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      864 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/unstable-dir.test
+-rw-r--r--   0 christian  (1000) christian  (1000)     1093 2023-02-01 23:09:39.000000 btest-1.0/testing/tests/unstable-subtest.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      476 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/unstable.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      291 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/verbose.test
+-rw-r--r--   0 christian  (1000) christian  (1000)      405 2022-12-09 22:08:00.000000 btest-1.0/testing/tests/versioning.test
+-rw-rw-r--   0 christian  (1000) christian  (1000)      709 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/xml.test
```

### Comparing `btest-0.71/Baseline/examples.t4/dots` & `btest-1.0/Baseline/examples.t4/dots`

 * *Files identical despite different names*

### Comparing `btest-0.71/CHANGES` & `btest-1.0/CHANGES`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,200 @@
+1.0 | 2023-02-01 16:07:31 -0700
+
+  * Release 1.0.
+
+0.72-71 | 2023-02-01 16:07:09 -0700
+
+  * Fix test cloning bug that caused "subtests" to run without numeric suffix (Christian Kreibich, Corelight)
+
+    When running with retries, failing tests created via @TEST-START-NEXT were
+    cloned for retry in a way that lost their numeric suffix, which could cause
+    btest to consult the wrong baselines.
+
+  * Add testcase for retried subtests (Christian Kreibich, Corelight)
+
+    This highlights a bug in which a subtest (via @TEST-START-NEXT) other than the
+    first always gets retried as the first, but with the wrong baseline.
+
+0.72-68 | 2023-01-31 18:29:53 -0800
+
+  * Automated code formatting and modernization (Christian Kreibich, Corelight)
+
+    - Final touches on top of automated reformatting.
+    - setup.cfg/pre-commit-config: Add flake8 hook and config
+    - Minor tweaks in preparation for flake8
+    - Automatically update Python sources to use python-3.7 syntax
+    - Minor tweaks to clue in pyupgrade
+    - Add `.git-blame-ignore-revs` file.
+    - Reformat Python code with Black.
+    - Minor Python tweaks in anticipation of reformatting
+    - Minor indentation tweak in pre-commit config
+    - Modernize action versions in pre-commit workflow
+    - Don't ignore the sphinx folder, it has revision-controlled content
+    - Remove unused .travis.yml setup
+
+0.72-55 | 2023-01-25 16:06:26 -0800
+
+  * Whitespace-align the thread prefixes in output handlers (Christian Kreibich, Corelight)
+
+  * Prevent output garbling when running with "-A -j" (Christian Kreibich, Corelight)
+
+  * Switch Console and CompactConsole to using base class's output file member (Christian Kreibich, Corelight)
+
+  * Make OutputHandler's default output file a constructor argument (Christian Kreibich, Corelight)
+
+  * Prevent console.test from garbling output (Christian Kreibich, Corelight)
+
+  * Comment-only tweaks, no other change (Christian Kreibich, Corelight)
+
+0.72-48 | 2023-01-13 15:53:55 -0700
+
+  * Add Windows Caveats to README, add bash.exe check at startup (Tim Wojtulewicz)
+
+  * Add tests.environment-windows btest (Tim Wojtulewicz)
+
+    The original tests.environment btest doesn't work on Windows due to some
+    path differences in the output. This adds a new test that does the same
+    things except does some additional conversions in the test script itself
+    to remove those differences.
+
+  * Open .stdout and .stderr in append mode (Tim Wojtulewicz)
+
+    This fixes a problem on Windows where multiple TEST-EXEC statements in a
+    test could cause those files to be overwritten by subsequent TEST-EXECs,
+    causing failures.
+
+  * Fix tests.multiple-baseline-dirs btest to use pathsep (Tim Wojtulewicz)
+
+  * Fix strip-test-base script to handle Windows paths correctly (Tim Wojtulewicz)
+
+  * Fix diff-remove-abspath to handle Windows drive letters (Tim Wojtulewicz)
+
+  * Add testing script to check for Windows, use it to disable some tests (Tim Wojtulewicz)
+
+  * Return error if trying to use Sphinx features on Windows (Tim Wojtulewicz)
+
+  * Force output to use unix-style line endings for consistency (Tim Wojtulewicz)
+
+  * Use binascii.crc32 for computing hashes for TEST-SERIALIZE commands (Tim Wojtulewicz)
+
+    Windows has some issue where `hash()` returns different values for the
+    same string in the different child processes. crc32() returns the same
+    values in each.
+
+  * Rework how test processes are called on Windows (Tim Wojtulewicz)
+
+    This changes how runSubprocess works on Windows to insert all of the
+    calls within a temporary bash script. This ensures that the entire
+    environment is available when running the processes, which doesn't
+    work when simply calling subprocess.check_call().
+
+  * Fix an error when attempting to delete the tmp dirs on Windows (Tim Wojtulewicz)
+
+  * Rebuild globals() table in child processes on Windows (Tim Wojtulewicz)
+
+    Using the 'spawn' method for multiprocessing causes the global
+    state to get lost when moving from the parent into the child
+    processes. Rebuilding it by looping over a subset and reinserting
+    them into globals() ensures that they exist.
+
+  * Move option parsing to a method (Tim Wojtulewicz)
+
+  * Use named pipes on Windows since AF_UNIX is not supported (Tim Wojtulewicz)
+
+  * Fix running tests with dot-notation for their name (Tim Wojtulewicz)
+
+  * Add method for normalizing paths on both Windows and POSIX (Tim Wojtulewicz)
+
+  * Avoid isinstance() to determine whether a cmd is a CmdSeq (Christian Kreibich, Corelight)
+
+    As per the comment, some serializer/unserializers don't produce the identical
+    type when unserializing, failing isinstance().
+
+  * Add -s/--set command-line argument for overriding config defaults (Tim Wojtulewicz)
+
+  * Switch to https://pypi.org/project/multiprocess/ on Windows (Tim Wojtulewicz)
+
+    The reason for this switch is primarily because the stock
+    multiprocessing library has very poor support for pickling of
+    non-primitive types on Windows.
+
+  * Move outputhandler creation to separate function (Tim Wojtulewicz)
+
+  * Rename WSL bash so it doesn't override Git bash for Windows CI builds (Tim Wojtulewicz)
+
+  * Set git's autocrlf option to false when running tests on Github (Tim Wojtulewicz)
+
+    If this option isn't here, the Windows runners will reset all of the
+    line endings when it clones to \r\n. This breaks a few of the tests
+    because the comparison will have the wrong line endings.
+
+  * Bump required python version to 3.7, update github workflows (Tim Wojtulewicz)
+
+    This also adds a new workflow to test setup.py to ensure that the
+    package installs correctly and you can run the internal tests against
+    the installed version.
+
+0.72-20 | 2022-12-13 09:12:13 +0100
+
+  * Add back CI run for Python 3.5. (Benjamin Bannier, Corelight)
+
+0.72-18 | 2022-12-09 14:08:00 -0800
+
+  * GH-75: Do not ignore case of options. (Benjamin Bannier, Corelight)
+
+0.72-16 | 2022-12-06 11:22:53 -0800
+
+  * CI: remove explicit use of Python 3.5, EOL (Christian Kreibich, Corelight)
+
+  * Explain recent alternatives-related changes in the README. (Christian Kreibich, Corelight)
+
+  * Fix handling of specific alternatives in combination with the default (Christian Kreibich, Corelight)
+
+  * Fail when -a/--alternative includes an alternative not defined in the config (Christian Kreibich, Corelight)
+
+  * Add test for use of an undefined alternative (Christian Kreibich, Corelight)
+
+0.72-10 | 2022-11-16 14:44:01 +0100
+
+  * Always use UTF-8 encoding for BTest input and output files.
+    (Benjamin Bannier, Corelight)
+
+0.72-7 | 2022-11-16 10:23:44 +0100
+
+  * Python cleanup (Benjamin Bannier, Corelight)
+
+    - Use `locale.getlocale` instead of deprecated `locale.getdefaultlocale`.
+
+    - Remove code for Python 2 compatibility.
+
+    - Use `python3` instead of `python` binary in test. Newer versions
+      of e.g., macOS do not provide a `python` binary anymore.
+
+  * Bump pre-commit checks. (Benjamin Bannier, Corelight)
+
+0.72-2 | 2022-11-08 10:34:21 +0100
+
+  * Remove dependency on distutils. The distutils module will be
+    removed from Python in 3.12. (Cyril Rolando)
+
+0.72 | 2022-03-22 09:21:34 +0100
+
+  * Release 0.72.
+
+0.71-4 | 2022-03-22 09:19:53 +0100
+
+  * Make test `duplication-selection` independent of actual
+    scheduling.
+
+0.71-2 | 2022-02-02 12:47:42 +0100
+
+  * Avoid assertion failure if same test required multiple times.
+    (Benjamin Bannier, Corelight)
+
 0.71 | 2021-11-01 12:04:45 -0700
 
   * Release 0.71.
 
 0.70-6 | 2021-11-01 12:03:30 -0700
 
   * Add PartInitializer option (Christian Kreibich, Corelight)
```

### Comparing `btest-0.71/COPYING` & `btest-1.0/COPYING`

 * *Files identical despite different names*

### Comparing `btest-0.71/MANIFEST` & `btest-1.0/sphinx/btest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# file GENERATED by distutils, do NOT edit
 CHANGES
 COPYING
-MANIFEST
 MANIFEST.in
 Makefile
 README
 VERSION
 btest
 btest-ask-update
 btest-bg-run
 btest-bg-run-helper
 btest-bg-wait
 btest-diff
 btest-progress
 btest-setsid
 btest.cfg.example
+setup.cfg
 setup.py
 Baseline/examples.t4/dots
 Baseline/examples.t5/output
 Baseline/examples.t5-2/output
 Baseline/examples.t6/output
 Baseline/examples.t7/output
 Baseline/examples.unstable/output
@@ -47,30 +46,33 @@
 examples/sphinx/tests/sphinx/hello-world.btest#2
 examples/sphinx/tests/sphinx/hello-world.btest#3
 sphinx/btest-diff-rst
 sphinx/btest-rst-cmd
 sphinx/btest-rst-include
 sphinx/btest-rst-pipe
 sphinx/btest-sphinx.py
-testing/.btest.failed.dat
+sphinx/btest.egg-info/PKG-INFO
+sphinx/btest.egg-info/SOURCES.txt
+sphinx/btest.egg-info/dependency_links.txt
+sphinx/btest.egg-info/top_level.txt
 testing/.gitignore
 testing/Makefile
 testing/btest.cfg
 testing/btest.tests.cfg
-testing/diag.log
 testing/Baseline/tests.abort-on-failure/output
 testing/Baseline/tests.abort-on-failure-with-only-known-fails/output
 testing/Baseline/tests.alternatives-environment/child-output
 testing/Baseline/tests.alternatives-environment/output
 testing/Baseline/tests.alternatives-filter/child-output
 testing/Baseline/tests.alternatives-filter/output
 testing/Baseline/tests.alternatives-keywords/output
 testing/Baseline/tests.alternatives-substitution/child-output
 testing/Baseline/tests.alternatives-substitution/output
 testing/Baseline/tests.alternatives-testbase/output
+testing/Baseline/tests.alternatives-undefined/output
 testing/Baseline/tests.brief/out1
 testing/Baseline/tests.brief/out2
 testing/Baseline/tests.btest-cfg/abspath
 testing/Baseline/tests.btest-cfg/nopath
 testing/Baseline/tests.btest-cfg/relpath
 testing/Baseline/tests.console/output
 testing/Baseline/tests.crlf-line-terminators/crlfs.dat
@@ -81,14 +83,15 @@
 testing/Baseline/tests.diag-file/output
 testing/Baseline/tests.diff-brief/output
 testing/Baseline/tests.diff-max-lines/output1
 testing/Baseline/tests.diff-max-lines/output2
 testing/Baseline/tests.doc/md
 testing/Baseline/tests.doc/rst
 testing/Baseline/tests.environment/output
+testing/Baseline/tests.environment-windows/output
 testing/Baseline/tests.exit-codes/out1
 testing/Baseline/tests.exit-codes/out2
 testing/Baseline/tests.groups/output
 testing/Baseline/tests.ignore/output
 testing/Baseline/tests.known-failure/output
 testing/Baseline/tests.known-failure-and-success/output
 testing/Baseline/tests.known-failure-succeeds/output
@@ -107,14 +110,15 @@
 testing/Baseline/tests.progress/output
 testing/Baseline/tests.progress-back-to-back/output
 testing/Baseline/tests.quiet/out1
 testing/Baseline/tests.quiet/out2
 testing/Baseline/tests.requires/output
 testing/Baseline/tests.requires-with-start-next/output
 testing/Baseline/tests.rerun/output
+testing/Baseline/tests.set-key/output
 testing/Baseline/tests.sphinx.rst-cmd/output
 testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt
 testing/Baseline/tests.start-file/output
 testing/Baseline/tests.start-next/output
 testing/Baseline/tests.start-next-dir/output
 testing/Baseline/tests.statefile/mystate1
 testing/Baseline/tests.statefile/mystate2
@@ -124,28 +128,32 @@
 testing/Baseline/tests.testdirs/out2
 testing/Baseline/tests.threads/output.j0
 testing/Baseline/tests.threads/output.j1
 testing/Baseline/tests.threads/output.j5
 testing/Baseline/tests.tracing/output
 testing/Baseline/tests.unstable/output
 testing/Baseline/tests.unstable-dir/output
+testing/Baseline/tests.unstable-subtest/.stderr
+testing/Baseline/tests.unstable-subtest/diag
 testing/Baseline/tests.verbose/output
 testing/Baseline/tests.versioning/output
 testing/Baseline/tests.xml/output-j2.xml
 testing/Baseline/tests.xml/output.xml
 testing/Files/local_alternative/btest.tests.cfg
 testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/output
 testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/output
 testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/output
 testing/Files/local_alternative/tests/local-alternative-found.test
 testing/Files/local_alternative/tests/local-alternative-show-env.test
 testing/Files/local_alternative/tests/local-alternative-show-test-baseline.test
 testing/Files/local_alternative/tests/local-alternative-show-testbase.test
+testing/Scripts/convert-path-list.sh
 testing/Scripts/diff-remove-abspath
 testing/Scripts/dummy-script
+testing/Scripts/is-windows
 testing/Scripts/script-command
 testing/Scripts/strip-iso8601-date
 testing/Scripts/strip-test-base
 testing/Scripts/test-filter
 testing/Scripts/test-perf
 testing/tests/abort-on-failure-with-only-known-fails.btest
 testing/tests/abort-on-failure.btest
@@ -154,14 +162,15 @@
 testing/tests/alternatives-filter.test
 testing/tests/alternatives-keywords.test
 testing/tests/alternatives-overwrite-env.test
 testing/tests/alternatives-reread-config-baselinedir.test
 testing/tests/alternatives-reread-config.test
 testing/tests/alternatives-substitution.test
 testing/tests/alternatives-testbase.test
+testing/tests/alternatives-undefined.test
 testing/tests/baseline-dir-env.test
 testing/tests/basic-fail.test
 testing/tests/basic-succeed.test
 testing/tests/binary-mode.test
 testing/tests/brief.test
 testing/tests/btest-cfg.test
 testing/tests/canonifier-cmdline.test
@@ -174,14 +183,17 @@
 testing/tests/diag-all.test
 testing/tests/diag-file.test
 testing/tests/diag.test
 testing/tests/diff-brief.test
 testing/tests/diff-max-lines.test
 testing/tests/diff.test
 testing/tests/doc.test
+testing/tests/duplicate-selection.test
+testing/tests/env-var-casing.test
+testing/tests/environment-windows.test
 testing/tests/environment.test
 testing/tests/exit-codes.test
 testing/tests/finalizer.test
 testing/tests/groups.test
 testing/tests/ignore.test
 testing/tests/initializer.test
 testing/tests/known-failure-and-success.btest
@@ -202,26 +214,28 @@
 testing/tests/ports.test
 testing/tests/progress-back-to-back.test
 testing/tests/progress.test
 testing/tests/quiet.test
 testing/tests/requires-with-start-next.test
 testing/tests/requires.test
 testing/tests/rerun.test
+testing/tests/set-key.test
 testing/tests/start-file.test
 testing/tests/start-next-dir.test
 testing/tests/start-next-naming.test
 testing/tests/start-next.test
 testing/tests/statefile-sorted.test
 testing/tests/statefile.test
 testing/tests/teardown.test
 testing/tests/test-base.test
 testing/tests/testdirs.test
 testing/tests/threads.test
 testing/tests/tmps.test
 testing/tests/tracing.test
 testing/tests/unstable-dir.test
+testing/tests/unstable-subtest.test
 testing/tests/unstable.test
 testing/tests/verbose.test
 testing/tests/versioning.test
 testing/tests/xml.test
 testing/tests/sphinx/rst-cmd.sh
-testing/tests/sphinx/run-sphinx
+testing/tests/sphinx/run-sphinx
```

### Comparing `btest-0.71/Makefile` & `btest-1.0/Makefile`

 * *Files identical despite different names*

### Comparing `btest-0.71/PKG-INFO` & `btest-1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: btest
-Version: 0.71
+Version: 1.0
 Summary: A powerful system testing framework
 Home-page: https://github.com/zeek/btest
-Author: Robin Sommer
-Author-email: robin@icir.org
+Author: The Zeek Team
+Author-email: info@zeek.org
 License: 3-clause BSD License
-Description: See https://github.com/zeek/btest
 Keywords: system tests testing framework baselines
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7
+License-File: COPYING
+
+See https://github.com/zeek/btest
```

### Comparing `btest-0.71/README` & `btest-1.0/README`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ..	-*- mode: rst-mode -*-
 ..
 .. Version number is filled in automatically.
 
-.. |version| replace:: 0.71
+.. |version| replace:: 1.0
 
 ==================================================
 BTest - A Generic Driver for Powerful System Tests
 ==================================================
 
 BTest is a powerful framework for writing system tests. Freely
 borrowing some ideas from other packages, its main objective is to
@@ -23,28 +23,43 @@
 .. contents::
 
 Prerequisites
 =============
 
 BTest has the following prerequisites:
 
-- Python version >= 3.5 (older versions may work, but are not
+- Python version >= 3.7 (older versions may work, but are not
   well-tested).
 
-- Bash (note that on FreeBSD and Alpine Linux, bash is not installed
-  by default).
+- Bash. Note that on FreeBSD and Alpine Linux, bash is not installed by
+  default. This is also required on Windows, in the form of Git's msys2, Cygwin,
+  etc.
 
 BTest has the following optional prerequisites to enable additional
 functionality:
 
-- Sphinx.
+- Sphinx. Sphinx functionality is currently disabled on Windows.
 
 - perf (Linux only).  Note that on Debian/Ubuntu, you also need to install
   the "linux-tools" package.
 
+Windows Caveats
+---------------
+
+When running BTest on Windows, you must have a bash shell installed of some
+sort. This can be from WSL, Cygwin, msys2, Git, or any number of other methods,
+but ``bash.exe`` must be available. BTest will check for its existence at
+startup and exit if it is not available.
+
+A minor change must be made to any configuration value that is a path list. For
+example, if you are setting the ``PATH`` environment variable from your
+btest.cfg. In these cases, you should use ``$(pathsep)s`` in the configuration
+instead of bare ``:`` or ``;`` values to separate the paths. This ensures that
+both POSIX and Windows systems handle the path lists correctly.
+
 Download and Installation
 =========================
 
 Installation is simple and standard via ``pip``::
 
     > pip install btest
 
@@ -249,17 +264,19 @@
 
 ``btest`` accepts the following options:
 
 -a ALTERNATIVE, --alternative=ALTERNATIVE
     Activates an alternative_ configuration defined in the
     configuration file. Multiple alternatives can be given as a
     comma-separated list (in this case, all specified tests are run
-    once for each specified alternative). If ``ALTERNATIVE`` is ``-``
-    that refers to running with the standard setup, which can be used
-    to run tests both with and without alternatives by giving both.
+    once for each specified alternative). The alternatives ``-``
+    and ``default`` refer to the standard setup, allowing tests to
+    run with combinations of the latter and select alternatives.
+    If an alternative is not defined in the configuration, ``btest``
+    fails with exit code 1 and an according error message on stderr.
 
 -A, --show-all
     Shows an output line for all tests that were run (this includes tests
     that passed, failed, or were skipped), rather than only failed tests.
     Note that this option has no effect when stdout is not a TTY
     (because all tests are shown in that case).
 
@@ -324,14 +341,21 @@
 -R FORMAT, --documentation=FORMAT
     Generates a reference of all tests and prints that to standard
     output. The output can be of two types, specified by
     ``FORMAT``: ``rst`` prints reStructuredText, and ``md`` prints
     Markdown. In the output each test includes the documentation
     string that's defined for it through ``@TEST-DOC``.
 
+-s <kv>, --set=<kv>
+    Takes a ``key=value`` argument and uses it to override a value
+    used during parsing of the configuration file read by btest at
+    startup. This can be used to override various default values
+    prior to parsing. Can be passed multiple times to override
+    different keys. See `defaults`_ for an example.
+
 -t, --tmp-keep
     Does not delete any temporary files created for running the
     tests (including their outputs). By default, the temporary
     files for a test will be located in ``.tmp/<test>/``, where
     ``<test>`` is the relative path of the test file with all slashes
     replaced with dots and the file extension removed (e.g., the files
     for ``example/t3.sh`` will be in ``.tmp/example.t3``).
@@ -369,16 +393,16 @@
     for a test.
 
 -x FILE, --xml=FILE
     Records test results in JUnit XML format to the given file.
     If the file exists already, it is overwritten.
 
 -z RETRIES, --retries=RETRIES
-     Retry any failed tests up to this many times to determine if
-     they are unstable.
+    Retry any failed tests up to this many times to determine if
+    they are unstable.
 
 .. _configuration file: configuration_
 .. _configuration:
 
 Configuration
 -------------
 
@@ -404,14 +428,38 @@
 due to Python's ``ConfigParser`` class).
 
 Furthermore, all values can use standard "backtick-syntax" to
 include the output of external commands (e.g., xyz=`\echo test\`).
 Note that the backtick expansion is performed after any ``%(..)``
 have already been replaced (including within the backticks).
 
+.. _default: `defaults`_
+.. _defaults:
+
+Defaults
+~~~~~~~~
+
+There is a special section that can be added to the configuration file that will
+set default values to be used during the parsing of other configuration
+directives. For example::
+
+    [DEFAULT]
+    val=abcd
+
+    [environment]
+    ENV_VALUE=%(val)s
+
+The configuration parser reads the keys and values from the DEFAULT section
+prior to reading the other sections. It uses those keys to replace the ``%()s``
+macros as described earlier. The values stored in these keys can be overridden
+at runtime by using the ``-s``/``--set`` command-line argument. For example to
+override the ``val`` default above, the ``-s val=other`` argument can be
+passed. In that case, ``ENV_VALUE`` would be set to ``other`` instead of
+``abcd``.
+
 .. _option: `options`_
 .. _options:
 
 Options
 ~~~~~~~
 
 The following options can be set in the ``btest`` section of the
```

### Comparing `btest-0.71/btest` & `btest-1.0/btest`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,134 @@
 #! /usr/bin/env python3
 #
 # Main test driver.
 #
-# pylint: disable=line-too-long,too-many-lines,invalid-name,missing-function-docstring,missing-class-docstring
-
-from __future__ import print_function
+# pylint: disable=line-too-long,too-many-lines,invalid-name,missing-function-docstring,
+# pylint: disable=missing-class-docstring
 
 import atexit
+import binascii
+import configparser
 import copy
 import fnmatch
 import glob
-import io
 import json
-import locale
-import multiprocessing
-import multiprocessing.managers
-import multiprocessing.sharedctypes
 import optparse
 import os
 import os.path
+import pathlib
 import platform as pform
 import re
+import shlex
 import shutil
 import signal
 import socket
 import subprocess
 import sys
 import tempfile
 import threading
 import time
 import uuid
 import xml.dom.minidom
 
 from datetime import datetime
 
-try:
-    import ConfigParser as configparser
-except ImportError:
-    import configparser
-
-VERSION = "0.71"  # Automatically filled in.
+# We require the external multiprocess library on Windows due to pickling issues
+# with the standard one.
+if sys.platform == "win32":
+    try:
+        import multiprocess as mp
+        import multiprocess.managers as mp_managers
+        import multiprocess.sharedctypes as mp_sharedctypes
+    except ImportError as error:
+        print(
+            "error: btest failed to import the 'multiprocess' library\n"
+            "\n"
+            "This library is required for btest to function on Windows. "
+            "It can be installed from pip like:\n"
+            "\n"
+            "    pip install multiprocess\n"
+            "\n"
+            "Also check the following exception output for possible alternate explanations:\n\n"
+            "{}: {}".format(type(error).__name__, error),
+            file=sys.stderr,
+        )
+else:
+    import multiprocessing as mp
+    import multiprocessing.managers as mp_managers
+    import multiprocessing.sharedctypes as mp_sharedctypes
 
-using_py3 = (sys.version_info[0] == 3)
+VERSION = "1.0"  # Automatically filled in.
 
 Name = "btest"
 Config = None
 
 try:
     ConfigDefault = os.environ["BTEST_CFG"]
 except KeyError:
     ConfigDefault = "btest.cfg"
 
 
+def normalize_path(path):
+    """Ensures that paths on Windows convert backslashes to forward slashes, to
+    make path handling easier in lots of other places. On non-Windows platforms
+    this is a no-op beyond converting things to absolute paths."""
+    os_path = os.path.abspath(path)
+    windows_path = pathlib.PureWindowsPath(os_path)
+    return windows_path.as_posix()
+
+
+def normalize_path_join(*args):
+    return normalize_path(os.path.join(*args))
+
+
+def reopen_std_file(stdfile):
+    """Reopens one of the stderr or stdout files, but resets the newline
+    used in the output to "\n" in order to force that line ending on Windows.
+    Without this, Windows will use "\r\n" which breaks a lot of tests."""
+    return open(
+        stdfile.fileno(),
+        mode=stdfile.mode,
+        buffering=1,
+        encoding=stdfile.encoding,
+        errors=stdfile.errors,
+        newline="\n",
+        closefd=False,
+    )
+
+
 def output(msg, nl=True, file=None):
     if not file:
-        file = sys.stderr
+        file = reopen_std_file(sys.__stderr__)
 
     if nl:
         print(msg, file=file)
     else:
         print(msg, end=" ", file=file)
 
 
 def warning(msg):
-    print("warning: %s" % msg, file=sys.stderr)
+    print(f"warning: {msg}", file=sys.stderr)
 
 
 def error(msg):
     print(msg, file=sys.stderr)
     sys.exit(1)
 
 
 def mkdir(folder):
     if not os.path.exists(folder):
         try:
             os.makedirs(folder)
         except OSError as exc:
-            error("cannot create directory %s: %s" % (folder, exc))
+            error(f"cannot create directory {folder}: {exc}")
 
     else:
         if not os.path.isdir(folder):
-            error("path %s exists but is not a directory" % folder)
+            error(f"path {folder} exists but is not a directory")
 
 
 def which(cmd):
     # Adapted from http://stackoverflow.com/a/377028
     def is_exe(fpath):
         return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
 
@@ -104,38 +148,36 @@
     return None
 
 
 def platform():
     return pform.system()
 
 
-def getDefaultBtestEncoding():
-    if locale.getdefaultlocale()[1] is None:
-        return 'utf-8'
-
-    return locale.getpreferredencoding()
-
-
 def validate_version_requirement(required: str, present: str):
-    '''Helper function to validate that a `present` version is semantically newer or equal than a `required` version.'''
+    """Validates that `present` version semantically satisfies `required` version."""
+
     def extract_version(v: str):
-        '''Helper function to extract version components from a string.'''
+        """Helper function to extract version components from a string."""
         try:
-            xyz = [int(x) for x in re.split(r'\.|-', v)]
+            xyz = [int(x) for x in re.split(r"[.-]", v)]
         except ValueError:
-            error("invalid version %s: versions must contain only numeric identifiers" % v)
+            error(
+                "invalid version %s: versions must contain only numeric identifiers" % v
+            )
 
         return xyz
 
     v_present = extract_version(present)
     v_required = extract_version(required)
 
     if v_present < v_required:
-        error("%s requires at least BTest %s, this is %s. Please upgrade." %
-              (Options.config, min_version, VERSION))
+        error(
+            "%s requires at least BTest %s, this is %s. Please upgrade."
+            % (Options.config, min_version, VERSION)
+        )
 
 
 # Get the value of the specified option in the specified section (or
 # section "btest" if not specified), or return the specified default value
 # if the option or section is not found.  The returned value has macros and
 # backticks from the config file expanded, but if the default value is returned
 # it will not be modified in any way.
@@ -144,15 +186,15 @@
         value = Config.get(section, key)
     except (configparser.NoSectionError, configparser.NoOptionError):
         return default
 
     return ExpandBackticks(value)
 
 
-reBackticks = re.compile(r"`(([^`]|\`)*)`")
+reBackticks = re.compile(r"`(([^`]|`)*)`")
 
 
 def readStateFile():
     try:
         # Read state file.
         tests = []
 
@@ -161,35 +203,67 @@
             if not line or line.startswith("#"):
                 continue
 
             tests += [line]
 
         tests = findTests(tests)
 
-    except IOError:
+    except OSError:
         return (False, [])
 
     return (True, tests)
 
 
+def _build_win_subprocess_cmd_script(cmd, tmpdir=None):
+    """
+    Builds a bash file for running subprocess commands under Windows.
+
+    :param cmd The command line to be run under bash.
+    :param tmpdir An optional directory path where the script file will be written.
+     If None, it will be written to the system's temp directory.
+    :return A tuple containing a file object pointing at the script file and a bash
+     command for running the script.
+    """
+    tf = tempfile.NamedTemporaryFile(
+        mode="w", encoding="utf-8", suffix=".sh", dir=tmpdir, delete=True
+    )
+    fcontents = f"#!/usr/bin/env bash\n{cmd}\n"
+    tf.write(fcontents)
+    tf.flush()
+
+    bash_cmd = ["bash.exe", "-c", normalize_path(tf.name)]
+    return tf, bash_cmd
+
+
 # Expand backticks in a config option value and return the result.
 def ExpandBackticks(origvalue):
     def _exec(m):
         cmd = m.group(1)
         if not cmd:
             return ""
 
-        try:
-            pp = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE)
-        except OSError as e:
-            error("cannot execute '%s': %s" % (cmd, e))
+        tf = None
+        if sys.platform == "win32":
+            try:
+                tf, bash_cmd = _build_win_subprocess_cmd_script(cmd, None)
+                pp = subprocess.Popen(bash_cmd, stdout=subprocess.PIPE)
+            except OSError as e:
+                error(f"cannot execute '{cmd}': {e}")
+        else:
+            try:
+                pp = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE)
+            except OSError as e:
+                error(f"cannot execute '{cmd}': {e}")
 
         out = pp.communicate()[0]
         out = out.decode()
 
+        if tf:
+            tf.close()
+
         return out.strip()
 
     value = reBackticks.sub(_exec, origvalue)
 
     return value
 
 
@@ -201,28 +275,52 @@
     # default section (the values are raw, so we need to fetch the actual
     # value below).
     try:
         items = self._sections[section].items()
     except KeyError:
         raise configparser.NoSectionError(section)
 
+    # Override any of the defaults with ones that we read from the command-line
+    # options before expanding macros below.
+    cfg_defaults = self.defaults()
+    if Options.defaults:
+        for d in Options.defaults:
+            k, v = d.split("=", 1)
+            cfg_defaults[k] = v.strip("'\"")
+
     result = {}
 
-    for (key, rawvalue) in items:
+    for key, rawvalue in items:
         # Python 2 includes a key of "__name__" that we don't want (Python 3
         # doesn't include this)
         if not key.startswith("__"):
             # Expand macros such as %(testbase)s.
             value = self.get(section, key)
             # Expand backticks (if any) in the value.
             result[key] = ExpandBackticks(value)
 
     return result.items()
 
 
+def getcfgparser(defaults):
+    configparser.ConfigParser.itemsNoDefaults = cpItemsNoDefaults
+
+    cfg = configparser.ConfigParser()
+
+    # We make all key lookups case-sensitive to avoid aliasing of
+    # case-sensitive environment variables.
+    cfg.optionxform = lambda optionstr: optionstr
+
+    default_section = cfg.defaults()
+    for key, value in defaults.items():
+        default_section[key] = value
+
+    return cfg
+
+
 # Replace environment variables in string.
 def replaceEnvs(s):
     def replace_with_env(m):
         try:
             return os.environ[m.group(1)]
         except KeyError:
             return ""
@@ -247,68 +345,81 @@
 
 # Runs a subprocess. Takes same arguments as subprocess.check_call()
 # and returns a 2-tuple (success, rc) where *success* is a boolean
 # indicating if the command executed, and *rc* is its exit code if it did.
 def runSubprocess(*args, **kwargs):
     def child(q):
         try:
-            subprocess.check_call(*args, **kwargs)
+            if sys.platform == "win32":
+                tmpdir = normalize_path(kwargs.get("cwd", ""))
+                if len(args) > 1:
+                    cmd = shlex.join(args)
+                else:
+                    cmd = args[0]
+
+                tf, bash_cmd = _build_win_subprocess_cmd_script(cmd, tmpdir)
+                with tf:
+                    subprocess.check_call(bash_cmd, **kwargs)
+            else:
+                subprocess.check_call(*args, **kwargs)
             success = True
             rc = 0
 
         except subprocess.CalledProcessError as e:
             success = False
             rc = e.returncode
 
         except KeyboardInterrupt:
             success = False
             rc = 0
 
         q.put([success, rc])
 
     try:
-        q = multiprocessing.Queue()
-        p = multiprocessing.Process(target=child, args=(q, ))
+        q = mp.Queue()
+        p = mp.Process(target=child, args=(q,))
         p.start()
         result = q.get()
         p.join()
 
     except KeyboardInterrupt:
         # Bail out here directly as otherwise we'd get a bunch of errors.
         # from all the childs.
-        os._exit(1)
+        sys.exit(1)
 
     return result
 
 
-def getcfgparser(defaults):
-    configparser.ConfigParser.itemsNoDefaults = cpItemsNoDefaults
-    cfg = configparser.ConfigParser(defaults)
-    return cfg
-
-
 # Description of an alternative configuration.
 class Alternative:
+    DEFAULT = "default"
+
     def __init__(self, name):
         self.name = name
         self.filters = {}
         self.substitutions = {}
         self.envs = {}
 
+    def is_default(self):
+        return self.name == Alternative.DEFAULT
+
+    def is_empty(self):
+        return not (self.filters or self.substitutions or self.envs)
+
 
 # Exception class thrown to signal manager to abort processing.
 # The message passed to the constructor will be printed to the console.
 class Abort(Exception):
     pass
 
 
 # Main class distributing the work across threads.
-class TestManager(multiprocessing.managers.SyncManager):
+class TestManager(mp_managers.SyncManager):
     def __init__(self, *args, **kwargs):
-        super(TestManager, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         self._output_handler = None
         self._lock = None
         self._succeeded = None
         self._failed = None
         self._failed_expected = None
         self._unstable = None
@@ -318,167 +429,219 @@
         self._num_tests = None
         self._timing = None
         self._ports = None
 
     def run(self, tests, output_handler):
         self.start()
 
+        mgr_data = self.dict()
+        mgr_data["Alternatives"] = Alternatives
+        mgr_data["BaselineDirs"] = BaselineDirs
+        mgr_data["Initializer"] = Initializer
+        mgr_data["Finalizer"] = Finalizer
+        mgr_data["Teardown"] = Teardown
+        mgr_data["Options"] = Options
+        mgr_data["TestBase"] = TestBase
+        mgr_data["TmpDir"] = TmpDir
+        mgr_data["RE_INPUT"] = RE_INPUT
+        mgr_data["RE_DIR"] = RE_DIR
+        mgr_data["RE_ENV"] = RE_ENV
+
         output_handler.prepare(self)
         self._output_handler = output_handler
         self._lock = self.RLock()
-        self._succeeded = multiprocessing.sharedctypes.RawValue('i', 0)
-        self._failed = multiprocessing.sharedctypes.RawValue('i', 0)
-        self._failed_expected = multiprocessing.sharedctypes.RawValue('i', 0)
-        self._unstable = multiprocessing.sharedctypes.RawValue('i', 0)
-        self._skipped = multiprocessing.sharedctypes.RawValue('i', 0)
+        self._succeeded = mp_sharedctypes.RawValue("i", 0)
+        self._failed = mp_sharedctypes.RawValue("i", 0)
+        self._failed_expected = mp_sharedctypes.RawValue("i", 0)
+        self._unstable = mp_sharedctypes.RawValue("i", 0)
+        self._skipped = mp_sharedctypes.RawValue("i", 0)
         self._tests = self.list(tests)
         self._failed_tests = self.list([])
         self._num_tests = len(self._tests)
         self._timing = self.loadTiming()
 
         port_range = getOption("PortRange", "1024-65535")
         port_range_lo = int(port_range.split("-")[0])
         port_range_hi = int(port_range.split("-")[1])
 
         if port_range_lo > port_range_hi:
-            error("invalid PortRange value: {0}".format(port_range))
+            error(f"invalid PortRange value: {port_range}")
 
         max_test_ports = 0
         test_with_most_ports = None
 
         for t in self._tests:
             if len(t.ports) > max_test_ports:
                 max_test_ports = len(t.ports)
                 test_with_most_ports = t
 
         if max_test_ports > port_range_hi - port_range_lo + 1:
-            error("PortRange {0} cannot satisfy requirement of {1} ports in test {2}".format(
-                port_range, max_test_ports, test_with_most_ports.name))
+            error(
+                "PortRange {} cannot satisfy requirement of {} ports in test {}".format(
+                    port_range, max_test_ports, test_with_most_ports.name
+                )
+            )
 
         self._ports = self.list([p for p in range(port_range_lo, port_range_hi + 1)])
 
         threads = []
 
         # With interactive input possibly required, we run tests
         # directly. This avoids noisy output appearing from detached
         # processes post-btest-exit when using CTRL-C during the input
         # stage.
         if Options.mode == "UPDATE_INTERACTIVE":
-            self.threadRun(0)
+            self.threadRun(0, mgr_data)
         else:
             try:
+                # Create a set of processes for running each of the tests. This isn't the actual
+                # zeek processes, but runner processes executing individual test commands.
                 for i in range(Options.threads):
-                    t = multiprocessing.Process(name="#%d" % (i + 1),
-                                                target=lambda: self.threadRun(i))
+                    t = mp.Process(
+                        name="#%d" % (i + 1), target=lambda: self.threadRun(i, mgr_data)
+                    )
                     t.start()
                     threads += [t]
 
                 for t in threads:
                     t.join()
 
             except KeyboardInterrupt:
                 for t in threads:
                     t.terminate()
                     t.join()
 
-        if Options.abort_on_failure and self._failed.value > 0 and self._failed.value > self._failed_expected.value:
+        if (
+            Options.abort_on_failure
+            and self._failed.value > 0
+            and self._failed.value > self._failed_expected.value
+        ):
             # Signal abort. The child processes will already have
             # finished because the join() above still ran.
             raise Abort("Aborted after first failure.")
 
         # Record failed tests if not updating.
         if Options.mode != "UPDATE" and Options.mode != "UPDATE_INTERACTIVE":
             try:
-                state = open(StateFile, "w")
-            except IOError:
+                state = open(StateFile, "w", encoding="utf-8")
+            except OSError:
                 error("cannot open state file %s" % StateFile)
 
             for t in sorted(self._failed_tests):
                 print(t, file=state)
 
             state.close()
 
-        return (self._succeeded.value, self._failed.value, self._skipped.value,
-                self._unstable.value, self._failed_expected.value)
+        return (
+            self._succeeded.value,
+            self._failed.value,
+            self._skipped.value,
+            self._unstable.value,
+            self._failed_expected.value,
+        )
 
     def percentage(self):
         if not self._num_tests:
             return 0
 
         count = self._succeeded.value + self._failed.value + self._skipped.value
         return 100.0 * count / self._num_tests
 
-    def threadRun(self, thread_num):
+    # Worker method for each of the "threads" specified by the "-j" argument passed
+    # at run time. This basically segments the list of tests into chunks and runs
+    # until we're out of chunks.
+    def threadRun(self, thread_num, mgr_data):
+        # This should prevent the child processes from receiving SIGINT signals and
+        # let the KeyboardInterrupt handler in the manager's run() method handle
+        # those.
         signal.signal(signal.SIGINT, signal.SIG_IGN)
 
         all_tests = []
 
+        # Globals get lost moving from the parent to the child on Windows, so we need to use
+        # the data proxied from the manager to rebuild the dict of globals before continuing.
+        if sys.platform == "win32":
+            for global_key, global_value in mgr_data.items():
+                globals()[global_key] = global_value
+
         while True:
-            tests = self.nextTests(thread_num)
-            if tests is None:
+            # Pull the next test from the list that was built at startup. This may
+            # be more than one test if there were alternatives requested in the
+            # arguments passed to btest.
+            thread_tests = self.nextTests(thread_num)
+            if thread_tests is None:
                 # No more work for us.
                 return
 
-            all_tests += tests
+            all_tests += thread_tests
 
-            for t in tests:
+            for t in thread_tests:
                 t.run(self)
                 self.testReplayOutput(t)
 
             if Options.update_times:
                 self.saveTiming(all_tests)
 
     def rerun(self, test):
         test.reruns += 1
         self._tests += [test.clone(increment=False)]
 
     def nextTests(self, thread_num):
         with self._lock:
-            if Options.abort_on_failure and self._failed.value > 0 and self._failed.value > self._failed_expected.value:
+            if (
+                Options.abort_on_failure
+                and self._failed.value > 0
+                and self._failed.value > self._failed_expected.value
+            ):
                 # Don't hand out any more tests if we are to abort after
                 # first failure. Doing so will let all the processes terminate.
                 return None
 
             for i in range(len(self._tests)):
                 t = self._tests[i]
 
                 if not t:
                     continue
 
-                if t.serialize and hash(t.serialize) % Options.threads != thread_num:
+                if t.serialize and t.serialize_hash() % Options.threads != thread_num:
                     # Not ours.
                     continue
 
                 # We'll execute it, delete from queue.
                 del self._tests[i]
 
                 if Options.alternatives:
                     tests = []
 
                     for alternative in Options.alternatives:
-
                         if alternative in t.ignore_alternatives:
                             continue
 
-                        if t.include_alternatives and alternative not in t.include_alternatives:
+                        if (
+                            t.include_alternatives
+                            and alternative not in t.include_alternatives
+                        ):
                             continue
 
                         alternative_test = copy.deepcopy(t)
 
-                        if alternative == "-":
+                        if alternative == Alternative.DEFAULT:
                             alternative = ""
 
                         alternative_test.setAlternative(alternative)
                         tests += [alternative_test]
 
                 else:
-                    if t.include_alternatives and "default" not in t.include_alternatives:
+                    if (
+                        t.include_alternatives
+                        and Alternative.DEFAULT not in t.include_alternatives
+                    ):
                         tests = []
 
-                    elif "default" in t.ignore_alternatives:
+                    elif Alternative.DEFAULT in t.ignore_alternatives:
                         tests = []
 
                     else:
                         tests = [t]
 
                 return tests
 
@@ -488,15 +651,14 @@
     def returnPorts(self, ports):
         with self._lock:
             for p in ports:
                 self._ports.append(p)
 
     def getAvailablePorts(self, count):
         with self._lock:
-
             if count > len(self._ports):
                 return []
 
             first_port = -1
             rval = []
 
             for _ in range(count):
@@ -525,22 +687,22 @@
                     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
                     # Setting REUSEADDR would allow ports to be recycled
                     # more quickly, but on macOS, seems to also have the
                     # effect of allowing multiple sockets to bind to the
                     # same port, even if REUSEPORT is off, so just try to
                     # ensure both are off.
-                    if hasattr(socket, 'SO_REUSEADDR'):
+                    if hasattr(socket, "SO_REUSEADDR"):
                         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 0)
-                    if hasattr(socket, 'SO_REUSEPORT'):
+                    if hasattr(socket, "SO_REUSEPORT"):
                         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 0)
 
                     try:
-                        sock.bind(('', next_port))
-                    except:
+                        sock.bind(("", next_port))
+                    except Exception:
                         self._ports.append(next_port)
                         continue
                     else:
                         break
 
                 rval.append(sock)
 
@@ -577,26 +739,26 @@
                 self._output_handler.testSucceeded(test, msg)
             else:
                 self._failed.value -= 1
                 if test.known_failure:
                     self._failed_expected.value -= 1
 
                 self._unstable.value += 1
-                msg += " on retry #{0}, unstable".format(test.reruns)
+                msg += f" on retry #{test.reruns}, unstable"
                 self._output_handler.testUnstable(test, msg)
 
             self._output_handler.testFinished(test, msg)
 
     def testFailed(self, test):
         test.parseProgress()
 
         msg = "failed"
 
         if test.reruns > 0:
-            msg += " on retry #{0}".format(test.reruns)
+            msg += f" on retry #{test.reruns}"
 
         if test.known_failure:
             msg += " (expected)"
 
         msg += test.timePostfix()
 
         with self._lock:
@@ -666,51 +828,54 @@
 
             path = self.timingPath()
             (dir, base) = os.path.split(path)
             mkdir(dir)
 
             out = open(path, "w")
 
-            for (k, v) in timing.items():
+            for k, v in timing.items():
                 print("%s %u" % (k, v), file=out)
 
             out.close()
 
 
 class CmdLine:
     """A single command to invoke.
 
     These commands can be provided by @TEST-{EXEC,REQUIRES} instructions, an
     Initializer, Finalizer, or Teardown, or their part-specific equivalents.
     """
+
     def __init__(self, cmdline, expect_success, part, file):
         self.cmdline = cmdline
         self.expect_success = expect_success
         self.part = part
         self.file = file
 
 
 class CmdSeq:
     """A sequence of commands, with potential subsequent teardown.
 
     Tracking the teardown separately allows us to skip to it when commands
     fail. Commands can be invidual CmdLines or CmdSeq instances. Test.run()
     processes the latter recursively.
     """
+
     def __init__(self):
         self.cmds = []  # CmdLine or CmdSeq instances
         self.teardown = None
 
 
 # One test.
-class Test(object):
+class Test:
     def __init__(self, file=None, directory=None):  # Allow dir to be directly defined
-
-        if file is not None: self.dir = os.path.abspath(os.path.dirname(file))
-        else: self.dir = directory
+        if file is not None:
+            self.dir = normalize_path(os.path.dirname(file))
+        else:
+            self.dir = normalize_path(directory)
 
         self.alternative = None
         self.baselines = []
         self.basename = None
         self.bound_ports = []
         self.cloned = False
         self.cmdseqs = []
@@ -746,116 +911,135 @@
         self.utime_exceeded = False
         self.utime_perc = 0.0
         self.verbose = None
 
     def __lt__(self, value):
         return self.name and value.name and self.name < value.name
 
+    def serialize_hash(self):
+        if not self.serialize:
+            return 0
+
+        return int(binascii.crc32(self.serialize.encode("utf-8")))
+
     def displayName(self):
         name = self.name
 
         if self.alternative:
-            name = "%s [%s]" % (name, self.alternative)
+            name = f"{name} [{self.alternative}]"
 
         return name
 
     def setAlternative(self, alternative):
         self.alternative = alternative
 
-        # Parse the test's content.
+    # Parse the test's content.
     def parse(self, content, file):
         cmds = {}
         for line in content:
-
             m = RE_IGNORE.search(line)
             if m:
                 # Ignore this file.
                 return False
 
-            for (tag, regexp, multiple, optional, group1, group2) in Commands:
+            for tag, regexp, multiple, optional, group1, group2 in Commands:
                 m = regexp.search(line)
 
                 if m:
                     value = None
 
                     if group1 >= 0:
                         value = m.group(group1)
 
                     if group2 >= 0:
                         value = (value, m.group(group2))
 
                     if not multiple:
                         if tag in cmds:
-                            error("%s: %s defined multiple times." % (file, tag))
+                            error(f"{file}: {tag} defined multiple times.")
 
                         cmds[tag] = value
 
                     else:
                         try:
                             cmds[tag] += [value]
                         except KeyError:
                             cmds[tag] = [value]
 
         # Make sure all non-optional commands are there.
-        for (tag, regexp, multiple, optional, group1, group2) in Commands:
+        for tag, regexp, multiple, optional, group1, group2 in Commands:
             if not optional and tag not in cmds:
                 if tag == "exec":
-                    error("%s: mandatory keyword '@TEST-EXEC' or '@TEST-EXEC-FAIL' is missing." %
-                          file)
+                    error(
+                        f"{file}: mandatory keyword '@TEST-EXEC' or '@TEST-EXEC-FAIL' is missing."
+                    )
                 else:
-                    error("%s: mandatory %s command not found." % (file, tag))
+                    error(f"{file}: mandatory {tag} command not found.")
 
         basename = file
 
         part = 1
         m = RE_PART.match(file)
 
         if m:
             basename = m.group(1)
             part = int(m.group(2))
 
         name = os.path.relpath(basename, TestBase)
         (name, ext) = os.path.splitext(name)
 
-        name = name.replace("/", ".")
+        name = name.replace(os.sep, ".")
         while name.startswith("."):
             name = name[1:]
 
         self.name = name
         self.part = part
         self.basename = name
         self.contents += [(file, content)]
 
         seq = CmdSeq()
 
         if PartInitializer:
             seq.cmds.append(
-                CmdLine("%s %s" % (PartInitializer, self.name), True, part, "<PartInitializer>"))
+                CmdLine(
+                    f"{PartInitializer} {self.name}",
+                    True,
+                    part,
+                    "<PartInitializer>",
+                )
+            )
 
-        for (cmd, success) in cmds["exec"]:
+        for cmd, success in cmds["exec"]:
             seq.cmds.append(CmdLine(cmd.strip(), success != "-FAIL", part, file))
 
         if PartFinalizer:
             seq.cmds.append(
-                CmdLine("%s %s" % (PartFinalizer, self.name), True, part, "<PartFinalizer>"))
+                CmdLine(
+                    f"{PartFinalizer} {self.name}",
+                    True,
+                    part,
+                    "<PartFinalizer>",
+                )
+            )
 
         if PartTeardown:
-            seq.teardown = CmdLine("%s %s" % (PartTeardown, self.name), True, part,
-                                   "<PartTeardown>")
+            seq.teardown = CmdLine(
+                f"{PartTeardown} {self.name}", True, part, "<PartTeardown>"
+            )
 
         self.cmdseqs.append(seq)
 
         if "serialize" in cmds:
             self.serialize = cmds["serialize"]
 
         if "port" in cmds:
-            self.ports |= set(cmd.strip() for cmd in cmds['port'])
+            self.ports |= {cmd.strip() for cmd in cmds["port"]}
 
         if "group" in cmds:
-            self.groups |= set(cmd.strip() for cmd in cmds["group"])
+            self.groups |= {cmd.strip() for cmd in cmds["group"]}
 
         if "requires" in cmds:
             for cmd in cmds["requires"]:
                 self.requires.append(CmdLine(cmd.strip(), True, part, file))
 
         if "copy-file" in cmds:
             self.copy_files += [cmd.strip() for cmd in cmds["copy-file"]]
@@ -876,22 +1060,25 @@
             self.doc = cmds["doc"]
 
         return True
 
     # Copies all control information over to a new Test but replacing the test's
     # content with a new one.
     def clone(self, content=None, increment=True):
-        clone = Test("")
+        # Cloning the class like this ensures that the globals continue to exist in
+        # cloned object just as they are in the original object.
+        clone = self.__class__("")
         clone.number = self.number
         clone.basename = self.basename
-        clone.name = self.basename
 
         if increment:
             clone.number = self.number + 1
             clone.name = "%s-%d" % (self.basename, clone.number)
+        elif self.name:
+            clone.name = self.name
 
         clone.requires = self.requires
         clone.reruns = self.reruns
         clone.serialize = self.serialize
         clone.ports = self.ports
         clone.groups = self.groups
         clone.cmdseqs = self.cmdseqs
@@ -908,17 +1095,18 @@
         clone.files = self.files
         clone.dir = self.dir
         self.cloned = True
 
         return clone
 
     def mergePart(self, part):
-
         if self.cloned or part.cloned:
-            error("cannot use @TEST-START-NEXT with tests split across parts (%s)" % self.basename)
+            error(
+                f"cannot use @TEST-START-NEXT with tests split across parts ({self.basename})"
+            )
 
         self.serialize += part.serialize
         self.ports |= part.ports
         self.groups |= part.groups
         self.cmdseqs += part.cmdseqs
         self.ignore_alternatives += part.ignore_alternatives
         self.include_alternatives += part.include_alternatives
@@ -941,18 +1129,21 @@
 
             if rval:
                 return rval
 
             attempts -= 1
 
             if attempts == 0:
-                error("failed to obtain {0} ports for test {1}".format(count, self.name))
+                error(f"failed to obtain {count} ports for test {self.name}")
 
-            warning("failed to obtain {0} ports for test {1}, will try {2} more times".format(
-                count, self.name, attempts))
+            warning(
+                "failed to obtain {} ports for test {}, will try {} more times".format(
+                    count, self.name, attempts
+                )
+            )
 
             time.sleep(15)
 
     def run(self, mgr):
         bound_sockets = self.getPorts(mgr, len(self.ports))
         self.bound_ports = [s.getsockname()[1] for s in bound_sockets]
 
@@ -960,77 +1151,79 @@
             bs.close()
 
         self.progress_lock = threading.Lock()
         self.start = time.time()
         self.mgr = mgr
         mgr.testStart(self)
 
-        self.tmpdir = os.path.abspath(os.path.join(TmpDir, self.name))
-        self.diag = os.path.join(self.tmpdir, ".diag")
-        self.verbose = os.path.join(self.tmpdir, ".verbose")
-        self.baselines = [os.path.abspath(os.path.join(d, self.name)) for d in BaselineDirs]
+        self.tmpdir = normalize_path_join(TmpDir, self.name)
+        self.diag = normalize_path_join(self.tmpdir, ".diag")
+        self.verbose = normalize_path_join(self.tmpdir, ".verbose")
+        self.baselines = []
+        for d in BaselineDirs:
+            self.baselines.append(normalize_path_join(d, self.name))
         self.diagmsgs = []
         self.utime = -1
         self.utime_base = self.mgr.testTimingBaseline(self)
         self.utime_perc = 0.0
         self.utime_exceeded = False
 
         self.rmTmp()
         mkdir(self.tmpdir)
 
         for d in self.baselines:
             mkdir(d)
 
-        for (fname, lines) in self.files:
+        for fname, lines in self.files:
             fname = os.path.join(self.tmpdir, fname)
 
             subdir = os.path.dirname(fname)
 
             if subdir != "":
                 mkdir(subdir)
             try:
-                ffile = open(fname, "w")
-            except IOError as e:
-                error("cannot write test's additional file '%s'" % fname)
+                ffile = open(fname, "w", newline="\n")
+            except OSError:
+                error(f"cannot write test's additional file '{fname}'")
 
             for line in lines:
                 ffile.write(line)
 
             ffile.close()
 
         for file in self.copy_files:
             src = replaceEnvs(file)
             try:
                 shutil.copy2(src, self.tmpdir)
-            except IOError as e:
-                error("cannot copy %s: %s" % (src, e))
+            except OSError as e:
+                error(f"cannot copy {src}: {e}")
 
-        for (file, content) in self.contents:
-            localfile = os.path.join(self.tmpdir, os.path.basename(file))
-            out = io.open(localfile, "w", encoding=getDefaultBtestEncoding())
+        for file, content in self.contents:
+            localfile = normalize_path_join(self.tmpdir, os.path.basename(file))
+            out = open(localfile, "w", encoding="utf-8", newline="\n")
 
             try:
                 for line in content:
                     out.write(line)
             except UnicodeEncodeError as e:
-                error("unicode encode error in file %s: %s" % (localfile, e))
+                error(f"unicode encode error in file {localfile}: {e}")
 
             out.close()
 
-        self.log = open(os.path.join(self.tmpdir, ".log"), "w")
-        self.stdout = open(os.path.join(self.tmpdir, ".stdout"), "w")
-        self.stderr = open(os.path.join(self.tmpdir, ".stderr"), "w")
+        self.log = open(os.path.join(self.tmpdir, ".log"), "w", encoding="utf-8")
+        self.stdout = open(os.path.join(self.tmpdir, ".stdout"), "a", encoding="utf-8")
+        self.stderr = open(os.path.join(self.tmpdir, ".stderr"), "a", encoding="utf-8")
 
         for cmd in self.requires:
             (success, rc) = self.execute(cmd, apply_alternative=self.alternative)
 
             if not success:
                 self.mgr.testSkipped(self)
                 if not Options.tmps:
-                    self.rmTmp()
+                    self.rmTmp(with_close=True)
                 self.finish()
                 return
 
         # Spawn thread that monitors for progress updates.
         # Note: We do indeed spawn a thread here, not a process, so
         # that the callback can modify the test object to maintain
         # state.
@@ -1046,23 +1239,25 @@
         # Run test's commands. First, construct a series of command sequences:
         # each sequence consists of test commands with an optional teardown that
         # always runs, regardless of prior test failures.
 
         seq = CmdSeq()
 
         if Initializer:
-            seq.cmds.append(CmdLine("%s %s" % (Initializer, self.name), True, 1, "<Initializer>"))
+            seq.cmds.append(
+                CmdLine(f"{Initializer} {self.name}", True, 1, "<Initializer>")
+            )
 
         seq.cmds += self.cmdseqs
 
         if Finalizer:
-            seq.cmds.append(CmdLine("%s %s" % (Finalizer, self.name), True, 1, "<Finalizer>"))
+            seq.cmds.append(CmdLine(f"{Finalizer} {self.name}", True, 1, "<Finalizer>"))
 
         if Teardown:
-            seq.teardown = CmdLine("%s %s" % (Teardown, self.name), True, 1, "<Teardown>")
+            seq.teardown = CmdLine(f"{Teardown} {self.name}", True, 1, "<Teardown>")
 
         failures = 0
         rc = 0
 
         # Executes the provided Cmdseq command sequence. Helper function, so we
         # can recurse when a Cmdseq's command list includes other sequences.
         def run_cmdseq(seq):
@@ -1076,22 +1271,30 @@
                 skip_part = -1
 
                 for cmd in seq.cmds:
                     # If the next command is a CmdSeq, process it recursively
                     # first. This processes teardowns for those sequences as
                     # needed, and skips them when nothing was actually run in a
                     # CmdSeq.
-                    if isinstance(cmd, CmdSeq):
+                    #
+                    # The use of isinstance() to determine "is a CmdSeq" is
+                    # dangerous since e.g. the dill serializer creates a
+                    # different type upon un-serializing, failing
+                    # isinstance(). So we take the class name as a sufficent
+                    # signal.
+                    if type(cmd).__name__ == "CmdSeq":
                         need_teardown |= run_cmdseq(cmd)
                         continue
 
                     if skip_part >= 0 and skip_part == cmd.part:
                         continue
 
-                    (success, rc) = self.execute(cmd, apply_alternative=self.alternative)
+                    (success, rc) = self.execute(
+                        cmd, apply_alternative=self.alternative
+                    )
                     need_teardown = True
 
                     if not success:
                         failures += 1
 
                         if Options.sphinx:
                             # We still execute the remaining commands and
@@ -1103,20 +1306,22 @@
                         if failures == 1:
                             self.mgr.testFailed(self)
 
                         if rc != 100:
                             break
 
             if need_teardown and seq.teardown:
-                (success, teardown_rc) = self.execute(seq.teardown,
-                                                      apply_alternative=self.alternative,
-                                                      addl_envs={
-                                                          'TEST_FAILED': int(failures > 0),
-                                                          'TEST_LAST_RETCODE': rc
-                                                      })
+                (success, teardown_rc) = self.execute(
+                    seq.teardown,
+                    apply_alternative=self.alternative,
+                    addl_envs={
+                        "TEST_FAILED": int(failures > 0),
+                        "TEST_LAST_RETCODE": rc,
+                    },
+                )
 
                 # A teardown can fail an otherwise successful test run, with the
                 # same special-casing of return codes 100 and 200. When failing
                 # on top of an already failing run, the return code will
                 # override the previous one. If a failing teardown wants to
                 # preserve the run's existing failing error code, it has access
                 # to it via the TEST_LAST_RETCODE environment variable.
@@ -1145,41 +1350,44 @@
         self.utime_exceeded = False
 
         if failures == 0:
             # If we don't have a timing baseline, we silently ignore that so that
             # on systems that can't measure execution time, the test will just pass.
             if self.utime_base >= 0 and self.utime >= 0:
                 delta = getOption("TimingDeltaPerc", "1.0")
-                self.utime_perc = (100.0 * (self.utime - self.utime_base) / self.utime_base)
-                self.utime_exceeded = (abs(self.utime_perc) > float(delta))
+                self.utime_perc = (
+                    100.0 * (self.utime - self.utime_base) / self.utime_base
+                )
+                self.utime_exceeded = abs(self.utime_perc) > float(delta)
 
             if self.utime_exceeded and not Options.update_times:
                 self.diagmsgs += [
-                    "'%s' exceeded permitted execution time deviation%s" %
-                    (self.name, self.timePostfix())
+                    "'%s' exceeded permitted execution time deviation%s"
+                    % (self.name, self.timePostfix())
                 ]
                 self.mgr.testFailed(self)
 
             else:
                 self.mgr.testSucceeded(self)
 
             if not Options.tmps and self.reruns == 0:
-                self.rmTmp()
+                self.rmTmp(with_close=True)
 
         self.finish()
 
     def finish(self):
         if self.bound_ports:
             self.mgr.returnPorts([p for p in self.bound_ports])
 
         self.bound_ports = []
 
         for d in self.baselines:
             try:
-                # Try removing the baseline directory. If it works, it's empty, i.e., no baseline was created.
+                # Try removing the baseline directory. If it works, it's empty,
+                # i.e., no baseline was created.
                 os.rmdir(d)
             except OSError:
                 pass
 
         self.log.close()
         self.stdout.close()
         self.stderr.close()
@@ -1191,74 +1399,84 @@
     def execute(self, cmd, apply_alternative=None, addl_envs=None):
         filter_cmd = None
         cmdline = cmd.cmdline
         env = {}
 
         # Apply alternative if requested.
         if apply_alternative:
-
             alt = Alternatives[apply_alternative]
 
             try:
                 (path, executable) = os.path.split(cmdline.split()[0])
                 filter_cmd = alt.filters[executable]
             except LookupError:
                 pass
 
-            for (key, val) in alt.substitutions.items():
+            for key, val in alt.substitutions.items():
                 cmdline = re.sub("\\b" + re.escape(key) + "\\b", val, cmdline)
 
             env = alt.envs
 
-        localfile = os.path.join(self.tmpdir, os.path.basename(cmd.file))
+        localfile = normalize_path_join(self.tmpdir, os.path.basename(cmd.file))
 
-        if filter_cmd and cmd.expect_success:  # Do not apply filter if we expect failure.
+        # Do not apply filter if we expect failure.
+        if filter_cmd and cmd.expect_success:
             # This is not quite correct as it does not necessarily need to be
             # the %INPUT file which we are filtering ...
-            filtered = os.path.join(self.tmpdir, "filtered-%s" % os.path.basename(localfile))
-
-            filter = CmdLine("%s %s %s" % (filter_cmd, localfile, filtered), True, 1, "<Filter>")
+            filtered = normalize_path_join(
+                self.tmpdir, "filtered-%s" % os.path.basename(localfile)
+            )
+
+            filter = CmdLine(
+                f"{filter_cmd} {localfile} {filtered}", True, 1, "<Filter>"
+            )
 
             (success, rc) = self.execute(filter, apply_alternative=None)
             if not success:
                 return (False, rc)
 
-            mv = CmdLine("mv %s %s" % (filtered, localfile), True, 1, "<Filter-Move>")
+            mv = CmdLine(f"mv {filtered} {localfile}", True, 1, "<Filter-Move>")
             (success, rc) = self.execute(mv, apply_alternative=None)
 
             if not success:
                 return (False, rc)
 
         self.mgr.testCommand(self, cmd)
 
         # Replace special names.
 
         if localfile:
             cmdline = RE_INPUT.sub(localfile, cmdline)
 
         cmdline = RE_DIR.sub(self.dir, cmdline)
 
-        print("%s (expect %s)" % (cmdline, ("failure", "success")[cmd.expect_success]),
-              file=self.log)
+        print(
+            f"{cmdline}: (expect {'success' if cmd.expect_success else 'failure'})",
+            file=self.log,
+        )
 
         # Additional environment variables provided by the caller override any
         # existing ones, but are generally not assumed to collide:
         if addl_envs:
             env.update(addl_envs)
 
         env = self.prepareEnv(cmd, env)
-        measure_time = self.measure_time and (Options.update_times or self.utime_base >= 0)
-
-        (success, rc, utime) = runTestCommandLine(cmdline,
-                                                  measure_time,
-                                                  cwd=self.tmpdir,
-                                                  shell=True,
-                                                  env=env,
-                                                  stderr=self.stderr,
-                                                  stdout=self.stdout)
+        measure_time = self.measure_time and (
+            Options.update_times or self.utime_base >= 0
+        )
+
+        (success, rc, utime) = runTestCommandLine(
+            cmdline,
+            measure_time,
+            cwd=self.tmpdir,
+            shell=True,
+            env=env,
+            stderr=self.stderr,
+            stdout=self.stdout,
+        )
 
         if utime > 0:
             self.utime += utime
 
         if success:
             if cmd.expect_success:
                 return (True, rc)
@@ -1266,44 +1484,51 @@
             self.diagmsgs += ["'%s' succeeded unexpectedly (exit code 0)" % cmdline]
             return (False, 0)
 
         else:
             if not cmd.expect_success:
                 return (True, rc)
 
-            self.diagmsgs += ["'%s' failed unexpectedly (exit code %s)" % (cmdline, rc)]
+            self.diagmsgs += [f"'{cmdline}' failed unexpectedly (exit code {rc})"]
             return (False, rc)
 
-    def rmTmp(self):
+    def rmTmp(self, *, with_close=False):
+        if with_close:
+            self.log.close()
+            self.stdout.close()
+            self.stderr.close()
+
         try:
             if os.path.isfile(self.tmpdir):
                 os.remove(self.tmpdir)
 
             if os.path.isdir(self.tmpdir):
-                subprocess.call("rm -rf %s 2>/dev/null" % self.tmpdir, shell=True)
+                subprocess.call(["rm", "-rf", self.tmpdir], stderr=subprocess.DEVNULL)
 
         except OSError as e:
-            error("cannot remove tmp directory %s: %s" % (self.tmpdir, e))
+            error(f"cannot remove tmp directory {self.tmpdir}: {e}")
 
     # Prepares the environment for the child processes.
-    def prepareEnv(self, cmd, addl={}):
+    def prepareEnv(self, cmd, addl=None):
+        if addl is None:
+            addl = {}
         env = copy.deepcopy(os.environ)
 
-        env["TEST_BASELINE"] = ":".join(self.baselines)
+        env["TEST_BASELINE"] = os.pathsep.join(self.baselines)
         env["TEST_DIAGNOSTICS"] = self.diag
         env["TEST_MODE"] = Options.mode.upper()
         env["TEST_NAME"] = self.name
         env["TEST_VERBOSE"] = self.verbose
         env["TEST_PART"] = str(cmd.part)
         env["TEST_BASE"] = TestBase
 
-        for (key, val) in addl.items():
+        for key, val in addl.items():
             # Convert val to string since otherwise os.environ (and our clone)
             # trigger a TypeError upon insertion, and the caller may be unaware.
-            env[key.upper()] = str(val)
+            env[key] = str(val)
 
         for idx, key in enumerate(sorted(self.ports)):
             env[key] = str(self.bound_ports[idx]) + "/tcp"
 
         return env
 
     def addFiles(self, files):
@@ -1326,36 +1551,39 @@
             for file in sorted(glob.glob(path)):
                 try:
                     for line in open(file):
                         msg = line.strip()
                         self.mgr.testProgress(self, msg)
 
                     os.unlink(file)
-                except (IOError, OSError):
+                except OSError:
                     pass
 
 
 ### Output handlers.
 
 
 class OutputHandler:
-    def __init__(self, options):
+    def __init__(self, options, outfile=sys.__stderr__):
         """Base class for reporting progress and results to user. We derive
         several classes from this one, with the one being used depending on
         which output the users wants.
 
         A handler's method are called from test TestMgr and may be called
         interleaved from different tests. However, the TestMgr locks before
         each call so that it's guaranteed that two calls don't run
         concurrently.
 
         options: An optparser with the global options.
+
+        outfile: The destination file object to write output to.
         """
         self._buffered_output = {}
         self._options = options
+        self._outfile = outfile
 
     def prepare(self, mgr):
         """The TestManager calls this with itself as an argument just before
         it starts running tests."""
         pass
 
     def options(self):
@@ -1363,21 +1591,25 @@
         return self._options
 
     def threadPrefix(self):
         """With multiple threads, returns a string with the thread's name in
         a form suitable to prefix output with. With a single thread, returns
         the empty string."""
         if self.options().threads > 1:
-            return "[%s]" % multiprocessing.current_process().name
+            # TestManager.run() defines the process names to "#<n>".  Align the
+            # prefixes by using enough space for the number of threads
+            # requested, plus 1 for "#".
+            pat = "[%%+%ds]" % (len(str(self.options().threads)) + 1)
+            return pat % mp.current_process().name
         else:
             return ""
 
     def _output(self, msg, nl=True, file=None):
         if not file:
-            file = sys.stderr
+            file = reopen_std_file(self._outfile)
 
         if nl:
             print(msg, file=file)
         else:
             if msg:
                 print(msg, end=" ", file=file)
 
@@ -1399,25 +1631,25 @@
             self._buffered_output[test.name] = [(msg, nl, file)]
 
     def replayOutput(self, test):
         """Prints out all output buffered in threaded mode by output()."""
         if test.name not in self._buffered_output:
             return
 
-        for (msg, nl, file) in self._buffered_output[test.name]:
+        for msg, nl, file in self._buffered_output[test.name]:
             self._output(msg, nl, file)
 
         self._buffered_output[test.name] = []
 
     # Methods to override.
     def testStart(self, test):
         """Called just before a test begins."""
 
     def testCommand(self, test, cmdline):
-        """Called just before a command line is exected for a trace."""
+        """Called just before a command line is executed for a trace."""
 
     def testProgress(self, test, msg):
         """Called when a test signals having made progress."""
 
     def testSucceeded(self, test, msg):
         """Called when a test was successful."""
 
@@ -1444,14 +1676,15 @@
     """
     Forwards output to several other handlers.
 
     options: An optparser with the global options.
 
     handlers: List of output handlers to forward to.
     """
+
     def __init__(self, options, handlers):
         OutputHandler.__init__(self, options)
         self._handlers = handlers
 
     def prepare(self, mgr):
         """Called just before test manager starts running tests."""
         for h in self._handlers:
@@ -1459,15 +1692,15 @@
 
     def testStart(self, test):
         """Called just before a test begins."""
         for h in self._handlers:
             h.testStart(test)
 
     def testCommand(self, test, cmdline):
-        """Called just before a command line is exected for a trace."""
+        """Called just before a command line is executed for a trace."""
         for h in self._handlers:
             h.testCommand(test, cmdline)
 
     def testProgress(self, test, msg):
         """Called when a test signals having made progress."""
         for h in self._handlers:
             h.testProgress(test, msg)
@@ -1501,14 +1734,21 @@
 
     def finished(self):
         for h in self._handlers:
             h.finished()
 
 
 class Standard(OutputHandler):
+    """
+    The default output handler, writing plain lines with test outcome.
+
+    Each test result is reported. For parallelized operation, the output
+    includes the thread number processing the test.
+    """
+
     def testStart(self, test):
         self.output(test, self.threadPrefix(), nl=False)
         self.output(test, "%s ..." % test.displayName(), nl=False)
         test._std_nl = False
 
     def testCommand(self, test, cmdline):
         pass
@@ -1540,150 +1780,161 @@
 
     def testUnstable(self, test, msg):
         self.finalMsg(test, msg)
 
 
 class Console(OutputHandler):
     """
-    Output handler that writes colorful progress report to the console.
+    Output handler that writes colorful progress report to stdout.
 
     This handler works well in settings that can handle coloring but not
     cursor placement commands (for example because moving to the beginning of
     the line overwrites other surrounding output); it's what the
     ``--show-all`` output uses. In contrast, the *CompactConsole* handler uses
     cursor placement in addition for a more space-efficient output.
     """
+
     Green = "\033[32m"
     Red = "\033[31m"
     Yellow = "\033[33m"
     Gray = "\033[37m"
     DarkGray = "\033[1;30m"
     Normal = "\033[0m"
 
     def __init__(self, options):
-        OutputHandler.__init__(self, options)
-        self.show_all = True
+        OutputHandler.__init__(self, options, reopen_std_file(sys.__stdout__))
 
     def testStart(self, test):
         msg = "[%3d%%] %s ..." % (test.mgr.percentage(), test.displayName())
-        self._consoleOutput(test, msg, False)
+        self.output(test, msg, nl=False)
 
     def testProgress(self, test, msg):
         """Called when a test signals having made progress."""
         msg = self.DarkGray + "(%s)" % msg + self.Normal
-        self._consoleOutput(test, msg, True)
+        self.output(test, msg)
 
     def testSucceeded(self, test, msg):
         if test.known_failure:
             msg = self.Yellow + msg + self.Normal
         else:
             msg = self.Green + msg + self.Normal
 
-        self._consoleOutput(test, msg, self.show_all)
+        self.output(test, msg)
 
     def testFailed(self, test, msg):
         if test.known_failure:
             msg = self.Yellow + msg + self.Normal
         else:
             msg = self.Red + msg + self.Normal
 
-        self._consoleOutput(test, msg, True)
+        self.output(test, msg)
 
     def testUnstable(self, test, msg):
         msg = self.Yellow + msg + self.Normal
-        self._consoleOutput(test, msg, True)
+        self.output(test, msg)
 
     def testSkipped(self, test, msg):
         msg = self.Gray + msg + self.Normal
-        self._consoleOutput(test, msg, self.show_all)
-
-    def finished(self):
-        sys.stdout.flush()
-
-    def _consoleOutput(self, test, msg, sticky):
-        self._consoleWrite(test, msg, sticky)
-
-    def _consoleWrite(self, test, msg, sticky):
-        sys.stdout.write(msg.strip() + " ")
-
-        if sticky:
-            sys.stdout.write("\n")
-
-        sys.stdout.flush()
+        self.output(test, msg)
 
 
 class CompactConsole(Console):
     """
     Output handler that writes compact, colorful progress report to
-    the console while also keeping the output compact by keeping
+    stdout while also keeping the output compact by keeping
     output only for failing tests.
 
     This handler adds cursor mods and navigation to the coloring provided by
     the Console class and hence needs settings that can handle both.
     """
+
     CursorOff = "\033[?25l"
     CursorOn = "\033[?25h"
     EraseToEndOfLine = "\033[2K"
 
     def __init__(self, options):
         Console.__init__(self, options)
-        self.show_all = False
 
         def cleanup():
-            sys.stdout.write(self.CursorOn)
+            self._outfile.write(self.CursorOn)
 
         atexit.register(cleanup)
 
     def testStart(self, test):
         test.console_last_line = None
         self._consoleOutput(test, "", False)
-        sys.stdout.write(self.CursorOff)
+        self._outfile.write(self.CursorOff)
 
     def testProgress(self, test, msg):
         """Called when a test signals having made progress."""
         msg = " " + self.DarkGray + "(%s)" % msg + self.Normal
         self._consoleAugment(test, msg)
 
+    def testSucceeded(self, test, msg):
+        if test.known_failure:
+            msg = self.Yellow + msg + self.Normal
+        else:
+            msg = self.Green + msg + self.Normal
+
+        self._consoleOutput(test, msg, False)
+
+    def testFailed(self, test, msg):
+        if test.known_failure:
+            msg = self.Yellow + msg + self.Normal
+        else:
+            msg = self.Red + msg + self.Normal
+
+        self._consoleOutput(test, msg, True)
+
     def testFinished(self, test, msg):
         test.console_last_line = None
 
+    def testUnstable(self, test, msg):
+        msg = self.Yellow + msg + self.Normal
+        self._consoleOutput(test, msg, True)
+
+    def testSkipped(self, test, msg):
+        msg = self.Gray + msg + self.Normal
+        self._consoleOutput(test, msg, False)
+
     def finished(self):
-        sys.stdout.write(self.EraseToEndOfLine)
-        sys.stdout.write("\r")
-        sys.stdout.write(self.CursorOn)
-        sys.stdout.flush()
+        self._outfile.write(self.EraseToEndOfLine)
+        self._outfile.write("\r")
+        self._outfile.write(self.CursorOn)
+        self._outfile.flush()
 
     def _consoleOutput(self, test, msg, sticky):
         line = "[%3d%%] %s ..." % (test.mgr.percentage(), test.displayName())
 
         if msg:
             line += " " + msg
 
         test.console_last_line = line
         self._consoleWrite(test, line, sticky)
 
     def _consoleAugment(self, test, msg):
-        sys.stdout.write(self.EraseToEndOfLine)
-        sys.stdout.write(" %s" % msg.strip())
-        sys.stdout.write("\r%s" % test.console_last_line)
-        sys.stdout.flush()
+        self._outfile.write(self.EraseToEndOfLine)
+        self._outfile.write(" %s" % msg.strip())
+        self._outfile.write("\r%s" % test.console_last_line)
+        self._outfile.flush()
 
     def _consoleWrite(self, test, msg, sticky):
-        sys.stdout.write(chr(27) + '[2K')
-        sys.stdout.write("\r%s" % msg.strip())
+        self._outfile.write(chr(27) + "[2K")
+        self._outfile.write("\r%s" % msg.strip())
 
         if sticky:
-            sys.stdout.write("\n")
+            self._outfile.write("\n")
             test.console_last_line = None
 
-        sys.stdout.flush()
+        self._outfile.flush()
 
 
 class Brief(OutputHandler):
     """Output handler for producing the brief output format."""
+
     def testStart(self, test):
         pass
 
     def testCommand(self, test, cmdline):
         pass
 
     def testProgress(self, test, msg):
@@ -1691,62 +1942,63 @@
         pass
 
     def testSucceeded(self, test, msg):
         pass
 
     def testFailed(self, test, msg):
         self.output(test, self.threadPrefix(), nl=False)
-        self.output(test, "%s ... %s" % (test.displayName(), msg))
+        self.output(test, f"{test.displayName()} ... {msg}")
 
     def testUnstable(self, test, msg):
         self.output(test, self.threadPrefix(), nl=False)
-        self.output(test, "%s ... %s" % (test.displayName(), msg))
+        self.output(test, f"{test.displayName()} ... {msg}")
 
     def testSkipped(self, test, msg):
         pass
 
 
 class Verbose(OutputHandler):
     """Output handler for producing the verbose output format."""
+
     def testStart(self, test):
         self.output(test, self.threadPrefix(), nl=False)
         self.output(test, "%s ..." % test.displayName())
 
     def testCommand(self, test, cmdline):
         part = ""
 
         if cmdline.part > 1:
             part = " [part #%d]" % cmdline.part
 
         self.output(test, self.threadPrefix(), nl=False)
-        self.output(test, "  > %s%s" % (cmdline.cmdline, part))
+        self.output(test, f"  > {cmdline.cmdline}{part}")
 
     def testProgress(self, test, msg):
         """Called when a test signals having made progress."""
         self.output(test, "  - " + msg)
 
     def testSucceeded(self, test, msg):
         self.output(test, self.threadPrefix(), nl=False)
         self.showTestVerbose(test)
-        self.output(test, "... %s %s" % (test.displayName(), msg))
+        self.output(test, f"... {test.displayName()} {msg}")
 
     def testFailed(self, test, msg):
         self.output(test, self.threadPrefix(), nl=False)
         self.showTestVerbose(test)
-        self.output(test, "... %s %s" % (test.displayName(), msg))
+        self.output(test, f"... {test.displayName()} {msg}")
 
     def testUnstable(self, test, msg):
         self.output(test, self.threadPrefix(), nl=False)
         self.showTestVerbose(test)
-        self.output(test, "... %s %s" % (test.displayName(), msg))
+        self.output(test, f"... {test.displayName()} {msg}")
 
     def testSkipped(self, test, msg):
         self.output(test, self.threadPrefix(), nl=False)
         self.showTestVerbose(test)
-        self.output(test, "... %s %s" % (test.displayName(), msg))
+        self.output(test, f"... {test.displayName()} {msg}")
 
     def showTestVerbose(self, test):
         if not os.path.exists(test.verbose):
             return
 
         for line in open(test.verbose):
             self.output(test, "  > [test-verbose] %s" % line.strip())
@@ -1790,100 +2042,105 @@
 
     def testCommand(self, test, cmdline):
         pass
 
     def testSucceeded(self, test, msg):
         if self._all:
             if self._file:
-                self.output(test, "%s ... %s" % (test.displayName(), msg), True, self._file)
+                self.output(test, f"{test.displayName()} ... {msg}", True, self._file)
 
             self.showDiag(test)
 
     def testFailed(self, test, msg):
         if self._file:
-            self.output(test, "%s ... %s" % (test.displayName(), msg), True, self._file)
+            self.output(test, f"{test.displayName()} ... {msg}", True, self._file)
 
         if (not test.known_failure) or self._all:
             self.showDiag(test)
 
     def testUnstable(self, test, msg):
         if self._file:
-            self.output(test, "%s ... %s" % (test.displayName(), msg), True, self._file)
+            self.output(test, f"{test.displayName()} ... {msg}", True, self._file)
 
     def testSkipped(self, test, msg):
         if self._file:
-            self.output(test, "%s ... %s" % (test.displayName(), msg), True, self._file)
+            self.output(test, f"{test.displayName()} ... {msg}", True, self._file)
 
 
 class SphinxOutput(OutputHandler):
     def __init__(self, options, all=False, file=None):
         """Output handler for producing output when running from
         Sphinx. The main point here is that we save all diagnostic output to
         $BTEST_RST_OUTPUT.
 
         options: An optparser with the global options.
         """
         OutputHandler.__init__(self, options)
 
         self._output = None
+        self._part = None
 
         try:
             self._rst_output = os.environ["BTEST_RST_OUTPUT"]
         except KeyError:
-            print("warning: environment variable BTEST_RST_OUTPUT not set, will not produce output",
-                  file=sys.stderr)
+            print(
+                "warning: environment variable BTEST_RST_OUTPUT not set, will not produce output",
+                file=sys.stderr,
+            )
             self._rst_output = None
 
     def testStart(self, test):
         self._output = None
 
     def testCommand(self, test, cmdline):
         if not self._rst_output:
             return
 
-        self._output = "%s#%s" % (self._rst_output, cmdline.part)
+        self._output = f"{self._rst_output}#{cmdline.part}"
         self._part = cmdline.part
 
     def testSucceeded(self, test, msg):
         pass
 
     def testFailed(self, test, msg):
         if not self._output:
             return
 
-        out = open(self._output, "a")
+        out = open(self._output, "a", newline="\n")
 
         print("\n.. code-block:: none ", file=out)
-        print("\n  ERROR executing test '%s' (part %s)\n" % (test.displayName(), self._part),
-              file=out)
+        print(
+            "\n  ERROR executing test '%s' (part %s)\n"
+            % (test.displayName(), self._part),
+            file=out,
+        )
 
         for line in test.diagmsgs:
             print("  % " + line, file=out)
 
         test.diagmsgs = []
 
         for f in (test.diag, os.path.join(test.tmpdir, ".stderr")):
             if not f:
                 continue
 
             if os.path.isfile(f):
                 print("  % cat " + os.path.basename(f), file=out)
-                for line in open(f):
+                for line in open(f, newline="\n"):
                     print("   %s" % line.strip(), file=out)
                 print(file=out)
 
     def testUnstable(self, test, msg):
         pass
 
     def testSkipped(self, test, msg):
         pass
 
 
 class XMLReport(OutputHandler):
-
     RESULT_PASS = "pass"
     RESULT_FAIL = "failure"
     RESULT_SKIP = "skipped"
     RESULT_UNSTABLE = "unstable"
 
     def __init__(self, options, xmlfile):
         """Output handler for producing an XML report of test results.
@@ -1892,26 +2149,28 @@
 
         file: Output into given file
         """
         OutputHandler.__init__(self, options)
         self._file = xmlfile
         self._start = time.time()
         self._timestamp = datetime.now().isoformat()
+        self._results = None
 
     def prepare(self, mgr):
         self._results = mgr.list([])
 
     def testStart(self, test):
         pass
 
     def testCommand(self, test, cmdline):
         pass
 
-    def makeTestCaseElement(self, doc, testsuite, name, duration):
-        parts = name.split('.')
+    @staticmethod
+    def makeTestCaseElement(doc, testsuite, name, duration):
+        parts = name.split(".")
         if len(parts) > 1:
             classname = ".".join(parts[:-1])
             name = parts[-1]
         else:
             classname = parts[0]
             name = parts[0]
 
@@ -1919,26 +2178,27 @@
         e.setAttribute("classname", classname)
         e.setAttribute("name", name)
         e.setAttribute("time", str(duration))
         testsuite.appendChild(e)
 
         return e
 
-    def getContext(self, test, context_file):
+    @staticmethod
+    def getContext(test, context_file):
         context = ""
         for line in test.diagmsgs:
             context += "  % " + line + "\n"
 
         for f in (test.diag, os.path.join(test.tmpdir, context_file)):
             if not f:
                 continue
 
             if os.path.isfile(f):
                 context += "  % cat " + os.path.basename(f) + "\n"
-                for line in open(f):
+                for line in open(f, newline="\n"):
                     context += "  " + line.strip() + "\n"
 
         return context
 
     def addTestResult(self, test, status):
         context = ""
 
@@ -1970,15 +2230,17 @@
         num_tests = 0
         num_failures = 0
         doc = xml.dom.minidom.Document()
         testsuite = doc.createElement("testsuite")
         doc.appendChild(testsuite)
 
         for res in self._results:
-            test_case = self.makeTestCaseElement(doc, testsuite, res["name"], res["duration"])
+            test_case = self.makeTestCaseElement(
+                doc, testsuite, res["name"], res["duration"]
+            )
 
             if res["status"] != self.RESULT_PASS:
                 e = doc.createElement(res["status"])
                 e.setAttribute("type", res["status"])
                 text_node = doc.createTextNode(res["context"])
                 e.appendChild(text_node)
                 test_case.appendChild(e)
@@ -2009,37 +2271,99 @@
 
 class ChromeTracing(OutputHandler):
     """Output in Chrome tracing format.
 
     Output files can be loaded into Chrome browser under about:tracing, or
     converted to standalone HTML files with `trace2html`.
     """
+
     def __init__(self, options, tracefile):
         OutputHandler.__init__(self, options)
         self._file = tracefile
+        self._results = None
 
     def prepare(self, mgr):
         self._results = mgr.list([])
 
     def testFinished(self, test, _):
-        self._results.append({
-            "name": test.name,
-            "ts": test.start * 1e6,
-            "tid": multiprocessing.current_process().pid,
-            "pid": 1,
-            "ph": "X",
-            "cat": "test",
-            "dur": (time.time() - test.start) * 1e6,
-        })
+        self._results.append(
+            {
+                "name": test.name,
+                "ts": test.start * 1e6,
+                "tid": mp.current_process().pid,
+                "pid": 1,
+                "ph": "X",
+                "cat": "test",
+                "dur": (time.time() - test.start) * 1e6,
+            }
+        )
 
     def finished(self):
         print(json.dumps(list(self._results)), file=self._file)
         self._file.close()
 
 
+def create_output_handler(options):
+    output_handlers = []
+
+    if options.verbose:
+        output_handlers += [Verbose(options)]
+
+    elif options.brief:
+        output_handlers += [Brief(options)]
+
+    else:
+        if sys.stdout.isatty():
+            if options.show_all:
+                output_handlers += [Console(options)]
+            else:
+                output_handlers += [CompactConsole(options)]
+        else:
+            output_handlers += [Standard(options)]
+
+    if options.diagall:
+        output_handlers += [Diag(options, True, None)]
+
+    elif options.diag:
+        output_handlers += [Diag(options, False, None)]
+
+    if options.diagfile:
+        try:
+            diagfile = open(options.diagfile, "w", 1, newline="\n")
+            output_handlers += [Diag(options, options.diagall, diagfile)]
+
+        except OSError as e:
+            print(f"cannot open {options.diagfile}: {e}", file=sys.stderr)
+
+    if options.sphinx:
+        if sys.platform == "win32":
+            print("Sphinx support is disabled on Windows", file=sys.stderr)
+            sys.exit(1)
+
+        output_handlers += [SphinxOutput(options)]
+
+    if options.xmlfile:
+        try:
+            xmlfile = open(options.xmlfile, "w", 1, newline="\n")
+            output_handlers += [XMLReport(options, xmlfile)]
+
+        except OSError as e:
+            print(f"cannot open {options.xmlfile}: {e}", file=sys.stderr)
+
+    if options.tracefile:
+        try:
+            tracefile = open(options.tracefile, "w", 1, newline="\n")
+            output_handlers += [ChromeTracing(options, tracefile)]
+
+        except OSError as e:
+            print(f"cannot open {options.tracefile}: {e}", file=sys.stderr)
+
+    return Forwarder(options, output_handlers)
+
+
 ### Timing measurements.
 
 
 # Base class for all timers.
 class TimerBase:
     # Returns true if time measurement are supported by this class on the
     # current platform. Must be overidden by derived classes.
@@ -2063,25 +2387,29 @@
         if not platform() == "Linux":
             return False
 
         if not self.perf or not os.path.exists(self.perf):
             return False
 
         # Make sure it works.
-        (success, rc) = runSubprocess("%s stat -o /dev/null true 2>/dev/null" % self.perf,
-                                      shell=True)
+        (success, rc) = runSubprocess(
+            "%s stat -o /dev/null true 2>/dev/null" % self.perf, shell=True
+        )
         return success and rc == 0
 
     def timeSubprocess(self, *args, **kwargs):
         assert self.perf
 
         cargs = args
         ckwargs = kwargs
 
+        # fmt: off
         targs = [self.perf, "stat", "-o", ".timing", "-x", " ", "-e", "instructions", "sh", "-c"]
+        # fmt: on
+
         targs += [" ".join(cargs)]
         cargs = [targs]
         del ckwargs["shell"]
 
         (success, rc) = runSubprocess(*cargs, **ckwargs)
 
         utime = -1
@@ -2092,77 +2420,82 @@
                 if "instructions" in line and "not supported" not in line:
                     try:
                         m = line.split()
                         utime = int(m[0])
                     except ValueError:
                         pass
 
-        except IOError:
+        except OSError:
             pass
 
         return (success, rc, utime)
 
 
 # Walk the given directory and return all test files.
 def findTests(paths, expand_globs=False):
     tests = []
 
     ignore_files = getOption("IgnoreFiles", "").split()
     ignore_dirs = getOption("IgnoreDirs", "").split()
 
-    expanded = []
+    expanded = set()
 
     for p in paths:
         p = os.path.join(TestBase, p)
 
         if expand_globs:
-            expanded += [d for d in glob.glob(p) if os.path.isdir(d)]
+            for d in glob.glob(p):
+                if os.path.isdir(d):
+                    expanded.add(d)
         else:
-            expanded.append(p)
+            expanded.add(p)
 
     for path in expanded:
         rpath = os.path.relpath(path, TestBase)
 
         if os.path.isdir(path) and os.path.basename(path) in ignore_dirs:
             continue
 
-        ignores = [os.path.join(path, dir) for dir in ignore_dirs]
+        ignores = [normalize_path_join(path, dir) for dir in ignore_dirs]
 
         m = RE_PART.match(rpath)
         if m:
-            error("Do not specify files with part numbers directly, use the base test name (%s)" %
-                  rpath)
+            error(
+                "Do not specify files with part numbers directly, use the base test name (%s)"
+                % rpath
+            )
 
         if os.path.isfile(path):
             tests += readTestFile(path)
 
             # See if there are more parts.
             for part in glob.glob("%s#*" % rpath):
                 tests += readTestFile(part)
 
         elif os.path.isdir(path):
-            for (dirpath, dirnames, filenames) in os.walk(path):
-
+            for dirpath, dirnames, filenames in os.walk(path):
                 ign = os.path.join(dirpath, ".btest-ignore")
 
                 if os.path.isfile(os.path.join(ign)):
-                    del dirnames[0:len(dirnames)]
+                    del dirnames[0 : len(dirnames)]
                     continue
 
                 for file in filenames:
                     for gl in ignore_files:
                         if fnmatch.fnmatch(file, gl):
                             break
                     else:
                         tests += readTestFile(os.path.join(dirpath, file))
 
                 # Don't recurse into these.
-                for (dir, path) in [(dir, os.path.join(dirpath, dir)) for dir in dirnames]:
+                for dir, dir_path in [
+                    (dir, normalize_path_join(dirpath, dir)) for dir in dirnames
+                ]:
                     for skip in ignores:
-                        if path == skip:
+                        if dir_path == skip:
                             dirnames.remove(dir)
 
         else:
             # See if we have test(s) named like this in our configured set.
             found = False
             for t in Config.configured_tests:
                 if t and rpath == t.name:
@@ -2213,16 +2546,16 @@
         else:
             return previous.clone(content)
 
     if os.path.basename(filename) == ".btest-ignore":
         return []
 
     try:
-        input = io.open(filename, encoding=getDefaultBtestEncoding(), newline='')
-    except IOError as e:
+        input = open(filename, encoding="utf-8", newline="")
+    except OSError as e:
         error("cannot read test file: %s" % e)
 
     tests = []
     files = []
 
     content = []
     previous = None
@@ -2235,28 +2568,27 @@
     except UnicodeDecodeError as e:
         # This error is caused by either a test file with an invalid UTF-8 byte
         # sequence, or if python makes the wrong assumption about the encoding
         # of a test file (this can happen if a test file has valid UTF-8 but
         # none of the locale environment variables LANG, LC_CTYPE, or LC_ALL,
         # were defined prior to running btest).  However, if all test files
         # are ASCII, then this error should never occur.
-        error("unicode decode error in file %s: %s" % (filename, e))
+        error(f"unicode decode error in file {filename}: {e}")
 
     for line in lines:
-
         if state == "test":
             m = RE_START_FILE.search(line)
             if m:
                 state = "file"
                 file = (m.group(1), [])
                 continue
 
             m = RE_END_FILE.search(line)
             if m:
-                error("%s: unexpected %sEND-FILE" % (filename, CommandPrefix))
+                error(f"{filename}: unexpected {CommandPrefix}END-FILE")
 
             m = RE_START_NEXT_TEST.search(line)
             if not m:
                 content += [line]
                 continue
 
             t = newTest(content, previous)
@@ -2294,17 +2626,17 @@
         if t:
             t.addFiles(files)
 
     return tests
 
 
 def jOption(option, _, __, parser):
-    val = multiprocessing.cpu_count()
+    val = mp.cpu_count()
 
-    if parser.rargs and not parser.rargs[0].startswith('-'):
+    if parser.rargs and not parser.rargs[0].startswith("-"):
         try:
             # Next argument should be the non-negative number of threads.
             # Turn 0 into 1, for backward compatibility.
             val = max(1, int(parser.rargs[0]))
             parser.rargs.pop(0)
         except ValueError:
             # Default to using all CPUs. Flagging this as error risks
@@ -2341,553 +2673,651 @@
 
         if fmt == "rst":
             print("%s" % s)
             print("-" * len(s))
             print()
 
             for t in tests:
-                print("%s``%s``:" % (indent(1), t.name))
+                print(f"{indent(1)}``{t.name}``:")
                 for d in doc(t):
-                    print("%s%s" % (indent(2), d))
+                    print(f"{indent(2)}{d}")
                 print()
 
         if fmt == "md":
             print("# %s" % s)
             print()
 
             for t in tests:
                 print("* `%s`:" % t.name)
                 for d in doc(t):
-                    print("%s%s" % (indent(1), d))
+                    print(f"{indent(1)}{d}")
 
             print()
 
 
+def parse_options():
+    optparser = optparse.OptionParser(
+        usage="%prog [options] <directories>", version=VERSION
+    )
+    optparser.add_option(
+        "-U",
+        "--update-baseline",
+        action="store_const",
+        dest="mode",
+        const="UPDATE",
+        help="create a new baseline from the tests' output",
+    )
+    optparser.add_option(
+        "-u",
+        "--update-interactive",
+        action="store_const",
+        dest="mode",
+        const="UPDATE_INTERACTIVE",
+        help="interactively asks whether to update baseline for a failed test",
+    )
+    optparser.add_option(
+        "-d",
+        "--diagnostics",
+        action="store_true",
+        dest="diag",
+        default=False,
+        help="show diagnostic output for failed tests",
+    )
+    optparser.add_option(
+        "-D",
+        "--diagnostics-all",
+        action="store_true",
+        dest="diagall",
+        default=False,
+        help="show diagnostic output for ALL tests",
+    )
+    optparser.add_option(
+        "-f",
+        "--file-diagnostics",
+        action="store",
+        type="string",
+        dest="diagfile",
+        default="",
+        help=(
+            "write diagnostic output for failed tests into file; "
+            "if file exists, it is overwritten"
+        ),
+    )
+    optparser.add_option(
+        "-v",
+        "--verbose",
+        action="store_true",
+        dest="verbose",
+        default=False,
+        help="show commands as they are executed",
+    )
+    optparser.add_option(
+        "-w",
+        "--wait",
+        action="store_true",
+        dest="wait",
+        default=False,
+        help="wait for <enter> after each failed (with -d) or all (with -D) tests",
+    )
+    optparser.add_option(
+        "-b",
+        "--brief",
+        action="store_true",
+        dest="brief",
+        default=False,
+        help="outputs only failed tests",
+    )
+    optparser.add_option(
+        "-c",
+        "--config",
+        action="store",
+        type="string",
+        dest="config",
+        default=ConfigDefault,
+        help="configuration file",
+    )
+    optparser.add_option(
+        "-t",
+        "--tmp-keep",
+        action="store_true",
+        dest="tmps",
+        default=False,
+        help="do not delete tmp files created for running tests",
+    )
+    optparser.add_option(
+        "-j",
+        "--jobs",
+        action="callback",
+        callback=jOption,
+        dest="threads",
+        default=1,
+        help="number of threads running tests in parallel; with no argument will use all CPUs",
+    )
+    optparser.add_option(
+        "-g",
+        "--groups",
+        action="store",
+        type="string",
+        dest="groups",
+        default="",
+        help="execute only tests of given comma-separated list of groups",
+    )
+    optparser.add_option(
+        "-r",
+        "--rerun",
+        action="store_true",
+        dest="rerun",
+        default=False,
+        help="execute commands for tests that failed last time",
+    )
+    optparser.add_option(
+        "-q",
+        "--quiet",
+        action="store_true",
+        dest="quiet",
+        default=False,
+        help="suppress information output other than about failed tests",
+    )
+    optparser.add_option(
+        "-x",
+        "--xml",
+        action="store",
+        type="string",
+        dest="xmlfile",
+        default="",
+        help=(
+            "write a report of test results in JUnit XML format to file; "
+            "if file exists, it is overwritten"
+        ),
+    )
+    optparser.add_option(
+        "-a",
+        "--alternative",
+        action="store",
+        type="string",
+        dest="alternatives",
+        default=None,
+        help="activate given alternative",
+    )
+    optparser.add_option(
+        "-S",
+        "--sphinx",
+        action="store_true",
+        dest="sphinx",
+        default=False,
+        help="indicates that we're running from inside Sphinx; for internal purposes",
+    )
+    optparser.add_option(
+        "-T",
+        "--update-times",
+        action="store_true",
+        dest="update_times",
+        default=False,
+        help="create a new timing baseline for tests being measured",
+    )
+    optparser.add_option(
+        "-R",
+        "--documentation",
+        action="store",
+        type="choice",
+        dest="doc",
+        choices=("rst", "md"),
+        metavar="format",
+        default=None,
+        help="Output documentation for tests, supported formats: rst, md",
+    )
+    optparser.add_option(
+        "-A",
+        "--show-all",
+        action="store_true",
+        default=False,
+        help=(
+            "For console output, show one-liners for passing/skipped tests "
+            "in addition to any failing ones"
+        ),
+    )
+    optparser.add_option(
+        "-z",
+        "--retries",
+        action="store",
+        dest="retries",
+        type="int",
+        default=0,
+        help="Retry failed tests this many times to determine if they are unstable",
+    )
+    optparser.add_option(
+        "--trace-file",
+        action="store",
+        dest="tracefile",
+        default="",
+        help="write Chrome tracing file to file; if file exists, it is overwritten",
+    )
+    optparser.add_option(
+        "-F",
+        "--abort-on-failure",
+        action="store_true",
+        dest="abort_on_failure",
+        help="terminate after first test failure",
+    )
+    optparser.add_option(
+        "-l",
+        "--list",
+        action="store_true",
+        dest="list",
+        default=False,
+        help="list available tests instead of executing them",
+    )
+    optparser.add_option(
+        "-s",
+        "--set",
+        action="append",
+        dest="defaults",
+        default=[],
+        help=(
+            "Override default key used in btest.cfg with another value. "
+            "Can be specified multiple times."
+        ),
+    )
+
+    optparser.set_defaults(mode="TEST")
+
+    (options, parsed_args) = optparser.parse_args()
+
+    # Update-interactive mode implies single-threaded operation
+    if options.mode == "UPDATE_INTERACTIVE" and options.threads > 1:
+        warning("ignoring requested parallelism in interactive-update mode")
+        options.threads = 1
+
+    if not os.path.exists(options.config):
+        error("configuration file '%s' not found" % options.config)
+
+    return options, parsed_args
+
+
 ### Main
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Python 3.8+ on macOS no longer uses "fork" as the default start-method
     # See https://github.com/zeek/btest/issues/26
     pyver_maj = sys.version_info[0]
     pyver_min = sys.version_info[1]
 
-    if (pyver_maj == 3 and pyver_min >= 8) or pyver_maj > 3:
-        multiprocessing.set_start_method('fork')
-
-optparser = optparse.OptionParser(usage="%prog [options] <directories>", version=VERSION)
-optparser.add_option("-U",
-                     "--update-baseline",
-                     action="store_const",
-                     dest="mode",
-                     const="UPDATE",
-                     help="create a new baseline from the tests' output")
-optparser.add_option("-u",
-                     "--update-interactive",
-                     action="store_const",
-                     dest="mode",
-                     const="UPDATE_INTERACTIVE",
-                     help="interactively asks whether to update baseline for a failed test")
-optparser.add_option("-d",
-                     "--diagnostics",
-                     action="store_true",
-                     dest="diag",
-                     default=False,
-                     help="show diagnostic output for failed tests")
-optparser.add_option("-D",
-                     "--diagnostics-all",
-                     action="store_true",
-                     dest="diagall",
-                     default=False,
-                     help="show diagnostic output for ALL tests")
-optparser.add_option(
-    "-f",
-    "--file-diagnostics",
-    action="store",
-    type="string",
-    dest="diagfile",
-    default="",
-    help="write diagnostic output for failed tests into file; if file exists, it is overwritten")
-optparser.add_option("-v",
-                     "--verbose",
-                     action="store_true",
-                     dest="verbose",
-                     default=False,
-                     help="show commands as they are executed")
-optparser.add_option("-w",
-                     "--wait",
-                     action="store_true",
-                     dest="wait",
-                     default=False,
-                     help="wait for <enter> after each failed (with -d) or all (with -D) tests")
-optparser.add_option("-b",
-                     "--brief",
-                     action="store_true",
-                     dest="brief",
-                     default=False,
-                     help="outputs only failed tests")
-optparser.add_option("-c",
-                     "--config",
-                     action="store",
-                     type="string",
-                     dest="config",
-                     default=ConfigDefault,
-                     help="configuration file")
-optparser.add_option("-t",
-                     "--tmp-keep",
-                     action="store_true",
-                     dest="tmps",
-                     default=False,
-                     help="do not delete tmp files created for running tests")
-optparser.add_option(
-    "-j",
-    "--jobs",
-    action="callback",
-    callback=jOption,
-    dest="threads",
-    default=1,
-    help="number of threads running tests in parallel; with no argument will use all CPUs")
-optparser.add_option("-g",
-                     "--groups",
-                     action="store",
-                     type="string",
-                     dest="groups",
-                     default="",
-                     help="execute only tests of given comma-separated list of groups")
-optparser.add_option("-r",
-                     "--rerun",
-                     action="store_true",
-                     dest="rerun",
-                     default=False,
-                     help="execute commands for tests that failed last time")
-optparser.add_option("-q",
-                     "--quiet",
-                     action="store_true",
-                     dest="quiet",
-                     default=False,
-                     help="suppress information output other than about failed tests")
-optparser.add_option(
-    "-x",
-    "--xml",
-    action="store",
-    type="string",
-    dest="xmlfile",
-    default="",
-    help=
-    "write a report of test results in JUnit XML format to file; if file exists, it is overwritten")
-optparser.add_option("-a",
-                     "--alternative",
-                     action="store",
-                     type="string",
-                     dest="alternatives",
-                     default=None,
-                     help="activate given alternative")
-optparser.add_option("-S",
-                     "--sphinx",
-                     action="store_true",
-                     dest="sphinx",
-                     default=False,
-                     help="indicates that we're running from inside Sphinx; for internal purposes")
-optparser.add_option("-T",
-                     "--update-times",
-                     action="store_true",
-                     dest="update_times",
-                     default=False,
-                     help="create a new timing baseline for tests being measured")
-optparser.add_option("-R",
-                     "--documentation",
-                     action="store",
-                     type="choice",
-                     dest="doc",
-                     choices=("rst", "md"),
-                     metavar="format",
-                     default=None,
-                     help="Output documentation for tests, supported formats: rst, md")
-optparser.add_option(
-    "-A",
-    "--show-all",
-    action="store_true",
-    default=False,
-    help=
-    "For console output, show one-liners for passing/skipped tests in addition to any failing ones")
-optparser.add_option("-z",
-                     "--retries",
-                     action="store",
-                     dest="retries",
-                     type="int",
-                     default=0,
-                     help="Retry failed tests this many times to determine if they are unstable")
-optparser.add_option("--trace-file",
-                     action="store",
-                     dest="tracefile",
-                     default="",
-                     help="write Chrome tracing file to file; if file exists, it is overwritten")
-optparser.add_option("-F",
-                     "--abort-on-failure",
-                     action="store_true",
-                     dest="abort_on_failure",
-                     help="terminate after first test failure")
-optparser.add_option("-l",
-                     "--list",
-                     action="store_true",
-                     dest="list",
-                     default=False,
-                     help="list available tests instead of executing them")
-
-optparser.set_defaults(mode="TEST")
-(Options, args) = optparser.parse_args()
-
-# Update-interactive mode implies single-threaded operation
-if Options.mode == "UPDATE_INTERACTIVE" and Options.threads > 1:
-    warning("ignoring requested parallelism in interactive-update mode")
-    Options.threads = 1
-
-if not os.path.exists(Options.config):
-    error("configuration file '%s' not found" % Options.config)
-
-# The defaults come from environment variables, plus a few additional items.
-defaults = {}
-# Changes to defaults should not change os.environ
-defaults.update(os.environ)
-defaults["default_path"] = os.environ["PATH"]
-
-dirname = os.path.dirname(Options.config)
-if not dirname:
-    dirname = os.getcwd()
-
-# If the BTEST_TEST_BASE envirnoment var is set, we'll use that as the testbase.
-# If not, we'll use the current directory.
-TestBase = os.path.abspath(os.environ.get("BTEST_TEST_BASE", dirname))
-defaults["testbase"] = TestBase
-defaults["baselinedir"] = os.path.abspath(
-    os.environ.get("BTEST_BASELINE_DIR", os.path.join(TestBase, "Baseline")))
-
-# Parse our config
-Config = getcfgparser(defaults)
-Config.read(Options.config)
-
-defaults["baselinedir"] = getOption("BaselineDir", defaults["baselinedir"])
-
-min_version = getOption("MinVersion", None)
-if min_version:
-    validate_version_requirement(min_version, VERSION)
-
-if Options.alternatives:
-    # Preprocess to split into list.
-    Options.alternatives = [alt.strip() for alt in Options.alternatives.split(",") if alt != "-"]
-
-    # Helper function that, if an option wasn't explicitly specified as an
-    # environment variable, checks if an alternative sets its through
-    # its own environment section. If so, we make that value our new default.
-    # If multiple alternatives set it, we pick the value from the first.
-    def get_env_from_alternative(env, opt, default, transform=None):
-        for tag in Options.alternatives:
-            value = getOption(env, None, section="environment-%s" % tag)
-            if value is not None:
-                if transform:
-                    value = transform(value)
-
-                defaults[opt] = value
-
-                # At this point, our defaults have changed, so we
-                # reread the configuration.
-                new_config = getcfgparser(defaults)
-                new_config.read(Options.config)
-                return new_config, value
-
-        return Config, default
-
-    (Config, TestBase) = get_env_from_alternative("BTEST_TEST_BASE", "testbase", TestBase,
-                                                  lambda x: os.path.abspath(x))
-    # Need to update BaselineDir - it may be interpolated from testbase.
-    defaults["baselinedir"] = getOption("BaselineDir", defaults["baselinedir"])
-    (Config, _) = get_env_from_alternative("BTEST_BASELINE_DIR", "baselinedir", None)
-
-os.chdir(TestBase)
-
-if Options.sphinx:
-    Options.quiet = True
-
-if Options.quiet:
-    Options.brief = True
-
-# Determine output handlers to use.
-
-output_handlers = []
-
-if Options.verbose:
-    output_handlers += [Verbose(Options, )]
-
-elif Options.brief:
-    output_handlers += [Brief(Options, )]
-
-else:
-    if sys.stdout.isatty():
-        if Options.show_all:
-            output_handlers += [Console(Options, )]
-        else:
-            output_handlers += [CompactConsole(Options, )]
-    else:
-        output_handlers += [Standard(Options, )]
-
-if Options.diagall:
-    output_handlers += [Diag(Options, True, None)]
-
-elif Options.diag:
-    output_handlers += [Diag(Options, False, None)]
-
-if Options.diagfile:
-    try:
-        diagfile = open(Options.diagfile, "w", 1)
-        output_handlers += [Diag(Options, Options.diagall, diagfile)]
-
-    except IOError as e:
-        print("cannot open %s: %s" % (Options.diagfile, e), file=sys.stderr)
-
-if Options.sphinx:
-    output_handlers += [SphinxOutput(Options)]
-
-if Options.xmlfile:
-    try:
-        xmlfile = open(Options.xmlfile, "w", 1)
-        output_handlers += [XMLReport(Options, xmlfile)]
-
-    except IOError as e:
-        print("cannot open %s: %s" % (Options.xmlfile, e), file=sys.stderr)
-
-if Options.tracefile:
-    try:
-        tracefile = open(Options.tracefile, "w", 1)
-        output_handlers += [ChromeTracing(Options, tracefile)]
-
-    except IOError as e:
-        print("cannot open %s: %s" % (Options.tracefile, e), file=sys.stderr)
+    if sys.platform == "win32":
+        # The "fork" method doesn't exist at all on Windows, so force over to
+        # "spawn" instead.
+        mp.set_start_method("spawn")
+
+        # Double-check that `bash.exe` exists and is executable, since it's
+        # required for pretty much anything here to work on Windows. Note we're
+        # doing this prior to parsing the config file because it's required for
+        # backtick-expansion there as well.
+        try:
+            subprocess.call(
+                ["bash.exe", "--version"],
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL,
+            )
+        except FileNotFoundError:
+            print(
+                "error: bash.exe is required to be in your PATH to run BTest.",
+                file=sys.stderr,
+            )
+            sys.exit(1)
 
-output_handler = Forwarder(Options, output_handlers)
+    elif (pyver_maj == 3 and pyver_min >= 8) or pyver_maj > 3:
+        mp.set_start_method("fork")
 
-# Determine Timer to use.
+    (Options, args) = parse_options()
 
-Timer = None
+    # The defaults come from environment variables, plus a few additional items.
+    defaults = {}
+    # Changes to defaults should not change os.environ
+    defaults.update(os.environ)
+    defaults["default_path"] = os.environ["PATH"]
+
+    dirname = os.path.dirname(Options.config)
+    if not dirname:
+        dirname = os.getcwd()
+
+    # If the BTEST_TEST_BASE envirnoment var is set, we'll use that as the testbase.
+    # If not, we'll use the current directory.
+    TestBase = normalize_path(os.environ.get("BTEST_TEST_BASE", dirname))
+    defaults["testbase"] = TestBase
+    defaults["baselinedir"] = normalize_path(
+        os.environ.get("BTEST_BASELINE_DIR", os.path.join(TestBase, "Baseline"))
+    )
+    defaults["pathsep"] = os.pathsep
+
+    # Parse our config
+    Config = getcfgparser(defaults)
+    Config.read(Options.config, encoding="utf-8")
 
-if platform() == "Linux":
-    t = LinuxTimer()
-    if t.available():
-        Timer = t
+    defaults["baselinedir"] = getOption("BaselineDir", defaults["baselinedir"])
 
-if Options.update_times and not Timer:
-    warning("unable to create timing baseline because timer is not available")
+    min_version = getOption("MinVersion", None)
+    if min_version:
+        validate_version_requirement(min_version, VERSION)
+
+    if Options.alternatives:
+        # Preprocess to split into list. "-" refers to the default setup, as a
+        # shorthand for "default", to allow combination with select alternatives.
+        Options.alternatives = [alt.strip() for alt in Options.alternatives.split(",")]
+        Options.alternatives = [
+            Alternative.DEFAULT if alt == "-" else alt for alt in Options.alternatives
+        ]
+
+        # Helper function that, if an option wasn't explicitly specified as an
+        # environment variable, checks if an alternative sets its through
+        # its own environment section. If so, we make that value our new default.
+        # If multiple alternatives set it, we pick the value from the first.
+        def get_env_from_alternative(env, opt, default, transform=None):
+            for tag in Options.alternatives:
+                value = getOption(env, None, section="environment-%s" % tag)
+                if value is not None:
+                    if transform:
+                        value = transform(value)
+
+                    defaults[opt] = value
+
+                    # At this point, our defaults have changed, so we
+                    # reread the configuration.
+                    new_config = getcfgparser(defaults)
+                    new_config.read(Options.config)
+                    return new_config, value
+
+            return Config, default
+
+        (Config, TestBase) = get_env_from_alternative(
+            "BTEST_TEST_BASE",
+            "testbase",
+            TestBase,
+            lambda x: normalize_path(os.path.abspath(x)),
+        )
+        # Need to update BaselineDir - it may be interpolated from testbase.
+        defaults["baselinedir"] = normalize_path(
+            getOption("BaselineDir", defaults["baselinedir"])
+        )
+        (Config, _) = get_env_from_alternative(
+            "BTEST_BASELINE_DIR",
+            "baselinedir",
+            None,
+            transform=lambda x: normalize_path(x),
+        )
+
+    os.chdir(TestBase)
+
+    if Options.sphinx:
+        Options.quiet = True
+
+    if Options.quiet:
+        Options.brief = True
+
+    # Determine output handlers to use.
+
+    output_handler = create_output_handler(Options)
+
+    # Determine Timer to use.
+
+    Timer = None
+
+    if platform() == "Linux":
+        t = LinuxTimer()
+        if t.available():
+            Timer = t
+
+    if Options.update_times and not Timer:
+        warning("unable to create timing baseline because timer is not available")
+
+    # Evaluate other command line options.
+
+    if Config.has_section("environment"):
+        for name, value in Config.itemsNoDefaults("environment"):
+            # Here we don't want to include items from defaults
+            os.environ[name] = value
 
-# Evaluate other command line options.
+    Alternatives = {}
 
-if Config.has_section("environment"):
-    for (name, value) in Config.itemsNoDefaults("environment"):
-        # Here we don't want to include items from defaults
-        os.environ[name.upper()] = value
+    if Options.alternatives:
+        for tag in Options.alternatives:
+            a = Alternative(tag)
 
-Alternatives = {}
+            try:
+                for name, value in Config.itemsNoDefaults("filter-%s" % tag):
+                    a.filters[name] = value
 
-if Options.alternatives:
-    for tag in Options.alternatives:
-        a = Alternative(tag)
+            except configparser.NoSectionError:
+                pass
 
-        try:
-            for (name, value) in Config.itemsNoDefaults("filter-%s" % tag):
-                a.filters[name] = value
+            try:
+                for name, value in Config.itemsNoDefaults("substitution-%s" % tag):
+                    a.substitutions[name] = value
 
-        except configparser.NoSectionError:
-            pass
+            except configparser.NoSectionError:
+                pass
 
-        try:
-            for (name, value) in Config.itemsNoDefaults("substitution-%s" % tag):
-                a.substitutions[name] = value
+            try:
+                for name, value in Config.itemsNoDefaults("environment-%s" % tag):
+                    a.envs[name] = value
 
-        except configparser.NoSectionError:
-            pass
+            except configparser.NoSectionError:
+                pass
 
-        try:
-            for (name, value) in Config.itemsNoDefaults("environment-%s" % tag):
-                a.envs[name] = value
+            if a.is_empty() and not a.is_default():
+                error('alternative "%s" is undefined' % tag)
 
-        except configparser.NoSectionError:
-            pass
+            Alternatives[tag] = a
 
-        Alternatives[tag] = a
+    CommandPrefix = getOption("CommandPrefix", "@TEST-")
 
-CommandPrefix = getOption("CommandPrefix", "@TEST-")
+    RE_INPUT = re.compile(r"%INPUT")
+    RE_DIR = re.compile(r"%DIR")
+    RE_ENV = re.compile(r"\$\{(\w+)}")
+    RE_PART = re.compile(r"^(.*)#([0-9]+)$")
+    RE_IGNORE = re.compile(CommandPrefix + "IGNORE")
+    RE_START_NEXT_TEST = re.compile(CommandPrefix + "START-NEXT")
+    RE_START_FILE = re.compile(CommandPrefix + "START-FILE +([^\r\n ]*)")
+    RE_END_FILE = re.compile(CommandPrefix + "END-FILE")
+
+    # Commands as tuple (tag, regexp, more-than-one-is-ok, optional, group-main, group-add)
+    # pylint: disable=bad-whitespace
+    # fmt: off
+    RE_EXEC                = ("exec",            re.compile(CommandPrefix + "EXEC(-FAIL)?: *(.*)"), True, False, 2, 1) # noqa
+    RE_REQUIRES            = ("requires",        re.compile(CommandPrefix + "REQUIRES: *(.*)"), True, True, 1, -1) # noqa
+    RE_GROUP               = ("group",           re.compile(CommandPrefix + "GROUP: *(.*)"), True, True, 1, -1) # noqa
+    RE_SERIALIZE           = ("serialize",       re.compile(CommandPrefix + "SERIALIZE: *(.*)"), False, True, 1, -1) # noqa
+    RE_PORT                = ("port",            re.compile(CommandPrefix + "PORT: *(.*)"), True, True, 1, -1) # noqa
+    RE_INCLUDE_ALTERNATIVE = ("alternative",     re.compile(CommandPrefix + "ALTERNATIVE: *(.*)"), True, True, 1, -1) # noqa
+    RE_IGNORE_ALTERNATIVE  = ("not-alternative", re.compile(CommandPrefix + "NOT-ALTERNATIVE: *(.*)"), True, True, 1, -1) # noqa
+    RE_COPY_FILE           = ("copy-file",       re.compile(CommandPrefix + "COPY-FILE: *(.*)"), True, True, 1, -1) # noqa
+    RE_KNOWN_FAILURE       = ("known-failure",   re.compile(CommandPrefix + "KNOWN-FAILURE"), False, True, -1, -1) # noqa
+    RE_MEASURE_TIME        = ("measure-time",    re.compile(CommandPrefix + "MEASURE-TIME"), False, True, -1, -1) # noqa
+    RE_DOC                 = ("doc",             re.compile(CommandPrefix + "DOC: *(.*)"), True, True, 1, -1) # noqa
+    # fmt: on
+    # pylint: enable=bad-whitespace
+
+    Commands = (
+        RE_EXEC,
+        RE_REQUIRES,
+        RE_GROUP,
+        RE_SERIALIZE,
+        RE_PORT,
+        RE_INCLUDE_ALTERNATIVE,
+        RE_IGNORE_ALTERNATIVE,
+        RE_COPY_FILE,
+        RE_KNOWN_FAILURE,
+        RE_MEASURE_TIME,
+        RE_DOC,
+    )
+
+    StateFile = normalize_path(
+        getOption("StateFile", os.path.join(defaults["testbase"], ".btest.failed.dat"))
+    )
+    TmpDir = normalize_path(
+        getOption("TmpDir", os.path.join(defaults["testbase"], ".tmp"))
+    )
+    BaselineDirs = [
+        normalize_path(dir) for dir in defaults["baselinedir"].split(os.pathsep)
+    ]
+    BaselineTimingDir = normalize_path(
+        getOption("TimingBaselineDir", os.path.join(BaselineDirs[0], "_Timing"))
+    )
+
+    Initializer = getOption("Initializer", "")
+    Finalizer = getOption("Finalizer", "")
+    Teardown = getOption("Teardown", "")
+
+    PartInitializer = getOption("PartInitializer", "")
+    PartFinalizer = getOption("PartFinalizer", "")
+    PartTeardown = getOption("PartTeardown", "")
+
+    Config.configured_tests = []
+
+    testdirs = getOption("TestDirs", "").split()
+    if testdirs:
+        Config.configured_tests = findTests(testdirs, True)
 
-RE_INPUT = re.compile(r"%INPUT")
-RE_DIR = re.compile(r"%DIR")
-RE_ENV = re.compile(r"\$\{(\w+)\}")
-RE_PART = re.compile(r"^(.*)#([0-9]+)$")
-RE_IGNORE = re.compile(CommandPrefix + "IGNORE")
-RE_START_NEXT_TEST = re.compile(CommandPrefix + "START-NEXT")
-RE_START_FILE = re.compile(CommandPrefix + "START-FILE +([^\r\n ]*)")
-RE_END_FILE = re.compile(CommandPrefix + "END-FILE")
-
-# Commands as tuple (tag, regexp, more-than-one-is-ok, optional, group-main, group-add)
-# pylint: disable=bad-whitespace
-# yapf: disable
-RE_EXEC                = ("exec",            re.compile(CommandPrefix + "EXEC(-FAIL)?: *(.*)"), True, False, 2, 1)
-RE_REQUIRES            = ("requires",        re.compile(CommandPrefix + "REQUIRES: *(.*)"), True, True, 1, -1)
-RE_GROUP               = ("group",           re.compile(CommandPrefix + "GROUP: *(.*)"), True, True, 1, -1)
-RE_SERIALIZE           = ("serialize",       re.compile(CommandPrefix + "SERIALIZE: *(.*)"), False, True, 1, -1)
-RE_PORT                = ("port",            re.compile(CommandPrefix + "PORT: *(.*)"), True, True, 1, -1)
-RE_INCLUDE_ALTERNATIVE = ("alternative",     re.compile(CommandPrefix + "ALTERNATIVE: *(.*)"), True, True, 1, -1)
-RE_IGNORE_ALTERNATIVE  = ("not-alternative", re.compile(CommandPrefix + "NOT-ALTERNATIVE: *(.*)"), True, True, 1, -1)
-RE_COPY_FILE           = ("copy-file",       re.compile(CommandPrefix + "COPY-FILE: *(.*)"), True, True, 1, -1)
-RE_KNOWN_FAILURE       = ("known-failure",   re.compile(CommandPrefix + "KNOWN-FAILURE"), False, True, -1, -1)
-RE_MEASURE_TIME        = ("measure-time",    re.compile(CommandPrefix + "MEASURE-TIME"), False, True, -1, -1)
-RE_DOC                 = ("doc",             re.compile(CommandPrefix + "DOC: *(.*)"), True, True, 1, -1)
-# yapf: enable
-# pylint: enable=bad-whitespace
-
-Commands = (RE_EXEC, RE_REQUIRES, RE_GROUP, RE_SERIALIZE, RE_PORT, RE_INCLUDE_ALTERNATIVE,
-            RE_IGNORE_ALTERNATIVE, RE_COPY_FILE, RE_KNOWN_FAILURE, RE_MEASURE_TIME, RE_DOC)
-
-StateFile = os.path.abspath(
-    getOption("StateFile", os.path.join(defaults["testbase"], ".btest.failed.dat")))
-TmpDir = os.path.abspath(getOption("TmpDir", os.path.join(defaults["testbase"], ".tmp")))
-BaselineDirs = [os.path.abspath(dir) for dir in defaults["baselinedir"].split(":")]
-BaselineTimingDir = os.path.abspath(
-    getOption("TimingBaselineDir", os.path.join(BaselineDirs[0], "_Timing")))
-
-Initializer = getOption("Initializer", "")
-Finalizer = getOption("Finalizer", "")
-Teardown = getOption("Teardown", "")
-
-PartInitializer = getOption("PartInitializer", "")
-PartFinalizer = getOption("PartFinalizer", "")
-PartTeardown = getOption("PartTeardown", "")
-
-Config.configured_tests = []
-
-testdirs = getOption("TestDirs", "").split()
-if testdirs:
-    Config.configured_tests = findTests(testdirs, True)
+    if args:
+        tests = findTests(args)
 
-if args:
-    tests = findTests(args)
+    else:
+        if Options.rerun:
+            (success, tests) = readStateFile()
 
-else:
-    if Options.rerun:
-        (success, tests) = readStateFile()
+            if success:
+                if not tests:
+                    output("no tests failed last time")
+                    sys.exit(0)
 
-        if success:
-            if not tests:
-                output("no tests failed last time")
-                sys.exit(0)
+            else:
+                warning("cannot read state file, executing all tests")
+                tests = Config.configured_tests
 
         else:
-            warning("cannot read state file, executing all tests")
             tests = Config.configured_tests
 
-    else:
-        tests = Config.configured_tests
+    if Options.groups:
+        groups = Options.groups.split(",")
+        Options.groups = {g for g in groups if not g.startswith("-")}
+        Options.no_groups = {g[1:] for g in groups if g.startswith("-")}
 
-if Options.groups:
-    groups = Options.groups.split(",")
-    Options.groups = set([g for g in groups if not g.startswith("-")])
-    Options.no_groups = set([g[1:] for g in groups if g.startswith("-")])
-
-    def rightGroup(t):
-        if not t:
-            return True
+        def rightGroup(t):
+            if not t:
+                return True
 
-        if t.groups & Options.groups:
-            return True
+            if t.groups & Options.groups:
+                return True
+
+            if "" in Options.no_groups:
+                if not t.groups:
+                    return True
+
+            elif Options.no_groups:
+                if t.groups & Options.no_groups:
+                    return False
 
-        if "" in Options.no_groups:
-            if not t.groups:
                 return True
 
-        elif Options.no_groups:
-            if t.groups & Options.no_groups:
-                return False
+            return False
 
-            return True
+        tests = [t for t in tests if rightGroup(t)]
 
-        return False
+    if not tests:
+        output("no tests to execute")
+        sys.exit(0)
 
-    tests = [t for t in tests if rightGroup(t)]
+    tests = mergeTestParts(tests)
 
-if not tests:
-    output("no tests to execute")
-    sys.exit(0)
+    if Options.doc:
+        outputDocumentation(tests, Options.doc)
+        sys.exit(0)
 
-tests = mergeTestParts(tests)
+    for d in BaselineDirs:
+        mkdir(d)
 
-if Options.doc:
-    outputDocumentation(tests, Options.doc)
-    sys.exit(0)
+    mkdir(TmpDir)
 
-for d in BaselineDirs:
-    mkdir(d)
+    if sys.platform == "win32":
+        # On win32 we have to use a named pipe so that python's multiprocessing
+        # chooses AF_PIPE as the family type.
+        addr = "\\\\.\\pipe\\btest-pipe-%s" % (os.getpid())
+    else:
+        # Building our own path to avoid "error: AF_UNIX path too long" on
+        # some platforms. See BIT-862.
+        sname = "btest-socket-%s" % (os.getpid())
+        addr = os.path.join(tempfile.gettempdir(), sname)
+
+        # Check if the pathname is too long to fit in struct sockaddr_un (the
+        # maximum length is system-dependent, so here we just use 100, which seems
+        # a safe default choice).
+        if len(addr) > 100:
+            # Try relative path to TmpDir (which would usually be ".tmp").
+            addr = os.path.join(os.path.relpath(TmpDir), sname)
+
+            # If the path is still too long, then use the global tmp directory.
+            if len(addr) > 100:
+                addr = os.path.join("/tmp", sname)
 
-mkdir(TmpDir)
+    mgr = TestManager(address=addr)
 
-# Building our own path to avoid "error: AF_UNIX path too long" on
-# some platforms. See BIT-862.
-sname = "btest-socket-%d" % os.getpid()
-addr = os.path.join(tempfile.gettempdir(), sname)
+    try:
+        if Options.list:
+            for test in sorted(tests):
+                if test.name:
+                    print(test.name)
+            sys.exit(0)
+        else:
+            (succeeded, failed, skipped, unstable, failed_expected) = mgr.run(
+                copy.deepcopy(tests), output_handler
+            )
+            total = succeeded + failed + skipped
+
+        output_handler.finished()
+
+    # Ctrl-C can lead to broken pipe (e.g. FreeBSD), so include IOError here:
+    except (Abort, KeyboardInterrupt, OSError) as exc:
+        output_handler.finished()
+        print(str(exc) or "Aborted with %s." % type(exc).__name__, file=sys.stderr)
+        sys.stderr.flush()
+        # Explicitly shut down sync manager to avoid leaking manager
+        # processes, particularly with --abort-on-failure:
+        mgr.shutdown()
+        sys.exit(1)
 
-# Check if the pathname is too long to fit in struct sockaddr_un (the
-# maximum length is system-dependent, so here we just use 100, which seems
-# a safe default choice).
-if len(addr) > 100:
-    # Try relative path to TmpDir (which would usually be ".tmp").
-    addr = os.path.join(os.path.relpath(TmpDir), sname)
+    skip = (", %d skipped" % skipped) if skipped > 0 else ""
+    unstablestr = (", %d unstable" % unstable) if unstable > 0 else ""
+    failed_expectedstr = (
+        (" (with %d expected to fail)" % failed_expected) if failed_expected > 0 else ""
+    )
+
+    if failed > 0:
+        if not Options.quiet:
+            output(
+                "%d of %d test%s failed%s%s%s"
+                % (
+                    failed,
+                    total,
+                    "s" if total > 1 else "",
+                    failed_expectedstr,
+                    skip,
+                    unstablestr,
+                )
+            )
 
-    # If the path is still too long, then use the global tmp directory.
-    if len(addr) > 100:
-        addr = os.path.join("/tmp", sname)
+        if failed == failed_expected:
+            sys.exit(0)
+        else:
+            sys.exit(1)
 
-mgr = TestManager(address=addr)
+    elif skipped > 0 or unstable > 0:
+        if not Options.quiet:
+            output(
+                "%d test%s successful%s%s"
+                % (succeeded, "s" if succeeded != 1 else "", skip, unstablestr)
+            )
 
-try:
-    if Options.list:
-        for test in sorted(tests):
-            if test.name:
-                print(test.name)
         sys.exit(0)
-    else:
-        (succeeded, failed, skipped, unstable,
-         failed_expected) = mgr.run(copy.deepcopy(tests), output_handler)
-        total = succeeded + failed + skipped
-
-    output_handler.finished()
-
-# Ctrl-C can lead to broken pipe (e.g. FreeBSD), so include IOError here:
-except (Abort, KeyboardInterrupt, IOError) as exc:
-    output_handler.finished()
-    print(str(exc) or "Aborted with %s." % type(exc).__name__, file=sys.stderr)
-    sys.stderr.flush()
-    # Explicitly shut down sync manager to avoid leaking manager
-    # processes, particularly with --abort-on-failure:
-    mgr.shutdown()
-    os._exit(1)
-
-skip = (", %d skipped" % skipped) if skipped > 0 else ""
-unstablestr = (", %d unstable" % unstable) if unstable > 0 else ""
-failed_expectedstr = (" (with %d expected to fail)" %
-                      failed_expected) if failed_expected > 0 else ""
-
-if failed > 0:
-    if not Options.quiet:
-        output("%d of %d test%s failed%s%s%s" %
-               (failed, total, "s" if total > 1 else "", failed_expectedstr, skip, unstablestr))
 
-    if failed == failed_expected:
-        sys.exit(0)
     else:
-        sys.exit(1)
-
-elif skipped > 0 or unstable > 0:
-    if not Options.quiet:
-        output("%d test%s successful%s%s" %
-               (succeeded, "s" if succeeded != 1 else "", skip, unstablestr))
-
-    sys.exit(0)
+        if not Options.quiet:
+            output("all %d tests successful" % total)
 
-else:
-    if not Options.quiet:
-        output("all %d tests successful" % total)
-
-    sys.exit(0)
+        sys.exit(0)
```

### Comparing `btest-0.71/btest-ask-update` & `btest-1.0/btest-ask-update`

 * *Files identical despite different names*

### Comparing `btest-0.71/btest-bg-run` & `btest-1.0/btest-bg-run`

 * *Files identical despite different names*

### Comparing `btest-0.71/btest-bg-wait` & `btest-1.0/btest-bg-wait`

 * *Files identical despite different names*

### Comparing `btest-0.71/btest-diff` & `btest-1.0/btest-diff`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,19 @@
 
 if [ "$#" -lt 1 ]; then
     echo "btest-diff: wrong number of arguments" >$TEST_DIAGNOSTICS
     exit 1
 fi
 
 # Split string with baseline directories into array.
-IFS=':' read -ra baseline_dirs <<<"$TEST_BASELINE"
+if [ "$(uname -s | cut -c 1-5)" == "MINGW" ]; then
+    IFS=';' read -ra baseline_dirs <<<"$TEST_BASELINE"
+else
+    IFS=':' read -ra baseline_dirs <<<"$TEST_BASELINE"
+fi
 
 input="$1"
 # shellcheck disable=SC2001
 canon=$(echo "$input" | sed 's#/#.#g')
 shift
 
 if [ ! -f "$input" ]; then
@@ -217,15 +221,15 @@
     fi
 
     if [ $error -eq 0 ]; then
         echo "== Diff ===============================" >>$TEST_DIAGNOSTICS
         if is_binary_mode; then
             diff -s "$@" "$canon_baseline" "$canon_output" >>$TEST_DIAGNOSTICS
         else
-            diff -au "$@" "$canon_baseline" "$canon_output" >>$TEST_DIAGNOSTICS
+            diff -au --strip-trailing-cr "$@" "$canon_baseline" "$canon_output" >>$TEST_DIAGNOSTICS
         fi
         result=$?
     fi
 elif [ "$TEST_MODE" = "TEST" ]; then
     echo "== Error ==============================" >>$TEST_DIAGNOSTICS
     echo "test-diff: no baseline found." >>$TEST_DIAGNOSTICS
     result=100
```

### Comparing `btest-0.71/btest-progress` & `btest-1.0/btest-progress`

 * *Files identical despite different names*

### Comparing `btest-0.71/examples/sphinx/Makefile` & `btest-1.0/examples/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `btest-0.71/examples/sphinx/conf.py` & `btest-1.0/examples/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `btest-0.71/examples/sphinx/index.rst` & `btest-1.0/examples/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `btest-0.71/sphinx/btest-rst-cmd` & `btest-1.0/sphinx/btest-rst-cmd`

 * *Files identical despite different names*

### Comparing `btest-0.71/sphinx/btest-sphinx.py` & `btest-1.0/sphinx/btest-sphinx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import os.path
-import tempfile
 import subprocess
 import re
 
-from docutils import nodes, statemachine, utils
-from docutils.parsers.rst import directives, Directive, DirectiveError, Parser
-from docutils.transforms import TransformError, Transform
-from sphinx.util.console import bold, purple, darkgreen, red, term_width_line
+from docutils import nodes, utils
+from docutils.parsers.rst import directives, Directive, Parser
+from docutils.transforms import Transform
+from sphinx.util.console import darkgreen, red
 from sphinx.errors import SphinxError
 from sphinx.directives.code import LiteralInclude
 from sphinx.util import logging
 
 logger = logging.getLogger(__name__)
 
 Initialized = False
@@ -40,15 +39,17 @@
     if not BTestBase:
         raise SphinxError("error: btest_base not set in config")
 
     if not BTestTests:
         raise SphinxError("error: btest_tests not set in config")
 
     if not os.path.exists(BTestBase):
-        raise SphinxError("error: btest_base directory '%s' does not exists" % BTestBase)
+        raise SphinxError(
+            "error: btest_base directory '%s' does not exists" % BTestBase
+        )
 
     joined = os.path.join(BTestBase, BTestTests)
 
     if not os.path.exists(joined):
         raise SphinxError("error: btest_tests directory '%s' does not exists" % joined)
 
     if not BTestTmp:
@@ -64,15 +65,15 @@
     parser = Parser()
     document = utils.new_document("<partial node>")
     document.settings = settings
     parser.parse(rawtext, document)
     return document.children
 
 
-class Test(object):
+class Test:
     def __init__(self):
         self.has_run = False
 
     def run(self):
         if self.has_run:
             return
 
@@ -81,41 +82,40 @@
         self.rst_output = os.path.join(BTestTmp, "%s" % self.tag)
         os.environ["BTEST_RST_OUTPUT"] = self.rst_output
 
         self.cleanTmps()
 
         try:
             subprocess.check_call("btest -S %s" % self.path, shell=True)
-        except (OSError, IOError, subprocess.CalledProcessError) as e:
+        except (OSError, subprocess.CalledProcessError) as e:
             # Equivalent to Directive.error(); we don't have an
             # directive object here and can't pass it in because
             # it doesn't pickle.
             logger.warning(red("BTest error: %s" % e))
 
     def cleanTmps(self):
         subprocess.call("rm %s#* 2>/dev/null" % self.rst_output, shell=True)
 
 
 class BTestTransform(Transform):
-
     default_priority = 800
 
     def apply(self):
         pending = self.startnode
         (test, part) = pending.details
 
         os.chdir(BTestBase)
 
-        if not test.tag in BTestTransform._run:
+        if test.tag not in BTestTransform._run:
             test.run()
             BTestTransform._run.add(test.tag)
 
         try:
             rawtext = open("%s#%d" % (test.rst_output, part)).read()
-        except IOError as e:
+        except OSError:
             rawtext = ""
 
         settings = self.document.settings
         content = parsePartial(rawtext, settings)
         pending.replace_self(content)
 
     _run = set()
@@ -143,16 +143,15 @@
         os.chdir(BTestBase)
 
         self.assert_has_content()
         document = self.state_machine.document
 
         tag = self.arguments[0]
 
-        if not tag in Tests:
-            import sys
+        if tag not in Tests:
             test = Test()
             test.tag = tag
             test.path = os.path.join(BTestTests, tag + ".btest")
             test.parts = 0
             Tests[tag] = test
 
         test = Tests[tag]
@@ -177,15 +176,15 @@
         document.note_pending(pending)
 
         return [pending]
 
 
 class BTestInclude(LiteralInclude):
     def __init__(self, *args, **kwargs):
-        super(BTestInclude, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def error(self, msg):
         self.state.document.settings.env.note_reread()
         msg = red(msg)
         msg = self.state.document.reporter.error(str(msg), line=self.lineno)
         return [msg]
 
@@ -195,50 +194,53 @@
     def run(self):
         if not Initialized:
             # FIXME: Better way to handle one-time initialization?
             init(self.state.document.settings, self.state.document.reporter)
 
         document = self.state.document
         if not document.settings.file_insertion_enabled:
-            return [document.reporter.warning('File insertion disabled', line=self.lineno)]
+            return [
+                document.reporter.warning("File insertion disabled", line=self.lineno)
+            ]
         env = document.settings.env
 
         expanded_arg = os.path.expandvars(self.arguments[0])
         sphinx_src_relation = os.path.relpath(expanded_arg, env.srcdir)
         self.arguments[0] = os.path.join(os.sep, sphinx_src_relation)
 
         (root, ext) = os.path.splitext(self.arguments[0])
 
         if ext.startswith("."):
             ext = ext[1:]
 
         if ext in ExtMappings:
             self.options["language"] = ExtMappings[ext]
         else:
-            # Note that we always need to set a language, otherwise the lineos/emphasis don't seem to work.
+            # Note that we always need to set a language, otherwise the
+            # linenos/emphasis don't seem to work.
             self.options["language"] = "none"
 
         self.options["linenos"] = True
         self.options["prepend"] = "%s\n" % os.path.basename(self.arguments[0])
         self.options["emphasize-lines"] = "1,1"
         self.options["style"] = "X"
 
-        retnode = super(BTestInclude, self).run()
+        retnode = super().run()
 
         os.chdir(BTestBase)
 
         tag = os.path.normpath(self.arguments[0])
         tag = os.path.relpath(tag, BTestBase)
         tag = re.sub("[^a-zA-Z0-9-]", "_", tag)
         tag = re.sub("__+", "_", tag)
 
         if tag.startswith("_"):
             tag = tag[1:]
 
-        test_path = ("include-" + tag + ".btest")
+        test_path = "include-" + tag + ".btest"
 
         if BTestTests:
             test_path = os.path.join(BTestTests, test_path)
 
         test_path = os.path.abspath(test_path)
 
         i = 1
@@ -261,18 +263,18 @@
 
         for node in retnode:
             node["classes"] += ["btest-include"]
 
         return retnode
 
 
-directives.register_directive('btest', BTest)
-directives.register_directive('btest-include', BTestInclude)
+directives.register_directive("btest", BTest)
+directives.register_directive("btest-include", BTestInclude)
 
 
 def setup(app):
     global App
     App = app
 
-    app.add_config_value('btest_base', None, 'env')
-    app.add_config_value('btest_tests', None, 'env')
-    app.add_config_value('btest_tmp', None, 'env')
+    app.add_config_value("btest_base", None, "env")
+    app.add_config_value("btest_tests", None, "env")
+    app.add_config_value("btest_tmp", None, "env")
```

### Comparing `btest-0.71/testing/Baseline/tests.alternatives-filter/child-output` & `btest-1.0/testing/Baseline/tests.alternatives-filter/child-output`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.diag/output` & `btest-1.0/testing/Baseline/tests.diag/output`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.diff-max-lines/output1` & `btest-1.0/testing/Baseline/tests.diff-max-lines/output1`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.diff-max-lines/output2` & `btest-1.0/testing/Baseline/tests.diff-max-lines/output2`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.doc/md` & `btest-1.0/testing/Baseline/tests.doc/md`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.doc/rst` & `btest-1.0/testing/Baseline/tests.doc/rst`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.environment/output` & `btest-1.0/testing/Baseline/tests.environment/output`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.measure-time-options/output` & `btest-1.0/testing/Baseline/tests.measure-time-options/output`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.progress-back-to-back/output` & `btest-1.0/testing/Baseline/tests.progress-back-to-back/output`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.sphinx.rst-cmd/output` & `btest-1.0/testing/Baseline/tests.sphinx.rst-cmd/output`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt` & `btest-1.0/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/Scripts/test-perf` & `btest-1.0/testing/Scripts/test-perf`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/btest.cfg` & `btest-1.0/testing/btest.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 BaselineDir = %(testbase)s/Baseline
 IgnoreDirs  = .svn CVS .tmp
 IgnoreFiles = *.tmp *.swp #*
 CommandPrefix = %%TEST-
 Initializer = test -f btest.cfg || cp %(testbase)s/btest.tests.cfg btest.cfg; echo >/dev/null
 
 [environment]
-PATH=%(testbase)s/..:%(testbase)s/../sphinx:%(testbase)s/Scripts:%(default_path)s
+PATH=%(testbase)s/..%(pathsep)s%(testbase)s/../sphinx%(pathsep)s%(testbase)s/Scripts%(pathsep)s%(default_path)s
 SCRIPTS=%(testbase)s/Scripts
 TMPDIR=%(testbase)s/.tmp
 # BTEST_CFG=%(testbase)s/btest.tests.cfg
```

### Comparing `btest-0.71/testing/btest.tests.cfg` & `btest-1.0/testing/btest.tests.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #
 # Configuration file used by individual tests.
 #
 # This is set so that all files will be created inside the current
 # sandbox.
 
+[DEFAULT]
+override=normal
+
 [btest]
 TmpDir      = `echo .tmp`
 BaselineDir = %(testbase)s/Baseline
 
 [environment]
 ORIGPATH=%(default_path)s
 ENV1=Foo
 ENV2=%(testbase)s
 ENV3=`expr 42`
 ENV4=`echo \(%(testbase)s=%(testbase)s\)`
+ENV5=%(override)s
 
 [environment-foo]
 FOO=BAR
 
 [filter-foo]
 cat=%(testbase)s/../../Scripts/test-filter
```

### Comparing `btest-0.71/testing/tests/abort-on-failure-with-only-known-fails.btest` & `btest-1.0/testing/tests/abort-on-failure-with-only-known-fails.btest`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/alternatives-baseline-dir.test` & `btest-1.0/testing/tests/alternatives-baseline-dir.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/alternatives-keywords.test` & `btest-1.0/testing/tests/alternatives-keywords.test`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # %TEST-EXEC: btest foo1 default1 notfoo1 notdefault1 >>output 2>&1
 # %TEST-EXEC: btest -a - foo1 default1 notfoo1 notdefault1 >>output 2>&1
 # %TEST-EXEC: btest -a foo foo1 default1 notfoo1 notdefault1 >>output 2>&1
-# %TEST-EXEC: btest -a notexist foo1 default1 notfoo1 notdefault1 >>output 2>&1
 # %TEST-EXEC: btest-diff output
 
 %TEST-START-FILE foo1
 @TEST-ALTERNATIVE: foo
 @TEST-EXEC: exit 0
 %TEST-END-FILE
```

### Comparing `btest-0.71/testing/tests/baseline-dir-env.test` & `btest-1.0/testing/tests/baseline-dir-env.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/binary-mode.test` & `btest-1.0/testing/tests/binary-mode.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/btest-cfg.test` & `btest-1.0/testing/tests/btest-cfg.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/canonifier-cmdline.test` & `btest-1.0/testing/tests/canonifier-cmdline.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/canonifier-conversion.test` & `btest-1.0/testing/tests/canonifier-conversion.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/canonifier-fail.test` & `btest-1.0/testing/tests/canonifier-fail.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/console.test` & `btest-1.0/testing/tests/console.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/diff-brief.test` & `btest-1.0/testing/tests/diff-brief.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/diff-max-lines.test` & `btest-1.0/testing/tests/diff-max-lines.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/doc.test` & `btest-1.0/testing/tests/doc.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/environment.test` & `btest-1.0/testing/tests/environment.test`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# %TEST-REQUIRES: ! ${SCRIPTS}/is-windows
 # %TEST-EXEC: btest -d %INPUT
 # %TEST-EXEC: btest -U %INPUT
 # %TEST-EXEC: btest-diff output
 
 @TEST-REQUIRES: test -n "${ENV2}"
 @TEST-EXEC-FAIL: test -z "${ENV2}"
```

### Comparing `btest-0.71/testing/tests/exit-codes.test` & `btest-1.0/testing/tests/exit-codes.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/groups.test` & `btest-1.0/testing/tests/groups.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/ignore.test` & `btest-1.0/testing/tests/ignore.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/measure-time-options.test` & `btest-1.0/testing/tests/measure-time-options.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/measure-time.tests` & `btest-1.0/testing/tests/measure-time.tests`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/multiple-baseline-dirs.test` & `btest-1.0/testing/tests/multiple-baseline-dirs.test`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,9 @@
 %TEST-START-FILE t4
 @TEST-EXEC: echo 4 >output
 @TEST-EXEC: btest-diff output
 %TEST-END-FILE
 
 %TEST-START-FILE btest.cfg
 [btest]
-BaselineDir = baseline1:baseline2:baseline3
+BaselineDir = baseline1%(pathsep)sbaseline2%(pathsep)sbaseline3
 %TEST-END-FILE
```

### Comparing `btest-0.71/testing/tests/parts-initializer-finalizer.test` & `btest-1.0/testing/tests/parts-initializer-finalizer.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/parts-teardown.test` & `btest-1.0/testing/tests/parts-teardown.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/progress-back-to-back.test` & `btest-1.0/testing/tests/progress-back-to-back.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/progress.test` & `btest-1.0/testing/tests/progress.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/statefile.test` & `btest-1.0/testing/tests/statefile.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/teardown.test` & `btest-1.0/testing/tests/teardown.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/threads.test` & `btest-1.0/testing/tests/threads.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/unstable-dir.test` & `btest-1.0/testing/tests/unstable-dir.test`

 * *Files identical despite different names*

### Comparing `btest-0.71/testing/tests/xml.test` & `btest-1.0/testing/tests/xml.test`

 * *Files identical despite different names*

