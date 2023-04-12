# Comparing `tmp/waveforms-1.5.82.tar.gz` & `tmp/waveforms-1.5.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveforms-1.5.82.tar", last modified: Sat Apr  1 02:19:07 2023, max compression
+gzip compressed data, was "waveforms-1.5.83.tar", last modified: Wed Apr 12 07:19:08 2023, max compression
```

## Comparing `waveforms-1.5.82.tar` & `waveforms-1.5.83.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-01 02:18:09.000000 waveforms-1.5.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-01 02:18:09.000000 waveforms-1.5.82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-01 02:19:07.975109 waveforms-1.5.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-01 02:18:09.000000 waveforms-1.5.82/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-01 02:18:09.000000 waveforms-1.5.82/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 02:19:07.975109 waveforms-1.5.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-01 02:18:09.000000 waveforms-1.5.82/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.963109 waveforms-1.5.82/src/
--rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-01 02:18:09.000000 waveforms-1.5.82/src/ikcp.c
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-01 02:18:09.000000 waveforms-1.5.82/src/ikcp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-01 02:18:09.000000 waveforms-1.5.82/src/kcp.c
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-01 02:18:09.000000 waveforms-1.5.82/src/prime.c
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-01 02:18:09.000000 waveforms-1.5.82/src/waveform.c
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-01 02:18:09.000000 waveforms-1.5.82/src/waveform.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.963109 waveforms-1.5.82/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_lisp.py
--rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_scan_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-01 02:18:09.000000 waveforms-1.5.82/tests/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.963109 waveforms-1.5.82/waveforms/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.963109 waveforms-1.5.82/waveforms/math/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fibheap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/math/fit/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/qubit_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/resonator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/fit/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/prime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/math/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/signal/demodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/signal/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/math/signal/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/qlisp/_antlr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/_antlr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/qlisp/libs/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/prog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/qlisp/qasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.967109 waveforms-1.5.82/waveforms/qlisp/qasm/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/libs/qelib1.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/qlisp/qasm/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/binaryop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/binaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/creg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/customunitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/expressionlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/gatebody.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/if_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/indexedid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/intnode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/nodeexception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/opaque.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/primarylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/qreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/node/unaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/qasmlexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/qasm/qasmparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/qlisp/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/simulator/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/simulator/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/quantum/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/quantum/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/arch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/assembly_left.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/assembly_right.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/library.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/qlisp.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/quantum/circuit/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/circuit/simulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.971109 waveforms-1.5.82/waveforms/quantum/clifford/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/clifford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/clifford/clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/clifford/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/clifford/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/clifford/seq2mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/rb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/transmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/quantum/xeb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    22550 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/scan_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/security/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/security/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/server/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/server/umsgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/sys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/sys/device/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/device/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/device/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/sys/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/ipy_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/sys/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/net/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/net/dhcpd.py
--rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/net/kad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/net/kcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/sys/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/storage/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/sys/storage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/units/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.975109 waveforms-1.5.82/waveforms/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/visualization/plot_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-01 02:18:09.000000 waveforms-1.5.82/waveforms/waveform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 02:19:07.963109 waveforms-1.5.82/waveforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-01 02:19:07.000000 waveforms-1.5.82/waveforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-01 02:19:07.000000 waveforms-1.5.82/waveforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 02:19:07.000000 waveforms-1.5.82/waveforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-01 02:19:07.000000 waveforms-1.5.82/waveforms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-01 02:19:07.000000 waveforms-1.5.82/waveforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-01 02:19:07.000000 waveforms-1.5.82/waveforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 07:18:15.000000 waveforms-1.5.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 07:18:15.000000 waveforms-1.5.83/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-12 07:19:08.978582 waveforms-1.5.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-12 07:18:15.000000 waveforms-1.5.83/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 07:18:15.000000 waveforms-1.5.83/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:19:08.978582 waveforms-1.5.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-12 07:18:15.000000 waveforms-1.5.83/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/ikcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/ikcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/kcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/prime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/waveform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-12 07:18:15.000000 waveforms-1.5.83/src/waveform.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_scan_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-12 07:18:15.000000 waveforms-1.5.83/tests/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fibheap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms/math/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/qubit_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/resonator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/fit/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/prime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/math/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/demodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/math/signal/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/_antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/_antlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/prog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.970581 waveforms-1.5.83/waveforms/qlisp/qasm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/libs/qelib1.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/qlisp/qasm/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/creg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/customunitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/expressionlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/gatebody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/indexedid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/intnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/nodeexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/primarylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/qreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/node/unaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/qasmlexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/qasm/qasmparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/qlisp/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/simulator/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/simulator/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/arch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/assembly_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/assembly_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/qlisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/circuit/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/circuit/simulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/quantum/clifford/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/clifford/seq2mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/quantum/xeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22550 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/scan_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.974581 waveforms-1.5.83/waveforms/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/security/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/server/umsgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/ipy_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/dhcpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/kad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/net/kcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/sys/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/storage/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/sys/storage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.978582 waveforms-1.5.83/waveforms/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/visualization/plot_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/visualization/plot_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-12 07:18:15.000000 waveforms-1.5.83/waveforms/waveform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:19:08.966581 waveforms-1.5.83/waveforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 07:19:08.000000 waveforms-1.5.83/waveforms.egg-info/top_level.txt
```

### Comparing `waveforms-1.5.82/LICENSE` & `waveforms-1.5.83/LICENSE`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/PKG-INFO` & `waveforms-1.5.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.82
+Version: 1.5.83
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.82/README.md` & `waveforms-1.5.83/README.md`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/pyproject.toml` & `waveforms-1.5.83/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/setup.py` & `waveforms-1.5.83/setup.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/src/ikcp.c` & `waveforms-1.5.83/src/ikcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/src/ikcp.h` & `waveforms-1.5.83/src/ikcp.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/src/kcp.c` & `waveforms-1.5.83/src/kcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/src/prime.c` & `waveforms-1.5.83/src/prime.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/src/waveform.c` & `waveforms-1.5.83/src/waveform.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/src/waveform.h` & `waveforms-1.5.83/src/waveform.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_compile.py` & `waveforms-1.5.83/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_dicttree.py` & `waveforms-1.5.83/tests/test_dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_lisp.py` & `waveforms-1.5.83/tests/test_lisp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_msgpack.py` & `waveforms-1.5.83/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_namespace.py` & `waveforms-1.5.83/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_registry.py` & `waveforms-1.5.83/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_scan_iter.py` & `waveforms-1.5.83/tests/test_scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_tomo.py` & `waveforms-1.5.83/tests/test_tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_vm.py` & `waveforms-1.5.83/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/tests/test_waveform.py` & `waveforms-1.5.83/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/__init__.py` & `waveforms-1.5.83/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/autoreload.py` & `waveforms-1.5.83/waveforms/autoreload.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/baseconfig.py` & `waveforms-1.5.83/waveforms/baseconfig.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/cache.py` & `waveforms-1.5.83/waveforms/cache.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/dicttree.py` & `waveforms-1.5.83/waveforms/dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/loader.py` & `waveforms-1.5.83/waveforms/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/bayes.py` & `waveforms-1.5.83/waveforms/math/bayes.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/fibheap.py` & `waveforms-1.5.83/waveforms/math/fibheap.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/fit/__init__.py` & `waveforms-1.5.83/waveforms/math/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/fit/delay.py` & `waveforms-1.5.83/waveforms/math/fit/delay.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Hashable, Optional
+from typing import Literal, Optional
 
 import numpy as np
 from scipy.optimize import minimize
 from scipy.signal import correlate
 from scipy.sparse import coo_matrix, diags, linalg
 
+from ..graph import graphs, minimum_spanning_tree
+
 
 def fit_relative_delay(waveform, data, sample_rate, fit=True):
     t = np.linspace(0, len(data) / sample_rate, len(data), endpoint=False)
     if isinstance(waveform, np.ndarray):
         fit = False
         corr = correlate(waveform, data, mode='same', method='fft')
     else:
@@ -56,28 +58,32 @@
             absolute_error = False
         else:
             y.append(delay[0])
             weight.append(1 / delay[1]**2)
 
     if reference_channel is None:
         reference_channel = channels[0]
+        reference = None
     note_channel(reference_channel)
     matrix.append([i + 1, channels_map[reference_channel], 1])
     y.append(0)
     weight.append(np.max(weight))
 
     row, col, data = list(zip(*matrix))
 
     X = coo_matrix((data, (row, col)), shape=(len(y), len(channels)))
     W = diags(weight, 0, shape=(len(y), len(y)))
 
     M = linalg.inv(X.T @ W @ X)
 
     beta = M @ X.T @ W @ y
-    offset = reference - beta[channels_map[reference_channel]]
+    if reference is None:
+        offset = -np.min(beta)
+    else:
+        offset = reference - beta[channels_map[reference_channel]]
 
     if full:
         if absolute_error:
             cov = linalg.inv(X.T @ W @ X)
         else:
             r = y - X @ beta
             chi_square = r.T @ W @ r
@@ -86,7 +92,33 @@
         errors = np.sqrt(cov.diagonal())
         return {
             ch: (v + offset, e)
             for ch, v, e in zip(channels, beta, errors)
         }
     else:
         return {ch: v + offset for ch, v in zip(channels, beta)}
+
+
+def relative_delay_to_absolute(relative_delays: dict[tuple[str, str], float],
+                               reference: float = 0,
+                               reference_channel: Optional[str] = None,
+                               method: Literal['mst', 'lsq'] = 'mst',
+                               full: bool = False) -> dict[str, float]:
+    groups = graphs(relative_delays.keys())
+    graph_list = []
+    if method == 'mst':
+        for group in groups:
+            edges = []
+            for k in group:
+                if isinstance(relative_delays[k], tuple):
+                    edges.append((*k, relative_delays[k][1]))
+                else:
+                    edges.append((*k, 1))
+            edges = minimum_spanning_tree(edges)
+            graph_list.append({k: relative_delays[k] for k in edges})
+    else:
+        for group in groups:
+            graph_list.append({k: relative_delays[k] for k in group})
+    ret = {}
+    for graph in graph_list:
+        ret.update(calc_delays(graph, reference, reference_channel, full))
+    return ret
```

### Comparing `waveforms-1.5.82/waveforms/math/fit/geo.py` & `waveforms-1.5.83/waveforms/math/fit/geo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/fit/readout.py` & `waveforms-1.5.83/waveforms/math/fit/readout.py`

 * *Files 6% similar despite different names*

```diff
@@ -234,19 +234,23 @@
 
 
 def readout_distribution(s, p, c0, c1, cov0, cov1):
     return gaussian_pdf_2d(s, c0, cov0) * p + gaussian_pdf_2d(s, c1,
                                                               cov1) * (1 - p)
 
 
+def median_complex(c, axis=None):
+    return np.median(c.real, axis=axis) + 1j * np.median(c.imag, axis=axis)
+
+
 def fit_readout_distribution(s0, s1):
-    center = 0.5 * (s0.mean() + s1.mean())
+    center = 0.5 * (median_complex(s0) + median_complex(s1))
     s0, s1 = s0 - center, s1 - center
 
-    scale = np.max([np.abs(s0.mean()), np.abs(s1.mean()), s0.std(), s1.std()])
+    scale = np.max([np.abs(median_complex(s0)), np.abs(median_complex(s1)), s0.std(), s1.std()])
 
     s0, s1 = s0 / scale, s1 / scale
 
     def a_b_phi_2_cov(a, b, phi):
         m = np.array([[np.cos(phi) * a, -np.sin(phi) * b],
                       [np.sin(phi) * a, np.cos(phi) * b]])
 
@@ -276,20 +280,20 @@
         return (
             -np.log(readout_distribution(s0, p0, c0, c1, cov0, cov1) +
                     eps).sum() -
             np.log(readout_distribution(s1, p1, c0, c1, cov0, cov1) +
                    eps).sum())
 
     res = minimize(loss, [
-        s0.real.mean(),
-        s1.real.mean(),
+        np.median(s0.real),
+        np.median(s1.real),
         s0.real.std(),
         s1.real.std(),
-        s0.imag.mean(),
-        s1.imag.mean(),
+        np.median(s0.imag),
+        np.median(s1.imag),
         s0.imag.std(),
         s1.imag.std(), 1, 0, 0, 0
     ],
                    args=(s0, s1),
                    bounds=[(None, None), (None, None), (1e-6, None),
                            (1e-6, None), (None, None), (None, None),
                            (1e-6, None), (1e-6, None), (0, 1), (0, 1),
```

### Comparing `waveforms-1.5.82/waveforms/math/fit/resonator.py` & `waveforms-1.5.83/waveforms/math/fit/resonator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/fit/simple.py` & `waveforms-1.5.83/waveforms/math/fit/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/fit/spectrum.py` & `waveforms-1.5.83/waveforms/math/fit/spectrum.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/graph.py` & `waveforms-1.5.83/waveforms/math/graph.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 from typing import Hashable
 
 
+class _Graph():
+
+    def __init__(self):
+        self._edges = []
+        self._nodes = set()
+
+    def add_edge(self, a, b):
+        self._edges.append((a, b))
+        self._nodes.add(a)
+        self._nodes.add(b)
+
+    def __or__(self, other):
+        self._edges.extend(other._edges)
+        self._nodes.update(other._nodes)
+        return self
+
+    def __contains__(self, item):
+        return item in self._nodes
+
+
 def graphs(
     edges: list[tuple[Hashable, Hashable]]
 ) -> list[list[tuple[Hashable, Hashable]]]:
     """
     graphs
 
     Args:
         edges: list of edges
 
     Returns:
         list of graphs
     """
-    groups = []
-    ret = []
-
+    graphs: list[_Graph] = []
     for a, b in edges:
-
-        group_a_index, group_b_index = None, None
-        for i, group in enumerate(groups):
-            if a in group and b in group:
-                break
-            elif a in group:
-                group_a_index = i
-            elif b in group:
-                group_b_index = i
-            else:
-                continue
-            if group_a_index is not None and group_b_index is not None:
-                group_a_index, group_b_index = sorted(
-                    [group_a_index, group_b_index])
-                group_b = groups.pop(group_b_index)
-                group_a = groups.pop(group_a_index)
-                groups.append(group_a | group_b)
-                x = ret.pop(group_b_index)
-                y = ret.pop(group_a_index)
-                ret.append([*x, *y, (a, b)])
+        extended = []
+        for i, g in enumerate(graphs):
+            if a in g and b in g:
+                g.add_edge(a, b)
                 break
+            elif a in g or b in g:
+                g.add_edge(a, b)
+                extended.append(i)
         else:
-            if group_a_index is None and group_b_index is None:
-                groups.append({a, b})
-                ret.append([(a, b)])
-            elif group_a_index is None:
-                groups[group_b_index].add(a)
-                ret.append([(a, b)])
-            elif group_b_index is None:
-                groups[group_a_index].add(b)
-                ret.append([(a, b)])
+            if len(extended) == 0:
+                g = _Graph()
+                g.add_edge(a, b)
+                graphs.append(g)
+        if len(extended) == 2:
+            graphs[extended[0]] = graphs[extended[0]] | graphs[extended[1]]
+            del graphs[extended[1]]
 
-    return ret
+    return [[tuple(e) for e in g._edges] for g in graphs]
 
 
 def minimum_spanning_tree(
     edges: list[tuple[Hashable, Hashable]]
     | list[tuple[Hashable, Hashable, float]]
 ) -> list[tuple[Hashable, Hashable]]:
     """
```

### Comparing `waveforms-1.5.82/waveforms/math/prime.py` & `waveforms-1.5.83/waveforms/math/prime.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/signal/demodulate.py` & `waveforms-1.5.83/waveforms/math/signal/demodulate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/signal/distortion.py` & `waveforms-1.5.83/waveforms/math/signal/distortion.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/math/signal/func.py` & `waveforms-1.5.83/waveforms/math/signal/func.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/namespace.py` & `waveforms-1.5.83/waveforms/namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/__init__.py` & `waveforms-1.5.83/waveforms/qlisp/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/arch/__init__.py` & `waveforms-1.5.83/waveforms/qlisp/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/assembly.py` & `waveforms-1.5.83/waveforms/qlisp/assembly.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/base.py` & `waveforms-1.5.83/waveforms/qlisp/base.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/commands.py` & `waveforms-1.5.83/waveforms/qlisp/commands.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/compiler.py` & `waveforms-1.5.83/waveforms/qlisp/compiler.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/config.py` & `waveforms-1.5.83/waveforms/qlisp/config.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/interpreter.py` & `waveforms-1.5.83/waveforms/qlisp/interpreter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/library.py` & `waveforms-1.5.83/waveforms/qlisp/library.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/libs/__init__.py` & `waveforms-1.5.83/waveforms/qlisp/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/macro.py` & `waveforms-1.5.83/waveforms/qlisp/macro.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/parse.py` & `waveforms-1.5.83/waveforms/qlisp/parse.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/prog.py` & `waveforms-1.5.83/waveforms/qlisp/prog.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/__init__.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/eval.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/eval.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/exceptions.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/exceptions.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/libs/qelib1.inc` & `waveforms-1.5.83/waveforms/qlisp/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/__init__.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/barrier.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/binaryop.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/binaryoperator.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/creg.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/customunitary.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/expressionlist.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/external.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/format.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/gate.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/gatebody.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/id.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/idlist.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/if_.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/indexedid.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/intnode.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/measure.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/node.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/nodeexception.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/opaque.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/prefix.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/primarylist.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/program.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/qreg.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/real.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/reset.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/node/unaryoperator.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/qasm.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/qasmlexer.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/qasm/qasmparser.py` & `waveforms-1.5.83/waveforms/qlisp/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/simulator/__init__.py` & `waveforms-1.5.83/waveforms/qlisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/simulator/mat.py` & `waveforms-1.5.83/waveforms/qlisp/simulator/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/simulator/simple.py` & `waveforms-1.5.83/waveforms/qlisp/simulator/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/tokenize.py` & `waveforms-1.5.83/waveforms/qlisp/tokenize.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/qlisp/utils.py` & `waveforms-1.5.83/waveforms/qlisp/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/clifford/clifford.py` & `waveforms-1.5.83/waveforms/quantum/clifford/clifford.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/clifford/db.py` & `waveforms-1.5.83/waveforms/quantum/clifford/db.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/clifford/mat.py` & `waveforms-1.5.83/waveforms/quantum/clifford/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/clifford/seq2mat.py` & `waveforms-1.5.83/waveforms/quantum/clifford/seq2mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/math.py` & `waveforms-1.5.83/waveforms/quantum/math.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/rb.py` & `waveforms-1.5.83/waveforms/quantum/rb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/tomo.py` & `waveforms-1.5.83/waveforms/quantum/tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/transmon.py` & `waveforms-1.5.83/waveforms/quantum/transmon.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/quantum/xeb.py` & `waveforms-1.5.83/waveforms/quantum/xeb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/registry.py` & `waveforms-1.5.83/waveforms/registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/scan_iter.py` & `waveforms-1.5.83/waveforms/scan_iter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/security/verify.py` & `waveforms-1.5.83/waveforms/security/verify.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/server/__init__.py` & `waveforms-1.5.83/waveforms/server/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/server/__main__.py` & `waveforms-1.5.83/waveforms/server/__main__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/server/umsgpack.py` & `waveforms-1.5.83/waveforms/server/umsgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/device/basedevice.py` & `waveforms-1.5.83/waveforms/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/device/loader.py` & `waveforms-1.5.83/waveforms/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/device/utils.py` & `waveforms-1.5.83/waveforms/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/drivers/FakeInstrument.py` & `waveforms-1.5.83/waveforms/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/ipy_events.py` & `waveforms-1.5.83/waveforms/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/net/dhcp.py` & `waveforms-1.5.83/waveforms/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/net/dhcpd.py` & `waveforms-1.5.83/waveforms/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/net/kad.py` & `waveforms-1.5.83/waveforms/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/net/kcp.py` & `waveforms-1.5.83/waveforms/sys/net/kcp.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
 from . import _kcp
 
 
 class KCPConnection():
 
     def __init__(self,
-                 address,
-                 transport,
-                 conv: int = 1234,
+                 address: tuple[str, int],
+                 transport: asyncio.DatagramTransport,
+                 conv: int,
                  nodelay: bool = True,
                  interval: int = 20,
                  resend: int = 2,
                  nc: bool = True):
         self._kcp = _kcp.kcp_create(conv, self)
         _kcp.kcp_nodelay(self._kcp, int(nodelay), interval, resend, int(nc))
+        self.interval = interval
         self.address = address
         self.transport = transport
         self.last_active = time.time()
         self.send_queue = asyncio.Queue()
         self.recv_queue = asyncio.Queue()
         self.fut = asyncio.create_task(self.run())
 
@@ -70,15 +71,15 @@
     async def update(self):
         while True:
             await asyncio.sleep(self.check() / 1000)
             self._update()
 
     async def sync(self):
         while True:
-            await asyncio.sleep(0.01)
+            await asyncio.sleep(self.interval / 1000)
             self.flush()
 
     async def run(self):
         await asyncio.gather(self.update(), self.sync())
 
     def flush(self):
         while True:
@@ -97,28 +98,35 @@
 
         return True
 
 
 class KCPProtocol(asyncio.DatagramProtocol):
 
     def __init__(self,
+                 conv: int,
                  ttl: int = 3600,
-                 conv: int = 1234,
                  nodelay: bool = True,
                  interval: int = 20,
                  resend: int = 2,
                  nc: bool = True):
         self.ttl = ttl
         self.conv = conv
         self.nodelay = nodelay
         self.interval = interval
         self.resend = resend
         self.nc = nc
         self.transport = None
         self.connections = {}
+        self.autoclean_loop: asyncio.Future = None
+        self.clean()
+
+    def connection_lost(self, exc):
+        self.autoclean_loop.cancel()
+        for address in self.connections:
+            del self.connections[address]
 
     def connection_made(self, transport):
         self.transport = transport
 
     def get_connection(self, address):
         if address not in self.connections:
             self.connections[address] = KCPConnection(address, self.transport,
@@ -144,19 +152,21 @@
         current = time.time()
         dead = []
         for address, conn in list(self.connections.items()):
             if current - conn.last_active > self.ttl:
                 dead.append(address)
         for address in dead:
             del self.connections[address]
+        loop = asyncio.get_running_loop()
+        self.autoclean_loop = loop.call_later(10, self.clean)
 
 
 async def listen(address: tuple[str, int],
-                 ttl: int = 3600,
                  conv: int = 1234,
+                 ttl: int = 3600,
                  nodelay: bool = True,
                  interval: int = 20,
                  resend: int = 2,
                  nc: bool = True):
     """
     Listen on a UDP address and return a KCPProtocol instance.
 
@@ -170,13 +180,13 @@
         nc (bool): Whether to enable congestion control.
 
     Returns:
         A KCPProtocol instance.
     """
 
     def protocol_factory():
-        return KCPProtocol(ttl, conv, nodelay, interval, resend, nc)
+        return KCPProtocol(conv, ttl, nodelay, interval, resend, nc)
 
     loop = asyncio.get_running_loop()
     transport, protocol = await loop.create_datagram_endpoint(
         protocol_factory, local_addr=address)
     return protocol
```

### Comparing `waveforms-1.5.82/waveforms/sys/progress.py` & `waveforms-1.5.83/waveforms/sys/progress.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/storage/crud.py` & `waveforms-1.5.83/waveforms/sys/storage/crud.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/sys/storage/models.py` & `waveforms-1.5.83/waveforms/sys/storage/models.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/units/__init__.py` & `waveforms-1.5.83/waveforms/units/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/visualization/__init__.py` & `waveforms-1.5.83/waveforms/visualization/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     ax3 = ax2.twinx()
     ax3.plot(x, a, '--', lw=1, color='C0')
     ax3.plot(x, b, '--', lw=1, color='C1')
     ax3.plot(x, c, 'k--', alpha=0.5, lw=1)
     ax3.set_ylim(0, 1.1)
     ax3.vlines(thr, 0, 1.1, 'k', alpha=0.5)
-    ax3.set_ylabel('Probility')
+    ax3.set_ylabel('Integral Probability')
 
     return info
 
 
 ALLXYSeq = [('I', 'I'), ('X', 'X'), ('Y', 'Y'), ('X', 'Y'), ('Y', 'X'),
             ('X/2', 'I'), ('Y/2', 'I'), ('X/2', 'Y/2'), ('Y/2', 'X/2'),
             ('X/2', 'Y'), ('Y/2', 'X'), ('X', 'Y/2'), ('Y', 'X/2'),
```

### Comparing `waveforms-1.5.82/waveforms/visualization/plot_layout.py` & `waveforms-1.5.83/waveforms/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/waveform.py` & `waveforms-1.5.83/waveforms/waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms/waveform_parser.py` & `waveforms-1.5.83/waveforms/waveform_parser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.82/waveforms.egg-info/PKG-INFO` & `waveforms-1.5.83/waveforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.82
+Version: 1.5.83
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.82/waveforms.egg-info/SOURCES.txt` & `waveforms-1.5.83/waveforms.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -157,8 +157,9 @@
 waveforms/sys/net/kad.py
 waveforms/sys/net/kcp.py
 waveforms/sys/storage/__init__.py
 waveforms/sys/storage/crud.py
 waveforms/sys/storage/models.py
 waveforms/units/__init__.py
 waveforms/visualization/__init__.py
-waveforms/visualization/plot_layout.py
+waveforms/visualization/plot_layout.py
+waveforms/visualization/plot_seq.py
```

