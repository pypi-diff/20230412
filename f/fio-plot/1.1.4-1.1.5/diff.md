# Comparing `tmp/fio-plot-1.1.4.tar.gz` & `tmp/fio-plot-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fio-plot-1.1.4.tar", last modified: Mon Apr 10 23:25:48 2023, max compression
+gzip compressed data, was "fio-plot-1.1.5.tar", last modified: Wed Apr 12 15:36:00 2023, max compression
```

## Comparing `fio-plot-1.1.4.tar` & `fio-plot-1.1.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.944866 fio-plot-1.1.4/
--rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.4/CHANGELOG.md
--rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.4/LICENSE
--rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.4/MANIFEST.in
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-10 23:25:48.943174 fio-plot-1.1.4/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.4/README.md
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.881432 fio-plot-1.1.4/bench_fio/
--rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.890225 fio-plot-1.1.4/bench_fio/benchlib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/benchlib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/checks.py
--rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/display.py
--rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/generatefio.py
--rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/benchlib/network.py
--rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/parseini.py
--rw-r--r--   0 nan03      (501) staff       (20)     6051 2023-04-10 23:24:41.000000 fio-plot-1.1.4/bench_fio/benchlib/runfio.py
--rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.4/bench_fio/benchlib/supporting.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.891713 fio-plot-1.1.4/bench_fio/scripts/
--rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/scripts/bench-fio.sh
--rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bench_fio/scripts/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.892700 fio-plot-1.1.4/bench_fio/templates/
--rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.4/bench_fio/templates/precondition.fio
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.894533 fio-plot-1.1.4/bin/
--rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bin/bench-fio
--rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.4/bin/fio-plot
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.910301 fio-plot-1.1.4/docs/
--rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.4/docs/bench_fio_call_graph.png
--rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.4/docs/fio_plot_call_graph.png
--rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.4/docs/generate_call_graph.sh
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.917275 fio-plot-1.1.4/fio_plot/
--rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.4/fio_plot/__main__.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.939329 fio-plot-1.1.4/fio_plot/fiolib/
--rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.4/fio_plot/fiolib/__init__.py
--rw-r--r--   0 nan03      (501) staff       (20)    11039 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/argparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     7426 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/bar2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-01-30 18:56:59.000000 fio-plot-1.1.4/fio_plot/fiolib/bar3d.py
--rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/barhistogram.py
--rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/dataimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/dataimport_support.py
--rw-r--r--   0 nan03      (501) staff       (20)      724 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/defaultsettings.py
--rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.4/fio_plot/fiolib/flightchecks.py
--rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/getdata.py
--rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/graph2d.py
--rw-r--r--   0 nan03      (501) staff       (20)     6513 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/graph2dsupporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     2328 2023-01-31 12:57:49.000000 fio-plot-1.1.4/fio_plot/fiolib/iniparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/jsonimport.py
--rw-r--r--   0 nan03      (501) staff       (20)     3265 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/jsonparsing.py
--rw-r--r--   0 nan03      (501) staff       (20)     5348 2023-04-10 22:59:50.000000 fio-plot-1.1.4/fio_plot/fiolib/jsonparsing_support.py
--rw-r--r--   0 nan03      (501) staff       (20)    14738 2023-03-31 17:52:35.000000 fio-plot-1.1.4/fio_plot/fiolib/shared_chart.py
--rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-10 22:59:44.000000 fio-plot-1.1.4/fio_plot/fiolib/supporting.py
--rw-r--r--   0 nan03      (501) staff       (20)     4021 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/table_support.py
--rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.4/fio_plot/fiolib/tables.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.921508 fio-plot-1.1.4/fio_plot.egg-info/
--rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/PKG-INFO
--rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/SOURCES.txt
--rw-r--r--   0 nan03      (501) staff       (20)        1 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/dependency_links.txt
--rw-r--r--   0 nan03      (501) staff       (20)       70 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/entry_points.txt
--rw-r--r--   0 nan03      (501) staff       (20)       40 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/requires.txt
--rw-r--r--   0 nan03      (501) staff       (20)       19 2023-04-10 23:25:48.000000 fio-plot-1.1.4/fio_plot.egg-info/top_level.txt
--rw-r--r--   0 nan03      (501) staff       (20)       38 2023-04-10 23:25:48.944967 fio-plot-1.1.4/setup.cfg
--rw-r--r--   0 nan03      (501) staff       (20)      909 2023-04-10 23:24:41.000000 fio-plot-1.1.4/setup.py
-drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-10 23:25:48.941427 fio-plot-1.1.4/tests/
--rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.4/tests/bench_fio_test.py
--rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.4/tests/test_3d.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.925628 fio-plot-1.1.5/
+-rw-r--r--   0 nan03      (501) staff       (20)      845 2023-01-30 18:56:59.000000 fio-plot-1.1.5/CHANGELOG.md
+-rw-r--r--   0 nan03      (501) staff       (20)     1500 2023-01-30 18:56:59.000000 fio-plot-1.1.5/LICENSE
+-rw-r--r--   0 nan03      (501) staff       (20)      143 2023-01-30 18:56:59.000000 fio-plot-1.1.5/MANIFEST.in
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-12 15:36:00.925173 fio-plot-1.1.5/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)    18093 2023-03-27 19:45:08.000000 fio-plot-1.1.5/README.md
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.873721 fio-plot-1.1.5/bench_fio/
+-rw-r--r--   0 nan03      (501) staff       (20)     1266 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)      191 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.881437 fio-plot-1.1.5/bench_fio/benchlib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/benchlib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10583 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6052 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/checks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2916 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3295 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/display.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2338 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/generatefio.py
+-rw-r--r--   0 nan03      (501) staff       (20)      901 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/benchlib/network.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1697 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/parseini.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6051 2023-04-10 23:24:41.000000 fio-plot-1.1.5/bench_fio/benchlib/runfio.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1766 2023-04-10 22:59:50.000000 fio-plot-1.1.5/bench_fio/benchlib/supporting.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.882905 fio-plot-1.1.5/bench_fio/scripts/
+-rwxr-xr-x   0 nan03      (501) staff       (20)     1164 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/scripts/bench-fio.sh
+-rwxr-xr-x   0 nan03      (501) staff       (20)      297 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bench_fio/scripts/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.883790 fio-plot-1.1.5/bench_fio/templates/
+-rw-r--r--   0 nan03      (501) staff       (20)      167 2023-03-27 19:45:08.000000 fio-plot-1.1.5/bench_fio/templates/precondition.fio
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.886794 fio-plot-1.1.5/bin/
+-rwxr-xr-x   0 nan03      (501) staff       (20)       90 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bin/bench-fio
+-rwxr-xr-x   0 nan03      (501) staff       (20)       88 2023-01-30 18:56:59.000000 fio-plot-1.1.5/bin/fio-plot
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.902758 fio-plot-1.1.5/docs/
+-rw-r--r--   0 nan03      (501) staff       (20)   650120 2023-03-27 19:45:08.000000 fio-plot-1.1.5/docs/bench_fio_call_graph.png
+-rw-r--r--   0 nan03      (501) staff       (20)  1915904 2023-03-27 19:45:08.000000 fio-plot-1.1.5/docs/fio_plot_call_graph.png
+-rwxr-xr-x   0 nan03      (501) staff       (20)      274 2023-03-27 19:45:09.000000 fio-plot-1.1.5/docs/generate_call_graph.sh
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.907239 fio-plot-1.1.5/fio_plot/
+-rw-r--r--   0 nan03      (501) staff       (20)     1371 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)       64 2023-01-30 18:56:59.000000 fio-plot-1.1.5/fio_plot/__main__.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.923275 fio-plot-1.1.5/fio_plot/fiolib/
+-rw-r--r--   0 nan03      (501) staff       (20)        0 2023-01-30 18:56:59.000000 fio-plot-1.1.5/fio_plot/fiolib/__init__.py
+-rw-r--r--   0 nan03      (501) staff       (20)    11216 2023-04-12 15:29:01.000000 fio-plot-1.1.5/fio_plot/fiolib/argparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     7815 2023-04-12 15:19:04.000000 fio-plot-1.1.5/fio_plot/fiolib/bar2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6386 2023-04-12 15:00:11.000000 fio-plot-1.1.5/fio_plot/fiolib/bar3d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4455 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/barhistogram.py
+-rw-r--r--   0 nan03      (501) staff       (20)    10238 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/dataimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1781 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/dataimport_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)      781 2023-04-12 15:29:38.000000 fio-plot-1.1.5/fio_plot/fiolib/defaultsettings.py
+-rw-r--r--   0 nan03      (501) staff       (20)     5864 2023-03-27 19:51:32.000000 fio-plot-1.1.5/fio_plot/fiolib/flightchecks.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3292 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/getdata.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4351 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/graph2d.py
+-rw-r--r--   0 nan03      (501) staff       (20)     6278 2023-04-12 15:26:01.000000 fio-plot-1.1.5/fio_plot/fiolib/graph2dsupporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     2349 2023-04-12 15:30:20.000000 fio-plot-1.1.5/fio_plot/fiolib/iniparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4183 2023-04-10 22:59:44.000000 fio-plot-1.1.5/fio_plot/fiolib/jsonimport.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3265 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/jsonparsing.py
+-rw-r--r--   0 nan03      (501) staff       (20)     5348 2023-04-10 22:59:50.000000 fio-plot-1.1.5/fio_plot/fiolib/jsonparsing_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)    14738 2023-03-31 17:52:35.000000 fio-plot-1.1.5/fio_plot/fiolib/shared_chart.py
+-rw-r--r--   0 nan03      (501) staff       (20)    16608 2023-04-10 22:59:44.000000 fio-plot-1.1.5/fio_plot/fiolib/supporting.py
+-rw-r--r--   0 nan03      (501) staff       (20)     4021 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/table_support.py
+-rw-r--r--   0 nan03      (501) staff       (20)     3660 2023-03-27 19:45:09.000000 fio-plot-1.1.5/fio_plot/fiolib/tables.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.910659 fio-plot-1.1.5/fio_plot.egg-info/
+-rw-r--r--   0 nan03      (501) staff       (20)    18342 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/PKG-INFO
+-rw-r--r--   0 nan03      (501) staff       (20)     1530 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/SOURCES.txt
+-rw-r--r--   0 nan03      (501) staff       (20)        1 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/dependency_links.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       70 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/entry_points.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       40 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/requires.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       19 2023-04-12 15:36:00.000000 fio-plot-1.1.5/fio_plot.egg-info/top_level.txt
+-rw-r--r--   0 nan03      (501) staff       (20)       38 2023-04-12 15:36:00.925722 fio-plot-1.1.5/setup.cfg
+-rw-r--r--   0 nan03      (501) staff       (20)      909 2023-04-12 15:30:52.000000 fio-plot-1.1.5/setup.py
+drwxr-xr-x   0 nan03      (501) staff       (20)        0 2023-04-12 15:36:00.924396 fio-plot-1.1.5/tests/
+-rw-r--r--   0 nan03      (501) staff       (20)     2367 2023-01-30 18:56:59.000000 fio-plot-1.1.5/tests/bench_fio_test.py
+-rw-r--r--   0 nan03      (501) staff       (20)     1235 2023-01-30 18:56:59.000000 fio-plot-1.1.5/tests/test_3d.py
```

### Comparing `fio-plot-1.1.4/CHANGELOG.md` & `fio-plot-1.1.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/LICENSE` & `fio-plot-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/PKG-INFO` & `fio-plot-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.4
+Version: 1.1.5
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.4/README.md` & `fio-plot-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/__init__.py` & `fio-plot-1.1.5/bench_fio/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/argparsing.py` & `fio-plot-1.1.5/bench_fio/benchlib/argparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/checks.py` & `fio-plot-1.1.5/bench_fio/benchlib/checks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/defaultsettings.py` & `fio-plot-1.1.5/bench_fio/benchlib/defaultsettings.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/display.py` & `fio-plot-1.1.5/bench_fio/benchlib/display.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/generatefio.py` & `fio-plot-1.1.5/bench_fio/benchlib/generatefio.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/network.py` & `fio-plot-1.1.5/bench_fio/benchlib/network.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/parseini.py` & `fio-plot-1.1.5/bench_fio/benchlib/parseini.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/runfio.py` & `fio-plot-1.1.5/bench_fio/benchlib/runfio.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/benchlib/supporting.py` & `fio-plot-1.1.5/bench_fio/benchlib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/bench_fio/scripts/bench-fio.sh` & `fio-plot-1.1.5/bench_fio/scripts/bench-fio.sh`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/docs/bench_fio_call_graph.png` & `fio-plot-1.1.5/docs/bench_fio_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/docs/fio_plot_call_graph.png` & `fio-plot-1.1.5/docs/fio_plot_call_graph.png`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/__init__.py` & `fio-plot-1.1.5/fio_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/argparsing.py` & `fio-plot-1.1.5/fio_plot/fiolib/argparsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,20 +178,26 @@
         type=int,
         help="The moving average helps to smooth out graphs,\
                          the argument is the size of the moving window\
                               (default is None to disable). Be carefull as this\
                                        setting may smooth out issues you may want to be aware of.",
     )
     ag.add_argument(
-        "-x",
-        "--min-y",
-        help="Optional minimal value for y-axis. Use 'None' to disable.",
-        type=str,
+        "--min-iops",
+        help=f"Optional minimal value for iops axis, default is {settings['min_iops']}",
+        type=int,
+        default=0,
+    )
+    ag.add_argument(
+        "--min-lat",
+        help=f"Optional minimal value for lat axis, default is {settings['min_lat']}",
+        type=int,
         default=0,
     )
+
     ag.add_argument(
         "-t",
         "--type",
         nargs="+",
         help="\
             This setting specifies which kind of metric you want to graph.",
         type=str,
```

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/bar2d.py` & `fio-plot-1.1.5/fio_plot/fiolib/bar2d.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,23 @@
         hostcounter += 1
         attr = data["x_axis"][counter-1]
         labels.append(f"{host}\n{settings['graphtype'][-2:]} {attr}")
         if hostcounter % divide == 0:
             counter += 1
     return labels
 
+def set_max_yaxis(settings, axes):
+    for ax in axes:
+        if ax.get_ylabel() == "IOPS":
+            if settings["max_iops"]:
+                ax.set_ylim(settings["min_iops"],settings["max_iops"])
+        if "Latency" in ax.get_ylabel():
+            if settings["max_lat"]:
+                ax.set_ylim(settings["min_lat"],settings["max_lat"])
+
 def calculate_font_size(settings, x_axis):
     max_label_width = max(ts.get_max_width([x_axis], len(x_axis)))
     #print(max_label_width)
     fontsize = 0
     #
     # This hard-coded font sizing is ugly but if somebody knows a better algorithm...
     #
@@ -75,14 +84,16 @@
                 x_axis = format_hostname_labels(settings, data)
         ltest = np.arange(0.45, (len(iops) * 2), 2)
 
     ax1.set_ylabel(data["y1_axis"]["format"])
     ax3.set_ylabel(data["y2_axis"]["format"])
     ax1.set_xlabel(settings["label"])
     ax1.set_xticks(ltest)
+
+    set_max_yaxis(settings, [ax1, ax3])
     
     fontsize = calculate_font_size(settings, x_axis)
     #print(fontsize)
     if settings["graphtype"] == "compare_graph":
         ax1.set_xticklabels(labels=x_axis, fontsize=fontsize)
     elif settings["graphtype"] == "bargraph2d_qd" or settings["graphtype"] == "bargraph2d_nj":
         ax1.set_xticklabels(labels=x_axis, fontsize=fontsize,)
```

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/bar3d.py` & `fio-plot-1.1.5/fio_plot/fiolib/bar3d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/barhistogram.py` & `fio-plot-1.1.5/fio_plot/fiolib/barhistogram.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/dataimport.py` & `fio-plot-1.1.5/fio_plot/fiolib/dataimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/dataimport_support.py` & `fio-plot-1.1.5/fio_plot/fiolib/dataimport_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/defaultsettings.py` & `fio-plot-1.1.5/fio_plot/fiolib/defaultsettings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sys
 
 def get_default_settings():
     settings = {}
+    settings["min_lat"] = 0
+    settings["min_iops"] = 0
     settings["filter"] = ['read','write']
     settings["type"] = []
     settings["dpi"] = 200
     settings["title_fontsize"] = 16
     settings["subtitle_fontsize"] = 10
     settings["credit_fontsize"] = 10
     settings["source_fontsize"] = 8
```

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/flightchecks.py` & `fio-plot-1.1.5/fio_plot/fiolib/flightchecks.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/getdata.py` & `fio-plot-1.1.5/fio_plot/fiolib/getdata.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/graph2d.py` & `fio-plot-1.1.5/fio_plot/fiolib/graph2d.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/graph2dsupporting.py` & `fio-plot-1.1.5/fio_plot/fiolib/graph2dsupporting.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,29 +52,21 @@
     if diff > 0:
         label = label + " " * diff
     return label
 
 
 def scale_2dgraph_yaxis(settings, item, rw, maximum):
     factordict = {"iops": 1.05, "lat": 1.25, "bw": 1.5, "slat": 1.25, "clat": 1.25 }
-    min_y = 0
-    if settings["min_y"] == "None":
-        min_y = None
-    else:
-        try:
-            min_y = int(settings["min_y"])
-        except ValueError:
-            print("Min_y value is invalid (not None or integer).")
 
     max_y = maximum["total"][item["type"]] * factordict[item["type"]]
 
     if settings[f"max_{item['type']}"]:
         max_y = settings[f"max_{item['type']}"]
 
-    return (min_y, max_y)
+    return (0, max_y)
 
 
 def validate_colors(colors):
     listofcolors = []
     listofcolors.extend(list(mcolors.TABLEAU_COLORS.keys()))
     listofcolors.extend(list(mcolors.CSS4_COLORS.keys()))
     listofcolors.extend(list(mcolors.XKCD_COLORS.keys()))
```

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/iniparsing.py` & `fio-plot-1.1.5/fio_plot/fiolib/iniparsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     else:
         print(f"\nConfig file {filename} is not a file.\n")
         sys.exit(1)
 
 def get_settings_from_ini(args):
     listtypes = ['input_directory','filter','colors','type']
     listinttypes = ['iodepth','numjobs']
-    integers = ['maxdepth','maxjobs','dpi','max_z','max_lat','max_iops','max_bw','xlabel_depth','xlabel_parent','xlabel_segment_size','line_width','source_fontsize','subtitle_fontsize','title_fontsize']
+    integers = ['maxdepth','maxjobs','dpi','max_z','max_lat','max_iops','min_lat','min_iops','max_bw','xlabel_depth','xlabel_parent','xlabel_segment_size','line_width','source_fontsize','subtitle_fontsize','title_fontsize']
     floats = ['percentile']
     booltypes = ['show_cpu','show_ss','table_lines','disable_grid','enable_markers','disable_fio_version','moving_average']
     returndict = {}
     if len(args) > 1:
         if not "-" in args[1][0]:
             filename = args[1]
             config = read_ini_file(filename)
```

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/jsonimport.py` & `fio-plot-1.1.5/fio_plot/fiolib/jsonimport.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/jsonparsing.py` & `fio-plot-1.1.5/fio_plot/fiolib/jsonparsing.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/jsonparsing_support.py` & `fio-plot-1.1.5/fio_plot/fiolib/jsonparsing_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/shared_chart.py` & `fio-plot-1.1.5/fio_plot/fiolib/shared_chart.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/supporting.py` & `fio-plot-1.1.5/fio_plot/fiolib/supporting.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/table_support.py` & `fio-plot-1.1.5/fio_plot/fiolib/table_support.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot/fiolib/tables.py` & `fio-plot-1.1.5/fio_plot/fiolib/tables.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/fio_plot.egg-info/PKG-INFO` & `fio-plot-1.1.5/fio_plot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fio-plot
-Version: 1.1.4
+Version: 1.1.5
 Summary: Create charts from FIO storage benchmark tool output
 Home-page: https://github.com/louwrentius/fio-plot/
 Author: louwrentius
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## fio-plot
```

### Comparing `fio-plot-1.1.4/fio_plot.egg-info/SOURCES.txt` & `fio-plot-1.1.5/fio_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/setup.py` & `fio-plot-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name="fio-plot",
-        version="1.1.4",
+        version="1.1.5",
         author="louwrentius",
         description="Create charts from FIO storage benchmark tool output",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/louwrentius/fio-plot/", 
         packages=setuptools.find_packages(),
         install_requires=['numpy','matplotlib','Pillow', 'pyan3', 'pyparsing'],
```

### Comparing `fio-plot-1.1.4/tests/bench_fio_test.py` & `fio-plot-1.1.5/tests/bench_fio_test.py`

 * *Files identical despite different names*

### Comparing `fio-plot-1.1.4/tests/test_3d.py` & `fio-plot-1.1.5/tests/test_3d.py`

 * *Files identical despite different names*

