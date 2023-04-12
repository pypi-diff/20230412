# Comparing `tmp/nlmod-0.5.2.tar.gz` & `tmp/nlmod-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlmod-0.5.2.tar", last modified: Wed Apr 12 10:40:27 2023, max compression
+gzip compressed data, was "nlmod-0.5.3.tar", last modified: Wed Apr 12 17:24:24 2023, max compression
```

## Comparing `nlmod-0.5.2.tar` & `nlmod-0.5.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.349893 nlmod-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-12 10:40:07.000000 nlmod-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 10:40:27.349893 nlmod-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 10:40:07.000000 nlmod-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.337893 nlmod-0.5.2/nlmod/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/data/geotop/
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/geotop/geo_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/geotop/litho_eenheden.csv
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.cpg
--rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.dbf
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.prj
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.qpj
--rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.shp
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/opp_water.shx
--rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/data/regis_2_2.gleg
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/dims/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    55292 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    35438 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/dims/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.341893 nlmod-0.5.2/nlmod/gwf/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/gwf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/horizontal_flow_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/lake.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/recharge.py
--rw-r--r--   0 runner    (1001) docker     (123)    36376 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwf/wells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/gwt/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/gwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/gwt/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/modpath/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/modpath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/modpath/modpath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/read/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/ahn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/bgt.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/brp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/jarkus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/knmi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/meteobase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/regis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/rws.py
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/waterboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/read/webservices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.345893 nlmod-0.5.2/nlmod/sim/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/sim/sim.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 10:40:07.000000 nlmod-0.5.2/nlmod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.337893 nlmod-0.5.2/nlmod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 10:40:27.000000 nlmod-0.5.2/nlmod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 10:40:27.349893 nlmod-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 10:40:07.000000 nlmod-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:40:27.349893 nlmod-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_001_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_002_regis_geotop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_003_mfpackages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_004_northsea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_005_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_006_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_007_run_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_008_waterschappen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_009_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_010_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_011_dcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_012_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_013_surface_water.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_014_gis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_015_gwf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_016_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 10:40:07.000000 nlmod-0.5.2/tests/test_017_metbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.495427 nlmod-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-12 17:24:14.000000 nlmod-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 17:24:24.495427 nlmod-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-12 17:24:14.000000 nlmod-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.483427 nlmod-0.5.3/nlmod/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.487427 nlmod-0.5.3/nlmod/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.487427 nlmod-0.5.3/nlmod/data/geotop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/geotop/geo_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/geotop/litho_eenheden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.cpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39628 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.dbf
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.prj
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.qpj
+-rw-r--r--   0 runner    (1001) docker     (123)  2803244 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.shp
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/opp_water.shx
+-rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/data/regis_2_2.gleg
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.487427 nlmod-0.5.3/nlmod/dims/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55292 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35438 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21894 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/dims/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/gwf/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/gwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/horizontal_flow_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/recharge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwf/wells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/gwt/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/gwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/gwt/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/modpath/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/modpath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/modpath/modpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/ahn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/bgt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/brp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/jarkus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/meteobase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/regis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/rws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/waterboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/read/webservices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.491427 nlmod-0.5.3/nlmod/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/sim/sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 17:24:14.000000 nlmod-0.5.3/nlmod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.483427 nlmod-0.5.3/nlmod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 17:24:24.000000 nlmod-0.5.3/nlmod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:24:24.495427 nlmod-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 17:24:14.000000 nlmod-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:24:24.495427 nlmod-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_001_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_002_regis_geotop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_003_mfpackages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_004_northsea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_005_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_006_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_007_run_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_008_waterschappen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_009_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_010_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_011_dcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_012_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_013_surface_water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_014_gis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_015_gwf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_016_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 17:24:14.000000 nlmod-0.5.3/tests/test_017_metbase.py
```

### Comparing `nlmod-0.5.2/LICENSE` & `nlmod-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/PKG-INFO` & `nlmod-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlmod
-Version: 0.5.2
+Version: 0.5.3
 Summary: nlmod module by Artesia
 Home-page: https://github.com/ArtesiaWater/nlmod
 Author: Artesia
 License: MIT
 Platform: Windows
 Platform: Mac OS-X
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nlmod-0.5.2/README.md` & `nlmod-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/cache.py` & `nlmod-0.5.3/nlmod/cache.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/data/geotop/geo_eenheden.csv` & `nlmod-0.5.3/nlmod/data/geotop/geo_eenheden.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv` & `nlmod-0.5.3/nlmod/data/geotop/hydraulische_parameterisering_geotop_noord-brabant_en_noord-_en_midden-limburg.csv`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/data/opp_water.dbf` & `nlmod-0.5.3/nlmod/data/opp_water.dbf`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/data/opp_water.qpj` & `nlmod-0.5.3/nlmod/data/opp_water.qpj`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/data/opp_water.shp` & `nlmod-0.5.3/nlmod/data/opp_water.shp`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/data/regis_2_2.gleg` & `nlmod-0.5.3/nlmod/data/regis_2_2.gleg`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dcs.py` & `nlmod-0.5.3/nlmod/dcs.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dims/base.py` & `nlmod-0.5.3/nlmod/dims/base.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dims/grid.py` & `nlmod-0.5.3/nlmod/dims/grid.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dims/layers.py` & `nlmod-0.5.3/nlmod/dims/layers.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dims/rdp.py` & `nlmod-0.5.3/nlmod/dims/rdp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dims/resample.py` & `nlmod-0.5.3/nlmod/dims/resample.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/dims/time.py` & `nlmod-0.5.3/nlmod/dims/time.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gis.py` & `nlmod-0.5.3/nlmod/gis.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwf/gwf.py` & `nlmod-0.5.3/nlmod/gwf/gwf.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwf/horizontal_flow_barrier.py` & `nlmod-0.5.3/nlmod/gwf/horizontal_flow_barrier.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwf/lake.py` & `nlmod-0.5.3/nlmod/gwf/lake.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwf/output.py` & `nlmod-0.5.3/nlmod/gwf/output.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwf/recharge.py` & `nlmod-0.5.3/nlmod/gwf/recharge.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwf/surface_water.py` & `nlmod-0.5.3/nlmod/gwf/surface_water.py`

 * *Files 0% similar despite different names*

```diff
@@ -704,15 +704,15 @@
     if columns is None:
         columns = ["summer_stage", "winter_stage"]
     gdf[columns] = np.NaN
     for wb in la.keys():
         if len(la[wb]) == 0:
             continue
         mask = gdf["bronhouder"] == config[wb]["bgt_code"]
-        gdf[mask] = add_info_to_gdf(
+        gdf.loc[mask] = add_info_to_gdf(
             la[wb],
             gdf[mask],
             columns=columns,
             min_total_overlap=min_total_overlap,
             desc=f"Adding {columns} from {wb}",
         )
     return gdf
@@ -760,15 +760,15 @@
     if columns is None:
         columns = ["bottom_height"]
     gdf[columns] = np.NaN
     for wb in wc.keys():
         if len(wc[wb]) == 0:
             continue
         mask = gdf["bronhouder"] == config[wb]["bgt_code"]
-        gdf[mask] = add_info_to_gdf(
+        gdf.loc[mask] = add_info_to_gdf(
             wc[wb],
             gdf[mask],
             columns=columns,
             min_total_overlap=min_total_overlap,
             desc=f"Adding {columns} from {wb}",
             geom_type=None,
         )
```

### Comparing `nlmod-0.5.2/nlmod/gwf/wells.py` & `nlmod-0.5.3/nlmod/gwf/wells.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwt/gwt.py` & `nlmod-0.5.3/nlmod/gwt/gwt.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwt/output.py` & `nlmod-0.5.3/nlmod/gwt/output.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/gwt/prepare.py` & `nlmod-0.5.3/nlmod/gwt/prepare.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/modpath/modpath.py` & `nlmod-0.5.3/nlmod/modpath/modpath.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/plot.py` & `nlmod-0.5.3/nlmod/plot.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/ahn.py` & `nlmod-0.5.3/nlmod/read/ahn.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/bgt.py` & `nlmod-0.5.3/nlmod/read/bgt.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/brp.py` & `nlmod-0.5.3/nlmod/read/brp.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/geotop.py` & `nlmod-0.5.3/nlmod/read/geotop.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/jarkus.py` & `nlmod-0.5.3/nlmod/read/jarkus.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/knmi.py` & `nlmod-0.5.3/nlmod/read/knmi.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/meteobase.py` & `nlmod-0.5.3/nlmod/read/meteobase.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/regis.py` & `nlmod-0.5.3/nlmod/read/regis.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/rws.py` & `nlmod-0.5.3/nlmod/read/rws.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/waterboard.py` & `nlmod-0.5.3/nlmod/read/waterboard.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/read/webservices.py` & `nlmod-0.5.3/nlmod/read/webservices.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/sim/sim.py` & `nlmod-0.5.3/nlmod/sim/sim.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/util.py` & `nlmod-0.5.3/nlmod/util.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/nlmod/version.py` & `nlmod-0.5.3/nlmod/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib import metadata
 from platform import python_version
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 
 def show_versions() -> None:
     """Method to print the version of dependencies."""
 
     msg = (
         f"Python version: {python_version()}\n"
```

### Comparing `nlmod-0.5.2/nlmod.egg-info/PKG-INFO` & `nlmod-0.5.3/nlmod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlmod
-Version: 0.5.2
+Version: 0.5.3
 Summary: nlmod module by Artesia
 Home-page: https://github.com/ArtesiaWater/nlmod
 Author: Artesia
 License: MIT
 Platform: Windows
 Platform: Mac OS-X
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nlmod-0.5.2/nlmod.egg-info/SOURCES.txt` & `nlmod-0.5.3/nlmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/setup.py` & `nlmod-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_001_model.py` & `nlmod-0.5.3/tests/test_001_model.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_002_regis_geotop.py` & `nlmod-0.5.3/tests/test_002_regis_geotop.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_003_mfpackages.py` & `nlmod-0.5.3/tests/test_003_mfpackages.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_004_northsea.py` & `nlmod-0.5.3/tests/test_004_northsea.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_005_external_data.py` & `nlmod-0.5.3/tests/test_005_external_data.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_006_caching.py` & `nlmod-0.5.3/tests/test_006_caching.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_007_run_notebooks.py` & `nlmod-0.5.3/tests/test_007_run_notebooks.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_008_waterschappen.py` & `nlmod-0.5.3/tests/test_008_waterschappen.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_009_layers.py` & `nlmod-0.5.3/tests/test_009_layers.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_010_wells.py` & `nlmod-0.5.3/tests/test_010_wells.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_012_plot.py` & `nlmod-0.5.3/tests/test_012_plot.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_013_surface_water.py` & `nlmod-0.5.3/tests/test_013_surface_water.py`

 * *Files identical despite different names*

### Comparing `nlmod-0.5.2/tests/test_015_gwf_output.py` & `nlmod-0.5.3/tests/test_015_gwf_output.py`

 * *Files identical despite different names*

