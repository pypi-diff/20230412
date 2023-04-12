# Comparing `tmp/pynwb-2.3.1.tar.gz` & `tmp/pynwb-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynwb-2.3.1.tar", last modified: Mon Feb 27 08:28:57 2023, max compression
+gzip compressed data, was "pynwb-2.3.2.tar", last modified: Wed Apr 12 01:17:22 2023, max compression
```

## Comparing `pynwb-2.3.1.tar` & `pynwb-2.3.2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.758656 pynwb-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-27 08:24:52.000000 pynwb-2.3.1/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-27 08:24:52.000000 pynwb-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-02-27 08:28:57.758656 pynwb-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-02-27 08:24:52.000000 pynwb-2.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-27 08:24:52.000000 pynwb-2.3.1/environment-ros3.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-02-27 08:24:52.000000 pynwb-2.3.1/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-27 08:24:52.000000 pynwb-2.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-27 08:24:52.000000 pynwb-2.3.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-27 08:24:52.000000 pynwb-2.3.1/requirements-min.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-27 08:24:52.000000 pynwb-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-27 08:28:57.758656 pynwb-2.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-02-27 08:24:52.000000 pynwb-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.730656 pynwb-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.758656 pynwb-2.3.1/src/pynwb/
--rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/_due.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-27 08:28:57.758656 pynwb-2.3.1/src/pynwb/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28432 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)    57672 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    45643 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.738655 pynwb-2.3.1/src/pynwb/io/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.738655 pynwb-2.3.1/src/pynwb/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.738655 pynwb-2.3.1/src/pynwb/legacy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/io/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/legacy/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.730656 pynwb-2.3.1/src/pynwb/nwb-schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.742656 pynwb-2.3.1/src/pynwb/nwb-schema/core/
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.behavior.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.ecephys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.epoch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.icephys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.misc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.ogen.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.ophys.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-02-27 08:24:54.000000 pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.742656 pynwb-2.3.1/src/pynwb/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/icephys_testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/make_test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.742656 pynwb-2.3.1/src/pynwb/testing/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/mock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/testh5io.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-02-27 08:24:52.000000 pynwb-2.3.1/src/pynwb/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.734655 pynwb-2.3.1/src/pynwb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-02-27 08:28:57.000000 pynwb-2.3.1/src/pynwb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-02-27 08:28:57.000000 pynwb-2.3.1/src/pynwb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 08:28:57.000000 pynwb-2.3.1/src/pynwb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 08:25:12.000000 pynwb-2.3.1/src/pynwb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-27 08:28:57.000000 pynwb-2.3.1/src/pynwb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-27 08:28:57.000000 pynwb-2.3.1/src/pynwb.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    14649 2023-02-27 08:24:52.000000 pynwb-2.3.1/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.742656 pynwb-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.750656 pynwb-2.3.1/tests/back_compat/
--rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.0.2_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.0.2_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.0.2_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143504 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.0.3_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.0.3_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.0.3_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   142512 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.1.0_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.1.0_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.1.0_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148288 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.1.2_nwbfile.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.1.2_str_experimenter.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.1.2_str_pub.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169624 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.5.1_imageseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.5.1_imageseries_no_unit.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169120 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.5.1_timeseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/1.5.1_timeseries_no_unit.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/2.1.0_imageseries_no_data.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/2.1.0_imageseries_non_external_format.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   184152 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/2.1.0_nwbfile_with_extension.nwb
--rw-r--r--   0 runner    (1001) docker     (123)   181616 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/2.2.0_subject_no_age__reference.nwb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/test_import_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/back_compat/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.750656 pynwb-2.3.1/tests/coverage/
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/coverage/runCoverage
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.750656 pynwb-2.3.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.750656 pynwb-2.3.1/tests/integration/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    24810 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_modular_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    26386 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_nwbfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/hdf5/test_scratch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.750656 pynwb-2.3.1/tests/integration/ros3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/ros3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/ros3/test_ros3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.750656 pynwb-2.3.1/tests/integration/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/integration/utils/test_io_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.754656 pynwb-2.3.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31128 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_core_NWBContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_ecephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_epoch_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_icephys.py
--rw-r--r--   0 runner    (1001) docker     (123)    66716 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_icephys_metadata_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_ogen.py
--rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_ophys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_retinotopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_scratch.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/unit/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 08:28:57.758656 pynwb-2.3.1/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-02-27 08:24:52.000000 pynwb-2.3.1/tests/validation/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-02-27 08:24:52.000000 pynwb-2.3.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    83021 2023-02-27 08:24:52.000000 pynwb-2.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 01:13:20.000000 pynwb-2.3.2/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 01:13:20.000000 pynwb-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-12 01:17:22.613450 pynwb-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-12 01:13:20.000000 pynwb-2.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 01:13:20.000000 pynwb-2.3.2/environment-ros3.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-12 01:13:20.000000 pynwb-2.3.2/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 01:13:20.000000 pynwb-2.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-12 01:17:22.613450 pynwb-2.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2352 2023-04-12 01:13:20.000000 pynwb-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.569450 pynwb-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/src/pynwb/
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/_due.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 01:17:22.613450 pynwb-2.3.2/src/pynwb/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28433 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18125 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57672 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45643 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17740 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.581450 pynwb-2.3.2/src/pynwb/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.581450 pynwb-2.3.2/src/pynwb/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.581450 pynwb-2.3.2/src/pynwb/legacy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/io/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/legacy/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.569450 pynwb-2.3.2/src/pynwb/nwb-schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.585450 pynwb-2.3.2/src/pynwb/nwb-schema/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.behavior.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ecephys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.epoch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21539 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16212 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.icephys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ogen.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ophys.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-12 01:13:23.000000 pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.585450 pynwb-2.3.2/src/pynwb/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/icephys_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/make_test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.589450 pynwb-2.3.2/src/pynwb/testing/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/mock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/testh5io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-12 01:13:20.000000 pynwb-2.3.2/src/pynwb/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.577450 pynwb-2.3.2/src/pynwb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:13:42.000000 pynwb-2.3.2/src/pynwb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 01:17:22.000000 pynwb-2.3.2/src/pynwb.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14813 2023-04-12 01:13:20.000000 pynwb-2.3.2/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.589450 pynwb-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.601450 pynwb-2.3.2/tests/back_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.2_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.2_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)    15632 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.2_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143504 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.3_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.3_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   144096 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.0.3_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   142512 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.0_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.0_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   143104 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.0_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148288 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.2_nwbfile.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.2_str_experimenter.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   148880 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.1.2_str_pub.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169624 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_unit.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169120 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   169408 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_unit.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_no_data.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_non_external_format.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   182272 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   184152 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.1.0_nwbfile_with_extension.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)   181616 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/2.2.0_subject_no_age__reference.nwb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/test_import_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/back_compat/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.601450 pynwb-2.3.2/tests/coverage/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/coverage/runCoverage
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.601450 pynwb-2.3.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.605450 pynwb-2.3.2/tests/integration/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25147 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_modular_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26387 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_nwbfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/hdf5/test_scratch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.605450 pynwb-2.3.2/tests/integration/ros3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/ros3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/ros3/test_ros3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.605450 pynwb-2.3.2/tests/integration/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/integration/utils/test_io_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31128 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_core_NWBContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_ecephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_epoch_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27739 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14961 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_icephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66716 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_icephys_metadata_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_ogen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19248 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_ophys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_retinotopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_scratch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/unit/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:17:22.613450 pynwb-2.3.2/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-04-12 01:13:20.000000 pynwb-2.3.2/tests/validation/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-12 01:13:20.000000 pynwb-2.3.2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    83021 2023-04-12 01:13:20.000000 pynwb-2.3.2/versioneer.py
```

### Comparing `pynwb-2.3.1/Legal.txt` & `pynwb-2.3.2/Legal.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/PKG-INFO` & `pynwb-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynwb
-Version: 2.3.1
+Version: 2.3.2
 Summary: Package for working with Neurodata stored in the NWB format
 Home-page: https://github.com/NeurodataWithoutBorders/pynwb
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: Neuroscience python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research PyNWB NWB NWB:N NeurodataWithoutBorders
 Classifier: Programming Language :: Python
```

### Comparing `pynwb-2.3.1/README.rst` & `pynwb-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/license.txt` & `pynwb-2.3.2/license.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/requirements-doc.txt` & `pynwb-2.3.2/requirements-doc.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # dependencies to generate the documentation for PyNWB and test run the sphinx gallery examples that do not require
 # ROS3 support in h5py. For those examples, use the conda env specified in environment-ros3.yml
 sphinx>=4  # improved support for docutils>=0.17
 sphinx_rtd_theme>=1  # <1 does not work with docutils>=0.17
 matplotlib
 sphinx-gallery
-allensdk>=2.13.2  # allensdk <=2.13.1 requires pynwb<2
-MarkupSafe==2.0.1  # resolve incompatibility between jinja2 and markupsafe: https://github.com/AllenInstitute/AllenSDK/issues/2308
+# allensdk>=2.13.2  # allensdk reinstalls pynwb and hdmf. TODO set up a separate workflow to test allensdk
+# MarkupSafe==2.0.1  # resolve incompatibility between jinja2 and markupsafe: https://github.com/AllenInstitute/AllenSDK/issues/2308
 Pillow
 sphinx-copybutton
 dataframe_image   # used to render large dataframe as image in the sphinx gallery to improve html display
 lxml  # used by dataframe_image when using the matplotlib backend
 hdf5plugin
```

### Comparing `pynwb-2.3.1/setup.cfg` & `pynwb-2.3.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -32,11 +32,14 @@
 	test.py:T201
 	scripts/*:T201
 extend-ignore = E203
 
 [metadata]
 description_file = README.rst
 
+[isort]
+profile = black
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pynwb-2.3.1/setup.py` & `pynwb-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 pkgs = find_packages('src', exclude=['data'])
 print('found these packages:', pkgs)
 
 schema_dir = 'nwb-schema/core'
 
 reqs = [
-    'h5py>=2.10,<4',
-    'hdmf>=3.5.1,<4',
-    'numpy>=1.16,<1.24',
-    'pandas>=1.1.5,<2',
-    'python-dateutil>=2.7.3,<3',
+    'h5py>=2.10',
+    'hdmf>=3.5.4',
+    'numpy>=1.16',
+    'pandas>=1.1.5',
+    'python-dateutil>=2.7.3',
     'setuptools'
 ]
 
 print(reqs)
 
 setup_args = {
     'name': 'pynwb',
```

### Comparing `pynwb-2.3.1/src/pynwb/__init__.py` & `pynwb-2.3.2/src/pynwb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,32 @@
 from hdmf.utils import docval, getargs, popargs, get_docval
 from hdmf.backends.io import HDMFIO
 from hdmf.backends.hdf5 import HDF5IO as _HDF5IO
 from hdmf.build import BuildManager, TypeMap
 import hdmf.common
 
 CORE_NAMESPACE = 'core'
-__core_ns_file_name = 'nwb.namespace.yaml'
 
 from .spec import NWBDatasetSpec, NWBGroupSpec, NWBNamespace  # noqa E402
 from .validate import validate  # noqa: F401, E402
 
 
 def __get_resources():
-    from pkg_resources import resource_filename
+    try:
+        from importlib.resources import files
+    except ImportError:
+        # TODO: Remove when python 3.9 becomes the new minimum
+        from importlib_resources import files
+
+    __location_of_this_file = files(__name__)
+    __core_ns_file_name = 'nwb.namespace.yaml'
+    __schema_dir = 'nwb-schema/core'
+
     ret = dict()
-    ret['namespace_path'] = os.path.join(resource_filename(__name__, 'nwb-schema/core'), __core_ns_file_name)
+    ret['namespace_path'] = str(__location_of_this_file / __schema_dir / __core_ns_file_name)
     return ret
 
 
 def _get_resources():
     # LEGACY: Needed to support legacy implementation.
     return __get_resources()
 
@@ -254,14 +262,19 @@
         # Get the version string for the NWB file
         try:
             nwb_version_string = self._file.attrs['nwb_version']
         #  KeyError occurs  when the file is empty (e.g., when creating a new file nothing has been written)
         #  or when the HDF5 file is not a valid NWB file
         except KeyError:
             return None, None
+        # Other system may have written nwb_version as a fixed-length string, resulting in a numpy.bytes_ object
+        # on read, rather than a variable-length string. To address this, decode the bytes if necessary.
+        if not isinstance(nwb_version_string, str):
+            nwb_version_string = nwb_version_string.decode()
+
         # Parse the version string
         nwb_version_parts = nwb_version_string.replace("-", ".").replace("_", ".").split(".")
         nwb_version = tuple([int(i) if i.isnumeric() else i
                              for i in nwb_version_parts])
         return nwb_version_string, nwb_version
 
     @docval(*get_docval(_HDF5IO.read),
```

### Comparing `pynwb-2.3.1/src/pynwb/_due.py` & `pynwb-2.3.2/src/pynwb/_due.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/base.py` & `pynwb-2.3.2/src/pynwb/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,15 @@
 
     def get(self, key, **kwargs):
         """
         Retrieve elements from this object.
 
         The function uses :py:class:`~pynwb.base.TimeSeriesReferenceVectorData.TIME_SERIES_REFERENCE_TUPLE`
         to describe individual records in the dataset. This allows the code to avoid exposing internal
-        details of the schema to the user and simplifies handling of missing values by explictly
+        details of the schema to the user and simplifies handling of missing values by explicitly
         representing missing values via
         :py:class:`~pynwb.base.TimeSeriesReferenceVectorData.TIME_SERIES_REFERENCE_NONE_TYPE`
         rather than the internal representation used for storage of ``(-1, -1, TimeSeries)``.
 
         :param key: Selection of the elements
         :param kwargs: Ignored
```

### Comparing `pynwb-2.3.1/src/pynwb/behavior.py` & `pynwb-2.3.2/src/pynwb/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/core.py` & `pynwb-2.3.2/src/pynwb/core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/device.py` & `pynwb-2.3.2/src/pynwb/device.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/ecephys.py` & `pynwb-2.3.2/src/pynwb/ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/epoch.py` & `pynwb-2.3.2/src/pynwb/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/file.py` & `pynwb-2.3.2/src/pynwb/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/icephys.py` & `pynwb-2.3.2/src/pynwb/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/image.py` & `pynwb-2.3.2/src/pynwb/image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/base.py` & `pynwb-2.3.2/src/pynwb/io/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/core.py` & `pynwb-2.3.2/src/pynwb/io/core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/epoch.py` & `pynwb-2.3.2/src/pynwb/io/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/file.py` & `pynwb-2.3.2/src/pynwb/io/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/icephys.py` & `pynwb-2.3.2/src/pynwb/io/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/misc.py` & `pynwb-2.3.2/src/pynwb/io/misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/ophys.py` & `pynwb-2.3.2/src/pynwb/io/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/io/utils.py` & `pynwb-2.3.2/src/pynwb/io/utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/__init__.py` & `pynwb-2.3.2/src/pynwb/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/base.py` & `pynwb-2.3.2/src/pynwb/legacy/io/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/behavior.py` & `pynwb-2.3.2/src/pynwb/legacy/io/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/epoch.py` & `pynwb-2.3.2/src/pynwb/legacy/io/epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/file.py` & `pynwb-2.3.2/src/pynwb/legacy/io/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/icephys.py` & `pynwb-2.3.2/src/pynwb/legacy/io/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/ogen.py` & `pynwb-2.3.2/src/pynwb/legacy/io/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/io/ophys.py` & `pynwb-2.3.2/src/pynwb/legacy/io/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/legacy/map.py` & `pynwb-2.3.2/src/pynwb/legacy/map.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/misc.py` & `pynwb-2.3.2/src/pynwb/misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.base.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.base.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.behavior.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.behavior.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.ecephys.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ecephys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.epoch.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.epoch.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.file.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.file.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.icephys.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.icephys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.image.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.image.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.misc.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.misc.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.namespace.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.namespace.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.ogen.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ogen.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.ophys.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.ophys.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml` & `pynwb-2.3.2/src/pynwb/nwb-schema/core/nwb.retinotopy.yaml`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/ogen.py` & `pynwb-2.3.2/src/pynwb/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/ophys.py` & `pynwb-2.3.2/src/pynwb/ophys.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     def __init__(self, **kwargs):
         keys_to_set = (
             "imaging_plane", "pmt_gain", "scan_line_rate", "exposure_time", "binning", "power", "intensity"
         )
         args_to_set = popargs_to_dict(keys_to_set, kwargs)
         super().__init__(**kwargs)
 
-        if args_to_set["binning"] < 0:
+        if args_to_set["binning"] is not None and args_to_set["binning"] < 0:
             raise ValueError(f"Binning value must be >= 0: {args_to_set['binning']}")
         if isinstance(args_to_set["binning"], int):
             args_to_set["binning"] = np.uint(args_to_set["binning"])
 
         for key, val in args_to_set.items():
             setattr(self, key, val)
```

### Comparing `pynwb-2.3.1/src/pynwb/retinotopy.py` & `pynwb-2.3.2/src/pynwb/retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/spec.py` & `pynwb-2.3.2/src/pynwb/spec.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/icephys_testutils.py` & `pynwb-2.3.2/src/pynwb/testing/icephys_testutils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/make_test_files.py` & `pynwb-2.3.2/src/pynwb/testing/make_test_files.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/__init__.py` & `pynwb-2.3.2/src/pynwb/testing/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/base.py` & `pynwb-2.3.2/src/pynwb/testing/mock/base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/behavior.py` & `pynwb-2.3.2/src/pynwb/testing/mock/behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/ecephys.py` & `pynwb-2.3.2/src/pynwb/testing/mock/ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/file.py` & `pynwb-2.3.2/src/pynwb/testing/mock/file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/icephys.py` & `pynwb-2.3.2/src/pynwb/testing/mock/icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/ogen.py` & `pynwb-2.3.2/src/pynwb/testing/mock/ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/ophys.py` & `pynwb-2.3.2/src/pynwb/testing/mock/ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/mock/utils.py` & `pynwb-2.3.2/src/pynwb/testing/mock/utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/testing/testh5io.py` & `pynwb-2.3.2/src/pynwb/testing/testh5io.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb/validate.py` & `pynwb-2.3.2/src/pynwb/validate.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/src/pynwb.egg-info/PKG-INFO` & `pynwb-2.3.2/src/pynwb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynwb
-Version: 2.3.1
+Version: 2.3.2
 Summary: Package for working with Neurodata stored in the NWB format
 Home-page: https://github.com/NeurodataWithoutBorders/pynwb
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: Neuroscience python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research PyNWB NWB NWB:N NeurodataWithoutBorders
 Classifier: Programming Language :: Python
```

### Comparing `pynwb-2.3.1/src/pynwb.egg-info/SOURCES.txt` & `pynwb-2.3.2/src/pynwb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/test.py` & `pynwb-2.3.2/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,28 @@
 
 
 ros3_examples = [
     os.path.join('general', 'read_basics.py'),
     os.path.join('advanced_io', 'streaming.py'),
 ]
 
+allensdk_examples = [
+    os.path.join('domain', 'brain_observatory.py'),  # TODO create separate workflow for this
+]
+
 
 def run_example_tests():
     """Run the Sphinx gallery example files, excluding ROS3-dependent ones, to check for errors."""
     logging.info('running example tests')
     examples_scripts = list()
     for root, dirs, files in os.walk(os.path.join(os.path.dirname(__file__), "docs", "gallery")):
         for f in files:
             if f.endswith(".py"):
                 name_with_parent_dir = os.path.join(os.path.basename(root), f)
-                if name_with_parent_dir in ros3_examples:
+                if name_with_parent_dir in ros3_examples or name_with_parent_dir in allensdk_examples:
                     logging.info("Skipping %s" % name_with_parent_dir)
                     continue
                 examples_scripts.append(os.path.join(root, f))
 
     __run_example_tests_helper(examples_scripts)
```

### Comparing `pynwb-2.3.1/tests/back_compat/1.0.2_nwbfile.nwb` & `pynwb-2.3.2/tests/back_compat/1.0.2_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.0.2_str_experimenter.nwb` & `pynwb-2.3.2/tests/back_compat/1.0.2_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.0.2_str_pub.nwb` & `pynwb-2.3.2/tests/back_compat/1.0.2_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.0.3_nwbfile.nwb` & `pynwb-2.3.2/tests/back_compat/1.0.3_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.0.3_str_experimenter.nwb` & `pynwb-2.3.2/tests/back_compat/1.0.3_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.0.3_str_pub.nwb` & `pynwb-2.3.2/tests/back_compat/1.0.3_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.1.0_nwbfile.nwb` & `pynwb-2.3.2/tests/back_compat/1.1.0_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.1.0_str_experimenter.nwb` & `pynwb-2.3.2/tests/back_compat/1.1.0_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.1.0_str_pub.nwb` & `pynwb-2.3.2/tests/back_compat/1.1.0_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.1.2_nwbfile.nwb` & `pynwb-2.3.2/tests/back_compat/1.1.2_nwbfile.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.1.2_str_experimenter.nwb` & `pynwb-2.3.2/tests/back_compat/1.1.2_str_experimenter.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.1.2_str_pub.nwb` & `pynwb-2.3.2/tests/back_compat/1.1.2_str_pub.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.5.1_imageseries_no_data.nwb` & `pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.5.1_imageseries_no_unit.nwb` & `pynwb-2.3.2/tests/back_compat/1.5.1_imageseries_no_unit.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.5.1_timeseries_no_data.nwb` & `pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/1.5.1_timeseries_no_unit.nwb` & `pynwb-2.3.2/tests/back_compat/1.5.1_timeseries_no_unit.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/2.1.0_imageseries_no_data.nwb` & `pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_no_data.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/2.1.0_imageseries_non_external_format.nwb` & `pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_non_external_format.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb` & `pynwb-2.3.2/tests/back_compat/2.1.0_imageseries_nonmatch_starting_frame.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/2.1.0_nwbfile_with_extension.nwb` & `pynwb-2.3.2/tests/back_compat/2.1.0_nwbfile_with_extension.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/2.2.0_subject_no_age__reference.nwb` & `pynwb-2.3.2/tests/back_compat/2.2.0_subject_no_age__reference.nwb`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/back_compat/test_import_structure.py` & `pynwb-2.3.2/tests/back_compat/test_import_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             "TimeSeries",
             "TypeMap",
             "_HDF5IO",
             "__NS_CATALOG",
             "__TYPE_MAP",
             "__builtins__",
             "__cached__",
-            "__core_ns_file_name",
             "__doc__",
             "__file__",
             "__get_resources",
             "__io",
             "__loader__",
             "__name__",
             "__package__",
```

### Comparing `pynwb-2.3.1/tests/back_compat/test_read.py` & `pynwb-2.3.2/tests/back_compat/test_read.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_base.py` & `pynwb-2.3.2/tests/integration/hdf5/test_base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_device.py` & `pynwb-2.3.2/tests/integration/hdf5/test_device.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_ecephys.py` & `pynwb-2.3.2/tests/integration/hdf5/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_icephys.py` & `pynwb-2.3.2/tests/integration/hdf5/test_icephys.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         self.pcs = PatchClampSeries(name="pcs", data=[1, 2, 3, 4, 5], unit='A',
                                     starting_time=123.6, rate=10e3, electrode=self.elec, gain=0.126,
                                     stimulus_description="gotcha ya!", sweep_number=np.uint(4711))
         # Create the SweepTable but ignore the DeprecationWarning
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter('ignore', DeprecationWarning)
             sweeptable = SweepTable(name='sweep_table')
-            # Reissue any other warnings that may have occured
+            # Reissue any other warnings that may have occurred
             for i in w:
                 warnings.warn(i.message, i.category)
         return sweeptable
 
     def addContainer(self, nwbfile):
         """
         Add the test SweepTable, PatchClampSeries, IntracellularElectrode, and Device to the given NWBFile
@@ -203,15 +203,15 @@
                                       starting_time=123.6, rate=10e3, electrode=self.elec, gain=0.126,
                                       stimulus_description="gotcha ya!", sweep_number=np.uint(4712))
 
         # Create the SweepTable but ignore the DeprecationWarning
         with warnings.catch_warnings(record=True) as w:
             warnings.simplefilter('ignore', DeprecationWarning)
             sweeptable = SweepTable(name='sweep_table')
-            # Reissue any other warnings that may have occured
+            # Reissue any other warnings that may have occurred
             for i in w:
                 warnings.warn(i.message, i.category)
         return sweeptable
 
     def addContainer(self, nwbfile):
         """
         Add the test SweepTable, PatchClampSeries, IntracellularElectrode, and Device to the given NWBFile
```

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_image.py` & `pynwb-2.3.2/tests/integration/hdf5/test_image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_io.py` & `pynwb-2.3.2/tests/integration/hdf5/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,14 +439,19 @@
                 self.assertEqual(io.nwb_version[0], ver[0])
                 self.assertTupleEqual(io.nwb_version[1], ver[1])
         # check empty version attribute
         with File(self.path, mode='a') as io:
             del io.attrs['nwb_version']
         with NWBHDF5IO(self.path, 'r') as io:
             self.assertTupleEqual(io.nwb_version, (None, None))
+        # check that it works when setting the attribute to a fixed-length numpy-bytes string
+        with File(self.path, mode='a') as io:
+            io.attrs['nwb_version'] = np.asarray("2.0.5", dtype=np.bytes_)[()]
+        with NWBHDF5IO(self.path, 'r') as io:
+            self.assertTupleEqual(io.nwb_version, ("2.0.5", (2, 0, 5)))
 
     def test_check_nwb_version_ok(self):
         """Test that opening a current NWBFile passes the version check"""
         with NWBHDF5IO(self.path, 'w') as io:
             io.write(self.nwbfile)
         with NWBHDF5IO(self.path, 'r') as io:
             self.assertIsNotNone(io.nwb_version[0])
```

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_misc.py` & `pynwb-2.3.2/tests/integration/hdf5/test_misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_modular_storage.py` & `pynwb-2.3.2/tests/integration/hdf5/test_modular_storage.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_nwbfile.py` & `pynwb-2.3.2/tests/integration/hdf5/test_nwbfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         """ Return placeholder epochs object. Tested epochs are added directly to the NWBFile in addContainer """
         return TimeIntervals('epochs')
 
     def addContainer(self, nwbfile):
         """ Add the test epochs to the given NWBFile """
         nwbfile.add_epoch_column(
             name='temperature',
-            description='average temperture (c) during epoch'
+            description='average temperature (c) during epoch'
         )
 
         nwbfile.add_epoch(
             start_time=5.3,
             stop_time=6.1,
             timeseries=[],
             tags='ambient',
```

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_ogen.py` & `pynwb-2.3.2/tests/integration/hdf5/test_ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_ophys.py` & `pynwb-2.3.2/tests/integration/hdf5/test_ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_retinotopy.py` & `pynwb-2.3.2/tests/integration/hdf5/test_retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/hdf5/test_scratch.py` & `pynwb-2.3.2/tests/integration/hdf5/test_scratch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/ros3/test_ros3.py` & `pynwb-2.3.2/tests/integration/ros3/test_ros3.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/integration/utils/test_io_utils.py` & `pynwb-2.3.2/tests/integration/utils/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_base.py` & `pynwb-2.3.2/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_behavior.py` & `pynwb-2.3.2/tests/unit/test_behavior.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_core.py` & `pynwb-2.3.2/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_core_NWBContainer.py` & `pynwb-2.3.2/tests/unit/test_core_NWBContainer.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_ecephys.py` & `pynwb-2.3.2/tests/unit/test_ecephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_epoch.py` & `pynwb-2.3.2/tests/unit/test_epoch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_epoch_legacy.py` & `pynwb-2.3.2/tests/unit/test_epoch_legacy.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     In NWB 2.5 TimeIntervals.timeseries was updated to use the TimeSeriesReferenceVectorData type and to
     keep the API consistent old files are migrated on read to present the same API for those files. This
     is possible because the previous and updated schema are identical aside from the fact that a dedicated
     neurodata_type was created for the TimeIntervals.timeseries columns which is also used in the
     IntracellularRecordingTable type.
 
     This is technically a round-trip test, but without round-trip we can't test the object-mapper and
-    including it here makes sure this get's included in code-coverage tests as well.
+    including it here makes sure this gets included in code-coverage tests as well.
     """
 
     def setUpContainer(self):
         """ Return placeholder epochs object. Tested epochs are added directly to the NWBFile in addContainer """
         return TimeIntervals('epochs')
 
     def addContainer(self, nwbfile):
@@ -29,18 +29,18 @@
         # Add some timeseries
         tsa, tsb = [
             TimeSeries(name='a', data=np.arange(11), unit='flubs', timestamps=np.linspace(0, 1.0, 11)),
             TimeSeries(name='b', data=np.arange(13), unit='flubs', timestamps=np.linspace(0.1, 2.0, 13)),
         ]
         nwbfile.add_acquisition(tsa)
         nwbfile.add_acquisition(tsb)
-        # Add a custom colum
+        # Add a custom column
         nwbfile.add_epoch_column(
             name='temperature',
-            description='average temperture (c) during epoch'
+            description='average temperature (c) during epoch'
         )
         # Add some epochs
         nwbfile.add_epoch(
             start_time=0.0,
             stop_time=0.5,
             timeseries=[tsa, tsb],
             tags='ambient',
```

### Comparing `pynwb-2.3.1/tests/unit/test_extension.py` & `pynwb-2.3.2/tests/unit/test_extension.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_file.py` & `pynwb-2.3.2/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_icephys.py` & `pynwb-2.3.2/tests/unit/test_icephys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_icephys_metadata_tables.py` & `pynwb-2.3.2/tests/unit/test_icephys_metadata_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
             ir.add_recording(
                 electrode=self.electrode,
                 stimulus=self.stimulus,
                 response_start_index=10,
                 response=self.response,
                 id=np.int64(10)
             )
-        # Stimulus/Reponse index count too large
+        # Stimulus/Response index count too large
         with self.assertRaises(IndexError):
             ir = IntracellularRecordingsTable()
             ir.add_recording(
                 electrode=self.electrode,
                 stimulus=self.stimulus,
                 stimulus_index_count=10,
                 response=self.response,
@@ -434,15 +434,15 @@
             ir.add_recording(
                 electrode=self.electrode,
                 stimulus=self.stimulus,
                 response_index_count=10,
                 response=self.response,
                 id=np.int64(10)
             )
-        # Stimulus/Reponse start+count combination too large
+        # Stimulus/Response start+count combination too large
         with self.assertRaises(IndexError):
             ir = IntracellularRecordingsTable()
             ir.add_recording(
                 electrode=self.electrode,
                 stimulus=self.stimulus,
                 stimulus_start_index=3,
                 stimulus_index_count=4,
@@ -1145,15 +1145,15 @@
     def test_icephys_filtering_roundtrip(self):
         # create the base file
         nwbfile = NWBFile(
             session_description='my first synthetic recording',
             identifier='EXAMPLE_ID',
             session_start_time=datetime.now(tzlocal())
         )
-        # set the icephys_filtering attribute and make sure we get a deprectation warning
+        # set the icephys_filtering attribute and make sure we get a deprecation warning
         with warnings.catch_warnings(record=True) as w:
             nwbfile.icephys_filtering = 'test filtering'
             assert issubclass(w[-1].category, DeprecationWarning)
         # write the test fil
         with NWBHDF5IO(self.path, 'w') as io:
             io.write(nwbfile)
         # read the test file and confirm icephys_filtering has been written
@@ -1322,15 +1322,15 @@
                                                  stimulus_type="MyStimulusType")
         # Check that the SimultaneousRecordingsTable table has been added
         self.assertIsNotNone(nwbfile.icephys_sequential_recordings)
         # Check that the values for our SimultaneousRecordingsTable table are correct
         res = nwbfile.icephys_sequential_recordings[0]
         # check the id value
         self.assertEqual(res.index[0], sequential_recording_id)
-        # Check that our sequential recording containts 1 simultaneous recording
+        # Check that our sequential recording contains 1 simultaneous recording
         assert_array_equal(res.loc[sequential_recording_id]['simultaneous_recordings'],
                            simultaneous_recordings_indices)
 
         #############################################
         #  Test adding a Run
         #############################################
         # Confirm that our RepetitionsTable table does not yet exist
```

### Comparing `pynwb-2.3.1/tests/unit/test_image.py` & `pynwb-2.3.2/tests/unit/test_image.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_misc.py` & `pynwb-2.3.2/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_mock.py` & `pynwb-2.3.2/tests/unit/test_mock.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_ogen.py` & `pynwb-2.3.2/tests/unit/test_ogen.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_ophys.py` & `pynwb-2.3.2/tests/unit/test_ophys.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_retinotopy.py` & `pynwb-2.3.2/tests/unit/test_retinotopy.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_scratch.py` & `pynwb-2.3.2/tests/unit/test_scratch.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/unit/test_spec.py` & `pynwb-2.3.2/tests/unit/test_spec.py`

 * *Files identical despite different names*

### Comparing `pynwb-2.3.1/tests/validation/test_validate.py` & `pynwb-2.3.2/tests/validation/test_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # so that we can both test pynwb.validate and compute code coverage from that test.
     # NOTE we also use "coverage run -p" which will generate a .coverage file with the
     # machine name, process id, and a random number appended to the filename to
     # simplify collecting and merging coverage data from multiple subprocesses. if "-p"
     # is not used, then each "coverage run" will overwrite the .coverage file from a
     # previous "coverage run".
     # NOTE the run_coverage.yml GitHub Action runs "python -m coverage combine" to
-    # combine the individual coverage reprots into one .coverage file.
+    # combine the individual coverage reports into one .coverage file.
 
     def test_validate_file_no_cache(self):
         """Test that validating a file with no cached spec against the core namespace succeeds."""
         result = subprocess.run(["coverage", "run", "-p", "-m", "pynwb.validate",
                                  "tests/back_compat/1.0.2_nwbfile.nwb"], capture_output=True)
 
         stderr_regex = re.compile(
```

### Comparing `pynwb-2.3.1/tox.ini` & `pynwb-2.3.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -182,37 +182,13 @@
 commands =
     python -m pip install -U --pre -e .
     python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
     python -m pip check
     python -m pip list
     python test.py --example
 
-# Test with python 3.8; pinned dev, doc, and optional reqs; upgraded run reqs
-[testenv:gallery-py38-upgraded]
-basepython = python3.8
-deps =
-    -rrequirements-dev.txt
-commands =
-    python -m pip install -U -e .
-    python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
-    python -m pip check
-    python -m pip list
-    python test.py --example
-
-# Test with python 3.8; pinned dev, doc, and optional reqs; pre-release run reqs
-[testenv:gallery-py38-prerelease]
-basepython = python3.8
-deps =
-    -rrequirements-dev.txt
-commands =
-    python -m pip install -U --pre -e .
-    python -m pip install -r requirements-doc.txt  # NOTE: allensdk (requirements-doc.txt) requires pynwb
-    python -m pip check
-    python -m pip list
-    python test.py --example
-
 # Test with python 3.7; pinned dev and doc reqs; minimum run reqs
 [testenv:gallery-py37-minimum]
 basepython = python3.7
 deps =
     -rrequirements-min.txt
 commands = {[testenv:gallery]commands}
```

### Comparing `pynwb-2.3.1/versioneer.py` & `pynwb-2.3.2/versioneer.py`

 * *Files identical despite different names*

