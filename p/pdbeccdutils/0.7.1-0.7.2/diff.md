# Comparing `tmp/pdbeccdutils-0.7.1.tar.gz` & `tmp/pdbeccdutils-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbeccdutils-0.7.1.tar", last modified: Tue Mar 21 14:21:18 2023, max compression
+gzip compressed data, was "pdbeccdutils-0.7.2.tar", last modified: Wed Apr 12 07:41:40 2023, max compression
```

## Comparing `pdbeccdutils-0.7.1.tar` & `pdbeccdutils-0.7.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.221562 pdbeccdutils-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-03-21 14:21:18.221562 pdbeccdutils-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.213562 pdbeccdutils-0.7.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.213562 pdbeccdutils-0.7.1/pdbeccdutils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.213562 pdbeccdutils-0.7.1/pdbeccdutils/computations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/computations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/computations/parity_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.213562 pdbeccdutils-0.7.1/pdbeccdutils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19853 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/bm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/ccd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    44145 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/ccd_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25946 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15066 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/depictions.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/fragment_library.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7973 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.213562 pdbeccdutils-0.7.1/pdbeccdutils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.217563 pdbeccdutils-0.7.1/pdbeccdutils/data/coordgen_templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/coordgen_templates/templates.mae
--rw-r--r--   0 runner    (1001) docker     (123)   160441 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/fragment_library.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.217563 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/adamantane.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/cube.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/decahydrocorrin.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/hem.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/nonbornane.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/phorbine.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/porphin.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/porphycene.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/ru_complex.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/ru_complex2.sdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.217563 pdbeccdutils-0.7.1/pdbeccdutils/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/helpers/cif_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/helpers/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/helpers/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/helpers/mol_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.217563 pdbeccdutils-0.7.1/pdbeccdutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14092 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/scripts/process_components_cif_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/scripts/setup_pubchem_library_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.221562 pdbeccdutils-0.7.1/pdbeccdutils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_bound_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_file_writing.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_fragment_library.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_inchi_key_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_load_eoh_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_parity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_process_components_cif_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_property_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_rdkit_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_scaffold_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_web_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/test_write_img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/tests/tst_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.221562 pdbeccdutils-0.7.1/pdbeccdutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/utils/pubchem_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/pdbeccdutils/utils/web_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 14:21:18.213562 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-21 14:21:18.000000 pdbeccdutils-0.7.1/pdbeccdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 14:21:18.221562 pdbeccdutils-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-21 14:21:08.000000 pdbeccdutils-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/pdbeccdutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/pdbeccdutils/computations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/computations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/computations/parity_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/bm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44291 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25946 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15066 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/depictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/fragment_library.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7973 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/data/coordgen_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/coordgen_templates/templates.mae
+-rw-r--r--   0 runner    (1001) docker     (123)   160441 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/fragment_library.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/adamantane.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/cube.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/decahydrocorrin.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/hem.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/nonbornane.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/phorbine.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphin.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphycene.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex2.sdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/cif_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/mol_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14092 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/scripts/process_components_cif_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/scripts/setup_pubchem_library_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/pdbeccdutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_bound_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_file_writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_fragment_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_inchi_key_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_load_eoh_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_process_components_cif_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_property_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_rdkit_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_scaffold_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_web_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_write_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/tst_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/pdbeccdutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/pubchem_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/web_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/setup.py
```

### Comparing `pdbeccdutils-0.7.1/LICENSE` & `pdbeccdutils-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/PKG-INFO` & `pdbeccdutils-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbeccdutils
-Version: 0.7.1
+Version: 0.7.2
 Summary: Toolkit to deal with wwPDB chemical components definitions for small molecules.
 Home-page: http://pypi.python.org/pypi/pdbeccdutils/
 Author: Protein Data Bank in Europe
 Author-email: pdbehelp@ebi.ac.uk
 License: Apache License 2.0.
 Project-URL: Source code, https://github.com/PDBeurope/ccdutils
 Project-URL: Documentation, https://pdbeurope.github.io/ccdutils/
```

### Comparing `pdbeccdutils-0.7.1/README.md` & `pdbeccdutils-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/doc/conf.py` & `pdbeccdutils-0.7.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/computations/parity_method.py` & `pdbeccdutils-0.7.2/pdbeccdutils/computations/parity_method.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/bm_reader.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/bm_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         ]
         properties = CCDProperties(
             id="",
             name="",
             formula=CalcMolFormula(comp.mol),
             modified_date="",
             pdbx_release_status="",
-            weight=round(comp.physchem_properties["exactmw"], 3),
+            weight="",
         )
         comp = Component(mol.GetMol(), cif_block, properties, descriptors)
         reader_result = ccd_reader.CCDReaderResult(
             warnings=warnings, errors=errors, component=comp, sanitized=sanitized
         )
 
         return reader_result
```

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/ccd_reader.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_reader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/ccd_writer.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1131,23 +1131,21 @@
     Args:
         cif_block_copy (Block: gemmi.cif.Block): Block representation of the molecule
         from gemmi.
     """
     category = "_software."
     sw_fields = ["name", "version", "description"]
     sw_loop = cif_block_copy.init_loop(category, sw_fields)
-    sw_loop.add_row(
-        cif.quote_list(["rdkit", rdkit.__version__, cif.quote("Core functionality.")])
-    )
+    sw_loop.add_row(cif.quote_list(["rdkit", rdkit.__version__, "Core functionality."]))
     sw_loop.add_row(
         cif.quote_list(
             [
                 "pdbeccdutils",
                 pdbeccdutils.__version__,
-                cif.quote("Wrapper to provide 2D templates and molecular fragments."),
+                "Wrapper to provide 2D templates and molecular fragments.",
             ]
         )
     )
 
 
 def _add_2d_depiction_cif(component, cif_block_copy):
     """Add 2D coordinates of the component depiction
@@ -1184,35 +1182,39 @@
     ]
     substructure_loop = cif_block_copy.init_loop(
         substructure_category, substructure_fields
     )
 
     for i, scaffold in enumerate(component.scaffolds):
         mol = rdkit.Chem.MolFromSmiles(scaffold.smiles)
+        inchi = rdkit.Chem.MolToInchi(mol)
+        inchikey = rdkit.Chem.MolToInchiKey(mol)
         new_row = [
             component.id,
             scaffold.name,
             f"S{i+1}",
             "scaffold",
             scaffold.smiles,
-            rdkit.Chem.MolToInchi(mol),
-            rdkit.Chem.MolToInchiKey(mol),
+            inchi if inchi else None,
+            inchikey if inchikey else None,
         ]
         substructure_loop.add_row(cif.quote_list(new_row))
 
     for j, fragment in enumerate(component.fragments):
         mol = rdkit.Chem.MolFromSmiles(fragment.smiles)
+        inchi = rdkit.Chem.MolToInchi(mol)
+        inchikey = rdkit.Chem.MolToInchiKey(mol)
         new_row = [
             component.id,
             fragment.name,
             f"F{j+1}",
             "fragment",
             fragment.smiles,
-            rdkit.Chem.MolToInchi(mol),
-            rdkit.Chem.MolToInchiKey(mol),
+            inchi if inchi else None,
+            inchikey if inchikey else None,
         ]
         substructure_loop.add_row(cif.quote_list(new_row))
 
     mapping_category = "_pdbe_chem_comp_substructure_mapping."
     mapping_fields = ["comp_id", "atom_id", "substructure_id", "substructure_ordinal"]
     mapping_loop = cif_block_copy.init_loop(mapping_category, mapping_fields)
```

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/component.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/component.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/depictions.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/depictions.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/fragment_library.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/fragment_library.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/core/models.py` & `pdbeccdutils-0.7.2/pdbeccdutils/core/models.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/coordgen_templates/templates.mae` & `pdbeccdutils-0.7.2/pdbeccdutils/data/coordgen_templates/templates.mae`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/fragment_library.tsv` & `pdbeccdutils-0.7.2/pdbeccdutils/data/fragment_library.tsv`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/adamantane.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/adamantane.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/cube.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/cube.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/decahydrocorrin.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/decahydrocorrin.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/hem.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/hem.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/nonbornane.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/nonbornane.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/phorbine.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/phorbine.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/porphin.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphin.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/porphycene.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphycene.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/ru_complex.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/data/general_templates/ru_complex2.sdf` & `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex2.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/helpers/cif_tools.py` & `pdbeccdutils-0.7.2/pdbeccdutils/helpers/cif_tools.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/helpers/conversions.py` & `pdbeccdutils-0.7.2/pdbeccdutils/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/helpers/drawing.py` & `pdbeccdutils-0.7.2/pdbeccdutils/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/helpers/helper.py` & `pdbeccdutils-0.7.2/pdbeccdutils/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/helpers/mol_tools.py` & `pdbeccdutils-0.7.2/pdbeccdutils/helpers/mol_tools.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/scripts/process_components_cif_cli.py` & `pdbeccdutils-0.7.2/pdbeccdutils/scripts/process_components_cif_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/scripts/setup_pubchem_library_cli.py` & `pdbeccdutils-0.7.2/pdbeccdutils/scripts/setup_pubchem_library_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/conftest.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_bound_molecule.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_bound_molecule.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_file_writing.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_file_writing.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import os
 import xml.etree.ElementTree as ET
 
 import pytest
 from pdbeccdutils.core import ccd_writer
 from pdbeccdutils.core.component import Component
 from pdbeccdutils.core.models import ConformerType
+from pdbeccdutils.core.fragment_library import FragmentLibrary
+from pdbeccdutils.core.exceptions import CCDUtilsError
 from gemmi import cif
 from rdkit import Chem
 
 must_have_categories = [
     "_chem_comp.",
     "_chem_comp_atom.",
     "_chem_comp_bond.",
@@ -205,7 +207,47 @@
         if component.id == "D3O" and rem_hs:  # D3O has single heavy atom
             to_check.pop(2)
 
         assert cif_block
         assert component.id == cif_block.name
         for c in to_check:
             assert c in cif_block.get_mmcif_category_names()
+
+    @staticmethod
+    def test_fragment_writing(component: Component, tmpdir):
+        path = tmpdir.join(f"{component.id}.cif")
+        fragment_library = FragmentLibrary()
+        component.library_search(fragment_library)
+        ccd_writer.write_molecule(str(path), component)
+        cif_block = cif.read(str(path)).sole_block()
+        assert cif_block
+        assert component.id == cif_block.name
+        cif_categories = cif_block.get_mmcif_category_names()
+        if component.fragments:
+            assert "_pdbe_chem_comp_substructure." in cif_categories
+            substructure = cif_block.get_mmcif_category("_pdbe_chem_comp_substructure.")
+            for _, values in substructure.items():
+                for value in values:
+                    if value is not None:
+                        assert len(value) > 0
+
+    @staticmethod
+    def test_scaffold_writing(component: Component, tmpdir):
+        path = tmpdir.join(f"{component.id}.cif")
+        try:
+            component.get_scaffolds()
+            ccd_writer.write_molecule(str(path), component)
+            cif_block = cif.read(str(path)).sole_block()
+            assert cif_block
+            assert component.id == cif_block.name
+            cif_categories = cif_block.get_mmcif_category_names()
+            if component.scaffolds:
+                assert "_pdbe_chem_comp_substructure." in cif_categories
+                substructure = cif_block.get_mmcif_category(
+                    "_pdbe_chem_comp_substructure."
+                )
+                for _, values in substructure.items():
+                    for value in values:
+                        if value is not None:
+                            assert len(value) > 0
+        except CCDUtilsError:
+            assert True
```

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_fragment_library.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_fragment_library.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_load_eoh_cif.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_load_eoh_cif.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_parity.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_process_components_cif_cli.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_process_components_cif_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_property_generation.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_property_generation.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_rdkit_fixtures.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_rdkit_fixtures.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_scaffold_generation.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_scaffold_generation.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_web_services.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_web_services.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/test_write_img.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_write_img.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/tests/tst_utilities.py` & `pdbeccdutils-0.7.2/pdbeccdutils/tests/tst_utilities.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/utils/pubchem_downloader.py` & `pdbeccdutils-0.7.2/pdbeccdutils/utils/pubchem_downloader.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils/utils/web_services.py` & `pdbeccdutils-0.7.2/pdbeccdutils/utils/web_services.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils.egg-info/PKG-INFO` & `pdbeccdutils-0.7.2/pdbeccdutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbeccdutils
-Version: 0.7.1
+Version: 0.7.2
 Summary: Toolkit to deal with wwPDB chemical components definitions for small molecules.
 Home-page: http://pypi.python.org/pypi/pdbeccdutils/
 Author: Protein Data Bank in Europe
 Author-email: pdbehelp@ebi.ac.uk
 License: Apache License 2.0.
 Project-URL: Source code, https://github.com/PDBeurope/ccdutils
 Project-URL: Documentation, https://pdbeurope.github.io/ccdutils/
```

### Comparing `pdbeccdutils-0.7.1/pdbeccdutils.egg-info/SOURCES.txt` & `pdbeccdutils-0.7.2/pdbeccdutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.1/setup.py` & `pdbeccdutils-0.7.2/setup.py`

 * *Files identical despite different names*

