# Comparing `tmp/openpmd-beamphysics-0.7.4.tar.gz` & `tmp/openpmd-beamphysics-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-sonb4e8x/openpmd-beamphysics-0.7.4.tar", last modified: Wed Mar 22 01:23:55 2023, max compression
+gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-8hlxxxtb/openpmd-beamphysics-0.7.5.tar", last modified: Wed Apr 12 21:26:55 2023, max compression
```

## Comparing `openpmd-beamphysics-0.7.4.tar` & `openpmd-beamphysics-0.7.5.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-22 01:23:41.000000 openpmd-beamphysics-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-22 01:23:41.000000 openpmd-beamphysics-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-22 01:23:41.000000 openpmd-beamphysics-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/fieldmesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/ansys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/astra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/bmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/elegant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/genesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/litrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/lucretia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/opal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/superfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/species.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/pmd_beamphysics/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 01:23:55.000000 openpmd-beamphysics-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/tests/test_particlegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-03-22 01:23:42.000000 openpmd-beamphysics-0.7.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/fieldmesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/ansys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/astra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/bmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/elegant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/litrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/lucretia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/opal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/simion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/superfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36467 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/species.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/pmd_beamphysics/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:26:55.000000 openpmd-beamphysics-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/tests/test_particlegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-04-12 21:26:46.000000 openpmd-beamphysics-0.7.5/versioneer.py
```

### Comparing `openpmd-beamphysics-0.7.4/LICENSE` & `openpmd-beamphysics-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/PKG-INFO` & `openpmd-beamphysics-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.4
+Version: 0.7.5
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.4/README.md` & `openpmd-beamphysics-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/PKG-INFO` & `openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.4
+Version: 0.7.5
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.4/openpmd_beamphysics.egg-info/SOURCES.txt` & `openpmd-beamphysics-0.7.5/openpmd_beamphysics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,10 @@
 pmd_beamphysics/interfaces/elegant.py
 pmd_beamphysics/interfaces/genesis.py
 pmd_beamphysics/interfaces/gpt.py
 pmd_beamphysics/interfaces/impact.py
 pmd_beamphysics/interfaces/litrack.py
 pmd_beamphysics/interfaces/lucretia.py
 pmd_beamphysics/interfaces/opal.py
+pmd_beamphysics/interfaces/simion.py
 pmd_beamphysics/interfaces/superfish.py
 tests/test_particlegroup.py
```

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/analysis.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/analysis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/conversion.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/conversion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/expansion.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/expansion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/fields/fieldmesh.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/fields/fieldmesh.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/ansys.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/ansys.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/astra.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/astra.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     t_ref = ref[6]*1e-9
     t_rel = data[1:,6]*1e-9
     #t = t_rel + t_ref
     
     # macro charge in Coulomb. The sign doesn't matter, so make positive
     qmacro = np.abs(data[1:,7]*1e-9)
     
-    species_index = data[1:,8].astype(np.int)
-    status = data[1:,9].astype(np.int)  
+    species_index = data[1:,8].astype(int)
+    status = data[1:,9].astype(int)  
     
     # Select particle by status 
     #probe_particles = np.where(status == 3) 
     #good_particles  = np.where(status == 5) 
 
     data = {}
     
@@ -141,15 +141,15 @@
         size += 6
         i_start += 6
     
 
     # Astra units and types
     #units = ['m', 'm', 'm', 'eV/c', 'eV/c', 'eV/c', 'ns', 'nC']
     names = ['x', 'y', 'z', 'px', 'py', 'pz', 't', 'q', 'index', 'status']
-    types = 8*[np.float] + 2*[np.int8]
+    types = 8*[float] + 2*[np.int8]
 
     
     # Reference particle
     ref_particle = {'q':0}
     sigma = {}
     for k in ['x', 'y', 'z', 'px', 'py', 'pz', 't']:
         ref_particle[k] = particle_group.avg(k)
```

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/bmad.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/bmad.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/elegant.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/elegant.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/genesis.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/genesis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/gpt.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/gpt.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/impact.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/impact.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/litrack.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/litrack.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/lucretia.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/lucretia.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/opal.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/opal.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/interfaces/superfish.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/interfaces/superfish.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/labels.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/labels.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/particles.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/particles.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pmd_beamphysics.interfaces.bmad import write_bmad
 from pmd_beamphysics.interfaces.genesis import write_genesis4_distribution, genesis2_beam_data,  write_genesis2_beam_file, write_genesis4_beam
 from pmd_beamphysics.interfaces.gpt import write_gpt
 from pmd_beamphysics.interfaces.impact import write_impact
 from pmd_beamphysics.interfaces.litrack import write_litrack
 from pmd_beamphysics.interfaces.lucretia import write_lucretia
 from pmd_beamphysics.interfaces.opal import write_opal
+from pmd_beamphysics.interfaces.simion import write_simion
 from pmd_beamphysics.interfaces.elegant import write_elegant
 
 from pmd_beamphysics.plot import density_plot, marginal_plot, slice_plot
 
 from pmd_beamphysics.readers import particle_array, particle_paths
 from pmd_beamphysics.species import charge_of, mass_of
 
@@ -789,14 +790,18 @@
                             include_header=include_header, verbose=verbose)          
         
     def write_litrack(self, filePath, p0c=None, verbose=False):        
         return write_litrack(self, outfile=filePath, p0c=p0c, verbose=verbose)      
         
     def write_lucretia(self, filePath, ele_name='BEGINNING', t_ref=0, stop_ix=None, verbose=False):       
         return write_lucretia(self, filePath, ele_name=ele_name, t_ref=t_ref, stop_ix=stop_ix)
+
+    def write_simion(self, filePath, color=0, flip_z_to_x=True, verbose=False):
+        return write_simion(self, filePath, verbose=verbose, color=color, flip_z_to_x=flip_z_to_x)
+
         
     def write_opal(self, filePath, verbose=False, dist_type='emitted'):
         return write_opal(self, filePath, verbose=verbose, dist_type=dist_type)
     
         
     # openPMD    
     def write(self, h5, name=None):
```

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/plot.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/plot.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/readers.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/readers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/species.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/species.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/statistics.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/statistics.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/tools.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/tools.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/units.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/units.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/pmd_beamphysics/writers.py` & `openpmd-beamphysics-0.7.5/pmd_beamphysics/writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     # write components (datasets)
     for key, val in data['components'].items():
         
         # Units
         u = pg_units(key)   
         
         # Ensure complex
-        val = val.astype(np.complex)
-        
+        val = val.astype(complex)
+
         # Write
         g2 = write_component_data(g, key, val, unit=u)            
     
     
 def write_component_data(h5, name, data, unit=None): 
     """
     Writes data to a dataset h5[name]
```

### Comparing `openpmd-beamphysics-0.7.4/setup.py` & `openpmd-beamphysics-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/tests/test_particlegroup.py` & `openpmd-beamphysics-0.7.5/tests/test_particlegroup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.4/versioneer.py` & `openpmd-beamphysics-0.7.5/versioneer.py`

 * *Files identical despite different names*

