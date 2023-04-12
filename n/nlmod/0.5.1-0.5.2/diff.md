# Comparing `tmp/nlmod-0.5.1.tar.gz` & `tmp/nlmod-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlmod-0.5.1.tar", last modified: Tue Feb 21 14:28:54 2023, max compression
+gzip compressed data, was "nlmod-0.5.2.tar", last modified: Wed Apr 12 10:40:27 2023, max compression
```

## Comparing `nlmod-0.5.1.tar` & `nlmod-0.5.2.tar`

### file list

```diff
@@ -1,78 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.784701 nlmod-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-21 14:28:41.000000 nlmod-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-21 14:28:54.784701 nlmod-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-02-21 14:28:41.000000 nlmod-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.772701 nlmod-0.5.1/nlmod/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.776701 nlmod-0.5.1/nlmod/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.776701 nlmod-0.5.1/nlmod/data/geotop/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/geotop/geo_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/geotop/litho_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/opp_water.cpg
--rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/opp_water.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/opp_water.prj
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/opp_water.qpj
--rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/opp_water.shp
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/opp_water.shx
--rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/data/regis_2_2.gleg
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.776701 nlmod-0.5.1/nlmod/dims/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    53673 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    35843 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/dims/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.780701 nlmod-0.5.1/nlmod/gwf/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/gwf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/horizontal_flow_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/recharge.py
--rw-r--r--   0 runner    (1001) docker     (123)    26752 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/gwf/wells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.780701 nlmod-0.5.1/nlmod/modpath/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/modpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/modpath/modpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.780701 nlmod-0.5.1/nlmod/read/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/ahn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/bgt.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/brp.py
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/jarkus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/regis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/rws.py
--rw-r--r--   0 runner    (1001) docker     (123)    22164 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/waterboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/read/webservices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.780701 nlmod-0.5.1/nlmod/sim/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/sim/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-21 14:28:41.000000 nlmod-0.5.1/nlmod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.772701 nlmod-0.5.1/nlmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-21 14:28:54.000000 nlmod-0.5.1/nlmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-02-21 14:28:54.000000 nlmod-0.5.1/nlmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 14:28:54.000000 nlmod-0.5.1/nlmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-21 14:28:54.000000 nlmod-0.5.1/nlmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-21 14:28:54.000000 nlmod-0.5.1/nlmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 14:28:54.784701 nlmod-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-21 14:28:41.000000 nlmod-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 14:28:54.784701 nlmod-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10682 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_001_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_002_regis_geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_003_mfpackages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_004_northsea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_005_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_006_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_007_run_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_008_waterschappen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_009_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_gwf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-02-21 14:28:41.000000 nlmod-0.5.1/tests/test_mtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.349893 nlmod-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-12 10:40:07.000000 nlmod-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 10:40:27.349893 nlmod-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 10:40:07.000000 nlmod-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.337893 nlmod-0.5.2/nlmod/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/data/geotop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/geotop/geo_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/geotop/litho_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.qpj
+-rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.shx
+-rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/regis_2_2.gleg
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/dims/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55292 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35438 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/gwf/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/gwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/horizontal_flow_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/recharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36376 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/wells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/gwt/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/gwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/modpath/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/modpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/modpath/modpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/ahn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/bgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/brp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/jarkus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/meteobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/regis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/rws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/waterboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/webservices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/sim/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.337893 nlmod-0.5.2/nlmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:40:27.349893 nlmod-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 10:40:07.000000 nlmod-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.349893 nlmod-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_001_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_002_regis_geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_003_mfpackages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_004_northsea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_005_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_006_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_007_run_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_008_waterschappen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_009_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_010_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_011_dcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_012_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_013_surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_014_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_015_gwf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_016_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_017_metbase.py
```

### Comparing `nlmod-0.5.1/LICENSE` & `nlmod-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/PKG-INFO` & `nlmod-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlmod
-Version: 0.5.1
+Version: 0.5.2
 Summary: nlmod module by Artesia
 Home-page: https://github.com/ArtesiaWater/nlmod
 Author: Artesia
 License: MIT
 Platform: Windows
 Platform: Mac OS-X
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nlmod-0.5.1/README.md` & `nlmod-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/cache.py` & `nlmod-0.5.2/nlmod/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     """
 
     # add cachedir and cachename to docstring
     _update_docstring_and_signature(func)
 
     @functools.wraps(func)
     def decorator(*args, cachedir=None, cachename=None, **kwargs):
-
         # 1 check if cachedir and name are provided
         if cachedir is None or cachename is None:
             return func(*args, **kwargs)
 
         if not cachename.endswith(".nc"):
             cachename += ".nc"
```

### Comparing `nlmod-0.5.1/nlmod/data/geotop/geo_eenheden.csv` & `nlmod-0.5.2/nlmod/data/geotop/geo_eenheden.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv` & `nlmod-0.5.2/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/data/opp_water.dbf` & `nlmod-0.5.2/nlmod/data/opp_water.dbf`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/data/opp_water.qpj` & `nlmod-0.5.2/nlmod/data/opp_water.qpj`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/data/opp_water.shp` & `nlmod-0.5.2/nlmod/data/opp_water.shp`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/data/regis_2_2.gleg` & `nlmod-0.5.2/nlmod/data/regis_2_2.gleg`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/dcs.py` & `nlmod-0.5.2/nlmod/dcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import flopy
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import xarray as xr
 from matplotlib.collections import LineCollection, PatchCollection
 from matplotlib.patches import Rectangle
-from shapely.geometry import LineString, Point, Polygon, MultiLineString
-import flopy
+from shapely.geometry import LineString, MultiLineString, Point, Polygon
 
 from .dims.grid import modelgrid_from_ds
 
 
 class DatasetCrossSection:
     # assumes:
     # x and y are 1d-vectors
```

### Comparing `nlmod-0.5.1/nlmod/dims/base.py` & `nlmod-0.5.2/nlmod/dims/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     anisotropy=10,
     fill_value_kh=1.0,
     fill_value_kv=0.1,
     xorigin=0.0,
     yorigin=0.0,
     angrot=0.0,
     drop_attributes=True,
+    transport=False,
 ):
     """Transform a regis datset to a model dataset with another resolution.
 
     Parameters
     ----------
     ds : xarray.dataset
         A layer model dataset.
@@ -113,15 +114,18 @@
     yorigin : int or float, optional
         lower left y coordinate of the model grid only used if angrot != 0.
         Default is 0.0.
     angrot : int or float, optinal
         the rotation of the grid in counter clockwise degrees, default is 0.0
     drop_attributes : bool, optional
         if True drop the attributes from the layer model dataset. Otherwise
-        keep the attributes. Default is True
+        keep the attributes. Default is True.
+    transport : bool, optional
+        flag indicating whether dataset includes data for a groundwater
+        transport model (GWT). Default is False, no transport.
 
     Returns
     -------
     ds : xarray.dataset
         the model Dataset.
     """
     if extent is None:
@@ -154,14 +158,15 @@
         raise TypeError("unexpected type for delr and/or delc")
 
     if extrapolate:
         ds = extrapolate_ds(ds)
 
     # add attributes
     ds = set_ds_attrs(ds, model_name, model_ws)
+    ds.attrs["transport"] = int(transport)
 
     # fill nan's and add idomain
     if fill_nan:
         ds = fill_nan_top_botm_kh_kv(
             ds,
             anisotropy=anisotropy,
             fill_value_kh=fill_value_kh,
@@ -197,15 +202,15 @@
     if mask is None:
         mask = np.isnan(ds["botm"]).all("layer").data
     if not mask.any():
         # all of the model cells are is inside the known area
         return ds
     if mask.all():
         raise (Exception("The model only contains NaNs"))
-    if ds.gridtype == "vertex":
+    if "gridtype" in ds.attrs and ds.gridtype == "vertex":
         x = ds.x.data
         y = ds.y.data
         dims = ("icell2d",)
     else:
         x, y = np.meshgrid(ds.x, ds.y)
         dims = ("y", "x")
     points = np.stack((x[~mask], y[~mask]), axis=1)
@@ -231,47 +236,50 @@
 
 def get_ds(
     extent,
     delr=100.0,
     delc=None,
     model_name=None,
     model_ws=None,
-    layer=10,
+    layer=None,
     top=0.0,
     botm=None,
     kh=10.0,
     kv=1.0,
     crs=28992,
     xorigin=0.0,
     yorigin=0.0,
     angrot=0.0,
     attrs=None,
     extrapolate=True,
     fill_nan=True,
+    transport=False,
     **kwargs,
 ):
     """Create a model dataset from scratch, so without a layer model.
 
     Parameters
     ----------
     extent : list, tuple or np.array
         desired model extent (xmin, xmax, ymin, ymax)
     delr : int, float, list, tuple or array, optional
         The gridsize along columns (dx). The default is 100. meter.
     delc : None, int, float, list, tuple or array, optional
-        The gridsize along rows (dy). Set to delr when None. If None delc=delr
-        The default is None.
+        The gridsize along rows (dy). Set to delr when None. If None delc=delr. The
+        default is None.
     model_name : str, optional
         name of the model. THe default is None
     model_ws : str, optional
-        workspace of the model. This is where modeldata is saved to. The
-        default is None
+        workspace of the model. This is where modeldata is saved to. The default is
+        None.
     layer : int, list, tuple or ndarray, optional
-        The layers of the model. When layer is an integer it is the number of
-        layers. The default is 10.
+        The names or index of the layers of the model. When layer is an integer it is
+        the number of layers. When layer is None, the number of layers is caluclated
+        from botm. When botm is None as well, the number of layers is set to 10. The
+        default is None.
     top : float, list or ndarray, optional
         The top of the model. It has to be of shape (len(y), len(x)) or it is
         transformed into that shape if top is a float. The default is 0.0.
     botm : list or ndarray, optional
         The botm of the model layers. It has to be of shape
         (len(layer), len(y), len(x)) or it is transformed to that shape if botm
         is or a list/array of len(layer). When botm is None, a botm is
@@ -296,20 +304,22 @@
     angrot : float, optional
         counter-clockwise rotation angle (in degrees) of the lower-left corner of the
         model grid. The default is 0.0
     attrs : dict, optional
         Attributes of the model dataset. The default is None.
     extrapolate : bool, optional
         When true, extrapolate data-variables, into the sea or other areas with
-        only nans. THe default is True
+        only nans. The default is True
     fill_nan : bool, optional
         if True nan values in the top, botm, kh and kv are filled using the
         fill_nan_top_botm_kh_kv function. Layers with only nan values in the
         botm are removed.
-
+    transport : bool, optional
+        flag indicating whether dataset includes data for a groundwater
+        transport model (GWT). Default is False, no transport.
 
 
     **kwargs : dict
         Kwargs are passed into mbase.to_ds. These can be the model_name
         or ds.
 
     Returns
@@ -324,25 +334,32 @@
         delr = np.asarray(delr)
 
     if isinstance(delc, (tuple, list)):
         delc = np.asarray(delc)
 
     if attrs is None:
         attrs = {}
+
+    if layer is None:
+        if botm is None:
+            layer = 10
+        else:
+            layer = len(botm)
     if isinstance(layer, int):
         layer = np.arange(1, layer + 1)
     if botm is None:
         botm = top - 10 * np.arange(1.0, len(layer) + 1)
 
     # check for nan
     for par in [top, botm, kh, kv]:
         if isinstance(par, numbers.Number):
             if np.isnan(par) and (extrapolate or fill_nan):
                 raise ValueError(
-                    "extrapolate and remove_nan_layer should be False when setting model parameters to nan"
+                    "extrapolate and remove_nan_layer should be "
+                    "False when setting model parameters to nan"
                 )
 
     resample._set_angrot_attributes(extent, xorigin, yorigin, angrot, attrs)
     x, y = resample.get_xy_mid_structured(attrs["extent"], delr, delc)
     coords = dict(x=x, y=y, layer=layer)
     if angrot != 0.0:
         affine = resample.get_affine_mod_to_world(attrs)
@@ -396,11 +413,12 @@
         model_ws=model_ws,
         extent=extent,
         delr=delr,
         delc=delc,
         drop_attributes=False,
         extrapolate=extrapolate,
         fill_nan=fill_nan,
+        transport=transport,
         **kwargs,
     )
     ds.rio.set_crs(crs)
     return ds
```

### Comparing `nlmod-0.5.1/nlmod/dims/grid.py` & `nlmod-0.5.2/nlmod/dims/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 import xarray as xr
 from flopy.discretization.structuredgrid import StructuredGrid
 from flopy.discretization.vertexgrid import VertexGrid
 from flopy.utils.gridgen import Gridgen
 from flopy.utils.gridintersect import GridIntersect
 from packaging import version
 from scipy.interpolate import griddata
-from shapely.geometry import Point, Polygon
 from shapely.affinity import affine_transform
+from shapely.geometry import Point, Polygon
 from tqdm import tqdm
 
 from .. import cache, util
 from .base import extrapolate_ds
 from .layers import fill_nan_top_botm_kh_kv, get_first_active_layer, set_idomain
 from .rdp import rdp
 from .resample import (
     affine_transform_gdf,
-    get_affine_world_to_mod,
     get_affine_mod_to_world,
+    get_affine_world_to_mod,
     structured_da_to_ds,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def xy_to_icell2d(xy, ds):
@@ -230,22 +230,23 @@
     model_coordinates=False,
 ):
     """Refine the grid (discretization by vertices, disv), using Gridgen.
 
     Parameters
     ----------
     ds : xarray.Datset
-        A structured model datset.
+        A structured model Dataset.
     model_ws : str, optional
         The working directory fpr GridGen. Get from ds when model_ws is None.
         The default is None.
-    refinement_features : list of tuple of length 2, optional
+    refinement_features : list of tuples of length 2 or 3, optional
         List of tuples containing refinement features. Each tuple must be of
-        the form (GeoDataFrame, level) or (geometry, shape_type, level). The
-        default is None.
+        the form (GeoDataFrame, level) or (geometry, shape_type, level). When
+        refinement_features is None, no refinement is added, but the structured model
+        Dataset is transformed to a Vertex Dataset. The default is None.
     exe_name : str, optional
         Filepath to the gridgen executable. The file path within nlmod is chose
         if exe_name is None. The default is None.
     remove_nan_layers : bool, optional
         if True layers that are inactive everywhere are removed from the model.
         If False nan layers are kept which might be usefull if you want
         to keep some layers that exist in other models. The default is True.
@@ -253,15 +254,15 @@
         When model_coordinates is True, the features supplied in refinement features are
         allready in model-coordinates. Only used when a grid is rotated. The default is
         False.
 
     Returns
     -------
     xarray.Dataset
-        The refined model dataset.
+        A Vertex model Dataset
     """
     assert ds.gridtype == "structured", "Can only refine a structured grid"
     logger.info("create vertex grid using gridgen")
 
     if exe_name is None:
         exe_name = util.get_exe_path("gridgen")
 
@@ -436,16 +437,16 @@
     method : str
         The method used for resampling layer_ds to the grid of ds.
     **kwargs : keyword arguments
         keyword arguments are passed to the fill_nan_top_botm_kh_kv-method.
 
     Returns
     -------
-    ds : TYPE
-        DESCRIPTION.
+    ds : xarray.Dataset
+        Dataset with variables from layer_ds.
     """
     if not layer_ds.layer.equals(ds.layer):
         # do not change the original Dataset
         layer_ds = layer_ds.copy()
         # update layers in ds
         drop_vars = []
         for var in ds.data_vars:
@@ -454,18 +455,23 @@
                     logger.info(
                         f"Variable {var} is dropped, as it has dimension layer, but is not defined in layer_ds"
                     )
                 drop_vars.append(var)
         if len(drop_vars) > 0:
             ds = ds.drop_vars(drop_vars)
         ds = ds.assign_coords({"layer": layer_ds.layer})
+    has_rotation = "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0
     if method in ["nearest", "linear"]:
-        layer_ds = layer_ds.interp(
-            x=ds.x, y=ds.y, method="nearest", kwargs={"fill_value": None}
-        )
+        if has_rotation:
+            x = ds.xc
+            y = ds.yc
+        else:
+            x = ds.x
+            y = ds.y
+        layer_ds = layer_ds.interp(x=x, y=y, method=method, kwargs={"fill_value": None})
         for var in layer_ds.data_vars:
             ds[var] = layer_ds[var]
     else:
         for var in layer_ds.data_vars:
             ds[var] = structured_da_to_ds(layer_ds[var], ds, method=method)
     ds = extrapolate_ds(ds)
     ds = fill_nan_top_botm_kh_kv(ds, **kwargs)
@@ -478,15 +484,15 @@
     This function is typically used to create a rec_array with stress period
     data for the modflow packages. Can be used for structured and
     vertex grids.
 
     Parameters
     ----------
     col_in : xarray.DatArray, str, int or float
-        if col_in is a str type it is the name of the column in ds.
+        if col_in is a str type it is the name of the column in ds (if it exists).
         if col_in is an int or a float it is a value that will be used for all
         cells in cellids.
     ds : xarray.Dataset
         dataset with model data. Can have dimension (layer, y, x) or
         (layer, icell2d).
     cellids : tuple of numpy arrays
         tuple with indices of the cells that will be used to create the list
@@ -502,15 +508,15 @@
 
     Returns
     -------
     col_lst : list
         raster values from ds presented in a list per cell.
     """
 
-    if isinstance(col_in, str):
+    if isinstance(col_in, str) and col_in in ds:
         col_in = ds[col_in]
     if isinstance(col_in, xr.DataArray):
         if len(cellids) == 3:
             # 3d grid
             col_lst = [
                 col_in.data[lay, row, col]
                 for lay, row, col in zip(cellids[0], cellids[1], cellids[2])
@@ -527,15 +533,17 @@
             raise ValueError(f"could not create a column list for col_in={col_in}")
     else:
         col_lst = [col_in] * len(cellids[0])
 
     return col_lst
 
 
-def lrc_to_reclist(layers, rows, columns, cellids, ds, col1=None, col2=None, col3=None):
+def lrc_to_reclist(
+    layers, rows, columns, cellids, ds, col1=None, col2=None, col3=None, aux=None
+):
     """Create a reclist for stress period data from a set of cellids.
 
     Used for structured grids.
 
 
     Parameters
     ----------
@@ -574,45 +582,68 @@
     col3 : str, int or float, optional
         3th column of the reclist, if None the reclist will be a list with
         ((layer,row,column), col1, col2) for each row.
 
         col3 should be the following value for each package (can also be the
             name of a timeseries):
 
+    aux : str or list of str
+        list of auxiliary variables to include in reclist
+
     Raises
     ------
     ValueError
         Question: will this error ever occur?.
 
     Returns
     -------
     reclist : list of tuples
         every row consist of ((layer,row,column), col1, col2, col3).
     """
-    if col1 is None:
-        reclist = list(zip(zip(layers, rows, columns)))
-    elif (col1 is not None) and col2 is None:
-        col1_lst = col_to_list(col1, ds, cellids)
-        reclist = list(zip(zip(layers, rows, columns), col1_lst))
-    elif (col2 is not None) and col3 is None:
-        col1_lst = col_to_list(col1, ds, cellids)
-        col2_lst = col_to_list(col2, ds, cellids)
-        reclist = list(zip(zip(layers, rows, columns), col1_lst, col2_lst))
-    elif col3 is not None:
-        col1_lst = col_to_list(col1, ds, cellids)
-        col2_lst = col_to_list(col2, ds, cellids)
-        col3_lst = col_to_list(col3, ds, cellids)
-        reclist = list(zip(zip(layers, rows, columns), col1_lst, col2_lst, col3_lst))
-    else:
-        raise ValueError("invalid combination of values for col1, col2 and col3")
+    cols = []
+
+    if col1 is not None:
+        cols.append(col_to_list(col1, ds, cellids))
+    if col2 is not None and len(cols) == 1:
+        cols.append(col_to_list(col2, ds, cellids))
+    elif col2 is not None and len(cols) != 1:
+        raise ValueError("col2 is set, but col1 is not!")
+    if col3 is not None and len(cols) == 2:
+        cols.append(col_to_list(col3, ds, cellids))
+    elif col3 is not None and len(cols) != 2:
+        raise ValueError("col3 is set, but col1 and/or col2 are not!")
+
+    if aux is not None:
+        if isinstance(aux, str):
+            aux = [aux]
+        elif isinstance(aux, (int, float)):
+            aux = [aux]
+
+        for i_aux in aux:
+            if isinstance(i_aux, str):
+                if "layer" in ds[i_aux].dims and len(cellids) != 3:
+                    cols.append(col_to_list(i_aux, ds, (np.array(layers),) + cellids))
+                else:
+                    cols.append(col_to_list(i_aux, ds, cellids))
+            else:
+                cols.append(col_to_list(i_aux, ds, cellids))
 
+    reclist = list(zip(zip(layers, rows, columns), *cols))
     return reclist
 
 
-def lcid_to_reclist(layers, cellids, ds, col1=None, col2=None, col3=None):
+def lcid_to_reclist(
+    layers,
+    cellids,
+    ds,
+    col1=None,
+    col2=None,
+    col3=None,
+    aux=None,
+):
     """Create a reclist for stress period data from a set of cellids.
 
     Used for vertex grids.
 
 
     Parameters
     ----------
@@ -645,52 +676,68 @@
 
     col3 : str, int or float, optional
         3th column of the reclist, if None the reclist will be a list with
         ((layer,icell2d), col1, col2) for each row. col3 should be the following
         value for each package (can also be the name of a timeseries):
         -   riv: bottom [L]
 
+    aux : str or list of str
+        list of auxiliary variables to include in reclist
+
     Raises
     ------
     ValueError
         Question: will this error ever occur?.
 
     Returns
     -------
     reclist : list of tuples
         every row consist of ((layer, icell2d), col1, col2, col3)
         grids.
     """
-    if col1 is None:
-        reclist = list(zip(zip(layers, cellids[-1])))
-    elif (col1 is not None) and col2 is None:
-        col1_lst = col_to_list(col1, ds, cellids)
-        reclist = list(zip(zip(layers, cellids[-1]), col1_lst))
-    elif (col2 is not None) and col3 is None:
-        col1_lst = col_to_list(col1, ds, cellids)
-        col2_lst = col_to_list(col2, ds, cellids)
-        reclist = list(zip(zip(layers, cellids[-1]), col1_lst, col2_lst))
-    elif col3 is not None:
-        col1_lst = col_to_list(col1, ds, cellids)
-        col2_lst = col_to_list(col2, ds, cellids)
-        col3_lst = col_to_list(col3, ds, cellids)
-        reclist = list(zip(zip(layers, cellids[-1]), col1_lst, col2_lst, col3_lst))
-    else:
-        raise ValueError("invalid combination of values for col1, col2 and col3")
+    cols = []
+
+    if col1 is not None:
+        cols.append(col_to_list(col1, ds, cellids))
+    if col2 is not None and len(cols) == 1:
+        cols.append(col_to_list(col2, ds, cellids))
+    elif col2 is not None and len(cols) != 1:
+        raise ValueError("col2 is set, but col1 is not!")
+    if col3 is not None and len(cols) == 2:
+        cols.append(col_to_list(col3, ds, cellids))
+    elif col3 is not None and len(cols) != 2:
+        raise ValueError("col3 is set, but col1 and/or col2 are not!")
+
+    if aux is not None:
+        if isinstance(aux, str):
+            aux = [aux]
+        elif isinstance(aux, (int, float)):
+            aux = [aux]
+
+        for i_aux in aux:
+            if isinstance(i_aux, str):
+                if "layer" in ds[i_aux].dims and len(cellids) != 2:
+                    cols.append(col_to_list(i_aux, ds, (np.array(layers),) + cellids))
+                else:
+                    cols.append(col_to_list(i_aux, ds, cellids))
+            else:
+                cols.append(col_to_list(i_aux, ds, cellids))
 
+    reclist = list(zip(zip(layers, cellids[-1]), *cols))
     return reclist
 
 
 def da_to_reclist(
     ds,
     mask,
     col1=None,
     col2=None,
     col3=None,
     layer=0,
+    aux=None,
     first_active_layer=False,
     only_active_cells=True,
 ):
     """Create a reclist for stress period data from a model dataset.
 
     Used for vertex grids.
 
@@ -724,14 +771,16 @@
     col3 : str, int or float, optional
         3th column of the reclist, if None the reclist will be a list with
         (cellid, col1, col2) for each row.
 
         col3 should be the following value for each package (can also be the
             name of a timeseries):
             riv: bottom [L]
+    aux : str or list of str, optional
+        list of auxiliary variables to include in reclist
     layer : int, optional
         layer used in the reclist. Not used if layer is in the dimensions of
         mask or if first_active_layer is True. The default is 0
     first_active_layer : bool, optional
         If True an extra mask is applied to use the first active layer of each
         cell in the grid. Not used if layer is in the dimensions of mask. The
         default is False.
@@ -753,20 +802,22 @@
                     f"ignore {ignore_cells} out of {np.sum(mask)} cells because idomain is inactive"
                 )
         else:
             cellids = np.where(mask)
 
         if "icell2d" in mask.dims:
             layers = cellids[0]
-            return lcid_to_reclist(layers, cellids, ds, col1, col2, col3)
+            return lcid_to_reclist(layers, cellids, ds, col1, col2, col3, aux=aux)
         else:
             layers = cellids[0]
             rows = cellids[1]
             columns = cellids[2]
-            return lrc_to_reclist(layers, rows, columns, cellids, ds, col1, col2, col3)
+            return lrc_to_reclist(
+                layers, rows, columns, cellids, ds, col1, col2, col3, aux=aux
+            )
     else:
         if first_active_layer:
             fal = get_first_active_layer(ds)
             cellids = np.where((mask) & (fal != fal.attrs["_FillValue"]))
             layers = col_to_list(fal, ds, cellids)
         elif only_active_cells:
             cellids = np.where((mask) & (ds["idomain"][layer] == 1))
@@ -777,20 +828,22 @@
                 )
             layers = col_to_list(layer, ds, cellids)
         else:
             cellids = np.where(mask)
             layers = col_to_list(layer, ds, cellids)
 
         if "icell2d" in mask.dims:
-            return lcid_to_reclist(layers, cellids, ds, col1, col2, col3)
+            return lcid_to_reclist(layers, cellids, ds, col1, col2, col3, aux=aux)
         else:
             rows = cellids[-2]
             columns = cellids[-1]
 
-            return lrc_to_reclist(layers, rows, columns, cellids, ds, col1, col2, col3)
+            return lrc_to_reclist(
+                layers, rows, columns, cellids, ds, col1, col2, col3, aux=aux
+            )
 
 
 def polygon_to_area(modelgrid, polygon, da, gridtype="structured"):
     """create a grid with the surface area in each cell based on a polygon
     value.
 
     Parameters
@@ -819,17 +872,16 @@
         )
 
     ix = GridIntersect(modelgrid, method="vertex")
     opp_cells = ix.intersect(polygon)
 
     if gridtype == "structured":
         area_array = util.get_da_from_da_ds(da, dims=("y", "x"), data=0)
-        for opp_row in opp_cells:
-            area = opp_row[-2]
-            area_array[opp_row[0][0], opp_row[0][1]] = area
+        for cellid, area in zip(opp_cells["cellids"], opp_cells["areas"]):
+            area_array[cellid[0], cellid[1]] = area
     elif gridtype == "vertex":
         area_array = util.get_da_from_da_ds(da, dims=("icell2d",), data=0)
         cids = opp_cells.cellids
         area = opp_cells.areas
         area_array[cids.astype(int)] = area
 
     return area_array
@@ -1137,14 +1189,19 @@
         xarray with model data
 
     Returns
     -------
     da : xr.DataArray
         1 if polygon is in cell, 0 otherwise. Grid dimensions according to ds.
     """
+    if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
+        # transform gdf into model coordinates
+        affine = get_affine_world_to_mod(ds)
+        gdf = affine_transform_gdf(gdf, affine)
+
     modelgrid = modelgrid_from_ds(ds)
 
     # build list of gridcells
     ix = GridIntersect(modelgrid, method="vertex")
 
     if ds.gridtype == "structured":
         da = util.get_da_from_da_ds(ds, dims=("y", "x"), data=0)
@@ -1159,15 +1216,15 @@
         geoms = [gdf]
 
     for geom in geoms:
         cids = ix.intersects(geom)["cellids"]
         if ds.gridtype == "structured":
             ncol = modelgrid.ncol
             for cid in cids:
-                if version.parse(flopy.__version__) < version.parse("3.3.6"):
+                if isinstance(cid, tuple):
                     i, j = cid
                 else:
                     # TODO: temporary fix until flopy intersect on structured
                     # grid returns row, col again.
                     i = int((cid) / ncol)
                     j = cid - i * ncol
                 da[i, j] = 1
@@ -1207,37 +1264,36 @@
     gdf,
     ml=None,
     method="vertex",
     ix=None,
     desc="Intersecting with grid",
     **kwargs,
 ):
-    """Cut a geodataframe gdf by the grid of a flopy modflow model ml. This
-    method is just a wrapper around the GridIntersect method from flopy.
+    """Cut a geodataframe gdf by the grid of a flopy modflow model ml. This method is a
+    wrapper around the GridIntersect method from flopy.
 
     Parameters
     ----------
     gdf : geopandas.GeoDataFrame
-        A GeoDataFrame that needs to be cut by the grid. The GeoDataFrame can
-        consist of multiple types (Point, LineString, Polygon and the Multi-
-        variants).
+        A GeoDataFrame that needs to be cut by the grid. The GeoDataFrame can consist of
+        multiple types (Point, LineString, Polygon and the Multi-variants).
     ml : flopy.modflow.Modflow or flopy.mf6.ModflowGwf or xarray.Dataset, optional
         The flopy model or xarray dataset that defines the grid. When a Dataset is
         supplied, and the grid is rotated, the geodataframe is transformed in model
         coordinates. The default is None.
     method : string, optional
         Method passed to the GridIntersect-class. The default is 'vertex'.
     ix : flopy.utils.GridIntersect, optional
         GridIntersect, if not provided the modelgrid in ml is used.
     **kwargs : keyword arguments
         keyword arguments are passed to the intersect_*-methods.
 
     Returns
     -------
-    geopandas.GeoDataFrame
+    gdfg : geopandas.GeoDataFrame
         The GeoDataFrame with the geometries per grid-cell.
     """
     if ml is None and ix is None:
         raise (Exception("Either specify ml or ix"))
 
     if ml is not None:
         if isinstance(ml, xr.Dataset):
@@ -1253,27 +1309,29 @@
                 raise NotImplementedError(
                     "please use a model dataset instead of a model"
                 )
 
     if ix is None:
         ix = flopy.utils.GridIntersect(modelgrid, method=method)
     shps = []
-    geometry = gdf._geometry_column_name
+    geometry = gdf.geometry.name
     for _, shp in tqdm(gdf.iterrows(), total=gdf.shape[0], desc=desc):
         r = ix.intersect(shp[geometry], **kwargs)
         for i in range(r.shape[0]):
             shpn = shp.copy()
             shpn["cellid"] = r["cellids"][i]
             shpn[geometry] = r["ixshapes"][i]
             if shp[geometry].geom_type == "LineString":
                 shpn["length"] = r["lengths"][i]
             elif shp[geometry].geom_type == "Polygon":
                 shpn["area"] = r["areas"][i]
             shps.append(shpn)
-    return gpd.GeoDataFrame(shps, geometry=geometry)
+    gdfg = gpd.GeoDataFrame(shps, geometry=geometry, crs=gdf.crs)
+    gdfg.index.name = gdf.index.name
+    return gdfg
 
 
 def get_thickness_from_topbot(top, bot):
     """get thickness from data arrays with top and bots.
 
     Parameters
     ----------
@@ -1286,34 +1344,34 @@
     Returns
     -------
     thickness : xr.DataArray
         raster with thickness of each cell. dimensions should be (layer, y,x)
         or (layer, icell2d).
     """
     warnings.warn(
-        "The method get_thickness_from_topbot is deprecated. Please use calculate_thickness instead",
+        "The method get_thickness_from_topbot is deprecated. Please use nlmod.layers.calculate_thickness instead",
         DeprecationWarning,
     )
 
     if np.ndim(top) > 2:
         raise NotImplementedError("function works only for 2d top")
 
     # get thickness
     if bot.ndim == 3:
         thickness = util.get_da_from_da_ds(bot, dims=("layer", "y", "x"))
     elif bot.ndim == 2:
         thickness = util.get_da_from_da_ds(bot, dims=("layer", "icell2d"))
     else:
         raise ValueError("function only support structured or vertex gridtypes")
 
-    for lay in range(len(bot)):
+    for lay, botlay in enumerate(bot):
         if lay == 0:
-            thickness[lay] = top - bot[lay]
+            thickness[lay] = top - botlay
         else:
-            thickness[lay] = bot[lay - 1] - bot[lay]
+            thickness[lay] = bot[lay - 1] - botlay
 
     return thickness
 
 
 def get_vertices_arr(ds, modelgrid=None, vert_per_cid=4, epsilon=0, rotated=False):
     """get vertices of a vertex modelgrid from a ds or the modelgrid. Only
     return the 4 corners of each cell and not the corners of adjacent cells
```

### Comparing `nlmod-0.5.1/nlmod/dims/layers.py` & `nlmod-0.5.2/nlmod/dims/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,258 +52,115 @@
                 thickness.attrs["units"] = "m"
             else:
                 thickness.attrs["units"] = ds[bot].units
 
     return thickness
 
 
-def layer_split_top_bot(ds, split_dict, layer="layer", top="top", bot="botm"):
-    """Calculate new tops and bottoms for split layers.
-
-    Parameters
-    ----------
-    ds : xarray.Dataset
-        xarray Dataset containing information about layers
-        (layers, top and bot)
-    split_dict : dict
-        dictionary with index of layers to split as keys and iterable
-        of fractions that add up to 1 to indicate how to split up layer.
-        E.g. {0: [0.25, 0.75]} will split layer 0 into 2 layers, with first
-        layer equal to 0.25 of original thickness and second layer 0.75 of
-        original thickness.
-    layer : str, optional
-        name of layer dimension, by default 'layer'
-    top : str, optional
-        name of data variable containing top of layers, by default 'top'
-    bot : str, optional
-        name of data variable containing bottom of layers, by default 'botm'
-
-    Returns
-    -------
-    new_top, new_bot : xarray.DataArrays
-        DataArrays containing new tops and bottoms after splitting layers.
-    reindexer : OrderedDict
-        dictionary mapping new to old layer indices.
-    """
-
-    # calculate thickness
-    thickness = calculate_thickness(ds, top=top, bot=bot)
-
-    # check if top is 2d or 3d
-    top3d = ds[top].ndim == ds[bot].ndim
-
-    # calculate new number of layers
-    new_nlay = (
-        ds[layer].size + sum((len(sf) for sf in split_dict.values())) - len(split_dict)
-    )
-
-    # create new DataArrays for storing new top/bot
-    new_bot = xr.DataArray(
-        data=np.nan,
-        dims=["layer", "y", "x"],
-        coords={"layer": np.arange(new_nlay), "y": ds.y.data, "x": ds.x.data},
-    )
-    new_top = xr.DataArray(
-        data=np.nan,
-        dims=["layer", "y", "x"],
-        coords={"layer": np.arange(new_nlay), "y": ds.y.data, "x": ds.x.data},
-    )
-
-    # dict to keep track of old and new layer indices
-    reindexer = OrderedDict()
-
-    j = 0  # new layer index
-    isplit = 0  # split layer index
-
-    # loop over original layers
-    for i in range(ds[layer].size):
-        # check if layer should be split
-        if i in split_dict:
-            # set new top based on old top
-            if top3d:
-                new_top.data[j] = ds[top].data[i]
-            else:
-                if i == 0:
-                    new_top.data[j] = ds[top].data
-                else:
-                    new_top.data[j] = ds[bot].data[i - 1]
-
-            # get split factors
-            sf = split_dict[i]
-
-            # check if factors add up to 1
-            if np.sum(sf) != 1.0:
-                raise ValueError("Sum of split factors for layer must equal 1.0!")
-            logger.debug(
-                f"{i}: Split layer {i} into {len(sf)} layers with fractions: {sf}"
-            )
-
-            # loop over split factors
-            for isf, factor in enumerate(sf):
-                logger.debug(
-                    f"  - {isf}: Calculate new top/bot for new layer index {j}"
-                )
-
-                # calculate new bot and new top
-                new_bot.data[j] = new_top.data[j] - (factor * thickness[i])
-                new_top.data[j + 1] = new_bot.data[j]
-
-                # store new and old layer index
-                reindexer[j] = i
-
-                # increase new index
-                j += 1
-
-            # go to next layer to split
-            isplit += 1
-
-        # no split, remap old layer to new layer index
-        else:
-            logger.debug(f"{i:2d}: No split: map layer {i} to new layer index {j}")
-            if top3d:
-                new_top.data[j] = ds[top].data[i]
-            else:
-                if i == 0:
-                    new_top.data[j] = ds[top].data.squeeze()
-                else:
-                    new_top.data[j] = ds[bot].data[i - 1]
-
-            new_bot.data[j] = ds[bot].data[i]
-            reindexer[j] = i
-            j += 1
-
-    return new_top, new_bot, reindexer
-
-
-def fill_data_split_layers(da, reindexer):
-    """Fill data for split layers with values from original layer.
-
-    Parameters
-    ----------
-    da : xarray.DataArray or numpy.ndarray
-        original array with data
-    reindexer : dict
-        dictionary containing mapping between new layer index and
-        original layer index.
-
-    Returns
-    -------
-    da_new : xarray.DataArray or numpy.ndarray
-        array with filled data for split layers
-    """
-    if isinstance(da, xr.DataArray):
-        da_new = xr.DataArray(
-            data=np.nan,
-            dims=["layer", "y", "x"],
-            coords={
-                "layer": np.arange(list(reindexer.keys())[-1] + 1),
-                "y": da["y"],
-                "x": da["x"],
-            },
-        )
-        for k, v in reindexer.items():
-            da_new.data[k] = da.data[v]
-    elif isinstance(da, np.ndarray):
-        da_new = np.zeros((list(reindexer.keys())[-1] + 1), *da.shape[1:])
-        for k, v in reindexer.items():
-            da_new[k] = da[v]
-    else:
-        raise TypeError(f"Cannot fill type: '{type(da)}'!")
-    return da_new
-
-
 def split_layers_ds(
-    ds, split_dict, layer="layer", top="top", bot="botm", kh="kh", kv="kv"
+    ds, split_dict, layer="layer", top="top", bot="botm", return_reindexer=False
 ):
     """Split layers based in Dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
-        xarray Dataset containing information about layers
-        (layers, top and bot)
+        xarray Dataset containing information about layers (layers, top and bot)
     split_dict : dict
-        dictionary with index of layers to split as keys and iterable
-        of fractions that add up to 1 to indicate how to split up layer.
-        E.g. {0: [0.25, 0.75]} will split layer 0 into 2 layers, with first
-        layer equal to 0.25 of original thickness and second layer 0.75 of
-        original thickness.
+        dictionary with name (string) or index (integer) of layers to split as keys.
+        There are two options for the values of the dictionary, to indicate how to split
+        up layer: an iterable of factors. E.g. {'BXk1': [1, 3]} will split layer 'BXk1'
+        into 2 layers, with the first layer equal to 0.25 of the original thickness and
+        the second layer equal to 0.75 of the original thickness.
+        The second option would be to set the value to the number of layers to split the
+        layer into, e.g. {'BXk1': 2}, which is equal to {'BXk1': [0.5, 0.5]}.
     layer : str, optional
         name of layer dimension, by default 'layer'
     top : str, optional
         name of data variable containing top of layers, by default 'top'
     bot : str, optional
         name of data variable containing bottom of layers, by default 'botm'
-    kh : str, opti
-        name of data variable containg horizontal hydraulic conductivity,
-        by default 'kh'
-    kv : str, optional
-        name of data variable containg vertical hydraulic conductivity,
-        by default 'kv'
+    return_reindexer : bool, optional
+        Return a OrderedDict that can be used to reindex variables from the original
+        layer-dimension to the new layer-dimension when True. The default is False.
 
     Returns
     -------
-    ds_split : xarray.Dataset
-        Dataset with new tops and bottoms taking into account split layers,
-        and filled data for hydraulic conductivities.
+    ds : xarray.Dataset
+        Dataset with new tops and bottoms taking into account split layers, and filled
+        data for other variables.
     """
 
-    parsed_dv = set([top, bot, kh, kv])
-
-    dropped_dv = set(ds.data_vars.keys()) - parsed_dv
-    if len(dropped_dv) > 0:
-        logger.warning(f"Following data variables will be dropped: {dropped_dv}")
-
-    # calculate new tops/bots
-    logger.info("Calculating new layer tops and bottoms...")
+    layers = list(ds.layer.data)
 
-    new_top, new_bot, reindexer = layer_split_top_bot(
-        ds, split_dict, layer=layer, top=top, bot=bot
-    )
-
-    # fill kh/kv
-    logger.info(f"Fill value '{kh}' for split layers with value original layer.")
-    da_kh = fill_data_split_layers(ds["kh"], reindexer)
-    logger.info(f"Fill value '{kv}' for split layers with value original layer.")
-    da_kv = fill_data_split_layers(ds["kv"], reindexer)
+    # do some input-checking on split_dict
+    for lay0 in list(split_dict):
+        if isinstance(lay0, int) & (ds.layer.dtype != int):
+            # if layer is an integer, and ds.layer is not of integer type
+            # replace lay0 by the name of the layer
+            split_dict[layers[lay0]] = split_dict.pop(lay0)
+            lay0 = layers[lay0]
+        if isinstance(split_dict[lay0], int):
+            # If split_dict[lay0] is of integer type
+            # split the layer in evenly thick layers
+            split_dict[lay0] = [1 / split_dict[lay0]] * split_dict[lay0]
+        else:
+            # make sure the fractions add up to 1
+            split_dict[lay0] = split_dict[lay0] / np.sum(split_dict[lay0])
 
-    # get new layer names
-    layer_names = []
-    for j, i in reindexer.items():
-        layercode = ds[layer].data[i]
+    logger.info(f"Splitting layers {list(split_dict)}")
 
-        if layercode in layer_names:
-            if isinstance(layercode, str):
-                ilay = (
-                    np.sum([1 for ilay in layer_names if ilay.startswith(layercode)])
-                    + 1
+    layers_org = layers.copy()
+    # add extra layers (keep the original ones for now, as we will copy data first)
+    for lay0 in split_dict:
+        for i in range(len(split_dict[lay0])):
+            index = layers.index(lay0)
+            layers.insert(index, lay0 + "_" + str(i + 1))
+            layers_org.insert(index, lay0)
+    ds = ds.reindex({"layer": layers})
+
+    # calclate a new top and botm, and fill other variables with original data
+    th = calculate_thickness(ds, top=top, bot=bot)
+    for lay0 in split_dict:
+        th0 = th.loc[lay0]
+        for var in ds:
+            if layer not in ds[var].dims:
+                continue
+            if lay0 == list(split_dict)[0] and var not in [top, bot]:
+                logger.info(
+                    f"Fill values of variable '{var}' of splitted layers with the values from the original layer."
                 )
-                layercode += f"_{ilay}"
-            else:
-                layercode = j
+            ds = _split_var(ds, var, lay0, th0, split_dict[lay0], top, bot)
 
-        layer_names.append(layercode)
+    # drop the original layers
+    ds = ds.drop_sel(layer=list(split_dict))
 
-    # assign new layer names
-    new_top = new_top.assign_coords(layer=layer_names)
-    new_bot = new_bot.assign_coords(layer=layer_names)
-    da_kh = da_kh.assign_coords(layer=layer_names)
-    da_kv = da_kv.assign_coords(layer=layer_names)
+    if return_reindexer:
+        # determine reindexer
+        reindexer = OrderedDict(zip(layers, layers_org))
+        for lay0 in split_dict:
+            reindexer.pop(lay0)
+        return ds, reindexer
+    return ds
 
-    # add reindexer to attributes
-    attrs = ds.attrs.copy()
-    attrs["split_reindexer"] = reindexer
 
-    # create new dataset
-    logger.info("Done! Created new dataset with split layers!")
-    ds_split = xr.Dataset(
-        {top: new_top, bot: new_bot, kh: da_kh, kv: da_kv}, attrs=attrs
-    )
-
-    return ds_split
+def _split_var(ds, var, layer, thickness, fctrs, top, bot):
+    """Internal method to split a variable of one layer in multiple layers"""
+    for i in range(len(fctrs)):
+        name = layer + "_" + str(i + 1)
+        if var == top:
+            # take orignal top and subtract thickness of higher splitted layers
+            ds[var].loc[name] = ds[var].loc[layer] - np.sum(fctrs[:i]) * thickness
+        elif var == bot:
+            # take original bottom and add thickness of lower splitted layers
+            ds[var].loc[name] = ds[var].loc[layer] + np.sum(fctrs[i + 1 :]) * thickness
+        else:
+            # take data from the orignal layer
+            ds[var].loc[name] = ds[var].loc[layer]
+    return ds
 
 
 def layer_combine_top_bot(ds, combine_layers, layer="layer", top="top", bot="botm"):
     """Calculate new tops and bottoms for combined layers.
 
     Parameters
     ----------
@@ -646,15 +503,15 @@
 
     Notes
     -----
     some model dataset, such as regis, also have 'c' and 'kd' values. These
     are ignored at the moment
     """
     warnings.warn(
-        "add_kh_kv_from_ml_layer_to_ds is deprecated. Please use update_ds_from_layer_ds instead.",
+        "add_kh_kv_from_ml_layer_to_ds is deprecated. Please use nlmod.grid.update_ds_from_layer_ds instead.",
         DeprecationWarning,
     )
 
     ds.attrs["anisotropy"] = anisotropy
     ds.attrs["fill_value_kh"] = fill_value_kh
     ds.attrs["fill_value_kv"] = fill_value_kv
 
@@ -782,69 +639,102 @@
 
     mask = (top - botm) > min_thickness
     new_botm = botm.where(mask, top - min_thickness)
     ds = set_layer_botm(ds, layer, new_botm)
     return ds
 
 
-def get_kh_kv(kh_in, kv_in, anisotropy, fill_value_kh=1.0, fill_value_kv=1.0):
+def get_kh_kv(kh, kv, anisotropy, fill_value_kh=1.0, fill_value_kv=0.1, idomain=None):
     """create kh en kv grid data for flopy from existing kh, kv and anistropy
     grids with nan values (typically from REGIS).
 
-    fill kh grid in these steps:
-    1. take kh from kh_in, if kh_in has nan values:
-    2. take kv from kv_in and multiply by anisotropy, if this is nan:
-    3. take fill_value_kh
-
-    fill kv grid in these steps:
-    1. take kv from kv_in, if kv_in has nan values:
-    2. take kh from kh_in and divide by anisotropy, if this is nan:
-    3. take fill_value_kv
+    fill nans in kh grid in these steps:
+    1. take kv and multiply by anisotropy, if this is nan:
+    2. take fill_value_kh
+
+    fill nans in kv grid in these steps:
+    1. take kh and divide by anisotropy, if this is nan:
+    2. take fill_value_kv
 
     Supports structured and vertex grids.
 
     Parameters
     ----------
-    kh_in : np.ndarray
+    kh : xarray.DataArray
         kh from regis with nan values shape(nlay, nrow, ncol) or
         shape(nlay, len(icell2d))
-    kv_in : np.ndarray
+    kv : xarray.DataArray
         kv from regis with nan values shape(nlay, nrow, ncol) or
         shape(nlay, len(icell2d))
     anisotropy : int or float
         factor to calculate kv from kh or the other way around
     fill_value_kh : int or float, optional
-        use this value for kh if there is no data in kh_in, kv_in and
+        use this value for kh if there is no data in kh, kv and
         anisotropy. The default is 1.0.
     fill_value_kv : int or float, optional
-        use this value for kv if there is no data in kv_in, kh_in and
+        use this value for kv if there is no data in kv, kh and
         anisotropy. The default is 1.0.
+    idomain : xarray.DataArray, optional
+        The idomain DataArray, used in log-messages, to report the number of active
+        cells that are filled. When idomain is None, the total number of cells that are
+        filled is reported, and not just the active cells. The default is None.
 
     Returns
     -------
-    kh_out : np.ndarray
+    kh : np.ndarray
         kh without nan values (nlay, nrow, ncol) or shape(nlay, len(icell2d))
-    kv_out : np.ndarray
+    kv : np.ndarray
         kv without nan values (nlay, nrow, ncol) or shape(nlay, len(icell2d))
     """
-    for layer in kh_in.layer.data:
-        if ~np.all(np.isnan(kh_in.loc[layer])):
+    for layer in kh.layer.data:
+        if ~np.all(np.isnan(kh.loc[layer])):
             logger.debug(f"layer {layer} has a kh")
-        elif ~np.all(np.isnan(kv_in.loc[layer])):
+        elif ~np.all(np.isnan(kv.loc[layer])):
             logger.debug(f"layer {layer} has a kv")
         else:
-            logger.debug(f"kv and kh both undefined in layer {layer}")
+            logger.info(f"kv and kh both undefined in layer {layer}")
 
-    kh_out = kh_in.where(~np.isnan(kh_in), kv_in * anisotropy)
-    kh_out = kh_out.where(~np.isnan(kh_out), fill_value_kh)
-
-    kv_out = kv_in.where(~np.isnan(kv_in), kh_in / anisotropy)
-    kv_out = kv_out.where(~np.isnan(kv_out), fill_value_kv)
-
-    return kh_out, kv_out
+    # fill kh by kv * anisotropy
+    msg_suffix = f" of kh by multipying kv by an anisotropy of {anisotropy}"
+    kh = _fill_var(kh, kv * anisotropy, idomain, msg_suffix)
+
+    # fill kv by kh / anisotropy
+    msg_suffix = f" of kv by dividing kh by an anisotropy of {anisotropy}"
+    kv = _fill_var(kv, kh / anisotropy, idomain, msg_suffix)
+
+    # fill kh by fill_value_kh
+    msg_suffix = f" of kh with a value of {fill_value_kh}"
+    if "units" in kh.attrs:
+        msg_suffix = f"{msg_suffix} {kh.units}"
+    kh = _fill_var(kh, fill_value_kh, idomain, msg_suffix)
+
+    # fill kv by fill_value_kv
+    msg_suffix = f" of kv with a value of {fill_value_kv}"
+    if "units" in kv.attrs:
+        msg_suffix = f"{msg_suffix} {kv.units}"
+    kv = _fill_var(kv, fill_value_kv, idomain, msg_suffix)
+
+    return kh, kv
+
+
+def _fill_var(var, by, idomain, msg_suffix=""):
+    mask = np.isnan(var)
+    if isinstance(by, xr.DataArray):
+        mask = mask & (~np.isnan(by))
+    if mask.any():
+        var = var.where(~mask, by)
+        if idomain is not None:
+            mask = mask & (idomain > 0)
+            if mask.any():
+                logger.info(
+                    f"Filling {int(mask.sum())} values in active cells{msg_suffix}"
+                )
+        else:
+            logger.info(f"Filling {int(mask.sum())} values {msg_suffix}")
+    return var
 
 
 def fill_top_bot_kh_kv_at_mask(ds, fill_mask):
     """Fill values in top, bot, kh and kv.
 
     Fill where:
     1. the cell is True in fill_mask
@@ -925,14 +815,15 @@
     # 3
     ds["kh"], ds["kv"] = get_kh_kv(
         ds["kh"],
         ds["kv"],
         anisotropy,
         fill_value_kh=fill_value_kh,
         fill_value_kv=fill_value_kv,
+        idomain=ds["idomain"],
     )
     return ds
 
 
 def fill_top_and_bottom(ds):
     """Remove Nans in botm variable, and change top from 3d to 2d if needed."""
     if "layer" in ds["top"].dims:
@@ -959,19 +850,21 @@
     ds : xr.Dataset
         The model Dataset.
     remove_nan_layers : bool, optional
         Removes layers which only contain inactive cells. The default is True.
 
     Returns
     -------
-    ds : TYPE
-        DESCRIPTION.
+    ds : xr.Dataset
+        Dataset with added idomain-variable.
     """
     # set idomain with a default of -1 (pass-through)
     ds["idomain"] = xr.full_like(ds["botm"], -1, int)
+    # drop attributes inherited from botm
+    ds["idomain"].attrs.clear()
     # set idomain of cells  with a positive thickness to 1
     thickness = calculate_thickness(ds)
     ds["idomain"].data[thickness.data > 0.0] = 1
     # set idomain to 0 in the inactive part of the model
     if "active" in ds:
         ds["idomain"] = ds["idomain"].where(ds["active"], 0)
     if remove_nan_layers:
@@ -984,15 +877,15 @@
 
 def get_first_active_layer(ds, **kwargs):
     """Get the first active layer in each cell from a model ds.
 
     Parameters
     ----------
     ds : xr.DataSet
-        DESCRIPTION.
+        Model Dataset with a variable idomain.
     **kwargs : dict
         Kwargs are passed on to get_first_active_layer_from_idomain.
 
     Returns
     -------
     first_active_layer : xr.DataArray
         raster in which each cell has the zero based number of the first
@@ -1074,7 +967,72 @@
             mask2 = (thick == 0) * mask * (idomain[ilay - 1] != 0)
             idomain[ilay] = xr.where(mask2, -1, idomain[ilay])
 
             mask3 = (thick != 0) * mask
             idomain[ilay] = xr.where(mask3, 1, idomain[ilay])
 
     return idomain
+
+
+def aggregate_by_weighted_mean_to_ds(ds, source_ds, var_name):
+    """Aggregate source data to a model dataset using the weighted mean.
+
+    The weighted average per model layer is calculated for the variable in the
+    source dataset. The datasets must have the same grid.
+
+    Parameters
+    ----------
+    ds : xr.Dataset
+        model dataset containing layer information (x, y, top, botm)
+    source_ds : xr.Dataset
+        dataset containing x, y, top, botm and a data variable to aggregate.
+    var_name : str
+        name of the data array to aggregate
+
+    Returns
+    -------
+    da : xarray.DataArray
+        data array containing aggregated values from source dataset
+
+    Raises
+    ------
+    ValueError
+        if source_ds does not have a layer dimension
+
+    See also
+    --------
+    nlmod.read.geotop.aggregate_to_ds
+
+    """
+    msg = "x and/or y coordinates do not match between 'ds' and 'source_ds'"
+    assert (ds.x == source_ds.x).all() and (ds.y == source_ds.y).all(), msg
+
+    if "layer" in ds["top"].dims:
+        # make sure there is no layer dimension in top
+        ds["top"] = ds["top"].max(dim="layer")
+
+    if "layer" not in source_ds.dims:
+        raise ValueError("Requires 'source_ds' to have a 'layer' dimension!")
+
+    agg_ar = []
+
+    for ilay in range(len(ds.layer)):
+        if ilay == 0:
+            top = ds["top"]
+        else:
+            top = ds["botm"][ilay - 1].drop_vars("layer")
+        bot = ds["botm"][ilay].drop_vars("layer")
+
+        s_top = source_ds.top
+        s_bot = source_ds.bottom
+        s_top = s_top.where(s_top < top, top)
+        s_top = s_top.where(s_top > bot, bot)
+        s_bot = s_bot.where(s_bot < top, top)
+        s_bot = s_bot.where(s_bot > bot, bot)
+        s_thk = s_top - s_bot
+
+        agg_ar.append(
+            (s_thk * source_ds[var_name]).sum("layer")
+            / s_thk.where(~np.isnan(source_ds[var_name])).sum("layer")
+        )
+
+    return xr.concat(agg_ar, ds.layer)
```

### Comparing `nlmod-0.5.1/nlmod/dims/rdp.py` & `nlmod-0.5.2/nlmod/dims/rdp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/dims/resample.py` & `nlmod-0.5.2/nlmod/dims/resample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """Created on Fri Apr  2 15:08:50 2021.
 
 @author: oebbe
 """
 import logging
 import numbers
+
 import numpy as np
 import rasterio
 import xarray as xr
 from affine import Affine
 from scipy.interpolate import griddata
 from scipy.spatial import cKDTree
 from shapely.affinity import affine_transform
@@ -381,22 +382,19 @@
         The model dataset with coordinates x and y.
     method : str, optional
         The interpolation method, see griddata. The default is "nearest".
 
     Returns
     -------
     xarray.DataArray
-        THe structured DataArray, with coordinates 'x' and 'y'
+        A DataArray, with the same gridtype as ds.
     """
 
-    if hasattr(ds.attrs, "gridtype") and ds.gridtype == "vertex":
-        raise (Exception("Resampling from vertex da to vertex ds not supported"))
-
     if "icell2d" not in da.dims:
-        return da
+        return structured_da_to_ds(da, ds, method=method)
     points = np.array((da.x.data, da.y.data)).T
 
     if "gridtype" in ds.attrs and ds.gridtype == "vertex":
         if len(da.dims) == 1:
             xi = list(zip(ds.x.values, ds.y.values))
             z = griddata(points, da.values, xi, method=method)
             coords = {"icell2d": ds.icell2d}
@@ -458,81 +456,106 @@
     method : string or rasterio.enums.Resampling, optional
         The method to resample the DataArray. Possible values are "linear",
         "nearest" and all the values in rasterio.enums.Resampling. These values
         can be provided as a string ('average') or as an attribute of
         rasterio.enums.Resampling (rasterio.enums.Resampling.average). When
         method is 'linear' or 'nearest' da.interp() is used. Otherwise
         da.rio.reproject_match() is used. The default is "average".
+    nodata : float, optional
+        THe nodata value in input and output. THe default is np.NaN.
 
     Returns
     -------
     da_out : xarray.DataArray
         The resampled DataArray
     """
     has_rotation = "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0
     if method in ["linear", "nearest"] and not has_rotation:
         kwargs = {}
         if ds.gridtype == "structured":
             kwargs["fill_value"] = "extrapolate"
+
         da_out = da.interp(x=ds.x, y=ds.y, method=method, kwargs=kwargs)
-        return da_out
+
+        # some stuff is added by the interp function that should not be there
+        added_coords = set(da_out.coords) - set(ds.coords)
+        return da_out.drop_vars(added_coords)
     if isinstance(method, rasterio.enums.Resampling):
         resampling = method
     else:
         if hasattr(rasterio.enums.Resampling, method):
             resampling = getattr(rasterio.enums.Resampling, method)
         else:
             raise (Exception(f"Unknown resample method: {method}"))
     # fill crs if it is None for da or ds
     if ds.rio.crs is None and da.rio.crs is None:
+        logger.info("No crs in da and ds. Assuming ds and da are both in EPSG:28992")
         ds = ds.rio.write_crs(28992)
         da = da.rio.write_crs(28992)
     elif ds.rio.crs is None:
+        logger.info(f"No crs in ds. Setting crs equal to da: {da.rio.crs}")
         ds = ds.rio.write_crs(da.rio.crs)
     elif da.rio.crs is None:
+        logger.info(f"No crs in da. Setting crs equal to ds: {ds.rio.crs}")
         da = da.rio.write_crs(ds.rio.crs)
     if ds.gridtype == "structured":
-        if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
-            affine = get_affine(ds)
-            # save crs as it is deleted by write_transform...
-            crs = ds.rio.crs
-            ds = ds.rio.write_transform(affine)
-            ds = ds.rio.write_crs(crs)
-        da_out = da.rio.reproject_match(ds, resampling, nodata=nodata)
-
+        da_out = da.rio.reproject(
+            dst_crs=ds.rio.crs,
+            shape=(len(ds.y), len(ds.x)),
+            transform=get_affine(ds),
+            resampling=resampling,
+            nodata=nodata,
+        )
+        if "x" not in da_out.coords or "y" not in da_out.coords:
+            # when grid-rotation is used, there are no x and y in coords
+            da_out = da_out.assign_coords(x=ds.x, y=ds.y)
     elif ds.gridtype == "vertex":
         # assume the grid is a quadtree grid, where cells are refined by splitting them
         # in 4
+        # We perform a reproject-match for every refinement-level
         dims = list(da.dims)
         dims.remove("y")
         dims.remove("x")
         dims.append("icell2d")
         da_out = get_da_from_da_ds(ds, dims=tuple(dims), data=nodata)
         for area in np.unique(ds["area"]):
             dx = dy = np.sqrt(area)
             x, y = get_xy_mid_structured(ds.extent, dx, dy)
-            da_temp = xr.DataArray(nodata, dims=["y", "x"], coords=dict(x=x, y=y))
-            if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
-                affine = get_affine(ds)
-                da_temp = da_temp.rio.write_transform(affine, inplace=True)
-            # make sure da_temp has a crs if da has a crs
-            da_temp = da_temp.rio.write_crs(da.rio.crs)
-            da_temp = da.rio.reproject_match(da_temp, resampling, nodata=nodata)
+            da_temp = da.rio.reproject(
+                dst_crs=ds.rio.crs,
+                shape=(len(y), len(x)),
+                transform=get_affine(ds, sx=dx, sy=-dy),
+                resampling=resampling,
+                nodata=nodata,
+            )
+            if "x" not in da_temp.coords or "y" not in da_temp.coords:
+                # when grid-rotation is used, there are no x and y in coords
+                da_temp = da_temp.assign_coords(x=x, y=y)
+
             mask = ds["area"] == area
             da_out.loc[dict(icell2d=mask)] = da_temp.sel(
                 y=ds["y"][mask], x=ds["x"][mask]
             )
     else:
         raise (Exception(f"Gridtype {ds.gridtype} not supported"))
 
-    # somehow the spatial_ref (jarkus) and band (ahn) coordinates are added by the reproject_match function
-    if "spatial_ref" in da_out.coords:
-        da_out = da_out.drop_vars("spatial_ref")
-        if "grid_mapping" in da_out.encoding:
-            del da_out.encoding["grid_mapping"]
+    # some stuff is added by the reproject_match function that should not be there
+    added_coords = set(da_out.coords) - set(ds.coords)
+    da_out = da_out.drop_vars(added_coords)
+
+    if "grid_mapping" in da_out.encoding:
+        del da_out.encoding["grid_mapping"]
+
+    # remove the long_name, standard_name and units attributes of the x and y coordinates
+    for coord in ["x", "y"]:
+        if coord not in da_out.coords:
+            continue
+        for name in ["long_name", "standard_name", "units", "axis"]:
+            if name in da_out[coord].attrs.keys():
+                del da_out[coord].attrs[name]
 
     return da_out
 
 
 def extent_to_polygon(extent):
     """Generate a shapely Polygon from an extent ([xmin, xmax, ymin, ymax])"""
     nw = (extent[0], extent[2])
@@ -598,23 +621,29 @@
     angrot = attrs["angrot"]
     return Affine.rotation(-angrot) * Affine.translation(-xorigin, -yorigin)
 
 
 def get_affine(ds, sx=None, sy=None):
     """Get the affine-transformation, from pixel to real-world coordinates."""
     attrs = _get_attrs(ds)
-    xorigin = attrs["xorigin"]
-    yorigin = attrs["yorigin"]
-    angrot = -attrs["angrot"]
-    # xorigin and yorigin represent the lower left corner, while for the transform we
-    # need the upper left
-    dy = attrs["extent"][3] - attrs["extent"][2]
-    xoff = xorigin + dy * np.sin(angrot * np.pi / 180)
-    yoff = yorigin + dy * np.cos(angrot * np.pi / 180)
-
     if sx is None:
         sx = attrs["delr"]
     if sy is None:
         sy = -attrs["delc"]
-    return (
-        Affine.translation(xoff, yoff) * Affine.scale(sx, sy) * Affine.rotation(angrot)
-    )
+    if "angrot" in attrs:
+        xorigin = attrs["xorigin"]
+        yorigin = attrs["yorigin"]
+        angrot = -attrs["angrot"]
+        # xorigin and yorigin represent the lower left corner, while for the transform we
+        # need the upper left
+        dy = attrs["extent"][3] - attrs["extent"][2]
+        xoff = xorigin + dy * np.sin(angrot * np.pi / 180)
+        yoff = yorigin + dy * np.cos(angrot * np.pi / 180)
+        return (
+            Affine.translation(xoff, yoff)
+            * Affine.scale(sx, sy)
+            * Affine.rotation(angrot)
+        )
+    else:
+        xoff = attrs["extent"][0]
+        yoff = attrs["extent"][3]
+        return Affine.translation(xoff, yoff) * Affine.scale(sx, sy)
```

### Comparing `nlmod-0.5.1/nlmod/dims/time.py` & `nlmod-0.5.2/nlmod/dims/time.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/gis.py` & `nlmod-0.5.2/nlmod/gis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 
 import geopandas as gpd
 import numpy as np
 
-from .dims.resample import get_affine_mod_to_world
 from .dims.grid import polygons_from_model_ds
+from .dims.resample import get_affine_mod_to_world
 
 logger = logging.getLogger(__name__)
 
 
 def vertex_da_to_gdf(model_ds, data_variables, polygons=None, dealing_with_time="mean"):
     """Convert one or more DataArrays from a vertex model dataset to a
     Geodataframe.
@@ -301,30 +301,32 @@
         return fname_gpkg
     else:
         return fnames
 
 
 def ds_to_ugrid_nc_file(
     model_ds,
-    fname,
+    fname=None,
     variables=None,
     dummy_var="mesh_topology",
     xv="xv",
     yv="yv",
     face_node_connectivity="icvert",
 ):
     """Save a model dataset to a UGRID NetCDF file, so it can be opened as a
     Mesh Layer in qgis.
 
     Parameters
     ----------
     model_ds : xr.DataSet
-        xarray with model data
-    fname : str
-        filename of the UGRID NetCDF-file, preferably with the extension .nc.
+        xarray Dataset with model data
+    fname : str, optional
+        filename of the UGRID NetCDF-file, preferably with the extension .nc. When fname
+        is None,only a ugird-ready Dataset is created, without saving this Dataset to
+        file. The defaults is None.
     variables : str or list of str, optional
         THe variables to be saved in the NetCDF file. The default is None,
         which means all variables will be saved in the file.
     dummy_var : str, optional
         The name of the new dummy-variable that contains the gridinformation in
         its attributes. The default is 'mesh_topology'.
     xv : str, optional
@@ -394,33 +396,49 @@
         if np.issubdtype(ds[var].dtype, np.datetime64):
             ds[var].encoding["dtype"] = np.float64
 
     # Convert boolean layers to integer and int64 to int32
     for var in variables:
         if np.issubdtype(ds[var].dtype, bool):
             ds[var].encoding["dtype"] = np.int
-        if np.issubdtype(ds[var].dtype, str):
+        elif np.issubdtype(ds[var].dtype, str) or np.issubdtype(ds[var].dtype, object):
             # convert the string to an index of unique strings
-            index = np.unique(model_ds[var], return_inverse=True)[1]
+            index = np.unique(ds[var], return_inverse=True)[1]
             ds[var] = ds[var].dims, index
         if np.issubdtype(ds[var].dtype, np.int64):
             ds[var].encoding["dtype"] = np.int32
 
     # Breaks down variables with a layer dimension into separate variables.
-    # Copied from imod-python.
-    for var in variables:
-        if "layer" in ds[var].dims:
-            stacked = ds[var]
-            ds = ds.drop_vars(var)
-            for layer in stacked["layer"].values:
-                name = f"{var}_layer_{layer}"
-                ds[name] = stacked.sel(layer=layer, drop=True)
-                variables.append(name)
-            variables.remove(var)
-    if "layer" in ds.coords:
-        ds = ds.drop_vars("layer")
+    ds, variables = _break_down_dimension(ds, variables, "layer")
+    # Breaks down variables with a time dimension into separate variables.
+    ds, variables = _break_down_dimension(ds, variables, "time")
 
     # only keep the selected variables
     ds = ds[variables + [dummy_var, xv, yv, face_node_connectivity]]
-    # and save to file
-    ds.to_netcdf(fname)
+    if fname is not None:
+        # and save to file
+        ds.to_netcdf(fname)
     return ds
+
+
+def _break_down_dimension(ds, variables, dim):
+    # Copied and altered from imod-python.
+    keep_vars = []
+    for var in variables:
+        if dim in ds[var].dims:
+            stacked = ds[var]
+            for value in stacked[dim].values:
+                name = f"{var}_{value}"
+                ds[name] = stacked.sel({dim: value}, drop=True)
+                if "long_name" in ds[name].attrs:
+                    long_name = ds[name].attrs["long_name"]
+                    ds[name].attrs["long_name"] = f"{long_name} {value}"
+                if "standard_name" in ds[name].attrs:
+                    standard_name = ds[name].attrs["standard_name"]
+                    ds[name].attrs["standard_name"] = f"{standard_name}_{value}"
+                keep_vars.append(name)
+        else:
+            keep_vars.append(var)
+    if dim in ds.coords:
+        ds = ds.drop_vars(dim)
+
+    return ds, keep_vars
```

### Comparing `nlmod-0.5.1/nlmod/gwf/gwf.py` & `nlmod-0.5.2/nlmod/gwf/gwf.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ..dims import grid
 from ..sim import ims, sim, tdis
 from . import recharge
 
 logger = logging.getLogger(__name__)
 
 
-def gwf(ds, sim, **kwargs):
+def gwf(ds, sim, under_relaxation=False, **kwargs):
     """create groundwater flow model from the model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data. Should have the dimension 'time' and the
         attributes: model_name, mfversion, model_ws, time_units, start,
@@ -37,44 +37,77 @@
 
     # start creating model
     logger.info("creating modflow GWF")
 
     # Create the Flopy groundwater flow (gwf) model object
     model_nam_file = f"{ds.model_name}.nam"
 
+    if "newtonoptions" in kwargs:
+        newtonoptions = kwargs.pop("newtonoptions")
+    elif under_relaxation:
+        newtonoptions = "under_relaxation"
+    else:
+        newtonoptions = None
+
     gwf = flopy.mf6.ModflowGwf(
-        sim, modelname=ds.model_name, model_nam_file=model_nam_file, **kwargs
+        sim,
+        modelname=ds.model_name,
+        model_nam_file=model_nam_file,
+        newtonoptions=newtonoptions,
+        **kwargs,
     )
 
     return gwf
 
 
 def dis(ds, gwf, length_units="METERS", pname="dis", **kwargs):
     """get discretisation package from the model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
-        groundwaterflow object.
+        groundwaterflow object
+    length_units : str, optional
+        length unit. The default is 'METERS'.
+    pname : str, optional
+        package name
+
+    Returns
+    -------
+    dis : flopy ModflowGwfdis
+        discretisation package.
+    """
+    return _dis(ds, gwf, length_units, pname, **kwargs)
+
+
+def _dis(ds, model, length_units="METERS", pname="dis", **kwargs):
+    """get discretisation package from the model dataset.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        dataset with model data.
+    model : flopy ModflowGwf or flopy ModflowGwt
+        groundwaterflow or groundwater transport object
     length_units : str, optional
         length unit. The default is 'METERS'.
     pname : str, optional
         package name
 
     Returns
     -------
-    dis : TYPE
+    dis : flopy ModflowGwfdis or flopy ModflowGwtdis
         discretisation package.
     """
     logger.info("creating modflow DIS")
 
     if ds.gridtype == "vertex":
-        return disv(ds, gwf, length_units=length_units)
+        return disv(ds, model, length_units=length_units)
 
     # check attributes
     for att in ["delr", "delc"]:
         if att in ds.attrs:
             if isinstance(ds.attrs[att], np.float32):
                 ds.attrs[att] = float(ds.attrs[att])
 
@@ -83,55 +116,99 @@
         yorigin = ds.attrs["yorigin"]
         angrot = ds.attrs["angrot"]
     else:
         xorigin = ds.extent[0]
         yorigin = ds.extent[2]
         angrot = 0.0
 
-    dis = flopy.mf6.ModflowGwfdis(
-        gwf,
-        pname=pname,
-        length_units=length_units,
-        xorigin=xorigin,
-        yorigin=yorigin,
-        angrot=angrot,
-        nlay=ds.dims["layer"],
-        nrow=ds.dims["y"],
-        ncol=ds.dims["x"],
-        delr=ds["delr"].values if "delr" in ds else ds.delr,
-        delc=ds["delc"].values if "delc" in ds else ds.delc,
-        top=ds["top"].data,
-        botm=ds["botm"].data,
-        idomain=ds["idomain"].data,
-        filename=f"{ds.model_name}.dis",
-        **kwargs,
-    )
+    if model.model_type == "gwf6":
+        dis = flopy.mf6.ModflowGwfdis(
+            model,
+            pname=pname,
+            length_units=length_units,
+            xorigin=xorigin,
+            yorigin=yorigin,
+            angrot=angrot,
+            nlay=ds.dims["layer"],
+            nrow=ds.dims["y"],
+            ncol=ds.dims["x"],
+            delr=ds["delr"].values if "delr" in ds else ds.delr,
+            delc=ds["delc"].values if "delc" in ds else ds.delc,
+            top=ds["top"].data,
+            botm=ds["botm"].data,
+            idomain=ds["idomain"].data,
+            filename=f"{ds.model_name}.dis",
+            **kwargs,
+        )
+    elif model.model_type == "gwt6":
+        dis = flopy.mf6.ModflowGwtdis(
+            model,
+            pname=pname,
+            length_units=length_units,
+            xorigin=xorigin,
+            yorigin=yorigin,
+            angrot=angrot,
+            nlay=ds.dims["layer"],
+            nrow=ds.dims["y"],
+            ncol=ds.dims["x"],
+            delr=ds["delr"].values if "delr" in ds else ds.delr,
+            delc=ds["delc"].values if "delc" in ds else ds.delc,
+            top=ds["top"].data,
+            botm=ds["botm"].data,
+            idomain=ds["idomain"].data,
+            filename=f"{ds.model_name}_gwt.dis",
+            **kwargs,
+        )
+    else:
+        raise ValueError("Unknown model type.")
 
     return dis
 
 
 def disv(ds, gwf, length_units="METERS", pname="disv", **kwargs):
     """get discretisation vertices package from the model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
-    gwf : flopy ModflowGwf
-        groundwaterflow object.
+    model : flopy ModflowGwf
+        groundwater flow object.
     length_units : str, optional
         length unit. The default is 'METERS'.
     pname : str, optional
         package name
 
     Returns
     -------
     disv : flopy ModflowGwfdisv
         disv package
     """
+    return _disv(ds, gwf, length_units, pname, **kwargs)
+
+
+def _disv(ds, model, length_units="METERS", pname="disv", **kwargs):
+    """get discretisation vertices package from the model dataset.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        dataset with model data.
+    model : flopy ModflowGwf or flopy ModflowGwt
+        groundwater flow or groundwater transport object.
+    length_units : str, optional
+        length unit. The default is 'METERS'.
+    pname : str, optional
+        package name
+
+    Returns
+    -------
+    disv : flopy ModflowGwfdisv or flopy ModflowGwtdisv
+        disv package
+    """
     logger.info("creating modflow DISV")
 
     if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
         xorigin = ds.attrs["xorigin"]
         yorigin = ds.attrs["yorigin"]
         angrot = ds.attrs["angrot"]
     elif "extent" in ds.attrs.keys():
@@ -141,33 +218,56 @@
     else:
         xorigin = 0.0
         yorigin = 0.0
         angrot = 0.0
 
     vertices = grid.get_vertices_from_ds(ds)
     cell2d = grid.get_cell2d_from_ds(ds)
-    disv = flopy.mf6.ModflowGwfdisv(
-        gwf,
-        idomain=ds["idomain"].data,
-        xorigin=xorigin,
-        yorigin=yorigin,
-        length_units=length_units,
-        angrot=angrot,
-        nlay=len(ds.layer),
-        ncpl=len(ds.icell2d),
-        nvert=len(ds.iv),
-        top=ds["top"].data,
-        botm=ds["botm"].data,
-        vertices=vertices,
-        cell2d=cell2d,
-        pname=pname,
-        **kwargs,
-    )
+    if model.model_type == "gwf6":
+        disv = flopy.mf6.ModflowGwfdisv(
+            model,
+            idomain=ds["idomain"].data,
+            xorigin=xorigin,
+            yorigin=yorigin,
+            length_units=length_units,
+            angrot=angrot,
+            nlay=len(ds.layer),
+            ncpl=len(ds.icell2d),
+            nvert=len(ds.iv),
+            top=ds["top"].data,
+            botm=ds["botm"].data,
+            vertices=vertices,
+            cell2d=cell2d,
+            pname=pname,
+            **kwargs,
+        )
+    elif model.model_type == "gwt6":
+        disv = flopy.mf6.ModflowGwtdisv(
+            model,
+            idomain=ds["idomain"].data,
+            xorigin=xorigin,
+            yorigin=yorigin,
+            length_units=length_units,
+            angrot=angrot,
+            nlay=len(ds.layer),
+            ncpl=len(ds.icell2d),
+            nvert=len(ds.iv),
+            top=ds["top"].data,
+            botm=ds["botm"].data,
+            vertices=vertices,
+            cell2d=cell2d,
+            pname=pname,
+            filename=f"{ds.model_name}_gwt.disv",
+            **kwargs,
+        )
+    else:
+        raise ValueError("Unknown model type.")
+
     if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
-        gwf.modelgrid.set_coord_info(xoff=xorigin, yoff=yorigin, angrot=angrot)
+        model.modelgrid.set_coord_info(xoff=xorigin, yoff=yorigin, angrot=angrot)
 
     return disv
 
 
 def npf(ds, gwf, icelltype=0, save_flows=False, pname="npf", **kwargs):
     """get node property flow package from model dataset.
 
@@ -210,27 +310,29 @@
         save_flows=save_flows,
         **kwargs,
     )
 
     return npf
 
 
-def ghb(ds, gwf, da_name, pname="ghb", **kwargs):
+def ghb(ds, gwf, da_name, pname="ghb", auxiliary=None, **kwargs):
     """get general head boundary from model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
         groundwaterflow object.
     da_name : str
         name of the ghb files in the model dataset.
     pname : str, optional
         package name
+    auxiliary : str or list of str
+        name(s) of data arrays to include as auxiliary data to reclist
 
     Raises
     ------
     ValueError
         raised if gridtype is not structured or vertex.
 
     Returns
@@ -244,30 +346,87 @@
         ds,
         ds[f"{da_name}_cond"] != 0,
         col1=f"{da_name}_peil",
         col2=f"{da_name}_cond",
         first_active_layer=True,
         only_active_cells=False,
         layer=0,
+        aux=auxiliary,
     )
 
     if len(ghb_rec) > 0:
         ghb = flopy.mf6.ModflowGwfghb(
             gwf,
+            auxiliary="CONCENTRATION" if auxiliary is not None else None,
             print_input=True,
             maxbound=len(ghb_rec),
             stress_period_data=ghb_rec,
             save_flows=True,
             pname=pname,
             **kwargs,
         )
+        if (auxiliary is not None) and (ds.transport == 1):
+            ssm_sources = ds.attrs["ssm_sources"]
+            if ghb.name not in ssm_sources:
+                ssm_sources += ghb.name
+                ds.attrs["ssm_sources"] = ssm_sources
         return ghb
 
     else:
-        print("no ghb cells added")
+        logger.warning("no ghb cells added")
+        return None
+
+
+def drn(ds, gwf, da_name, pname="drn", layer=None, **kwargs):
+    """get drain from model dataset.
+
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        dataset with model data.
+    gwf : flopy ModflowGwf
+        groundwaterflow object.
+    da_name : str
+        name of the drn files in the model dataset
+    pname : str, optional
+        package name
+
+    Returns
+    -------
+    drn : flopy ModflowGwfdrn
+        drn package
+    """
+    logger.info("creating modflow DRN")
+
+    first_active_layer = layer is None
+
+    drn_rec = grid.da_to_reclist(
+        ds,
+        ds[f"{da_name}_cond"] != 0,
+        col1=f"{da_name}_peil",
+        col2=f"{da_name}_cond",
+        first_active_layer=first_active_layer,
+        only_active_cells=False,
+        layer=layer,
+    )
+
+    if len(drn_rec) > 0:
+        drn = flopy.mf6.ModflowGwfdrn(
+            gwf,
+            print_input=True,
+            maxbound=len(drn_rec),
+            stress_period_data=drn_rec,
+            save_flows=True,
+            pname=pname,
+            **kwargs,
+        )
+        return drn
+
+    else:
+        logger.warning("no drn cells added")
 
         return None
 
 
 def ic(ds, gwf, starting_head="starting_head", pname="ic", **kwargs):
     """get initial condictions package from model dataset.
 
@@ -322,15 +481,15 @@
     gwf : flopy ModflowGwf
         groundwaterflow object.
     sy : float, optional
         specific yield. The default is 0.2.
     ss : float, optional
         specific storage. The default is 0.000001.
     iconvert : int, optional
-        See description in ModflowGwfsto. The default is 1.
+        See description in ModflowGwfsto. The default is 1 (differs from FloPY).
     save_flows : bool, optional
         value is passed to flopy.mf6.ModflowGwfsto() to determine if flows
         should be saved to the cbb file. Default is False
     pname : str, optional
         package name
 
     Returns
@@ -366,15 +525,17 @@
             steady_state=sts_spd,
             transient=trn_spd,
             **kwargs,
         )
         return sto
 
 
-def chd(ds, gwf, chd="chd", head="starting_head", pname="chd", **kwargs):
+def chd(
+    ds, gwf, chd="chd", head="starting_head", pname="chd", auxiliary=None, **kwargs
+):
     """get constant head boundary at the model's edges from the model dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data.
     gwf : flopy ModflowGwf
@@ -383,33 +544,41 @@
         name of data variable in ds that is 1 for cells with a constant
         head and zero for all other cells. The default is 'chd'.
     head : str, optional
         name of data variable in ds that is used as the head in the chd
         cells. The default is 'starting_head'.
     pname : str, optional
         package name
+    auxiliary : str or list of str
+        name(s) of data arrays to include as auxiliary data to reclist
 
     Returns
     -------
     chd : flopy ModflowGwfchd
         chd package
     """
     logger.info("creating modflow CHD")
 
     # get the stress_period_data
-    chd_rec = grid.da_to_reclist(ds, ds[chd] != 0, col1=head)
+    chd_rec = grid.da_to_reclist(ds, ds[chd] != 0, col1=head, aux=auxiliary)
 
     chd = flopy.mf6.ModflowGwfchd(
         gwf,
+        auxiliary="CONCENTRATION" if auxiliary is not None else None,
         pname=pname,
         maxbound=len(chd_rec),
         stress_period_data=chd_rec,
         save_flows=True,
         **kwargs,
     )
+    if (auxiliary is not None) and (ds.transport == 1):
+        ssm_sources = ds.attrs["ssm_sources"]
+        if chd.name not in ssm_sources:
+            ssm_sources += chd.name
+            ds.attrs["ssm_sources"] = ssm_sources
 
     return chd
 
 
 def surface_drain_from_ds(ds, gwf, resistance, pname="drn", **kwargs):
     """get surface level drain (maaivelddrainage in Dutch) from the model
     dataset.
@@ -501,33 +670,78 @@
 
     # create recharge package
     evt = recharge.model_datasets_to_evt(gwf, ds, pname=pname, **kwargs)
 
     return evt
 
 
-def _set_record(head, budget):
+def _set_record(out, budget, output="head"):
     record = []
-    if isinstance(head, bool):
-        if head:
-            head = "LAST"
+    if isinstance(out, bool):
+        if out:
+            out = "LAST"
         else:
-            head = None
-    if head is not None:
-        record.append(("HEAD", head))
+            out = None
+    if out is not None:
+        record.append((output.upper(), out))
     if isinstance(budget, bool):
         if budget:
             budget = "LAST"
         else:
             budget = None
     if budget is not None:
         record.append(("BUDGET", budget))
     return record
 
 
+def buy(ds, gwf, pname="buy", **kwargs):
+    """create buoyancy package from model dataset.
+    Parameters
+    ----------
+    ds : xarray.Dataset
+        dataset with model data.
+    gwf : flopy ModflowGwf
+        groundwaterflow object.
+    pname : str, optional
+        package name, by default "buy"
+
+    Returns
+    -------
+    buy : flopy ModflowGwfbuy
+        buy package
+
+    Raises
+    ------
+    ValueError
+        if transport is not
+    """
+    if not ds.transport:
+        logger.error("BUY package requires a groundwater transport model")
+        raise ValueError(
+            "BUY package requires a groundwater transport model. "
+            "Set 'transport' to True in model dataset."
+        )
+
+    drhodc = kwargs.pop("drhodc", ds.drhodc)
+    crhoref = kwargs.pop("crhoref", ds.crhoref)
+    denseref = kwargs.pop("denseref", ds.denseref)
+
+    pdata = [(0, drhodc, crhoref, f"{ds.model_name}_gwt", "none")]
+
+    buy = flopy.mf6.ModflowGwfbuy(
+        gwf,
+        denseref=denseref,
+        nrhospecies=len(pdata),
+        packagedata=pdata,
+        pname=pname,
+        **kwargs,
+    )
+    return buy
+
+
 def oc(
     ds,
     gwf,
     save_head=True,
     save_budget=True,
     print_head=False,
     print_budget=False,
@@ -553,31 +767,31 @@
     logger.info("creating modflow OC")
 
     # Create the output control package
     headfile = f"{ds.model_name}.hds"
     head_filerecord = [headfile]
     budgetfile = f"{ds.model_name}.cbc"
     budget_filerecord = [budgetfile]
-    saverecord = _set_record(save_head, save_budget)
-    printrecord = _set_record(print_head, print_budget)
+    saverecord = _set_record(save_head, save_budget, output="head")
+    printrecord = _set_record(print_head, print_budget, output="head")
 
     oc = flopy.mf6.ModflowGwfoc(
         gwf,
         pname=pname,
         saverecord=saverecord,
         printrecord=printrecord,
         head_filerecord=head_filerecord,
         budget_filerecord=budget_filerecord,
         **kwargs,
     )
 
     return oc
 
 
-def ds_to_gwf(ds):
+def ds_to_gwf(ds, complexity="MODERATE", icelltype=0, under_relaxation=False):
     """Generate Simulation and GWF model from model DataSet.
 
     Builds the following packages:
     - sim
     - tdis
     - ims
     - gwf
@@ -602,29 +816,29 @@
     # create simulation
     mf_sim = sim(ds)
 
     # create time discretisation
     tdis(ds, mf_sim)
 
     # create ims
-    ims(mf_sim)
+    ims(mf_sim, complexity=complexity)
 
     # create groundwater flow model
-    mf_gwf = gwf(ds, mf_sim)
+    mf_gwf = gwf(ds, mf_sim, under_relaxation=under_relaxation)
 
     # Create discretization
     if ds.gridtype == "structured":
         dis(ds, mf_gwf)
     elif ds.gridtype == "vertex":
         disv(ds, mf_gwf)
     else:
         raise TypeError("gridtype not recognized.")
 
     # create node property flow
-    npf(ds, mf_gwf)
+    npf(ds, mf_gwf, icelltype=icelltype)
 
     # Create the initial conditions package
     starting_head = "starting_head"
     if starting_head not in ds:
         starting_head = 0.0
     ic(ds, mf_gwf, starting_head=starting_head)
```

### Comparing `nlmod-0.5.1/nlmod/gwf/horizontal_flow_barrier.py` & `nlmod-0.5.2/nlmod/gwf/horizontal_flow_barrier.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
     cells = line2hfb(linestrings, gwf)
 
     spd = []
 
     # hydchr = 1 / 100  # resistance of 100 days
     for icell2d1, icell2d2 in cells:
-
         # TODO: Improve assumption of the thickness between the cells.
         thicki = (thick[:, icell2d1] + thick[:, icell2d2]) / 2
         topi = (tops[:, icell2d1] + tops[:, icell2d2]) / 2
 
         for ilay in range(gwf.disv.nlay.array):
             cellid1 = (ilay, icell2d1)
             cellid2 = (ilay, icell2d2)
@@ -211,15 +210,14 @@
         cellids.append(list(segments.loc[[tuple(seg)]].values[:, 0]))
     return cellids
 
 
 def polygon_to_hfb(
     gdf, ds, column=None, gwf=None, lay=0, hydchr=1 / 100, add_data=False
 ):
-
     if isinstance(gdf, str):
         da = ds[gdf]
     else:
         if column is None:
             column = gdf.index.name
             if column is None:
                 column = "index"
```

### Comparing `nlmod-0.5.1/nlmod/gwf/recharge.py` & `nlmod-0.5.2/nlmod/gwf/recharge.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 
 from ..dims.grid import da_to_reclist
 from ..sim.sim import get_tdis_perioddata
 
 logger = logging.getLogger(__name__)
 
 
-def model_datasets_to_rch(gwf, ds, pname="rch", **kwargs):
+def model_datasets_to_rch(gwf, ds, mask=None, pname="rch", **kwargs):
     """Convert the recharge data in the model dataset to a rch package with
     time series.
 
     Parameters
     ----------
     gwf : flopy.mf6.modflow.mfgwf.ModflowGwf
         groundwater flow model.
     ds : xr.DataSet
         dataset containing relevant model grid information
+    mask : xr.DataArray
+        data array containing mask, recharge is only added where mask is True
     pname : str, optional
         package name. The default is 'rch'.
 
     Returns
     -------
     rch : flopy.mf6.modflow.mfgwfrch.ModflowGwfrch
         recharge package
@@ -35,15 +37,19 @@
     # check for nan values
     if ds["recharge"].isnull().any():
         raise ValueError("please remove nan values in recharge data array")
 
     # get stress period data
     rch_name_arr, rch_unique_dic = _get_unique_series(ds, "recharge", pname)
     ds["rch_name"] = ds["top"].dims, rch_name_arr
-    mask = ds["rch_name"] != ""
+    if mask is not None:
+        mask = (ds["rch_name"] != "") & mask
+    else:
+        mask = ds["rch_name"] != ""
+
     recharge = "rch_name"
 
     spd = da_to_reclist(
         ds,
         mask,
         col1=recharge,
         first_active_layer=True,
```

### Comparing `nlmod-0.5.1/nlmod/gwf/surface_water.py` & `nlmod-0.5.2/nlmod/gwf/surface_water.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
 from shapely.geometry import Polygon
 from shapely.strtree import STRtree
 from tqdm import tqdm
 
-
 from ..dims.grid import gdf_to_grid
 from ..dims.resample import get_extent_polygon
 from ..read import bgt, waterboard
 
 logger = logging.getLogger(__name__)
 
 
@@ -46,15 +45,14 @@
         raise ValueError(f"Missing columns in DataFrame: {missing_cols}")
 
     # Post process intersection result
     gr = gdf.groupby(by="cellid")
     celldata = pd.DataFrame(index=gr.groups.keys())
 
     for cid, group in tqdm(gr, desc="Aggregate surface water data"):
-
         stage, cond, rbot = get_surfacewater_params(group, method, cid=cid, ds=ds)
 
         celldata.loc[cid, "stage"] = stage
         celldata.loc[cid, "cond"] = cond
         celldata.loc[cid, "rbot"] = rbot
         celldata.loc[cid, "area"] = group.area.sum()
 
@@ -77,15 +75,14 @@
         # cond
         c0 = agg_max_area(group, "c0")
         cond = group.area.sum() / c0
         # rbot
         rbot = group["botm"].min()
 
     elif method == "de_lange":
-
         # get additional requisite parameters
         if delange_params is None:
             delange_params = {}
 
         # defaults
         c1 = delange_params.pop("c1", 0.0)
         N = delange_params.pop("N", 1e-3)
@@ -384,20 +381,25 @@
     spd = []
 
     top = ds.top.data
     botm = ds.botm.data
     idomain = ds.idomain.data
     kh = ds.kh.data
 
+    # ignore records without a stage
+    mask = celldata["stage"].isna()
+    if mask.any():
+        logger.warning(f"{mask.sum()} records without a stage ignored")
+        celldata = celldata[~mask]
+
     for cellid, row in tqdm(
         celldata.iterrows(),
         total=celldata.index.size,
         desc=f"Building stress period data {pkg}",
     ):
-
         # check if there is an active layer for this cell
         if ds.gridtype == "vertex":
             idomain_cell = idomain[:, cellid]
             botm_cell = botm[:, cellid]
         elif ds.gridtype == "structured":
             idomain_cell = idomain[:, cellid[0], cellid[1]]
             botm_cell = botm[:, cellid[0], cellid[1]]
@@ -413,17 +415,14 @@
             raise ValueError("Column 'rbot' required for building RIV package!")
         else:
             rbot = np.nan
 
         # stage
         stage = row["stage"]
 
-        if np.isnan(stage):
-            raise ValueError(f"stage is NaN in cell {cellid}")
-
         if (stage < rbot) and np.isfinite(rbot):
             logger.warning(
                 f"WARNING: stage below bottom elevation in {cellid}, "
                 "stage reset to rbot!"
             )
             stage = rbot
 
@@ -549,133 +548,366 @@
         # when the minimum surface level is above the stage
         # or when no stage is available
         # use the minimum surface level
         stage = pd.concat((stage, gdf["ahn_min"]), axis=1).max(axis=1)
     return stage
 
 
-def download_level_areas(gdf, extent=None, config=None):
-    """Download level areas (peilgebieden) of bronhouders."""
+def download_level_areas(gdf, extent=None, config=None, raise_exceptions=True):
+    """
+    Download level areas (peilgebieden) of bronhouders.
+
+    Parameters
+    ----------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, containing the column "bronhouder".
+    extent : list, tuple or np.array
+        Model extent (xmin, xmax, ymin, ymax). When extent is None, all data of the
+        water boards in gdf are downloaded downloaded.
+    config : dict, optional
+        A dictionary with information about the webservices of the water boards. When
+        config is None, it is created with nlmod.read.waterboard.get_configuration().
+        The default is None.
+    raise_exceptions : bool, optional
+        Raises exceptions, mostly caused by a webservice that is offline. When
+        raise_exceptions is False, the error is raised as a warning. The default is
+        True.
+
+    Returns
+    -------
+    la : dict
+        A dictionary with the name of the waterboards as keys and GeoDataFrames with
+        level areas as values.
+
+    """
     if config is None:
         config = waterboard.get_configuration()
     bronhouders = gdf["bronhouder"].unique()
-    pg = {}
+    la = {}
     data_kind = "level_areas"
     for wb in config.keys():
         if config[wb]["bgt_code"] in bronhouders:
             logger.info(f"Downloading {data_kind} for {wb}")
             try:
-                pg[wb] = waterboard.get_data(wb, data_kind, extent)
-                mask = ~pg[wb].is_valid
+                lawb = waterboard.get_data(wb, data_kind, extent)
+                if len(lawb) == 0:
+                    logger.info(f"No {data_kind} for {wb} found within model area")
+                    continue
+                la[wb] = lawb
+                mask = ~la[wb].is_valid
                 if mask.any():
                     logger.warning(
                         f"{mask.sum()} geometries of level areas of {wb} are invalid. Thet are made valid by adding a buffer of 0.0."
                     )
                     # first copy to prevent ValueError: assignment destination is read-only
-                    pg[wb] = pg[wb].copy()
-                    pg[wb].loc[mask, "geometry"] = pg[wb][mask].buffer(0.0)
+                    la[wb] = la[wb].copy()
+                    la[wb].loc[mask, "geometry"] = la[wb][mask].buffer(0.0)
             except Exception as e:
                 if str(e) == f"{data_kind} not available for {wb}":
                     logger.warning(e)
-                else:
+                elif raise_exceptions:
                     raise
-    return pg
+                else:
+                    logger.warning(e)
+    return la
+
+
+def download_watercourses(gdf, extent=None, config=None, raise_exceptions=True):
+    """
+    Download watercourses of bronhouders.
+
+    Parameters
+    ----------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, containing the column "bronhouder".
+    extent : list, tuple or np.array
+        Model extent (xmin, xmax, ymin, ymax). When extent is None, all data of the
+        water boards in gdf are downloaded downloaded.
+    config : dict, optional
+        A dictionary with information about the webservices of the water boards. When
+        config is None, it is created with nlmod.read.waterboard.get_configuration().
+        The default is None.
+    raise_exceptions : bool, optional
+        Raises exceptions, mostly caused by a webservice that is offline. When
+        raise_exceptions is False, the error is raised as a warning. The default is
+        True.
 
+    Returns
+    -------
+    wc : dict
+        A dictionary with the name of the waterboards as keys and GeoDataFrames with
+        watercourses as values.
 
-def download_watercourses(gdf, extent=None, config=None):
-    """Download watercourses of bronhouders."""
+    """
     if config is None:
         config = waterboard.get_configuration()
     bronhouders = gdf["bronhouder"].unique()
     wc = {}
     data_kind = "watercourses"
     for wb in config.keys():
         if config[wb]["bgt_code"] in bronhouders:
             logger.info(f"Downloading {data_kind} for {wb}")
             try:
-                wc[wb] = waterboard.get_data(wb, data_kind, extent)
+                wcwb = waterboard.get_data(wb, data_kind, extent)
+                if len(wcwb) == 0:
+                    logger.info(f"No {data_kind} for {wb} found within model area")
+                    continue
+                wc[wb] = wcwb
             except Exception as e:
                 if str(e) == f"{data_kind} not available for {wb}":
                     logger.warning(e)
-                else:
+                elif raise_exceptions:
                     raise
+                else:
+                    logger.warning(e)
     return wc
 
 
-def add_stages_from_waterboards(gdf, pg=None, extent=None, columns=None, config=None):
-    """Add information from level areas (peilgebieden) to bgt-polygons."""
-    if pg is None:
-        pg = download_level_areas(gdf, extent=extent)
+def add_stages_from_waterboards(
+    gdf, la=None, extent=None, columns=None, config=None, min_total_overlap=0.0
+):
+    """
+    Add information from level areas (peilgebieden) to bgt-polygons.
+
+    Parameters
+    ----------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, containing the column "bronhouder".
+    la : dict, optional
+        A dictionary with the name of the waterboards as keys and GeoDataFrames with
+        level areas as values. It is generated by download_level_areas when None.
+        The default is None.
+    extent : list, tuple or np.array
+        Model extent (xmin, xmax, ymin, ymax). When extent is None, all data of the
+        water boards in gdf are downloaded downloaded.
+    columns : TYPE, optional
+        The columns that are added to gdf. Columns defaults to 'summer_stage' and
+        'winter_stage' when None. The default is None.
+    config : dict, optional
+        A dictionary with information about the webservices of the water boards. When
+        config is None, it is created with nlmod.read.waterboard.get_configuration().
+        The default is None.
+    min_total_overlap : float, optional
+        Only add data from waterboards to gdf when the total overlap between a feature
+        in gdf with all the features from the waterboard is larger than the fraction
+        min_total_overlap. The default is 0.0.
+
+    Returns
+    -------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, with the added columns
+
+    """
     if config is None:
         config = waterboard.get_configuration()
+    if la is None:
+        la = download_level_areas(gdf, extent=extent, config=config)
     if columns is None:
         columns = ["summer_stage", "winter_stage"]
     gdf[columns] = np.NaN
-    for wb in pg.keys():
+    for wb in la.keys():
+        if len(la[wb]) == 0:
+            continue
+        mask = gdf["bronhouder"] == config[wb]["bgt_code"]
+        gdf[mask] = add_info_to_gdf(
+            la[wb],
+            gdf[mask],
+            columns=columns,
+            min_total_overlap=min_total_overlap,
+            desc=f"Adding {columns} from {wb}",
+        )
+    return gdf
+
+
+def add_bottom_height_from_waterboards(
+    gdf, wc=None, extent=None, columns=None, config=None, min_total_overlap=0.0
+):
+    """
+    Add information from watercourses to bgt-polygons.
+
+    Parameters
+    ----------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, containing the column "bronhouder".
+    wc : dict, optional
+        A dictionary with the name of the waterboards as keys and GeoDataFrames with
+        watercourses as values. It is generated by download_watercourses when None.
+        The default is None.
+    extent : list, tuple or np.array
+        Model extent (xmin, xmax, ymin, ymax). When extent is None, all data of the
+        water boards in gdf are downloaded downloaded.
+    columns : TYPE, optional
+        The columns that are added to gdf. Columns defaults to 'bottom_height' when
+        None. The default is None.
+    config : dict, optional
+        A dictionary with information about the webservices of the water boards. When
+        config is None, it is created with nlmod.read.waterboard.get_configuration().
+        The default is None.
+    min_total_overlap : float, optional
+        Only add data from waterboards to gdf when the total overlap between a feature
+        in gdf with all the features from the waterboard is larger than the fraction
+        min_total_overlap. The default is 0.0.
+
+    Returns
+    -------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, with the added columns
+
+    """
+    if config is None:
+        config = waterboard.get_configuration()
+    if wc is None:
+        wc = download_watercourses(gdf, extent=extent, config=config)
+    if columns is None:
+        columns = ["bottom_height"]
+    gdf[columns] = np.NaN
+    for wb in wc.keys():
+        if len(wc[wb]) == 0:
+            continue
         mask = gdf["bronhouder"] == config[wb]["bgt_code"]
         gdf[mask] = add_info_to_gdf(
-            pg[wb],
+            wc[wb],
             gdf[mask],
             columns=columns,
-            min_total_overlap=0.0,
+            min_total_overlap=min_total_overlap,
             desc=f"Adding {columns} from {wb}",
+            geom_type=None,
         )
     return gdf
 
 
-def get_gdf(ds=None, extent=None, fname_ahn=None):
+def get_gdf(ds=None, extent=None, fname_ahn=None, ahn=None, buffer=0.0):
+    """
+    Generate a GeoDataFrame based on BGT-data and data from waterboards.
+
+    Parameters
+    ----------
+    ds : TYPE, optional
+        The Model Dataset, used to determine the extent (when None) and to grid the
+        surface level features. The default is None.
+    extent : list, tuple or np.array
+        Model extent (xmin, xmax, ymin, ymax). When extent is None, extent is extracted
+        from ds
+    fname_ahn : str, optional
+        When not None, fname_ahn is the path to a tiff-file with ahn-data, to calculate
+        the minimum height of the surface level near the surface water features. The
+        default is None.
+    ahn : xarray.DataArray, optional
+        When not None, ahn is a DataArray containing the height of the surface level and
+        is used to calculate the minimum height of the surface level near the surface
+        water features. The default is None.
+    buffer : float, optional
+        The buffer that is applied around surface water features to calculate the
+        minimum surface level near these features. The default is 0.0.
+
+    Returns
+    -------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, with added columns from waterboards
+        and gridded to the model grid (when ds is aupplied)
+
+    """
     if extent is None:
+        if ds is None:
+            raise (Exception("Please supply either ds or extent to get_gdf"))
         extent = get_extent_polygon(ds)
     gdf = bgt.get_bgt(extent)
     if fname_ahn is not None:
         from rasterstats import zonal_stats
 
-        stats = zonal_stats(gdf.geometry.buffer(1.0), fname_ahn, stats="min")
+        stats = zonal_stats(gdf.geometry.buffer(buffer), fname_ahn, stats="min")
         gdf["ahn_min"] = [x["min"] for x in stats]
+    if ahn is not None:
+        if fname_ahn is not None:
+            logger.warning("Data from {fname_ahn} is overwritten by data from ahn")
+        gdf = add_min_ahn_to_gdf(gdf, ahn, buffer=buffer)
     if isinstance(extent, Polygon):
         bs = extent.bounds
         extent = [bs[0], bs[2], bs[1], bs[3]]
     gdf = add_stages_from_waterboards(gdf, extent=extent)
+    gdf = add_bottom_height_from_waterboards(gdf, extent=extent)
     if ds is not None:
         return gdf_to_grid(gdf, ds).set_index("cellid")
     return gdf
 
 
+def add_min_ahn_to_gdf(gdf, ahn, buffer=0.0, column="ahn_min"):
+    """
+    Add a column names with the minimum surface level height near surface water features
+
+    Parameters
+    ----------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features
+    ahn : xarray.DataArray
+        A DataArray containing the height of the surface level.
+    buffer : float, optional
+        The buffer that is applied around surface water features to calculate the
+        minimum surface level near these features. The default is 0.0.
+    column : string, optional
+        The name of the new column in gdf containing the minimum surface level height.
+        The default is 'ahn_min'.
+
+    Returns
+    -------
+    gdf : geopandas.GeoDataFrame
+        A GeoDataFrame with surface water features, with an added column containing the
+        minimum surface level height near the features.
+
+    """
+    from geocube.api.core import make_geocube
+    from functools import partial
+    from geocube.rasterize import rasterize_image
+
+    # use geocube
+    gc = make_geocube(
+        vector_data=gdf.buffer(buffer).reset_index().rename_geometry("geometry"),
+        measurements=["index"],
+        like=ahn,  # ensure the data are on the same grid
+        rasterize_function=partial(rasterize_image, all_touched=True),
+    )
+    gc["ahn"] = ahn
+
+    ahn_min = gc.groupby("index").min()["ahn"].to_pandas()
+    ahn_min.index = ahn_min.index.astype(int)
+    gdf[column] = ahn_min
+    return gdf
+
+
 def gdf_to_seasonal_pkg(
     gdf,
     gwf,
     ds,
     pkg="DRN",
     default_water_depth=0.5,
     boundname_column="identificatie",
     c0=1.0,
     summer_months=(4, 5, 6, 7, 8, 9),
     layer_method="lay_of_rbot",
     **kwargs,
 ):
-    """Add a  surface water package to a groundwater-model, based on input from
-    a GeoDataFrame. This method adds two boundary conditions for each record in
-    the geodataframe: one for the winter_stage and one for the summer_stage.
-    The conductance of each record is a time-series called 'winter' or 'summer'
-    with values of either 0 or 1. These conductance values are multiplied by an
-    auxiliary variable that contains the actual conductance.
+    """Add a surface water package to a groundwater-model, based on input from a
+    GeoDataFrame. This method adds two boundary conditions for each record in the
+    GeoDataFrame: one for the winter_stage and one for the summer_stage.
+    The conductance of each record is a time-series called 'winter' or 'summer' with
+    values of either 0 or 1. These conductance values are multiplied by an auxiliary
+    variable that contains the actual conductance.
 
     Parameters
     ----------
     gdf : GeoDataFrame
-        A GeoDataFrame with Polygon-data. Cellid must be the index (it will be
-        calculated if it is not) and must have columns 'winter_stage' and
-        'summer_stage'.
+        A GeoDataFrame with Polygon-data. Cellid must be the index and must have columns
+        'winter_stage' and 'summer_stage'.
     gwf : flopy ModflowGwf
         groundwaterflow object.
     ds : xarray.Dataset
         Dataset with model data
     pkg: str, optional
         The package to generate. Possible options are 'DRN', 'RIV' and 'GHB'.
-        The default is pkg.
+        The default is 'DRN'.
     default_water_depth : float, optional
         The default water depth, only used when there is no 'rbot' column in
         gdf or when this column contains nans. The default is 0.5.
     boundname_column : str, optional
         THe name of the column in gdf to use for the boundnames. The default is
         "identificatie", which is a unique identifier in the BGT.
     c0 : float, optional
@@ -685,15 +917,15 @@
         THe months in which 'summer_stage' is active. The default is
         (4, 5, 6, 7, 8, 9), which means summer is from april through september.
     layer_method : str, optional
         The method used to distribute the conductance over the layers. Possible
         values are 'lay_of_rbot' and 'distribute_cond_over_lays'. The default
         is "lay_of_rbot".
     **kwargs : dict
-        Kwargs are passed onto ModflowGwfdrn.
+        Kwargs are passed onto ModflowGwfdrn, ModflowGwfriv or ModflowGwfghb.
 
     Returns
     -------
     package : ModflowGwfdrn, ModflowGwfriv or ModflowGwfghb
         The generated flopy-package
     """
     if gdf.index.name != "cellid":
@@ -710,40 +942,42 @@
     )
 
     # make sure we have a bottom height
     if "rbot" not in gdf:
         gdf["rbot"] = np.NaN
     mask = gdf["rbot"].isna()
     if mask.any():
+        logger.info(
+            f"Filling {mask.sum()} NaN's in rbot using a water depth of {default_water_depth} meter."
+        )
         min_stage = pd.concat(stages, axis=1).min(axis=1)
-        gdf.loc[mask, "rbot"] = min_stage - default_water_depth
+        gdf.loc[mask, "rbot"] = min_stage[mask] - default_water_depth
 
     if "cond" not in gdf:
+        logger.info(
+            f"Calcluating {pkg}-conductance based on as resistance of {c0} days."
+        )
         gdf["cond"] = gdf.geometry.area / c0
 
     if boundname_column is not None:
         gdf["boundname"] = gdf[boundname_column]
 
     spd = []
-    for iseason, season in enumerate(["winter", "summer"]):
+    seasons = ["winter", "summer"]
+    for iseason, season in enumerate(seasons):
         # use  a winter and summer level
-
         gdf["stage"] = stages[iseason]
 
         mask = gdf["stage"] < gdf["rbot"]
         gdf.loc[mask, "stage"] = gdf.loc[mask, "rbot"]
         gdf["aux"] = season
 
-        # ignore records without a stage
-        mask = gdf["stage"].isna()
-        if mask.any():
-            logger.warning(f"{mask.sum()} records without an elevation ignored")
         spd.extend(
             build_spd(
-                gdf[~mask],
+                gdf,
                 pkg,
                 ds,
                 layer_method=layer_method,
             )
         )
     # from the release notes (6.3.0):
     # When this AUXMULTNAME option is used, the multiplier value in the
@@ -776,14 +1010,25 @@
         boundnames=boundname_column is not None,
         auxmultname="cond_fact",
         auxiliary=["cond_fact"],
         observations=observations,
         **kwargs,
     )
     # add timeseries for the seasons 'winter' and 'summer'
+    add_season_timeseries(ds, package, summer_months=summer_months, seasons=seasons)
+    return package
+
+
+def add_season_timeseries(
+    ds,
+    package,
+    summer_months=(4, 5, 6, 7, 8, 9),
+    filename="season.ts",
+    seasons=("winter", "summer"),
+):
     tmin = pd.to_datetime(ds.time.start)
     if tmin.month in summer_months:
         ts_data = [(0.0, 0.0, 1.0)]
     else:
         ts_data = [(0.0, 1.0, 0.0)]
     tmax = pd.to_datetime(ds["time"].data[-1])
     years = range(tmin.year, tmax.year + 1)
@@ -796,20 +1041,19 @@
         # add a record for the start of winter, on oktober 1
         time = pd.Timestamp(year=year, month=summer_months[-1] + 1, day=1)
         time = (time - tmin) / pd.to_timedelta(1, "D")
         if time > 0:
             ts_data.append((time, 1.0, 0.0))
 
     package.ts.initialize(
-        filename="season.ts",
+        filename=filename,
         timeseries=ts_data,
-        time_series_namerecord=["winter", "summer"],
+        time_series_namerecord=seasons,
         interpolation_methodrecord=["stepwise", "stepwise"],
     )
-    return package
 
 
 def rivdata_from_xylist(gwf, xylist, layer, stage, cond, rbot):
     # TODO: temporary fix until flopy is patched
     if gwf.modelgrid.grid_type == "structured":
         gi = flopy.utils.GridIntersect(gwf.modelgrid, rtree=False)
         cellids = gi.intersect(xylist, shapetype="linestring")["cellids"]
```

### Comparing `nlmod-0.5.1/nlmod/gwf/wells.py` & `nlmod-0.5.2/nlmod/gwf/wells.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     top="top",
     botm="botm",
     Q="Q",
     aux=None,
     boundnames=None,
     **kwargs,
 ):
-
     # collect data
     well_lrcd = []
 
     for _, irow in tqdm(df.iterrows(), total=df.index.size, desc="Adding WELs"):
         try:
             cid1 = gwf.modelgrid.intersect(irow[x], irow[y], irow[top], forgive=False)
             cid2 = gwf.modelgrid.intersect(irow[x], irow[y], irow[botm], forgive=False)
@@ -69,15 +68,14 @@
     Q="Q",
     rw="rw",
     condeqn="THIEM",
     strt=0.0,
     boundnames=None,
     **kwargs,
 ):
-
     maw_pakdata = []
     maw_conndata = []
     maw_perdata = []
 
     for iw, irow in tqdm(df.iterrows(), total=df.index.size, desc="Adding MAWs"):
         try:
             cid1 = gwf.modelgrid.intersect(irow[x], irow[y], irow[top], forgive=False)
```

### Comparing `nlmod-0.5.1/nlmod/modpath/modpath.py` & `nlmod-0.5.2/nlmod/modpath/modpath.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/plot.py` & `nlmod-0.5.2/nlmod/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 import warnings
 
 import flopy
 import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
 from matplotlib.collections import PatchCollection
+from matplotlib.colors import ListedColormap, Normalize
 from matplotlib.patches import Patch, Polygon
 from matplotlib.ticker import FuncFormatter, MultipleLocator
-from matplotlib.colors import ListedColormap, Normalize
 
+from .dcs import DatasetCrossSection
 from .dims.grid import get_vertices, modelgrid_from_ds
 from .dims.resample import get_affine_mod_to_world, get_extent
-from .read import rws, geotop
-from .dcs import DatasetCrossSection
+from .read import geotop, rws
 
 
-def surface_water(model_ds, ax=None):
+def surface_water(model_ds, ax=None, **kwargs):
     surf_water = rws.get_gdf_surface_water(model_ds)
 
     if ax is None:
         _, ax = plt.subplots()
-    surf_water.plot(ax=ax)
+    surf_water.plot(ax=ax, **kwargs)
 
     return ax
 
 
 def modelgrid(ds, ax=None, add_surface_water=False, **kwargs):
     if ax is None:
         _, ax = plt.subplots(figsize=(10, 10))
@@ -394,15 +394,15 @@
         y = da.y
         if rotated:
             if ds is None:
                 raise (Exception("Supply model dataset (ds) for grid information"))
             if "angrot" in ds.attrs and ds.attrs["angrot"] != 0.0:
                 affine = get_affine_mod_to_world(ds)
                 x, y = affine * np.meshgrid(x, y)
-        return ax.pcolormesh(x, y, da, shading="nearest", **kwargs)
+        return ax.pcolormesh(x, y, da, shading="nearest", edgecolor=edgecolor, **kwargs)
 
 
 def get_patches(ds, rotated=False):
     """Get the matplotlib patches for a vertex grid, which can be used in
     da()"""
     assert "icell2d" in ds.dims
     xy = np.column_stack((ds["xv"].data, ds["yv"].data))
@@ -697,21 +697,22 @@
     cs = DatasetCrossSection(gt, line, layer="z", ax=ax, **kwargs)
     lithoks = gt["lithok"].data
     lithok_un = np.unique(lithoks[~np.isnan(lithoks)])
     array = np.full(lithoks.shape, np.NaN)
 
     colors = []
     for i, lithok in enumerate(lithok_un):
+        lithok = int(lithok)
         array[lithoks == lithok] = i
         colors.append(lithok_props.at[lithok, "color"])
     cmap = ListedColormap(colors)
     norm = Normalize(-0.5, np.nanmax(array) + 0.5)
     cs.plot_array(array, norm=norm, cmap=cmap)
     if legend:
         # make a legend with dummy handles
         handles = []
         for i, lithok in enumerate(lithok_un):
-            label = lithok_props.at[lithok, "name"]
+            label = lithok_props.at[int(lithok), "name"]
             handles.append(Patch(facecolor=colors[i], label=label))
         ax.legend(handles=handles, loc=legend_loc)
 
     return cs
```

### Comparing `nlmod-0.5.1/nlmod/read/ahn.py` & `nlmod-0.5.2/nlmod/read/ahn.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/read/bgt.py` & `nlmod-0.5.2/nlmod/read/bgt.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,52 +4,62 @@
 from io import BytesIO
 from zipfile import ZipFile
 
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import requests
-import shapely
 from shapely.geometry import LineString, MultiPolygon, Point, Polygon
 
 from ..dims.resample import extent_to_polygon
 
 
-def get_bgt(extent, layer="waterdeel", cut_by_extent=True, fname=None, geometry=None):
+def get_bgt(
+    extent,
+    layer="waterdeel",
+    cut_by_extent=True,
+    make_valid=False,
+    fname=None,
+    geometry=None,
+    remove_expired=True,
+):
     """Get geometries within an extent or polygon from the Basis Registratie
     Grootschalige Topografie (BGT)
 
     Parameters
     ----------
     extent : list or tuple of length 4 or shapely Polygon
         The extent (xmin, xmax, ymin, ymax) or polygon for which shapes are
         requested.
     layer : string, optional
         The layer for which shapes are requested. The default is "waterdeel".
     cut_by_extent : bool, optional
         Only return the intersection with the extent if True. The default is
         True
+    make_valid : bool, optional
+        Make geometries valid by appying a buffer of 0 m when True. THe defaults is
+        False.
     fname : string, optional
         Save the zipfile that is received by the request to file. The default
         is None, which does not save anything to file.
     geometry: string, optional
-        When geometry is specified, the gml inside the received zipfile is read
-        using an xml-reader (instead of fiona). For the layer 'waterdeel' the
-        geometry-field is 'geometrie2dWaterdeel', and for the layer 'pand' the
-        geometry-field is 'geometrie2dGrondvlak'. To determine the geometry
-        field of other layers, use fname to save a response and inspect the
-        gml-file. The default is None, which results in fiona reading the data.
-        This can cause problems when there are multiple geometrie-fields inside
-        each object. This happens in the layer 'pand', where each buidling
-        (polygon) also contains a Point-geometry for the label.
+        When geometry is specified, this attribute is used as the geometry of the
+        resulting GeoDataFrame. Some layers have multiple geometry-attributes. An
+        example is the layer 'pand', where each buidling (polygon) also contains a
+        Point-geometry for the label. When geometry is None, the last attribute starting
+        with the word "geometrie" is used as the geometry. The default is None.
+    remove_expired: bool, optional
+        Remove expired items (that contain a value for 'eindRegistratie') when True. The
+        default is True.
 
     Returns
     -------
-    gdf : GeoPandas GeoDataFrame
-        A GeoDataFrame containing all geometries and properties.
+    gdf : GeoPandas GeoDataFrame or dict of GeoPandas GeoDataFrame
+        A GeoDataFrame (when only one layer is requested) or a dict of GeoDataFrames
+        containing all geometries and properties.
     """
     if layer == "all":
         layer = get_bgt_layers()
     if isinstance(layer, str):
         layer = [layer]
 
     api_url = "https://api.pdok.nl"
@@ -92,46 +102,98 @@
     href = response.json()["_links"]["download"]["href"]
     response = requests.get(f"{api_url}{href}", timeout=1200)  # 20 minutes
 
     if fname is not None:
         with open(fname, "wb") as file:
             file.write(response.content)
 
-    gdf = {}
-
     zipfile = BytesIO(response.content)
-    gdf = read_bgt_zipfile(zipfile, geometry=geometry)
+    gdf = read_bgt_zipfile(
+        zipfile,
+        geometry=geometry,
+        cut_by_extent=cut_by_extent,
+        make_valid=make_valid,
+        extent=polygon,
+        remove_expired=remove_expired,
+    )
 
-    for key in gdf:
-        if gdf[key] is not None and "eindRegistratie" in gdf[key]:
-            # remove double features
-            # by removing features with an eindRegistratie
-            gdf[key] = gdf[key][gdf[key]["eindRegistratie"].isna()]
-
-        if cut_by_extent and isinstance(gdf[key], gpd.GeoDataFrame):
-            try:
-                gdf[key].geometry = gdf[key].intersection(polygon)
-                gdf[key] = gdf[key][~gdf[key].is_empty]
-            except shapely.geos.TopologicalError:
-                print(f"Cutting by extent failed for {key}")
     if len(layer) == 1:
         gdf = gdf[layer[0]]
     return gdf
 
 
-def read_bgt_zipfile(fname, geometry=None, files=None):
+def read_bgt_zipfile(
+    fname,
+    geometry=None,
+    files=None,
+    cut_by_extent=True,
+    make_valid=False,
+    extent=None,
+    remove_expired=True,
+):
+    """
+    Read data from a zipfile that was downloaded using get_bgt().
+
+    Parameters
+    ----------
+    fname : string
+        The filename of the zip-file containing the BGT-data.
+    geometry : str, optional
+        DESCRIPTION. The default is None.
+    files : string of list of strings, optional
+        The files to read from the zipfile. Read all files when files is None. The
+        default is None.
+    cut_by_extent : bool, optional
+        Cut the geoemetries by the supplied extent. When no extent is supplied,
+        cut_by_extent is set to False. The default is True.
+    make_valid : bool, optional
+        Make geometries valid by appying a buffer of 0 m when True. THe defaults is
+        False.
+    extent : list or tuple of length 4 or shapely Polygon
+        The extent (xmin, xmax, ymin, ymax) or polygon by which the geometries are
+        clipped. Only used when cut_by_extent is True. The defult is None.
+    remove_expired: bool, optional
+        Remove expired items (that contain a value for 'eindRegistratie') when True. The
+        default is True.
+
+    Returns
+    -------
+    gdf : dict of GeoPandas GeoDataFrame
+        A dict of GeoDataFrames containing all geometries and properties.
+
+    """
     zf = ZipFile(fname)
     gdf = {}
     if files is None:
         files = zf.namelist()
     elif isinstance(files, str):
         files = [files]
+    if extent is None:
+        cut_by_extent = False
+    else:
+        if isinstance(extent, Polygon):
+            polygon = extent
+        else:
+            polygon = extent_to_polygon(extent)
     for file in files:
         key = file[4:-4]
         gdf[key] = read_bgt_gml(zf.open(file), geometry=geometry)
+
+        if remove_expired and gdf[key] is not None and "eindRegistratie" in gdf[key]:
+            # remove double features
+            # by removing features with an eindRegistratie
+            gdf[key] = gdf[key][gdf[key]["eindRegistratie"].isna()]
+
+        if make_valid:
+            gdf[key].geometry = gdf[key].geometry.buffer(0.0)
+
+        if cut_by_extent and isinstance(gdf[key], gpd.GeoDataFrame):
+            gdf[key].geometry = gdf[key].intersection(polygon)
+            gdf[key] = gdf[key][~gdf[key].is_empty]
+
     return gdf
 
 
 def read_bgt_gml(fname, geometry="geometrie2dGrondvlak", crs="epsg:28992"):
     def get_xy(text):
         xy = [float(val) for val in text.split()]
         xy = np.array(xy).reshape(int(len(xy) / 2), 2)
@@ -169,15 +231,15 @@
         for segment in curve.find(f"{ns}segments"):
             xy = np.vstack((xy, get_xy(segment.find(f"{ns}posList").text)))
         return xy
 
     def read_linestring(linestring):
         return get_xy(linestring.find(f"{ns}posList").text)
 
-    def _read_label(child, d):
+    def read_label(child, d):
         ns = "{http://www.geostandaarden.nl/imgeo/2.1}"
         label = child.find(f"{ns}Label")
         d["label"] = label.find(f"{ns}tekst").text
         positie = label.find(f"{ns}positie").find(f"{ns}Labelpositie")
         xy = read_point(
             positie.find(f"{ns}plaatsingspunt").find(
                 "{http://www.opengis.net/gml}Point"
@@ -228,26 +290,26 @@
                     else:
                         raise (Exception((f"Unsupported tag: {child[0].tag}")))
                 elif key == "nummeraanduidingreeks":
                     ns = "{http://www.geostandaarden.nl/imgeo/2.1}"
                     nar = child.find(f"{ns}Nummeraanduidingreeks").find(
                         f"{ns}nummeraanduidingreeks"
                     )
-                    _read_label(nar, d)
+                    read_label(nar, d)
                 elif key.startswith("kruinlijn"):
                     ns = "{http://www.opengis.net/gml}"
                     if child[0].tag == f"{ns}LineString":
                         ls = child.find(f"{ns}LineString")
                         d[key] = LineString(read_linestring(ls))
                     elif child[0].tag == f"{ns}Curve":
                         d[key] = LineString(read_curve(child[0]))
                     else:
                         raise (Exception((f"Unsupported tag: {child[0].tag}")))
                 elif key == "openbareRuimteNaam":
-                    _read_label(child, d)
+                    read_label(child, d)
                 else:
                     raise (Exception((f"Unknown key: {key}")))
         data.append(d)
     if len(data) > 0:
         if geometry is None:
             return pd.DataFrame(data)
         else:
```

### Comparing `nlmod-0.5.1/nlmod/read/brp.py` & `nlmod-0.5.2/nlmod/read/brp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/nlmod/read/geotop.py` & `nlmod-0.5.2/nlmod/read/geotop.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 GEOTOP_URL = r"http://www.dinodata.nl/opendap/GeoTOP/geotop.nc"
 
 
 def get_lithok_props(rgb_colors=True):
     fname = os.path.join(NLMOD_DATADIR, "geotop", "litho_eenheden.csv")
     df = pd.read_csv(fname, index_col=0)
     if rgb_colors:
-        df["color"] = get_lithok_colors()
+        df["color"] = pd.Series(get_lithok_colors())
     return df
 
 
 def get_lithok_colors():
     colors = {
         0: (200, 200, 200),
         1: (157, 78, 64),
@@ -119,22 +119,22 @@
     for dim in ["x", "y"]:
         old_dim = gt[dim].values
         gt[dim] = old_dim + (old_dim[1] - old_dim[0]) / 2
 
     # slice extent
     gt = gt.sel(x=slice(extent[0], extent[1]), y=slice(extent[2], extent[3]))
 
-    # change order of dimensions from x, y, z to z, y, x
-    gt = gt.transpose("z", "y", "x")
-    gt = gt.sortby("z", ascending=False)
-    gt = gt.sortby("y", ascending=False)
-
     if drop_probabilities:
         gt = gt[["strat", "lithok"]]
 
+    # change order of dimensions from x, y, z to z, y, x
+    gt = gt.transpose("z", "y", "x")
+    gt = gt.sortby("z", ascending=False)  # uses a lot of RAM
+    gt = gt.sortby("y", ascending=False)  # uses a lot of RAM
+
     return gt
 
 
 def convert_geotop_to_ml_layers(
     geotop_ds_raw,
     strat_props=None,
     **kwargs,
@@ -282,15 +282,18 @@
     Add kh and kv variables to the voxels of the GeoTOP Dataset.
 
     Parameters
     ----------
     gt : xr.Dataset
         The geotop dataset, at least with variable lithok.
     df : pd.DataFrame
-        A DataFrame with .
+        A DataFrame with information about the kh and optionally kv, for different
+        lithoclasses or stratigraphic units. The DataFrame must contain the columns
+        'lithok' and 'kh', and optionally 'strat' and 'kv'. As an example see
+        nlmod.read.geotop.get_kh_kv_table().
     stochastic : bool, str or None, optional
         When stochastic is True or a string, use the stochastic data of GeoTOP. The only
         supported method right now is "linear", which means kh and kv are determined
         from a linear weighted mean of the voxels. For kh the method from kh_method is
         used to calculate the mean. For kv the method from kv_method is used. When
         stochastic is False or None, the stochastic data of GeoTOP is not used. The
         default is None.
@@ -316,16 +319,16 @@
     Raises
     ------
 
         DESCRIPTION.
 
     Returns
     -------
-    gt : TYPE
-        DESCRIPTION.
+    gt : xr.Dataset
+        Datset with voxel-data, with the added variables 'kh' and 'kv'.
 
     """
     if isinstance(stochastic, bool):
         if stochastic:
             stochastic = "linear"
         else:
             stochastic = None
@@ -335,19 +338,19 @@
         raise (Exception("Unknown kv_method: {kv_method}"))
     strat = gt["strat"].data
     msg = "Determining kh and kv of geotop-data based on lithoclass"
     if df.index.name in ["lithok", "strat"]:
         df = df.reset_index()
     if "strat" in df:
         msg = f"{msg} and stratigraphy"
-    logging.info(msg)
+    logger.info(msg)
     if kh_df not in df:
         raise (Exception(f"No {kh_df} defined in df"))
     if kv_df not in df:
-        logging.info(f"Setting kv equal to kh / {anisotropy}")
+        logger.info(f"Setting kv equal to kh / {anisotropy}")
     if stochastic is None:
         # calculate kh and kv from most likely lithoclass
         lithok = gt["lithok"].data
         kh_ar = np.full(lithok.shape, np.NaN)
         kv_ar = np.full(lithok.shape, np.NaN)
         if "strat" in df:
             combs = np.column_stack((strat.ravel(), lithok.ravel()))
@@ -432,22 +435,22 @@
 
 
 def _get_kh_kv_from_df(df, ilithok, istrat=None, anisotropy=1.0, mask=None):
     mask_df = df["lithok"] == ilithok
     if istrat is not None:
         mask_df = mask_df & (df["strat"] == istrat)
     if not np.any(mask_df):
-        msg = f"No conductivities found for stratigraphy-unit {istrat}"
+        msg = f"No conductivities found for stratigraphic unit {istrat}"
         if istrat is not None:
             msg = f"{msg} and lithoclass {ilithok}"
         if mask is None:
             msg = f"{msg}. Setting values of voxels to NaN."
         else:
             msg = f"{msg}. Setting values of {mask.sum()} voxels to NaN."
-        logging.warning(msg)
+        logger.warning(msg)
         return np.NaN, np.NaN
 
     kh = df.loc[mask_df, "kh"].mean()
     if "kv" in df:
         kv = df.loc[mask_df, "kv"].mean()
         if np.isnan(kv):
             kv = kh / anisotropy
```

### Comparing `nlmod-0.5.1/nlmod/read/jarkus.py` & `nlmod-0.5.2/nlmod/read/jarkus.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 Note: if you like jazz please check this out: https://www.northseajazz.com
 """
 import datetime as dt
 import logging
 import os
 
 import numpy as np
+import pandas as pd
 import requests
 import xarray as xr
 
 from .. import cache
 from ..dims.resample import fillnan_da, structured_da_to_ds
 from ..util import get_da_from_da_ds, get_ds_empty
 
 logger = logging.getLogger(__name__)
 
 
 @cache.cache_netcdf
-def get_bathymetry(ds, northsea, method="average"):
+def get_bathymetry(ds, northsea, kind="jarkus", method="average"):
     """get bathymetry of the Northsea from the jarkus dataset.
 
     Parameters
     ----------
     ds : xarray.Dataset
         dataset with model data where bathymetry is added to
     northsea : ??
@@ -54,16 +55,15 @@
     # no bathymetry if we don't have northsea
     if (northsea == 0).all():
         ds_out["bathymetry"] = get_da_from_da_ds(northsea, northsea.dims, data=np.nan)
         return ds_out
 
     # try to get bathymetry via opendap
     try:
-        url = "https://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc"
-        jarkus_ds = get_dataset_jarkus(ds.extent, url)
+        jarkus_ds = get_dataset_jarkus(ds.extent, kind=kind)
     except OSError:
         import gdown
 
         logger.warning(
             "cannot access Jarkus netCDF link, copy file from google drive instead"
         )
         fname_jarkus = os.path.join(ds.model_ws, "jarkus_nhflopy.nc")
@@ -81,90 +81,135 @@
 
     # bathymetry projected on model grid
     da_bathymetry = structured_da_to_ds(da_bathymetry_filled, ds, method=method)
 
     ds_out["bathymetry"] = xr.where(northsea, da_bathymetry, np.nan)
 
     for datavar in ds_out:
-        ds_out[datavar].attrs["source"] = "Jarkus"
-        ds_out[datavar].attrs["url"] = url
-        ds_out[datavar].attrs["source"] = dt.datetime.now().strftime("%Y%m%d")
+        ds_out[datavar].attrs["source"] = kind
+        ds_out[datavar].attrs["date"] = dt.datetime.now().strftime("%Y%m%d")
         if datavar == "bathymetry":
             ds_out[datavar].attrs["units"] = "mNAP"
 
     return ds_out
 
 
-def get_dataset_jarkus(
-    extent,
-    url="http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc",
-):
-    """Get bathymetry from Jarkus within a certain extent. The following steps
-    are used:
-
-       1. find Jarkus tiles within the extent
-       2. combine netcdf urls of Jarkus tiles
-       3. read Jarkus tiles and combine the 'z' parameter of the last time step
-          of each tile, to a dataarray.
+def get_dataset_jarkus(extent, kind="jarkus", return_tiles=False, time=-1):
+    """Get bathymetry from Jarkus within a certain extent. If return_tiles is False, the
+    following actions are performed:
+    1. find Jarkus tiles within the extent
+    2. download netcdf files of Jarkus tiles
+    3. read Jarkus tiles and combine the 'z' parameter of the last time step of each
+    tile (when time=1), to a dataarray.
 
     Parameters
     ----------
     extent : list, tuple or np.array
         extent (xmin, xmax, ymin, ymax) of the desired grid. Should be RD-new
-        coordinates (EPSG:28992)
+        coördinates (EPSG:28992)
+    kind : str, optional
+        The kind of data. Can be "jarkus", "kusthoogte" or "vaklodingen". The default is
+        "jarkus".
+    return_tiles : bool, optional
+        Return the individual tiles when True. The default is False.
+    time : str, int or pd.TimeStamp, optional
+        The time to return data for. When time="last_non_nan", this returns the last
+        non-NaN-value for each pixel. This can take a while, as all tiles need to be
+        checked. When time is an integer, it is used as the time index. When set to -1,
+        this then downloads the last time available in each tile  (which can contain
+        large areas with NaN-values). When time is a string (other than "last_non_nan")
+        or a pandas Timestamp, only data on this exact time are downloaded. The default
+        is -1.
 
     Returns
     -------
     z : xr.DataSet
         dataset containing bathymetry data
+
     """
 
     extent = [int(x) for x in extent]
-    netcdf_tile_names = get_jarkus_tilenames(extent, url=url)
-    tiles = [xr.open_dataset(name) for name in netcdf_tile_names]
-    # only use the last timestep
-    tiles = [tile.isel(time=-1) for tile in tiles]
-    z_dataset = xr.combine_by_coords(tiles, combine_attrs="drop")
 
+    netcdf_tile_names = get_jarkus_tilenames(extent, kind)
+    tiles = [xr.open_dataset(name.strip()) for name in netcdf_tile_names]
+    if return_tiles:
+        return tiles
+    if time is not None:
+        if time == "last_non_nan":
+            tiles_last = []
+            for tile in tiles:
+                time = (~np.isnan(tile["z"])).cumsum("time").argmax("time")
+                tiles_last.append(tile.isel(time=time))
+            tiles = tiles_last
+        elif isinstance(time, int):
+            # only use the last timestep
+            tiles = [tile.isel(time=time) for tile in tiles]
+        else:
+            time = pd.to_datetime(time)
+            tiles_left = []
+            for tile in tiles:
+                if time in tile.time:
+                    tiles_left.append(tile.sel(time=time))
+                else:
+                    extent_tile = list(
+                        np.hstack(
+                            (
+                                tile.attrs["projectionCoverage_x"],
+                                tile.attrs["projectionCoverage_y"],
+                            )
+                        )
+                    )
+                    logger.info(
+                        f"no time={time} in {kind}-tile with extent {extent_tile}"
+                    )
+            tiles = tiles_left
+    z_dataset = xr.combine_by_coords(tiles, combine_attrs="drop")
     return z_dataset
 
 
-def get_jarkus_tilenames(
-    extent,
-    url="http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc",
-):
-    """Find all Jarkus tilenames within a certain extent.
+def get_jarkus_tilenames(extent, kind="jarkus"):
+    """Find all Jarkus tilenames within a certain extent
 
     Parameters
     ----------
     extent : list, tuple or np.array
         extent (xmin, xmax, ymin, ymax) of the desired grid. Should be RD-new
         coördinates (EPSG:28992)
 
     Returns
     -------
     netcdf_urls : list of str
         list of the urls of all netcdf files of the tiles with Jarkus data.
+
     """
+    if kind == "jarkus":
+        url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc"
+    elif kind == "kusthoogte":
+        url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/kusthoogte/catalog.nc"
+    elif kind == "vaklodingen":
+        url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/vaklodingen/catalog.nc"
+    else:
+        raise (Exception(f"Unsupported kind: {kind}"))
+
     ds_jarkus_catalog = xr.open_dataset(url)
-    ew_x = ds_jarkus_catalog["projectionCoverage_x"]
-    sn_y = ds_jarkus_catalog["projectionCoverage_y"]
+    ew_x = ds_jarkus_catalog["projectionCoverage_x"].values
+    sn_y = ds_jarkus_catalog["projectionCoverage_y"].values
 
     mask_ew = (ew_x[:, 1] > extent[0]) & (ew_x[:, 0] < extent[1])
     mask_sn = (sn_y[:, 1] > extent[2]) & (sn_y[:, 0] < extent[3])
 
     indices_tiles = np.where(mask_ew & mask_sn)[0]
-    all_netcdf_tilenames = get_netcdf_tiles()
+    all_netcdf_tilenames = get_netcdf_tiles(kind)
 
     netcdf_tile_names = [all_netcdf_tilenames[i] for i in indices_tiles]
 
     return netcdf_tile_names
 
 
-def get_netcdf_tiles():
+def get_netcdf_tiles(kind="jarkus"):
     """Find all Jarkus netcdf tile names.
 
     Returns
     -------
     netcdf_urls : list of str
         list of the urls of all netcdf files of the tiles with Jarkus data.
 
@@ -173,16 +218,23 @@
     This function would be redundant if the jarkus catalog
     (http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc)
     had a proper way of displaying the url's of each tile. It seems like an
     attempt was made to do this because there is a data variable
     named 'urlPath' in the catalog. However the dataarray of 'urlPath' has the
     same string for each tile.
     """
-    url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc.ascii"
-    req = requests.get(url, timeout=1200)  # 20 minutes time out
+    if kind == "jarkus":
+        url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/jarkus/grids/catalog.nc.ascii"
+    elif kind == "kusthoogte":
+        url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/kusthoogte/catalog.nc.ascii"
+    elif kind == "vaklodingen":
+        url = "http://opendap.deltares.nl/thredds/dodsC/opendap/rijkswaterstaat/vaklodingen/catalog.nc.ascii"
+    else:
+        raise (Exception(f"Unsupported kind: {kind}"))
+    req = requests.get(url, timeout=5)
     s = req.content.decode("ascii")
     start = s.find("urlPath", s.find("urlPath") + 1)
     end = s.find("projectionCoverage_x", s.find("projectionCoverage_x") + 1)
     netcdf_urls = list(eval(s[start + 12 : end - 2]))
     return netcdf_urls
```

### Comparing `nlmod-0.5.1/nlmod/read/knmi.py` & `nlmod-0.5.2/nlmod/read/knmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,18 @@
             # get locations with the same prec and evap station
             loc_sel = locations.loc[
                 (locations["prec_point"] == prec_stn)
                 & (locations["evap_point"] == evap_stn)
             ]
 
             # calculate recharge time series
-            prec = oc_knmi_prec.loc[prec_stn, "obs"]["RD"]
-            evap = oc_knmi_evap.loc[evap_stn, "obs"]["EV24"]
+            prec = oc_knmi_prec.loc[prec_stn,
+                                    "obs"]["RD"].resample('D').nearest()
+            evap = oc_knmi_evap.loc[evap_stn,
+                                    "obs"]["EV24"].resample('D').nearest()
             ts = (prec - evap).dropna()
             ts.name = f"{prec.name}-{evap.name}"
 
             _add_ts_to_ds(ts, loc_sel, "recharge", ds_out)
 
     elif method == "separate":
         ds_out["recharge"] = dims, np.zeros(shape)
@@ -126,15 +128,16 @@
     return ds_out
 
 
 def _add_ts_to_ds(timeseries, loc_sel, variable, ds):
     """Add a timeseries to a variable at location loc_sel in model DataSet."""
     end = pd.Timestamp(ds.time.data[-1])
     if timeseries.index[-1] < end:
-        raise ValueError(f"no recharge available at {timeseries.name} for date {end}")
+        raise ValueError(
+            f"no recharge available at {timeseries.name} for date {end}")
 
     # fill recharge data array
     model_recharge = pd.Series(index=ds.time, dtype=float)
     for j, ts in enumerate(model_recharge.index):
         if j == 0:
             start = ds.time.start
         else:
@@ -145,15 +148,16 @@
         # when the model frequency is higher than the timeseries-frequency,
         # there will be NaN's, which we fill by backfill
         model_recharge = model_recharge.fillna(method="bfill")
         if model_recharge.isna().any():
             raise (Exception("There are NaN-values in {variable}"))
 
     # add data to ds
-    values = np.repeat(model_recharge.values[:, np.newaxis], loc_sel.shape[0], 1)
+    values = np.repeat(
+        model_recharge.values[:, np.newaxis], loc_sel.shape[0], 1)
     if ds.gridtype == "structured":
         ds[variable].data[:, loc_sel.row, loc_sel.col] = values
     elif ds.gridtype == "vertex":
         ds[variable].data[:, loc_sel.index] = values
 
 
 def get_locations_vertex(ds):
```

### Comparing `nlmod-0.5.1/nlmod/read/regis.py` & `nlmod-0.5.2/nlmod/read/regis.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,18 @@
     # set x and y dimensions to cell center
     ds["x"] = ds.x_bounds.mean("bounds")
     ds["y"] = ds.y_bounds.mean("bounds")
 
     # slice extent
     ds = ds.sel(x=slice(extent[0], extent[1]), y=slice(extent[2], extent[3]))
 
+    if len(ds.x) == 0 or len(ds.y) == 0:
+        msg = "No data found. Please supply valid extent in the Netherlands in RD-coordinates"
+        raise (Exception(msg))
+
     # make sure layer names are regular strings
     ds["layer"] = ds["layer"].astype(str)
 
     # make sure y is descending
     ds = ds.sortby("y", ascending=False)
 
     # slice layers
@@ -149,14 +153,17 @@
 
     # rename bottom to botm, as it is called in FloPy
     ds = ds.rename_vars({"bottom": "botm"})
 
     if remove_nan_layers:
         # only keep layers with at least one active cell
         ds = ds.sel(layer=~(np.isnan(ds["botm"])).all(ds["botm"].dims[1:]))
+        if len(ds.layer) == 0:
+            msg = "No data found. Please supply valid extent in the Netherlands in RD-coordinates"
+            raise (Exception(msg))
 
     # slice data vars
     ds = ds[list(variables)]
 
     ds.attrs["extent"] = extent
     for datavar in ds:
         ds[datavar].attrs["grid_mapping"] = "crs"
```

### Comparing `nlmod-0.5.1/nlmod/read/rws.py` & `nlmod-0.5.2/nlmod/read/rws.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 """functions to add surface water to a mf model using the ghb package."""
 
 import datetime as dt
 import logging
 import os
 
 import geopandas as gpd
-import nlmod
 import xarray as xr
 
+import nlmod
+
 from .. import cache, dims, util
 from . import jarkus
 
 logger = logging.getLogger(__name__)
 
 
 def get_gdf_surface_water(ds):
```

### Comparing `nlmod-0.5.1/nlmod/read/waterboard.py` & `nlmod-0.5.2/nlmod/read/waterboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,48 +74,46 @@
 
     config["Brabantse Delta"] = {
         "bgt_code": "W0652",
         "watercourses": {
             # legger
             "url": "https://geoservices.brabantsedelta.nl/arcgis/rest/services/EXTERN/WEB_Vastgestelde_Legger_Oppervlaktewaterlichamen/FeatureServer",
             "layer": 11,  # categorie A
+            "bottom_width": "WS_BODEMBREEDTE_L",
+            "bottom_height": [["WS_BH_BENEDENSTROOMS_L", "WS_BH_BOVENSTROOMS_L"]],
             # "layer": 12,  # categorie B
             # beheer
             # "url": "https://geoservices.brabantsedelta.nl/arcgis/rest/services/EXTERN/WEB_Beheerregister_Waterlopen_en_Kunstwerken/FeatureServer",
             # "layer": 13,  # categorie A
             # "layer": 14,  # categorie B
             # "layer": 15,  # categorie C
         },
         "level_areas": {
-            # "url": "https://geoservices.brabantsedelta.nl/arcgis/rest/services/EXTERN/WEB_Beheerregister_Waterlopen_en_Kunstwerken/FeatureServer",
-            # "layer": 19,
-            "url": "https://maps.brabantsedelta.nl/arcgis/rest/services/Extern/Legger/MapServer",
-            "layer": 6,
+            "url": "https://geoservices.brabantsedelta.nl/arcgis/rest/services/EXTERN/WEB_Peilbesluiten/MapServer",
+            "layer": 0,  # Peilgebied vigerend
+            # "layer": 1, # Peilgebied praktijk
             "summer_stage": [
                 "WS_ZOMERPEIL",
                 "WS_VAST_PEIL",
-                "WS_STREEFPEIL",
-                "WS_MAXIMUM_PEIL",
-                "WS_MINIMUM_PEIL",
+                "WS_MAXIMUM",
             ],
             "winter_stage": [
                 "WS_WINTERPEIL",
                 "WS_VAST_PEIL",
-                "WS_STREEFPEIL",
-                "WS_MINIMUM_PEIL",
-                "WS_MAXIMUM_PEIL",
+                "WS_MINIMUM",
             ],
         },
     }
 
     config["De Dommel"] = {
         "bgt_code": "W0539",
         "watercourses": {
             "url": "https://services8.arcgis.com/dmR647kStmcYa6EN/arcgis/rest/services/LW_2021_20211110/FeatureServer",
             "layer": 9,  # LOW_2021_A_Water
+            "index": "LOKAALID",
             # "layer": 10,  # LOW_2021_A_Water_Afw_Afv
             # "layer": 11,  # LOW_2021_B_Water
             # "layer": 2,  # LOW_2021_Profielpunt
             # "layer": 13,  # LOW_2021_Profiellijn
             # "index": "WS_PROFIELID",
         },
     }
@@ -347,14 +345,15 @@
 
     config["Scheldestromen"] = {
         "bgt_code": "W0661",
         "watercourses": {
             "url": "https://geo.scheldestromen.nl/arcgis/rest/services/Extern/EXT_WB_Legger_Oppervlaktewaterlichamen_Vastgesteld/MapServer",
             "layer": 6,
             "index": "OAFIDENT",
+            "bottom_height": "OAFBODHG",
         },
         "level_areas": {
             "url": "https://geo.scheldestromen.nl/arcgis/rest/services/Extern/EXT_WB_Waterbeheer/FeatureServer",
             "layer": 14,  # Peilgebieden (praktijk)
             "index": "GPGIDENT",
             # "layer": 15,  # Peilgebieden (juridisch)
             # "index": "GJPIDENT",
```

### Comparing `nlmod-0.5.1/nlmod/read/webservices.py` & `nlmod-0.5.2/nlmod/read/webservices.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def arcrest(
     url,
     layer,
     extent=None,
     sr=28992,
     f="geojson",
     max_record_count=None,
-    timeout=1200,
+    timeout=120,
 ):
     """Download data from an arcgis rest FeatureServer."""
     params = {
         "f": f,
         "outFields": "*",
         "outSR": sr,
         "where": "1=1",
@@ -103,25 +103,29 @@
                 and "y" in feature["geometry"]
             ):
                 geometry = Point(feature["geometry"]["x"], feature["geometry"]["y"])
             else:
                 raise (Exception("Not supported yet"))
             feature["attributes"]["geometry"] = geometry
             data.append(feature["attributes"])
-        gdf = gpd.GeoDataFrame(data)
+        gdf = gpd.GeoDataFrame(data, crs=sr)
     else:
         # for geojson-data we can transform to GeoDataFrame right away
-        gdf = gpd.GeoDataFrame.from_features(features)
+        if len(features) == 0:
+            # Assigning CRS to a GeoDataFrame without a geometry column is not supported
+            gdf = gpd.GeoDataFrame()
+        else:
+            gdf = gpd.GeoDataFrame.from_features(features, crs=sr)
     return gdf
 
 
-def _get_data(url, params, timeout=1200):
+def _get_data(url, params, timeout=120):
     r = requests.get(url, params=params, timeout=timeout)
     if not r.ok:
-        raise (Exception("Request not successful"))
+        raise (Exception(f"Request not successful: {r.url}"))
     data = r.json()
     if "error" in data:
         code = data["error"]["code"]
         message = data["error"]["message"]
         raise (Exception(f"Error code {code}: {message}"))
     return data
 
@@ -142,17 +146,17 @@
     else:
         params["typeName"] = layer
     if extent is not None:
         params["bbox"] = f"{extent[0]},{extent[2]},{extent[1]},{extent[3]}"
     if paged:
         # wfs = WebFeatureService(url)
         # get the maximum number of features
-        r = requests.get(f"{url}&request=getcapabilities", timeout=1200)
+        r = requests.get(f"{url}&request=getcapabilities", timeout=120)
         if not r.ok:
-            raise (Exception("Request not successful"))
+            raise (Exception(f"Request not successful: {r.url}"))
         root = ET.fromstring(r.text)
         ns = {"ows": "http://www.opengis.net/ows/1.1"}
 
         constraints = {}
 
         def add_constrains(elem, constraints):
             for child in elem.findall("ows:Constraint", ns):
@@ -183,15 +187,15 @@
         if max_record_count is None:
             max_record_count = constraints["CountDefault"]
         else:
             max_record_count = min(max_record_count, constraints["CountDefault"])
 
         # get the number of features
         params["resultType"] = "hits"
-        r = requests.get(url, params=params, timeout=1200)
+        r = requests.get(url, params=params, timeout=120)
         params.pop("resultType")
         root = ET.fromstring(r.text)
         if "ExceptionReport" in root.tag:
             raise Exception(root[0].attrib)
         if version == "1.1.0":
             n = int(root.attrib["numberOfFeatures"])
         else:
```

### Comparing `nlmod-0.5.1/nlmod/sim/sim.py` & `nlmod-0.5.2/nlmod/sim/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,31 @@
         1. write the model dataset to cache
         2. copy the modelscript (typically a Jupyter Notebook) to the model
            workspace with a timestamp.
 
 
     Parameters
     ----------
-    sim : flopy.mf6.MFSimulation
-        MF6 Simulation object.
+    sim : flopy.mf6.MFSimulation or flopy.mf6.ModflowGwf
+        MF6 Simulation or MF6 Groundwater Flow object.
     ds : xarray.Dataset
         dataset with model data.
     write_ds : bool, optional
         if True the model dataset is cached to a NetCDF-file (.nc) with a name equal
         to its attribute called "model_name". The default is True.
     nb_path : str or None, optional
         full path of the Jupyter Notebook (.ipynb) with the modelscript. The
         default is None. Preferably this path does not have to be given
         manually but there is currently no good option to obtain the filename
         of a Jupyter Notebook from within the notebook itself.
     silent : bool, optional
         write and run model silently
     """
+    if isinstance(sim, flopy.mf6.ModflowGwf):
+        sim = sim.simulation
 
     if nb_path is not None:
         new_nb_fname = (
             f'{dt.datetime.now().strftime("%Y%m%d")}' + os.path.split(nb_path)[-1]
         )
         dst = os.path.join(ds.model_ws, new_nb_fname)
         logger.info(f"write script {new_nb_fname} to model workspace")
@@ -104,15 +106,15 @@
         nstp = [ds.time.nstp] * len(perlen)
 
     if "tsmult" in ds:
         tsmult = ds["tsmult"].values
     else:
         tsmult = [ds.time.tsmult] * len(perlen)
 
-    tdis_perioddata = [(p, n, t) for p, n, t in zip(perlen, nstp, tsmult)]
+    tdis_perioddata = list(zip(perlen, nstp, tsmult))
 
     return tdis_perioddata
 
 
 def sim(ds, exe_name=None):
     """create sim from the model dataset.
 
@@ -204,16 +206,20 @@
     ims : flopy ModflowIms
         ims object.
     """
 
     logger.info("creating modflow IMS")
 
     # Create the Flopy iterative model solver (ims) Package object
-    ims = flopy.mf6.modflow.mfims.ModflowIms(
+    ims = flopy.mf6.ModflowIms(
         sim,
         pname=pname,
         print_option="summary",
         complexity=complexity,
         **kwargs,
     )
 
     return ims
+
+
+def register_ims_package(sim, model, ims):
+    sim.register_ims_package(ims, [model.name])
```

### Comparing `nlmod-0.5.1/nlmod/util.py` & `nlmod-0.5.2/nlmod/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -303,15 +303,15 @@
         gdf = gdf.loc[gdf.within(gdf_extent.geometry.values[0])]
     else:
         raise TypeError("Function is not tested for geometry type: " f"{geom_types[0]}")
 
     return gdf
 
 
-def get_google_drive_filename(fid):
+def get_google_drive_filename(fid, timeout=120):
     """get the filename of a google drive file.
 
     Parameters
     ----------
     fid : str
         google drive id name of a file.
 
@@ -325,15 +325,15 @@
         DeprecationWarning,
     )
 
     if isinstance(id, requests.Response):
         response = id
     else:
         url = "https://drive.google.com/uc?export=download&id=" + fid
-        response = requests.get(url)
+        response = requests.get(url, timeout=timeout)
     header = response.headers["Content-Disposition"]
     file_name = re.search(r'filename="(.*)"', header).group(1)
     return file_name
 
 
 def download_file_from_google_drive(fid, destination=None):
     """download a file from google drive using it's id.
@@ -383,93 +383,14 @@
         if os.path.isdir(destination):
             filename = get_google_drive_filename(fid)
             destination = os.path.join(destination, filename)
 
     save_response_content(response, destination)
 
 
-# %% helper functions (from USGS)
-
-
-def get_platform(pltfrm):
-    """Determine the platform in order to construct the zip file name.
-
-    Source: USGS
-
-    Parameters
-    ----------
-    pltfrm : str, optional
-        check if platform string is correct for downloading binaries,
-        default is None and will determine platform string based on system
-
-    Returns
-    -------
-    pltfrm : str
-        return platform string
-    """
-    if pltfrm is None:
-        if sys.platform.lower() == "darwin":
-            pltfrm = "mac"
-        elif sys.platform.lower().startswith("linux"):
-            pltfrm = "linux"
-        elif "win" in sys.platform.lower():
-            is_64bits = sys.maxsize > 2**32
-            if is_64bits:
-                pltfrm = "win64"
-            else:
-                pltfrm = "win32"
-        else:
-            errmsg = "Could not determine platform" f".  sys.platform is {sys.platform}"
-            raise Exception(errmsg)
-    else:
-        assert pltfrm in ["mac", "linux", "win32", "win64"]
-    return pltfrm
-
-
-def getmfexes(pth=".", version="", pltfrm=None):
-    """Get the latest MODFLOW binary executables from a github site
-    (https://github.com/MODFLOW-USGS/executables) for the specified operating
-    system and put them in the specified path.
-
-    Source: USGS
-
-    Parameters
-    ----------
-    pth : str
-        Location to put the executables (default is current working directory)
-
-    version : str
-        Version of the MODFLOW-USGS/executables release to use.
-
-    pltfrm : str
-        Platform that will run the executables.  Valid values include mac,
-        linux, win32 and win64.  If platform is None, then routine will
-        download the latest appropriate zipfile from the github repository
-        based on the platform running this script.
-    """
-    try:
-        import pymake
-    except ModuleNotFoundError as e:
-        print(
-            "Install pymake with "
-            "`pip install "
-            "https://github.com/modflowpy/pymake/zipball/master`"
-        )
-        raise e
-    # Determine the platform in order to construct the zip file name
-    pltfrm = get_platform(pltfrm)
-    zipname = f"{pltfrm}.zip"
-
-    # Determine path for file download and then download and unzip
-    url = "https://github.com/MODFLOW-USGS/executables/" f"releases/download/{version}/"
-    assets = {p: url + p for p in ["mac.zip", "linux.zip", "win32.zip", "win64.zip"]}
-    download_url = assets[zipname]
-    pymake.download_and_unzip(download_url, pth)
-
-
 def get_heads_dataarray(ds, fill_nans=False, fname_hds=None):
     """reads the heads from a modflow .hds file and returns an xarray
     DataArray.
 
     Parameters
     ----------
     ds : TYPE
@@ -535,44 +456,49 @@
         if True the nan values are filled with the heads in the cells below
 
     Returns
     -------
     head_ar : np.ndarray
         heads array.
     """
+    logger.warning(
+        "nlmod.util.get_heads_array is deprecated. "
+        "Please use nlmod.gwf.get_heads_da instead"
+    )
     hdobj = flopy.utils.HeadFile(fname_hds)
     head = hdobj.get_alldata()
     head[head == 1e30] = np.nan
 
     if fill_nans:
         for lay in range(head.shape[1] - 2, -1, -1):
             head[:, lay] = np.where(
                 np.isnan(head[:, lay]), head[:, lay + 1], head[:, lay]
             )
     return head
 
 
-def download_mfbinaries(binpath=None, version="8.0"):
+def download_mfbinaries(bindir=None):
     """Download and unpack platform-specific modflow binaries.
 
     Source: USGS
 
     Parameters
     ----------
     binpath : str, optional
         path to directory to download binaries to, if it doesnt exist it
         is created. Default is None which sets dir to nlmod/bin.
     version : str, optional
         version string, by default 8.0
     """
-    if binpath is None:
-        binpath = os.path.join(os.path.dirname(__file__), "bin")
-    pltfrm = get_platform(None)
-    # Download and unpack mf6 exes
-    getmfexes(pth=binpath, version=version, pltfrm=pltfrm)
+
+    if bindir is None:
+        bindir = os.path.join(os.path.dirname(__file__), "bin")
+    if not os.path.isdir(bindir):
+        os.makedirs(bindir)
+    flopy.utils.get_modflow(bindir)
 
 
 def check_presence_mfbinaries(exe_name="mf6", binpath=None):
     """Check if exe_name is present in the binpath folder.
 
     Parameters
     ----------
```

### Comparing `nlmod-0.5.1/nlmod.egg-info/PKG-INFO` & `nlmod-0.5.2/nlmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlmod
-Version: 0.5.1
+Version: 0.5.2
 Summary: nlmod module by Artesia
 Home-page: https://github.com/ArtesiaWater/nlmod
 Author: Artesia
 License: MIT
 Platform: Windows
 Platform: Mac OS-X
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nlmod-0.5.1/nlmod.egg-info/SOURCES.txt` & `nlmod-0.5.2/nlmod.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,33 @@
 nlmod/dims/layers.py
 nlmod/dims/rdp.py
 nlmod/dims/resample.py
 nlmod/dims/time.py
 nlmod/gwf/__init__.py
 nlmod/gwf/gwf.py
 nlmod/gwf/horizontal_flow_barrier.py
+nlmod/gwf/lake.py
 nlmod/gwf/output.py
 nlmod/gwf/recharge.py
 nlmod/gwf/surface_water.py
 nlmod/gwf/wells.py
+nlmod/gwt/__init__.py
+nlmod/gwt/gwt.py
+nlmod/gwt/output.py
+nlmod/gwt/prepare.py
 nlmod/modpath/__init__.py
 nlmod/modpath/modpath.py
 nlmod/read/__init__.py
 nlmod/read/ahn.py
 nlmod/read/bgt.py
 nlmod/read/brp.py
 nlmod/read/geotop.py
 nlmod/read/jarkus.py
 nlmod/read/knmi.py
+nlmod/read/meteobase.py
 nlmod/read/regis.py
 nlmod/read/rws.py
 nlmod/read/waterboard.py
 nlmod/read/webservices.py
 nlmod/sim/__init__.py
 nlmod/sim/sim.py
 tests/test_001_model.py
@@ -57,9 +63,15 @@
 tests/test_003_mfpackages.py
 tests/test_004_northsea.py
 tests/test_005_external_data.py
 tests/test_006_caching.py
 tests/test_007_run_notebooks.py
 tests/test_008_waterschappen.py
 tests/test_009_layers.py
-tests/test_gwf_output.py
-tests/test_mtime.py
+tests/test_010_wells.py
+tests/test_011_dcs.py
+tests/test_012_plot.py
+tests/test_013_surface_water.py
+tests/test_014_gis.py
+tests/test_015_gwf_output.py
+tests/test_016_time.py
+tests/test_017_metbase.py
```

### Comparing `nlmod-0.5.1/setup.py` & `nlmod-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/tests/test_001_model.py` & `nlmod-0.5.2/tests/test_001_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,101 +9,65 @@
 tst_model_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)), "data")
 
 
 def test_model_directories(tmpdir):
     model_ws = os.path.join(tmpdir, "test_model")
     figdir, cachedir = nlmod.util.get_model_dirs(model_ws)
 
-    return model_ws, figdir, cachedir
 
-
-def test_ds_time_steady(tmpdir, modelname="test"):
+def get_ds_time_steady(tmpdir, modelname="test"):
     model_ws = os.path.join(tmpdir, "test_model")
     ds = nlmod.base.set_ds_attrs(xr.Dataset(), modelname, model_ws)
     ds = nlmod.time.set_ds_time(ds, start_time="2015-1-1", steady_state=True)
     return ds
 
 
-def test_ds_time_transient(tmpdir, modelname="test"):
+def get_ds_time_transient(tmpdir, modelname="test"):
     model_ws = os.path.join(tmpdir, "test_model")
     ds = nlmod.base.set_ds_attrs(xr.Dataset(), modelname, model_ws)
     ds = nlmod.time.set_ds_time(
         ds,
         start_time="2015-1-1",
         steady_state=False,
         steady_start=True,
         transient_timesteps=10,
     )
     return ds
 
 
 def test_get_ds():
     model_ws = os.path.join(tmpdir, "test_model_ds")
-    ds = nlmod.get_ds(
+    nlmod.get_ds(
         [-500, 500, -500, 500],
         delr=10.0,
         layer=3,
         top=0.0,
         botm=[-10, -20, -30],
         kh=[100, 1, 5],
         kv=[10, 0.1, 0.5],
         model_ws=model_ws,
         model_name="test_ds",
     )
 
-    ds
-
-    return ds
-
 
 def test_get_ds_variable_delrc():
     model_ws = os.path.join(tmpdir, "test_model_ds")
-    ds = nlmod.get_ds(
+    nlmod.get_ds(
         extent=[-500, 500, -500, 500],
         delr=[100] * 5 + [20] * 5 + [100] * 4,
         delc=[100] * 4 + [20] * 5 + [100] * 5,
         layer=3,
         top=0.0,
         botm=[-10, -20, -30],
         kh=[100, 1, 5],
         kv=[10, 0.1, 0.5],
         model_ws=model_ws,
         model_name="test_ds",
     )
 
-    ds
-
-    return ds
-
-
-@pytest.mark.slow
-def test_create_seamodel_grid_only_without_northsea(tmpdir, model_name="test"):
-    extent = [95000.0, 105000.0, 494000.0, 500000.0]
-    # extent, _, _ = nlmod.read.regis.fit_extent_to_regis(extent, 100, 100)
-    regis_geotop_ds = nlmod.read.regis.get_combined_layer_models(
-        extent, use_regis=True, use_geotop=True
-    )
-
-    ds = nlmod.base.to_model_ds(
-        regis_geotop_ds, model_name, str(tmpdir), delr=100.0, delc=100.0
-    )
-
-    ds = nlmod.time.set_ds_time(
-        ds,
-        start_time="2015-1-1",
-        steady_state=False,
-        steady_start=True,
-        transient_timesteps=10,
-    )
-
-    # save ds
-    ds.to_netcdf(os.path.join(tst_model_dir, "basic_sea_model.nc"))
-
-    return ds
-
 
 @pytest.mark.slow
 def test_create_small_model_grid_only(tmpdir, model_name="test"):
     extent = [98700.0, 99000.0, 489500.0, 489700.0]
     # extent, nrow, ncol = nlmod.read.regis.fit_extent_to_regis(extent, 100, 100)
     regis_geotop_ds = nlmod.read.regis.get_combined_layer_models(
         extent, regis_botm_layer="KRz5", use_regis=True, use_geotop=True
@@ -136,16 +100,14 @@
 
     # Create discretization
     _ = nlmod.gwf.dis(ds, gwf)
 
     # save ds
     ds.to_netcdf(os.path.join(tst_model_dir, "small_model.nc"))
 
-    return ds, gwf
-
 
 @pytest.mark.slow
 def test_create_sea_model_grid_only(tmpdir, model_name="test"):
     extent = [95000.0, 105000.0, 494000.0, 500000.0]
     # extent, nrow, ncol = nlmod.read.regis.fit_extent_to_regis(extent, 100, 100)
     regis_geotop_ds = nlmod.read.regis.get_combined_layer_models(
         extent, use_regis=True, use_geotop=True
@@ -160,37 +122,33 @@
         start_time="2015-1-1",
         steady_state=False,
         steady_start=True,
         transient_timesteps=10,
     )
 
     # save ds
-    ds.to_netcdf(os.path.join(tst_model_dir, "sea_model_grid.nc"))
-
-    return ds
+    ds.to_netcdf(os.path.join(tst_model_dir, "basic_sea_model.nc"))
 
 
 @pytest.mark.slow
 def test_create_sea_model_grid_only_delr_delc_50(tmpdir, model_name="test"):
-    ds = test_ds_time_transient(tmpdir)
+    ds = get_ds_time_transient(tmpdir)
     extent = [95000.0, 105000.0, 494000.0, 500000.0]
     # extent, nrow, ncol = nlmod.read.regis.fit_extent_to_regis(extent, 50.0, 50.0)
     regis_geotop_ds = nlmod.read.regis.get_combined_layer_models(
         extent, use_regis=True, use_geotop=True
     )
     model_ws = os.path.join(tmpdir, model_name)
     ds = nlmod.base.to_model_ds(
         regis_geotop_ds, model_name, model_ws, delr=50.0, delc=50.0
     )
 
     # save ds
     ds.to_netcdf(os.path.join(tst_model_dir, "sea_model_grid_50.nc"))
 
-    return ds
-
 
 @pytest.mark.slow
 def test_create_sea_model(tmpdir):
     ds = xr.open_dataset(
         os.path.join(tst_model_dir, "basic_sea_model.nc"), mask_and_scale=False
     )
     # create simulation
@@ -233,41 +191,41 @@
     # add knmi recharge to the model datasets
     ds.update(nlmod.read.knmi.get_recharge(ds))
     # create recharge package
     _ = nlmod.gwf.rch(ds, gwf)
 
     _ = nlmod.sim.write_and_run(sim, ds)
 
-    return ds, gwf
-
 
 @pytest.mark.slow
 def test_create_sea_model_perlen_list(tmpdir):
     ds = xr.open_dataset(os.path.join(tst_model_dir, "basic_sea_model.nc"))
 
+    # update model_ws
+    model_ws = os.path.join(tmpdir, "test_model_perlen_list")
+    ds = nlmod.base.set_ds_attrs(ds, ds.model_name, model_ws)
+
     # create transient with perlen list
     perlen = [3650, 14, 10, 11]  # length of the time steps
     transient_timesteps = 3
+    start_time = ds.time.start
+
+    # drop time dimension before setting time
+    ds = ds.drop_dims("time")
 
     # update current ds with new time dicretisation
-    model_ws = os.path.join(tmpdir, "test_model")
-    new_ds = nlmod.base.set_ds_attrs(xr.Dataset(), "test", model_ws)
-    new_ds = nlmod.time.set_ds_time(
-        new_ds,
-        start_time=ds.time.start,
+    ds = nlmod.time.set_ds_time(
+        ds,
+        start_time=start_time,
         steady_state=False,
         steady_start=True,
         perlen=perlen,
         transient_timesteps=transient_timesteps,
     )
 
-    # modfiy time
-    ds = ds.drop_dims("time")
-    ds.update(new_ds)
-
     # create simulation
     sim = nlmod.sim.sim(ds)
 
     # create time discretisation
     _ = nlmod.sim.tdis(ds, sim)
 
     # create groundwater flow model
@@ -304,40 +262,41 @@
     # add knmi recharge to the model datasets
     ds.update(nlmod.read.knmi.get_recharge(ds))
     # create recharge package
     nlmod.gwf.rch(ds, gwf)
 
     nlmod.sim.write_and_run(sim, ds)
 
-    return ds, gwf
-
 
 @pytest.mark.slow
 def test_create_sea_model_perlen_14(tmpdir):
     ds = xr.open_dataset(os.path.join(tst_model_dir, "basic_sea_model.nc"))
 
+    # update model_ws
+    model_ws = os.path.join(tmpdir, "test_model_perlen_14")
+    ds = nlmod.base.set_ds_attrs(ds, ds.model_name, model_ws)
+
     # create transient with perlen list
     perlen = 14  # length of the time steps
     transient_timesteps = 3
+    start_time = ds.time.start
+
+    # drop time dimension before setting time
+    ds = ds.drop_dims("time")
 
     # update current ds with new time dicretisation
-    model_ws = os.path.join(tmpdir, "test_model")
-    new_ds = nlmod.base.set_ds_attrs(xr.Dataset(), "test", model_ws)
-    new_ds = nlmod.time.set_ds_time(
-        new_ds,
-        start_time=ds.time.start,
+    ds = nlmod.time.set_ds_time(
+        ds,
+        start_time=start_time,
         steady_state=False,
         steady_start=True,
         perlen=perlen,
         transient_timesteps=transient_timesteps,
     )
 
-    ds = ds.drop_dims("time")
-    ds.update(new_ds)
-
     # create simulation
     sim = nlmod.sim.sim(ds)
 
     # create time discretisation
     _ = nlmod.sim.tdis(ds, sim)
 
     # create ims
@@ -374,21 +333,18 @@
     # add knmi recharge to the model datasets
     ds.update(nlmod.read.knmi.get_recharge(ds))
     # create recharge package
     nlmod.gwf.rch(ds, gwf)
 
     nlmod.sim.write_and_run(sim, ds)
 
-    return ds, gwf
-
 
 # obtaining the test models
-def test_get_ds_from_cache(name="small_model"):
+def get_ds_from_cache(name="small_model"):
     ds = xr.open_dataset(os.path.join(tst_model_dir, name + ".nc"))
-
     return ds
 
 
 # other functions
 def _check_tmpdir(tmpdir):
     # pytest uses a LocalPath object for the tmpdir argument when testing
     # this function convert a LocalPath object to a string
```

### Comparing `nlmod-0.5.1/tests/test_002_regis_geotop.py` & `nlmod-0.5.2/tests/test_002_regis_geotop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 # -*- coding: utf-8 -*-
 """Created on Thu Jan  7 16:23:35 2021.
 
 @author: oebbe
 """
 
 import nlmod
-from nlmod.read import geotop, regis
-
-import test_001_model
 
 
 # @pytest.mark.skip(reason="too slow")
 def test_get_regis(extent=[98600.0, 99000.0, 489400.0, 489700.0]):
-    regis_ds = regis.get_regis(extent)
+    regis_ds = nlmod.read.regis.get_regis(extent)
 
     assert regis_ds.dims["layer"] == 20
 
-    return regis_ds
-
 
 # @pytest.mark.skip(reason="too slow")
 def test_get_regis_botm_layer_BEk1(
     extent=[98700.0, 99000.0, 489500.0, 489700.0],
     botm_layer="MSc",
 ):
-    regis_ds = regis.get_regis(extent, botm_layer)
+    regis_ds = nlmod.read.regis.get_regis(extent, botm_layer)
     assert regis_ds.dims["layer"] == 15
     assert regis_ds.layer.values[-1] == botm_layer
-    return regis_ds
+
+
+def test_get_geotop_raw(extent=[98600.0, 99000.0, 489400.0, 489700.0]):
+    geotop_ds = nlmod.read.geotop.get_geotop_raw_within_extent(extent)
+    line = [(extent[0], extent[2]), (extent[1], extent[3])]
+    # also test the plot-method
+    nlmod.plot.geotop_lithok_in_cross_section(line, geotop_ds)
 
 
 # @pytest.mark.skip(reason="too slow")
 def test_get_geotop(extent=[98600.0, 99000.0, 489400.0, 489700.0]):
-    geotop_ds = geotop.get_geotop(extent)
-    return geotop_ds
+    nlmod.read.geotop.get_geotop(extent)
 
 
 # @pytest.mark.skip(reason="too slow")
 def test_get_regis_geotop(extent=[98600.0, 99000.0, 489400.0, 489700.0]):
-    regis_geotop_ds = regis.get_combined_layer_models(
+    regis_geotop_ds = nlmod.read.regis.get_combined_layer_models(
         extent, use_regis=True, use_geotop=True
     )
     regis_geotop_ds = nlmod.base.to_model_ds(regis_geotop_ds)
     assert regis_geotop_ds.dims["layer"] == 24
-    return regis_geotop_ds
 
 
 # @pytest.mark.skip(reason="too slow")
 def test_get_regis_geotop_keep_all_layers(
     extent=[98600.0, 99000.0, 489400.0, 489700.0],
 ):
-    regis_geotop_ds = regis.get_combined_layer_models(
+    regis_geotop_ds = nlmod.read.regis.get_combined_layer_models(
         extent, use_regis=True, use_geotop=True, remove_nan_layers=False
     )
     assert regis_geotop_ds.dims["layer"] == 137
-    return regis_geotop_ds
```

### Comparing `nlmod-0.5.1/tests/test_003_mfpackages.py` & `nlmod-0.5.2/tests/test_003_mfpackages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # -*- coding: utf-8 -*-
 """Created on Thu Jan  7 16:24:03 2021.
 
 @author: oebbe
 """
 import nlmod
-import pytest
-
 import test_001_model
 
 
-def test_sim_tdis_gwf_ims_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("basic_sea_model")
+def sim_tdis_gwf_ims_from_ds(tmpdir):
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # create simulation
     sim = nlmod.sim.sim(ds)
 
     # create time discretisation
     _ = nlmod.sim.tdis(ds, sim)
 
@@ -24,91 +22,66 @@
     # create groundwater flow model
     gwf = nlmod.gwf.gwf(ds, sim)
 
     return sim, gwf
 
 
 def dis_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
-
-    dis = nlmod.gwf.dis(ds, gwf)
-
-    return dis
+    ds = test_001_model.get_ds_from_cache("small_model")
 
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
 
-@pytest.mark.slow
-def disv_from_ds(tmpdir):
-    ds, gwf, gridprops = test_001_model.test_create_inf_panden_model(tmpdir)
-
-    disv = nlmod.gwf.disv(ds, gwf, gridprops)
-
-    return disv
+    nlmod.gwf.dis(ds, gwf)
 
 
 def npf_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
+    ds = test_001_model.get_ds_from_cache("small_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
     nlmod.gwf.dis(ds)
-    npf = nlmod.gwf.npf(ds, gwf)
-
-    return npf
+    nlmod.gwf.npf(ds, gwf)
 
 
 def oc_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
-    oc = nlmod.gwf.oc(ds, gwf)
-
-    return oc
+    ds = test_001_model.get_ds_from_cache("small_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
+    nlmod.gwf.oc(ds, gwf)
 
 
 def sto_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
-    sto = nlmod.gwf.sto(ds, gwf)
-
-    return sto
+    ds = test_001_model.get_ds_from_cache("small_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
+    nlmod.gwf.sto(ds, gwf)
 
 
 def ghb_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("full_sea_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
+    ds = test_001_model.get_ds_from_cache("full_sea_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
     _ = nlmod.gwf.dis(ds, gwf)
 
-    ghb = nlmod.gwf.ghb(ds, gwf, "surface_water")
-
-    return ghb
+    nlmod.gwf.ghb(ds, gwf, "surface_water")
 
 
 def rch_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("full_sea_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
+    ds = test_001_model.get_ds_from_cache("full_sea_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
     _ = nlmod.gwf.dis(ds, gwf)
 
-    rch = nlmod.gwf.rch(ds, gwf)
-
-    return rch
+    nlmod.gwf.rch(ds, gwf)
 
 
 def drn_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("full_sea_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
+    ds = test_001_model.get_ds_from_cache("full_sea_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
     _ = nlmod.gwf.dis(ds, gwf)
-    drn = nlmod.gwf.surface_drain_from_ds(ds, gwf, 1.0)
-
-    return drn
+    nlmod.gwf.surface_drain_from_ds(ds, gwf, 1.0)
 
 
 def chd_from_ds(tmpdir):
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-    _, gwf = test_sim_tdis_gwf_ims_from_ds(tmpdir)
+    ds = test_001_model.get_ds_from_cache("small_model")
+    _, gwf = sim_tdis_gwf_ims_from_ds(tmpdir)
     _ = nlmod.gwf.dis(ds, gwf)
 
     _ = nlmod.gwf.ic(ds, gwf, starting_head=1.0)
 
     # add constant head cells at model boundaries
     ds.update(nlmod.grid.mask_model_edge(ds, ds["idomain"]))
-    chd = nlmod.gwf.chd(ds, gwf, chd="edge_mask", head="starting_head")
-
-    return chd
+    nlmod.gwf.chd(ds, gwf, chd="edge_mask", head="starting_head")
```

### Comparing `nlmod-0.5.1/tests/test_004_northsea.py` & `nlmod-0.5.2/tests/test_004_northsea.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,102 +2,82 @@
 
 import nlmod
 
 import test_001_model
 
 
 def test_get_gdf_opp_water():
-    ds = test_001_model.test_get_ds_from_cache()
-    gdf_surface_water = nlmod.read.rws.get_gdf_surface_water(ds)
-
-    return gdf_surface_water
+    ds = test_001_model.get_ds_from_cache()
+    nlmod.read.rws.get_gdf_surface_water(ds)
 
 
 def test_surface_water_to_dataset():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("sea_model_grid")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
     name = "surface_water"
-    ds_surfwat = nlmod.read.rws.get_surface_water(ds, name)
-
-    return ds_surfwat
+    nlmod.read.rws.get_surface_water(ds, name)
 
 
 def test_get_northsea_seamodel():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("basic_sea_model")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
     ds_sea = nlmod.read.rws.get_northsea(ds)
 
     assert (ds_sea.northsea == 1).sum() > 0
 
-    return ds_sea
-
 
 def test_get_northsea_nosea():
     # model without sea
-    ds = test_001_model.test_get_ds_from_cache("small_model")
+    ds = test_001_model.get_ds_from_cache("small_model")
     ds_sea = nlmod.read.rws.get_northsea(ds)
 
     assert (ds_sea.northsea == 1).sum() == 0
 
-    return ds_sea
-
 
 def test_fill_top_bot_kh_kv_seamodel():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("basic_sea_model")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
     ds.update(nlmod.read.rws.get_northsea(ds))
 
     fal = nlmod.layers.get_first_active_layer(ds)
     fill_mask = (fal == fal._FillValue) * ds["northsea"]
-    ds = nlmod.layers.fill_top_bot_kh_kv_at_mask(ds, fill_mask)
-
-    return ds
+    nlmod.layers.fill_top_bot_kh_kv_at_mask(ds, fill_mask)
 
 
 def test_fill_top_bot_kh_kv_nosea():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("small_model")
+    ds = test_001_model.get_ds_from_cache("small_model")
     ds.update(nlmod.read.rws.get_northsea(ds))
 
     fal = nlmod.layers.get_first_active_layer(ds)
     fill_mask = (fal == fal._FillValue) * ds["northsea"]
-    ds = nlmod.layers.fill_top_bot_kh_kv_at_mask(ds, fill_mask)
-
-    return ds
+    nlmod.layers.fill_top_bot_kh_kv_at_mask(ds, fill_mask)
 
 
 def test_get_bathymetry_seamodel():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("basic_sea_model")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
     ds.update(nlmod.read.rws.get_northsea(ds))
     ds_bathymetry = nlmod.read.jarkus.get_bathymetry(ds, ds["northsea"])
 
     assert (~ds_bathymetry.bathymetry.isnull()).sum() > 0
 
-    return ds_bathymetry
-
 
 def test_get_bathymetrie_nosea():
     # model without sea
-    ds = test_001_model.test_get_ds_from_cache("small_model")
+    ds = test_001_model.get_ds_from_cache("small_model")
     ds.update(nlmod.read.rws.get_northsea(ds))
     ds_bathymetry = nlmod.read.jarkus.get_bathymetry(ds, ds["northsea"])
 
     assert (~ds_bathymetry.bathymetry.isnull()).sum() == 0
 
-    return ds_bathymetry
-
 
 def test_add_bathymetrie_to_top_bot_kh_kv_seamodel():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("basic_sea_model")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
     ds.update(nlmod.read.rws.get_northsea(ds))
     ds.update(nlmod.read.jarkus.get_bathymetry(ds, ds["northsea"]))
 
     fal = nlmod.layers.get_first_active_layer(ds)
     fill_mask = (fal == fal._FillValue) * ds["northsea"]
 
-    ds = nlmod.read.jarkus.add_bathymetry_to_top_bot_kh_kv(
-        ds, ds["bathymetry"], fill_mask
-    )
-
-    return ds
+    nlmod.read.jarkus.add_bathymetry_to_top_bot_kh_kv(ds, ds["bathymetry"], fill_mask)
```

### Comparing `nlmod-0.5.1/tests/test_005_external_data.py` & `nlmod-0.5.2/tests/test_005_external_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 import nlmod
 
 import test_001_model
 
 
 def test_get_recharge():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("sea_model_grid")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # add knmi recharge to the model dataset
     ds.update(nlmod.read.knmi.get_recharge(ds))
 
-    return ds
-
 
 def test_get_recharge_steady_state():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("sea_model_grid")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # modify mtime
     ds = ds.drop_dims("time")
     ds = nlmod.time.set_ds_time(ds, start_time="2000-1-1", perlen=3650)
 
     # add knmi recharge to the model dataset
     ds.update(nlmod.read.knmi.get_recharge(ds))
 
-    return ds
-
 
 def test_ahn_within_extent():
     extent = [95000.0, 105000.0, 494000.0, 500000.0]
     da = nlmod.read.ahn.get_ahn_from_wcs(extent)
 
     assert not da.isnull().all(), "AHN only has nan values"
 
-    return da
-
 
 def test_ahn_split_extent():
     extent = [95000.0, 105000.0, 494000.0, 500000.0]
     da = nlmod.read.ahn.get_ahn_from_wcs(extent, maxsize=1000)
 
     assert not da.isnull().all(), "AHN only has nan values"
 
-    return da
-
 
 def test_get_ahn3():
     extent = [98000.0, 100000.0, 494000.0, 496000.0]
     da = nlmod.read.ahn.get_ahn3(extent)
 
     assert not da.isnull().all(), "AHN only has nan values"
 
@@ -57,27 +49,25 @@
     da = nlmod.read.ahn.get_ahn4(extent)
 
     assert not da.isnull().all(), "AHN only has nan values"
 
 
 def test_get_ahn():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("sea_model_grid")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # add ahn data to the model dataset
     ahn_ds = nlmod.read.ahn.get_ahn(ds)
 
     assert not ahn_ds["ahn"].isnull().all(), "AHN only has nan values"
 
-    return ahn_ds
-
 
 def test_get_surface_water_ghb():
     # model with sea
-    ds = test_001_model.test_get_ds_from_cache("sea_model_grid")
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
 
     # create simulation
     sim = nlmod.sim.sim(ds)
 
     # create time discretisation
     tdis = nlmod.sim.tdis(ds, sim)
 
@@ -88,13 +78,11 @@
     ims = nlmod.sim.ims(sim)
 
     nlmod.gwf.dis(ds, gwf)
 
     # add surface water levels to the model dataset
     ds.update(nlmod.read.rws.get_surface_water(ds, "surface_water"))
 
-    return ds
-
 
 def test_get_brp():
     extent = [116500, 120000, 439000, 442000]
-    return nlmod.read.brp.get_percelen(extent)
+    nlmod.read.brp.get_percelen(extent)
```

### Comparing `nlmod-0.5.1/tests/test_006_caching.py` & `nlmod-0.5.2/tests/test_006_caching.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,75 +12,73 @@
 import test_001_model
 
 tmpdir = tempfile.gettempdir()
 
 
 def test_ds_check_true():
     # two models with the same grid and time dicretisation
-    ds = test_001_model.test_get_ds_from_cache("small_model")
+    ds = test_001_model.get_ds_from_cache("small_model")
     ds2 = ds.copy()
 
     check = nlmod.cache._check_ds(ds, ds2)
 
     assert check
 
 
 def test_ds_check_time_false():
     # two models with a different time discretisation
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-    ds2 = test_001_model.test_ds_time_steady(tmpdir)
+    ds = test_001_model.get_ds_from_cache("small_model")
+    ds2 = test_001_model.get_ds_time_steady(tmpdir)
 
     check = nlmod.cache._check_ds(ds, ds2)
 
-    assert check == False
+    assert not check
 
 
 def test_ds_check_time_attributes_false():
     # two models with a different time discretisation
-    ds = test_001_model.test_get_ds_from_cache("small_model")
+    ds = test_001_model.get_ds_from_cache("small_model")
     ds2 = ds.copy()
 
     ds2.time.attrs["time_units"] = "MONTHS"
 
     check = nlmod.cache._check_ds(ds, ds2)
 
-    assert check == False
+    assert not check
 
 
 @pytest.mark.slow
 def test_ds_check_grid_false(tmpdir):
     # two models with a different grid and same time dicretisation
-    ds = test_001_model.test_get_ds_from_cache("small_model")
-    ds2 = test_001_model.test_ds_time_transient(tmpdir)
+    ds = test_001_model.get_ds_from_cache("small_model")
+    ds2 = test_001_model.get_ds_time_transient(tmpdir)
     extent = [99100.0, 99400.0, 489100.0, 489400.0]
     regis_ds = nlmod.read.regis.get_combined_layer_models(
         extent,
         use_regis=True,
         use_geotop=False,
         cachedir=tmpdir,
         cachename="comb.nc",
     )
     ds2 = nlmod.base.to_model_ds(regis_ds, delr=50.0, delc=50.0)
 
     check = nlmod.cache._check_ds(ds, ds2)
 
-    assert check == False
+    assert not check
 
 
 @pytest.mark.skip("too slow")
 def test_use_cached_regis(tmpdir):
     extent = [98700.0, 99000.0, 489500.0, 489700.0]
     regis_ds1 = nlmod.read.regis.get_regis(extent, cachedir=tmpdir, cachename="reg.nc")
 
     regis_ds2 = nlmod.read.regis.get_regis(extent, cachedir=tmpdir, cachename="reg.nc")
 
     assert regis_ds1.equals(regis_ds2)
 
-    return regis_ds2
-
 
 @pytest.mark.skip("too slow")
 def test_do_not_use_cached_regis(tmpdir):
     # cache regis
     extent = [98700.0, 99000.0, 489500.0, 489700.0]
     regis_ds1 = nlmod.read.regis.get_regis(
         extent, cachedir=tmpdir, cachename="regis.nc"
@@ -89,9 +87,7 @@
     # do not use cache because extent is different
     extent = [99100.0, 99400.0, 489100.0, 489400.0]
     regis_ds2 = nlmod.read.regis.get_regis(
         extent, cachedir=tmpdir, cachename="regis.nc"
     )
 
     assert not regis_ds1.equals(regis_ds2)
-
-    return regis_ds2
```

### Comparing `nlmod-0.5.1/tests/test_007_run_notebooks.py` & `nlmod-0.5.2/tests/test_007_run_notebooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,19 @@
     ep = ExecutePreprocessor(timeout=6000)
     out = ep.preprocess(nb, {"metadata": {"path": nbdir}})
 
     return out
 
 
 @pytest.mark.notebooks
+def test_run_notebook_00_model_from_scratch():
+    _run_notebook(nbdir, "00_model_from_scratch.ipynb")
+
+
+@pytest.mark.notebooks
 def test_run_notebook_01_basic_model():
     _run_notebook(nbdir, "01_basic_model.ipynb")
 
 
 @pytest.mark.notebooks
 def test_run_notebook_02_surface_water():
     _run_notebook(nbdir, "02_surface_water.ipynb")
@@ -31,15 +36,14 @@
 
 @pytest.mark.notebooks
 def test_run_notebook_03_local_grid_refinement():
     _run_notebook(nbdir, "03_local_grid_refinement.ipynb")
 
 
 @pytest.mark.notebooks
-@pytest.mark.skip("requires art_tools")
 def test_run_notebook_04_modifying_layermodels():
     _run_notebook(nbdir, "04_modifying_layermodels.ipynb")
 
 
 @pytest.mark.notebooks
 def test_run_notebook_05_caching():
     _run_notebook(nbdir, "05_caching.ipynb")
@@ -47,14 +51,19 @@
 
 @pytest.mark.notebooks
 def test_run_notebook_06_compare_layermodels():
     _run_notebook(nbdir, "06_compare_layermodels.ipynb")
 
 
 @pytest.mark.notebooks
+def test_run_notebook_07_gridding_vector_data():
+    _run_notebook(nbdir, "07_gridding_vector_data.ipynb")
+
+
+@pytest.mark.notebooks
 def test_run_notebook_07_resampling():
     _run_notebook(nbdir, "07_resampling.ipynb")
 
 
 @pytest.mark.notebooks
 def test_run_notebook_08_gis():
     _run_notebook(nbdir, "08_gis.ipynb")
@@ -79,7 +88,22 @@
 def test_run_notebook_12_layer_generation():
     _run_notebook(nbdir, "12_layer_generation.ipynb")
 
 
 @pytest.mark.notebooks
 def test_run_notebook_13_plot_methods():
     _run_notebook(nbdir, "13_plot_methods.ipynb")
+
+
+@pytest.mark.notebooks
+def test_run_notebook_14_stromingen_example():
+    _run_notebook(nbdir, "14_stromingen_example.ipynb")
+
+
+@pytest.mark.notebooks
+def test_run_notebook_15_geotop():
+    _run_notebook(nbdir, "15_geotop.ipynb")
+
+
+@pytest.mark.notebooks
+def test_run_notebook_16_groundwater_transport():
+    _run_notebook(nbdir, "16_groundwater_transport.ipynb")
```

### Comparing `nlmod-0.5.1/tests/test_008_waterschappen.py` & `nlmod-0.5.2/tests/test_008_waterschappen.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 """
 
 import nlmod
 import pytest
 
 
 def test_download_polygons():
-    return nlmod.read.waterboard.get_polygons()
+    nlmod.read.waterboard.get_polygons()
 
 
 def test_get_config():
-    return nlmod.read.waterboard.get_configuration()
+    nlmod.read.waterboard.get_configuration()
 
 
 def test_bgt_waterboards():
     extent = [116500, 120000, 439000, 442000]
     bgt = nlmod.read.bgt.get_bgt(extent)
-    pg = nlmod.gwf.surface_water.download_level_areas(bgt, extent=extent)
-    bgt = nlmod.gwf.surface_water.add_stages_from_waterboards(bgt, pg=pg)
-    return bgt
+    la = nlmod.gwf.surface_water.download_level_areas(
+        bgt, extent=extent, raise_exceptions=False
+    )
+    bgt = nlmod.gwf.surface_water.add_stages_from_waterboards(bgt, la=la)
 
 
 @pytest.mark.skip("too slow")
 def test_download_peilgebieden(plot=True):
     waterboards = nlmod.read.waterboard.get_polygons()
     data_kind = "level_areas"
 
@@ -71,15 +72,15 @@
         # elif wb == "Brabantse Delta":
         #    extent = [100000, 105000, 405000, 410000]
         # elif wb == "Waterschap Scheldestromen":
         #    extent = [57000, 58000, 378000, 379000]
         return extent
 
     data_kind = "watercourses"
-    # data_kind = "peilgebieden"
+    # data_kind = "level_areas"
     waterboards = nlmod.read.waterboard.get_polygons()
     gdf = {}
     for wb in waterboards.index:
         print(wb)
         extent = get_extent(waterboards, wb)
         try:
             gdf[wb] = nlmod.read.waterboard.get_data(wb, data_kind, extent)
```

### Comparing `nlmod-0.5.1/tests/test_009_layers.py` & `nlmod-0.5.2/tests/test_009_layers.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.1/tests/test_gwf_output.py` & `nlmod-0.5.2/tests/test_015_gwf_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import tempfile
+import test_001_model
 
 import nlmod
 import numpy as np
 from nlmod.gwf import get_heads_da
 from nlmod.dims.grid import refine
 
 tmpdir = tempfile.gettempdir()
@@ -124,7 +125,13 @@
     fname_hds = os.path.join(ds.model_ws, ds.model_name + ".hds")
     da = get_heads_da(ds=ds_unstr, gwf=None, fname_hds=fname_hds)
     assert np.array_equal(da.values, heads_correct, equal_nan=True)
 
     fname_hds = os.path.join(ds.model_ws, ds.model_name + ".hds")
     da = get_heads_da(ds=None, gwf=gwf_unstr, fname_hds=fname_hds)
     assert np.array_equal(da.values, heads_correct, equal_nan=True)
+
+
+def test_gxg():
+    ds = test_001_model.get_ds_from_cache("basic_sea_model")
+    head = nlmod.gwf.get_heads_da(ds)
+    nlmod.gwf.calculate_gxg(head)
```

