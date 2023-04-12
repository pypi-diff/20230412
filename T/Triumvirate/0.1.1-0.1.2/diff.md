# Comparing `tmp/Triumvirate-0.1.1.tar.gz` & `tmp/Triumvirate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Triumvirate-0.1.1.tar", last modified: Fri Apr  7 00:04:52 2023, max compression
+gzip compressed data, was "Triumvirate-0.1.2.tar", last modified: Wed Apr 12 08:16:35 2023, max compression
```

## Comparing `Triumvirate-0.1.1.tar` & `Triumvirate-0.1.2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.653652 Triumvirate-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    49031 2023-04-07 00:04:52.653652 Triumvirate-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6100 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-07 00:04:52.653652 Triumvirate-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    21704 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.633650 Triumvirate-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.637650 Triumvirate-0.1.1/src/Triumvirate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    49031 2023-04-07 00:04:52.000000 Triumvirate-0.1.1/src/Triumvirate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-07 00:04:52.000000 Triumvirate-0.1.1/src/Triumvirate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:04:52.000000 Triumvirate-0.1.1/src/Triumvirate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-07 00:04:52.000000 Triumvirate-0.1.1/src/Triumvirate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 00:04:52.000000 Triumvirate-0.1.1/src/Triumvirate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.637650 Triumvirate-0.1.1/src/triumvirate/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_bihankel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_fftlog.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_particles.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_particles.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_threept.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_twopt.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_valid_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/_winconv.py
--rw-r--r--   0 runner    (1001) docker     (123)    27588 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/dataobjs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/dataobjs.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.641651 Triumvirate-0.1.1/src/triumvirate/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/arrayops.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/dataobjs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/fftlog.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/field.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/io.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/maths.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/monitor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/parameters.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/particles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/threept.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/include/twopt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/parameters.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    24801 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/parameters.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.641651 Triumvirate-0.1.1/src/triumvirate/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/resources/params_template.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/resources/params_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.641651 Triumvirate-0.1.1/src/triumvirate/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.641651 Triumvirate-0.1.1/src/triumvirate/src/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/arrayops.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/dataobjs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/fftlog.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74090 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/field.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/io.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/maths.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/monitor.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25628 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/parameters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/particles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    74238 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/threept.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/modules/twopt.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/src/triumvirate.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    60607 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/threept.py
--rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/src/triumvirate/twopt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.645651 Triumvirate-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.645651 Triumvirate-0.1.1/tests/test_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_build/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_dataobjs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.633650 Triumvirate-0.1.1/tests/test_input/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.645651 Triumvirate-0.1.1/tests/test_input/ctlgs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/ctlgs/sample_catalogue.dat
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/ctlgs/sample_catalogue.fits
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/ctlgs/sample_catalogue.h5
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/ctlgs/sample_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/ctlgs/test_data_catalogue.txt
--rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/ctlgs/test_rand_catalogue.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.649651 Triumvirate-0.1.1/tests/test_input/params/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/params/test_params.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/params/test_params.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/params/tmpl_params.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:04:52.653652 Triumvirate-0.1.1/tests/test_input/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/bk000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/bk000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/bk000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/bk000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/bk202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/bk202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/pk0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/pk0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/pk2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/pk2_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/xi0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/xi0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/xi2_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/xi2_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/xiw0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/xiw2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zeta000_bin0_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zeta000_bin0_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zeta000_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zeta000_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zeta202_diag_gpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zeta202_diag_lpp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zetaw000_bin0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zetaw000_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_input/stats/zetaw202_diag.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_threept.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-07 00:04:25.000000 Triumvirate-0.1.1/tests/test_twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35149 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    49100 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6169 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22697 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.601791 Triumvirate-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.609791 Triumvirate-0.1.2/src/Triumvirate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49100 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 08:16:35.000000 Triumvirate-0.1.2/src/Triumvirate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.617792 Triumvirate-0.1.2/src/triumvirate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_bihankel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_fftlog.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_particles.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_particles.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_threept.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_twopt.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_valid_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/_winconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27588 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/dataobjs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/dataobjs.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.621791 Triumvirate-0.1.2/src/triumvirate/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/arrayops.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/dataobjs.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/fftlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25731 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/field.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/io.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/maths.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/monitor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/parameters.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/particles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/threept.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/include/twopt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/parameters.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    24801 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/parameters.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.625792 Triumvirate-0.1.2/src/triumvirate/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/resources/params_template.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/resources/params_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.625792 Triumvirate-0.1.2/src/triumvirate/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.629792 Triumvirate-0.1.2/src/triumvirate/src/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/arrayops.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/dataobjs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/fftlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74090 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/field.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/io.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/maths.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/monitor.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25628 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/parameters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/particles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    74238 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/threept.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25335 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/modules/twopt.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/src/triumvirate.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    60607 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45237 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/src/triumvirate/twopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.629792 Triumvirate-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.629792 Triumvirate-0.1.2/tests/test_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_build/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    10584 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_dataobjs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.605791 Triumvirate-0.1.2/tests/test_input/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.633792 Triumvirate-0.1.2/tests/test_input/ctlgs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/test_data_catalogue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3044753 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/ctlgs/test_rand_catalogue.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.637792 Triumvirate-0.1.2/tests/test_input/params/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/params/test_params.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/params/test_params.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/params/tmpl_params.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:16:35.645792 Triumvirate-0.1.2/tests/test_input/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk2_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/pk2_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi2_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xi2_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xiw0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/xiw2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_gpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_lpp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zetaw000_bin0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zetaw000_diag.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_input/stats/zetaw202_diag.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_threept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-12 08:16:01.000000 Triumvirate-0.1.2/tests/test_twopt.py
```

### Comparing `Triumvirate-0.1.1/LICENCE` & `Triumvirate-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/MANIFEST.in` & `Triumvirate-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/Makefile` & `Triumvirate-0.1.2/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -50,29 +50,28 @@
 
 # ------------------------------------------------------------------------
 # OS-dependent Compilation
 # ------------------------------------------------------------------------
 
 # -- Compiler ------------------------------------------------------------
 
-# Assume GCC compiler by default. [modify]
+# Assume GCC compiler by default. [adapt]
 ifeq ($(shell uname -s), Linux)
 
 CXX ?= g++
 
 else ifeq ($(shell uname -s), Darwin)
 
 # Use GCC compiler from Homebrew (brew formula 'gcc').
 # The compiler binary provided may have the suffix '-<version>';
 # check the version number with `brew info gcc` (here 'g++-11' is assumed).
 CXX_DIR = $(shell brew --prefix gcc)/bin
 CXX_BIN = $(shell ls ${CXX_DIR} | grep '^g++')
 CXX ?= ${CXX_DIR}/${CXX_BIN}
 
-# Others: GCC compiler by default. [modify]
 else  # uname -s
 
 CXX ?= g++
 
 endif  # uname -s
 
 
@@ -114,35 +113,38 @@
 # ------------------------------------------------------------------------
 
 # OpenMP: enabled with `useomp=(true|1)`; disabled otherwise.
 ifdef useomp
 
 ifeq ($(strip ${useomp}), $(filter $(strip ${useomp}), true 1))
 
-# Assume GCC OpenMP implementation by default. [modify]
+# Assume GCC OpenMP implementation by default. [adapt]
 ifeq ($(shell uname -s), Linux)
 
-# Pass...
+CXXFLAGS_OMP ?= -fopenmp
+LDFLAGS_OMP ?= -fopenmp
 
 else ifeq ($(shell uname -s), Darwin)
 
-# For LLVM OpenMP implementation, use 'libomp' from Homebrew
-# (brew formula 'libomp'). Set also the following flags.
-# CXXFLAGS += -Xpreprocessor
-# LDFLAGS_OMP = -L$(shell brew --prefix libomp)/lib -lomp
+CXXFLAGS_OMP ?= -fopenmp
+LDFLAGS_OMP ?= -fopenmp
 
-# Pass...
+# For LLVM OpenMP implementation, set the following flags to use the
+# '-Xpreprocessor' option and 'libomp' from Homebrew (brew formula 'libomp').
+# CXXFLAGS_OMP ?= -Xpreprocessor -fopenmp
+# LDFLAGS_OMP ?= -L$(shell brew --prefix libomp)/lib -lomp
 
 else  # uname -s
 
-# Pass...
+CXXFLAGS_OMP ?= -fopenmp
+LDFLAGS_OMP ?= -fopenmp
 
 endif  # uname -s
 
-CXXFLAGS += -fopenmp -DTRV_USE_OMP -DTRV_USE_FFTWOMP
+CXXFLAGS += -DTRV_USE_OMP -DTRV_USE_FFTWOMP ${CXXFLAGS_OMP}
 LDFLAGS += -lfftw3_omp ${LDFLAGS_OMP}
 
 endif  # useomp=(true|1)
 
 else  # useomp
 
 # NOTE: Use `undefine` for make>=3.82.
@@ -179,15 +181,14 @@
 # ------------------------------------------------------------------------
 
 # Python: export CXX compilation options as environmental variables.
 export PY_CXX=${CXX}
 export PY_CXXFLAGS=${CXXFLAGS}
 export PY_LDFLAGS=${LDFLAGS}
 export PY_INCLUDES=${INCLUDES}
-# export PY_OPTS_OMP=${LDFLAGS_OMP}
 ifndef useomp
 export PY_NO_OMP
 endif  # !useomp
 export PY_BUILD_PARALLEL=${MAKEFLAGS_JOBS}
 
 
 # ========================================================================
```

### Comparing `Triumvirate-0.1.1/PKG-INFO` & `Triumvirate-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -734,16 +734,16 @@
 =============
 
 Comprehensive documentation including the `scientific background
 <https://triumvirate.readthedocs.io/en/latest/background.html>`_,
 `installation instructions
 <https://triumvirate.readthedocs.io/en/latest/installation.html>`_,
 `tutorials
-<https://triumvirate.readthedocs.io/en/latest/tutorials.html>`_
-and `API reference
+<https://triumvirate.readthedocs.io/en/latest/tutorials.html>`_ and
+`API reference
 <https://triumvirate.readthedocs.io/en/latest/apiref.html>`_
 can be found at `triumvirate.readthedocs.io
 <https://triumvirate.readthedocs.io/en/latest/>`_.
 
 
 Installation
 ============
@@ -799,32 +799,33 @@
 
     $ make clean
     $ make [py|cpp]install [useomp=(true|1)]
 
 where ``cpplibinstall`` or ``cppappbuild`` respectively builds the C++
 static library or binary executable only, ``cppinstall`` builds both,
 ``pyinstall`` builds the Python package only, and ``install`` builds
-all of the above. To enable OpenMP parallelisation, append ``useomp=true`` or ``useomp=1`` to the end of the second line as shown above.
+all of the above. To enable OpenMP parallelisation, append ``useomp=true``
+or ``useomp=1`` to the end of the second line as shown above.
 
 .. note::
 
     The latest release is on the |main|_ branch. The default |Makefile|_
     (located at the repository directory root) should work in most
     build environments, but may need to be modified as appropriate.
 
 .. note::
 
     See the `Installation
     <https://triumvirate.readthedocs.io/en/latest/installation.html#dependencies>`__
     page in the documentation for more details about dependency requirements.
 
-.. warning::
+.. note::
 
-    Ensure your C++ compiler used supports OpenMP and is configured
-    accordingly. The default |Makefile|_ (located at the repository
+    If enabling OpenMP, ensure the C++ compiler used supports it and is
+    configured accordingly. The default |Makefile|_ (located at the repository
     directory root) assumes the GCC compiler and OpenMP library. See the
     `Installation
     <https://triumvirate.readthedocs.io/en/latest/installation.html#openmp-support>`__
     page in the documentation for more details.
 
 .. note::
 
@@ -833,20 +834,20 @@
     parallel jobs; see `GNU Make Manual
     <https://www.gnu.org/software/make/manual/html_node/Options-Summary.html>`_).
 
 
 Attribution
 ===========
 
-.. image:: https://img.shields.io/badge/JOSS-doi-brightgreen
-    :target: https://joss.theoj.org/papers/?/status.svg
+.. image:: https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f/status.svg
+    :target: https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f
     :alt: JOSS
 
-.. image:: https://img.shields.io/badge/arXiv-yymm.%3F-b31b1b
-    :target: https://arxiv.org/abs/?.?
+.. image:: https://img.shields.io/badge/arXiv-2304.03643-b31b1b
+    :target: https://arxiv.org/abs/2304.03643
     :alt: arXiv
 
 .. image:: https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fsty3249-informational
     :target: https://doi.org/10.1093/mnras/sty3249
     :alt: MNRAS
 
 .. image:: https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fstx2333-informational
@@ -899,15 +900,15 @@
 |Triumvirate| is made freely available under the `GPL-3.0 licence
 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_. Please see |Licence|_
 (located at the repository directory root) for full terms and conditions.
 
 &copy; 2023 Mike S Wang & Naonori S Sugiyama
 
 
-.. |Triumvirate| replace:: Triumvirate
+.. |Triumvirate| replace:: ``Triumvirate``
 
 .. |hitomi| replace:: ``hitomi``
 .. _hitomi: https://github.com/naonori/hitomi
 
 .. |main| replace:: ``main``
 .. _main: https://github.com/MikeSWang/Triumvirate/tree/main
```

### Comparing `Triumvirate-0.1.1/README.md` & `Triumvirate-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 ## Documentation
 
 Comprehensive documentation including the [scientific background](
 https://triumvirate.readthedocs.io/en/latest/background.html),
 [installation instructions](
 https://triumvirate.readthedocs.io/en/latest/installation.html),
 [tutorials](https://triumvirate.readthedocs.io/en/latest/tutorials.html) and
-[API reference](https://triumvirate.readthedocs.io/en/latest/apiref.html) can
-be found at [triumvirate.readthedocs.io](
+[API reference](https://triumvirate.readthedocs.io/en/latest/apiref.html)
+can be found at [triumvirate.readthedocs.io](
 https://triumvirate.readthedocs.io/en/latest/).
 
 
 ## Installation
 
 ### Python package
 
@@ -79,31 +79,31 @@
 > [``Makefile``](Makefile) (located at the repository directory root) should
 > work in most build environments, but may need to be modified as appropriate.
 
 > :bulb: See the [Installation](
 > https://triumvirate.readthedocs.io/en/latest/installation.html#dependencies)
 > page in the documentation for more details about dependency requirements.
 
-> :warning: Ensure the C++ compiler used supports OpenMP and is configured
-> accordingly. The default [``Makefile``](Makefile) (located at the repository
-> directory root) assumes the GCC compiler and OpenMP library. See the
-> [Installation](
+> :warning: If enabling OpenMP, ensure the C++ compiler used supports it and is
+> configured accordingly. The default [``Makefile``](Makefile) (located at the
+> repository directory root) assumes the GCC compiler and OpenMP library. See
+> the [Installation](
 > https://triumvirate.readthedocs.io/en/latest/installation.html#openmp-support)
 > page in the documentation for more details.
 
 > :bulb: Pass option ``-j[N] -O`` to `make` to run multiple concurrent jobs
 > for parallel building (optional parameter ``N`` is the number of
 > parallel jobs; see [GNU Make Manual](
 > https://www.gnu.org/software/make/manual/html_node/Options-Summary.html)).
 
 
 ## Attribution
 
-[![JOSS](https://img.shields.io/badge/JOSS-doi-brightgreen)](https://joss.theoj.org/papers/?/status.svg)
-[![arXiv](https://img.shields.io/badge/arXiv-yymm.%3F-b31b1b)](https://arxiv.org/abs/?.?)
+[![JOSS](https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f/status.svg)](https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f)
+[![arXiv](https://img.shields.io/badge/arXiv-2304.03643-b31b1b)](https://arxiv.org/abs/2304.03643)
 [![MNRAS](https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fsty3249-informational)](https://doi.org/10.1093/mnras/sty3249)
 [![MNRAS](https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fstx2333-informational)](https://doi.org/10.1093/mnras/stx2333)
 
 To acknowledge the use of ``Triumvirate`` in your published research, please
 cite the publications linked above which contain the relevant information
 in the BibTeX format.
```

### Comparing `Triumvirate-0.1.1/README.rst` & `Triumvirate-0.1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 =============
 
 Comprehensive documentation including the `scientific background
 <https://triumvirate.readthedocs.io/en/latest/background.html>`_,
 `installation instructions
 <https://triumvirate.readthedocs.io/en/latest/installation.html>`_,
 `tutorials
-<https://triumvirate.readthedocs.io/en/latest/tutorials.html>`_
-and `API reference
+<https://triumvirate.readthedocs.io/en/latest/tutorials.html>`_ and
+`API reference
 <https://triumvirate.readthedocs.io/en/latest/apiref.html>`_
 can be found at `triumvirate.readthedocs.io
 <https://triumvirate.readthedocs.io/en/latest/>`_.
 
 
 Installation
 ============
@@ -97,32 +97,33 @@
 
     $ make clean
     $ make [py|cpp]install [useomp=(true|1)]
 
 where ``cpplibinstall`` or ``cppappbuild`` respectively builds the C++
 static library or binary executable only, ``cppinstall`` builds both,
 ``pyinstall`` builds the Python package only, and ``install`` builds
-all of the above. To enable OpenMP parallelisation, append ``useomp=true`` or ``useomp=1`` to the end of the second line as shown above.
+all of the above. To enable OpenMP parallelisation, append ``useomp=true``
+or ``useomp=1`` to the end of the second line as shown above.
 
 .. note::
 
     The latest release is on the |main|_ branch. The default |Makefile|_
     (located at the repository directory root) should work in most
     build environments, but may need to be modified as appropriate.
 
 .. note::
 
     See the `Installation
     <https://triumvirate.readthedocs.io/en/latest/installation.html#dependencies>`__
     page in the documentation for more details about dependency requirements.
 
-.. warning::
+.. note::
 
-    Ensure your C++ compiler used supports OpenMP and is configured
-    accordingly. The default |Makefile|_ (located at the repository
+    If enabling OpenMP, ensure the C++ compiler used supports it and is
+    configured accordingly. The default |Makefile|_ (located at the repository
     directory root) assumes the GCC compiler and OpenMP library. See the
     `Installation
     <https://triumvirate.readthedocs.io/en/latest/installation.html#openmp-support>`__
     page in the documentation for more details.
 
 .. note::
 
@@ -131,20 +132,20 @@
     parallel jobs; see `GNU Make Manual
     <https://www.gnu.org/software/make/manual/html_node/Options-Summary.html>`_).
 
 
 Attribution
 ===========
 
-.. image:: https://img.shields.io/badge/JOSS-doi-brightgreen
-    :target: https://joss.theoj.org/papers/?/status.svg
+.. image:: https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f/status.svg
+    :target: https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f
     :alt: JOSS
 
-.. image:: https://img.shields.io/badge/arXiv-yymm.%3F-b31b1b
-    :target: https://arxiv.org/abs/?.?
+.. image:: https://img.shields.io/badge/arXiv-2304.03643-b31b1b
+    :target: https://arxiv.org/abs/2304.03643
     :alt: arXiv
 
 .. image:: https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fsty3249-informational
     :target: https://doi.org/10.1093/mnras/sty3249
     :alt: MNRAS
 
 .. image:: https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fstx2333-informational
@@ -197,15 +198,15 @@
 |Triumvirate| is made freely available under the `GPL-3.0 licence
 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_. Please see |Licence|_
 (located at the repository directory root) for full terms and conditions.
 
 &copy; 2023 Mike S Wang & Naonori S Sugiyama
 
 
-.. |Triumvirate| replace:: Triumvirate
+.. |Triumvirate| replace:: ``Triumvirate``
 
 .. |hitomi| replace:: ``hitomi``
 .. _hitomi: https://github.com/naonori/hitomi
 
 .. |main| replace:: ``main``
 .. _main: https://github.com/MikeSWang/Triumvirate/tree/main
```

### Comparing `Triumvirate-0.1.1/pyproject.toml` & `Triumvirate-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -89,27 +89,23 @@
 ]
 before-build = [
     "export PY_BUILD_PARALLEL=-j",
 ]
 test-requires = "pytest"
 test-command = "pytest {project}/tests"
 
-# Use images that support `apt` as `yum` hangs in CentOS.
+# BUG: Use images that support `apt` as `yum` hangs in CentOS.
 manylinux-x86_64-image = 'manylinux_2_24'
 manylinux-aarch64-image = 'manylinux_2_24'
 
 [tool.cibuildwheel.linux]
 before-all = [
     "apt-get update",
     "apt-get install -y libgsl-dev libfftw3-dev",
 ]
 
 [tool.cibuildwheel.macos]
 before-all = [
+    # Optional: Homebrew update is slow.
     # "brew update",
     "brew install gsl fftw",
 ]
-before-build = [
-    "export PY_CXX_DIR=$(brew --prefix gcc)/bin",
-    "export PY_CXX_BIN=$(ls ${PY_CXX_DIR} | grep '^g++')",
-    "export PY_CXX=${PY_CXX_DIR}/${PY_CXX_BIN}",
-]
```

### Comparing `Triumvirate-0.1.1/setup.cfg` & `Triumvirate-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/setup.py` & `Triumvirate-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import numpy
 from Cython.Build import cythonize
 from Cython.Distutils import build_ext, Extension
 from extension_helpers._openmp_helpers import check_openmp_support
 from extension_helpers._setup_helpers import pkg_config
 
 
-distutils_logger = logging.getLogger()  # recycled from :mod:`distutils`
+distutils_logger = logging.getLogger()  # recycled from :mod:`distutils._log`
 
 
 # ========================================================================
 # Package
 # ========================================================================
 
 PROJECT_NAME = 'Triumvirate'
@@ -87,15 +87,15 @@
         C++ source directory.
 
     """
     return os.path.join(get_pkg_dir(), subdir)
 
 
 # ========================================================================
-# Commands
+# Build
 # ========================================================================
 
 class BuildExt(build_ext):
     """Modified :class:`Cython.Distutils.build_ext`.
 
     """
     def finalize_options(self):
@@ -194,16 +194,17 @@
 
     """
     PY_ENV_VARS = [
         'PY_CXX',
         'PY_CXXFLAGS',
         'PY_LDFLAGS',
         'PY_INCLUDES',
-        'PY_OPTS_OMP',
         'PY_NO_OMP',
+        'PY_CXXFLAGS_OMP',
+        'PY_LDFLAGS_OMP',
         'PY_BUILD_PARALLEL',
     ]
     for env_var in PY_ENV_VARS:
         prioprint("{}={}".format(env_var, os.environ.get(env_var)))
 
 
 def display_py_options():
@@ -222,34 +223,19 @@
         prioprint("{}={}".format(opt_type, globals().get(opt_type)))
 
 
 # ========================================================================
 # Compilation
 # ========================================================================
 
-# -- Language ------------------------------------------------------------
-
 EXT_LANG = 'c++'
 
 
 # -- Environment ---------------------------------------------------------
 
-# Default to GCC compiler and OpenMP implementation.
-COMPILERS = {
-    'default': 'g++',
-    'linux': 'g++',
-    'darwin': 'g++',  # alternatively 'clang++'
-}
-OPENMP_LIBS = {
-    'default': 'gomp',  # alternatively 'omp'
-    'linux': '',  # set by ``-fopenmp``
-    'darwin': '',  # set by ``-fopenmp``
-}
-
-
 def get_platform():
     """Get the build platform.
 
     Returns
     -------
     {'linux', 'darwin', 'default'}
 
@@ -257,49 +243,91 @@
     build_platform = platform.system().lower()
     if build_platform not in ['linux', 'darwin']:
         build_platform = 'default'
 
     return build_platform
 
 
+# -- Compiler ------------------------------------------------------------
+
+# List default compilers (GCC assumed).
+COMPILERS = {
+    'default': 'g++',
+    'linux': 'g++',
+    'darwin': 'g++',
+}
+
+
 def get_compiler():
     """Get the build compiler.
 
     Returns
     -------
     str
+        Build compiler.
 
     """
     compiler = os.environ.get('PY_CXX', COMPILERS[get_platform()])
 
     return compiler
 
 
 def set_cli_compiler(compiler=None):
-    """Set command-line compiler through the ``CC``, ``CXX`` and ``CPP``
+    """Set command-line compiler through the ``CC``and ``CXX``
     environmental variables.
 
     """
-    compiler = compiler or get_compiler()
+    _compiler = compiler or get_compiler()
 
-    os.environ['CC'] = compiler
-    os.environ['CXX'] = compiler
-    os.environ['CPP'] = compiler
+    os.environ['CC'] = _compiler
+    os.environ['CXX'] = _compiler
 
 
 # -- Dependencies --------------------------------------------------------
 
+# Default to GCC OpenMP implementation.
+OPENMP_LIBS = {
+    'default': 'gomp',  # 'omp'
+    'linux': '',  # set by ``-fopenmp`` or environment
+    'darwin': '',  # set by ``-fopenmp`` or environment
+}
+
+
 LIBS_CORE = ['gsl', 'fftw3',]  # noqa: E231
 LIBS_FULL = ['gsl', 'gslcblas', 'm', 'fftw3',]  # noqa: E231
 
 PKG_LIB_NAME = 'trv'
 
 
 # -- Options -------------------------------------------------------------
 
+def convert_macro(macro):
+    """Convert a macro flag to a tuple.
+
+    Parameters
+    ----------
+    macro : str
+        Macro as a flag
+
+    Returns
+    -------
+    tuple (str, Union[str, None])
+        Macro as a tuple
+
+    """
+    macro_ = macro.lstrip('-D').split('=')
+    if len(macro_) == 1:
+        return (macro_.pop(), None)
+    if len(macro_) == 2:
+        return tuple(macro_)
+    raise ValueError(
+        "Invalid macro to convert: {}.".format(macro_)
+    )
+
+
 def parse_cli_cflags():
     """Parse command-line ``PY_CXXFLAGS`` components for extension
     keyword arguments.
 
     Returns
     -------
     list of str, list of str
@@ -307,23 +335,15 @@
 
     """
     cli_cflags = os.environ.get('PY_CXXFLAGS', '').split()
 
     parsed_macros, parsed_cflags = [], []
     for cflag_ in cli_cflags:
         if cflag_.startswith('-D'):
-            macro_ = cflag_.lstrip('-D').split('=')
-            if len(macro_) == 1:
-                parsed_macros.append((macro_.pop(), None))
-            elif len(macro_) == 2:
-                parsed_macros.append(tuple(macro_))
-            else:
-                raise ValueError(
-                    "Invalid macro in CXXFLAGS: {}.".format(cflag_)
-                )
+            parsed_macros.append(convert_macro(cflag_))
         else:
             parsed_cflags.append(cflag_)
 
     return parsed_macros, parsed_cflags
 
 
 def parse_cli_ldflags():
@@ -362,21 +382,48 @@
     """
     parsed_include_dirs = \
         os.environ.get('PY_INCLUDES', '').replace('-I', '').split()
 
     return parsed_include_dirs
 
 
-def parse_cli_opts_omp():
-    """Parse command-line ``PY_OPTS_OMP`` components for extension
+def parse_cli_cflags_omp():
+    """Parse command-line ``PY_CXXFLAGS_OMP`` components for extension
+    keyword arguments.
+
+    """
+    cli_cflags_omp = os.environ.get('PY_CXXFLAGS_OMP', '').split()
+    if not cli_cflags_omp:
+        return None
+
+    parsed_macros_omp, parsed_cflags_omp = [], []
+    for cflag_ in cli_cflags_omp:
+        if cflag_.startswith('-D'):
+            macro_ = cflag_.lstrip('-D').split('=')
+            if len(macro_) == 1:
+                parsed_macros_omp.append((macro_.pop(), None))
+            elif len(macro_) == 2:
+                parsed_macros_omp.append(tuple(macro_))
+            else:
+                raise ValueError(
+                    "Invalid macro in CXXFLAG_OMP: {}.".format(cflag_)
+                )
+        else:
+            parsed_cflags_omp.append(cflag_)
+
+    return parsed_macros_omp, parsed_cflags_omp
+
+
+def parse_cli_ldflags_omp():
+    """Parse command-line ``PY_LDFLAGS_OMP`` components for extension
     keyword arguments.
 
     """
-    cli_ldflags_omp = os.environ.get('PY_OPTS_OMP')
-    if cli_ldflags_omp is None:
+    cli_ldflags_omp = os.environ.get('PY_LDFLAGS_OMP', '').split()
+    if not cli_ldflags_omp:
         return None
 
     parsed_ldflags_omp, parsed_libs_omp, parsed_lib_dirs_omp = [], [], []
     for ldflag_ in cli_ldflags_omp:
         if ldflag_.startswith('-l'):
             parsed_libs_omp.append(ldflag_.lstrip('-l'))
         elif ldflag_.startswith('-L'):
@@ -422,16 +469,16 @@
 
     """
     libs_core = deepcopy(LIBS_CORE)
     libs_full = deepcopy(LIBS_FULL)
 
     for lib_ in libs:
         if lib_ not in libs_full:
-            libs_full.append(lib_)
             libs_core.append(lib_)
+            libs_full.append(lib_)
 
     checked_options = pkg_config(libs_core, default_libraries=libs_full)
 
     for macro_ in checked_options['define_macros']:
         if macro_ not in macros:
             macros.append(macro_)
     for macro_ in checked_options['undef_macros']:
@@ -448,17 +495,19 @@
             lib_dirs.append(lib_dir_)
 
     libs = checked_options['libraries']
 
     return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
 
-def add_options_openmp(macros, cflags, ldflags, libs, lib_dirs, include_dirs):
+def add_options_omp(macros, cflags, ldflags, libs, lib_dirs, include_dirs):
     """Add OpenMP options, if enabled.
 
+    By default, GCC OpenMP is assumed.
+
     Parameters
     ----------
     macros : list of tuple (str, Union[str, None])
         Macros without '-D' prefix.
     cflags : list of str
         ``CXXFLAGS`` components.
     ldflags : list of str
@@ -473,15 +522,15 @@
     Returns
     -------
     macros : list of tuple (str, Union[str, None])
         Processed macros without '-D' prefix.
     cflags : list of str
         Processed ``CXXFLAGS`` components.
     ldflags : list of str
-        Processed ``LDFLAGS`` components without '-l' prefix.
+        Processed ``LDFLAGS`` components non-'-l' prefix.
     libs : list of str
         Libraries without the '-l' prefix.
     lib_dirs : list of str
         Library directories without the '-L' prefix.
     include_dirs :list of str
         ``INCLUDES`` directories without the '-I' prefix.
 
@@ -495,50 +544,50 @@
     if not check_openmp_support():
         prioprint(
             "OpenMP is disabled as "
             "it is not supported in this build enviromnent."
         )
         return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
-    # Otherwise, enabled OpenMP by default.
+    # Enable OpenMP by default otherwise.
     prioprint("OpenMP is enabled by default.")
 
-    # Adapt macros, with the removal of duplicate options from `cflags`.
-    MACROS_OMP = [
+    # Adapt macros and `cflags`.
+    MACROS_OMP_RELATED = [
         ('TRV_USE_OMP', None),
         ('TRV_USE_FFTWOMP', None),
     ]
-
-    for macro_ in MACROS_OMP:
+    for macro_ in MACROS_OMP_RELATED:
         if macro_ not in macros:
             macros.append(macro_)
 
-        macro_cflag_ = '-D' + macro_[0]
-        if macro_cflag_ in cflags:
-            cflags.remove(macro_cflag_)
-
-    # Adapt `cflags`.
-    CXXFLAGS_OMP = [
-        '-fopenmp',
-    ]
+    try:
+        macros_omp, cflags_omp = parse_cli_cflags_omp()
+    except TypeError:
+        macros_omp = []
+        cflags_omp = ['-fopenmp',]  # noqa: E231
 
-    for cflag_ in CXXFLAGS_OMP:
+    for macro_ in macros_omp:
+        macro_ = convert_macro(macro_)
+        if macro_ not in macros:
+            macros.append(macro_)
+    for cflag_ in cflags_omp:
         if cflag_ not in cflags:
             cflags.append(cflag_)
 
     # Adapt `ldflags`, `libs` and `lib_dirs`.
     LIBS_OMP_BASED = [
         'fftw3_omp',
     ]  # noqa: E231
     for lib_ in LIBS_OMP_BASED:
         if lib_ and lib_ not in libs:
             libs.append(lib_)
 
     try:
-        ldflags_omp, libs_omp, lib_dirs_omp = parse_cli_opts_omp()
+        ldflags_omp, libs_omp, lib_dirs_omp = parse_cli_ldflags_omp()
     except TypeError:
         ldflags_omp = ['-fopenmp',]  # noqa: E231
         libs_omp = [OPENMP_LIBS[get_platform()],]  # noqa: E231
         lib_dirs_omp = []  # noqa: E231
 
     for ldflag_ in ldflags_omp:
         if ldflag_ not in ldflags:
@@ -574,15 +623,15 @@
     Returns
     -------
     macros : list of tuple (str, Union[str, None])
         Processed macros without '-D' prefix.
     cflags : list of str
         Processed ``CXXFLAGS`` components.
     ldflags : list of str
-        Processed ``LDFLAGS`` components without '-l' prefix.
+        Processed ``LDFLAGS`` components non-'-l' prefix.
     libs : list of str
         Libraries without the '-l' prefix.
     lib_dirs : list of str
         Library directories without the '-L' prefix.
     include_dirs : list of str
         ``INCLUDES`` directories without the '-I' prefix.
 
@@ -616,20 +665,15 @@
         if include_dir_ not in include_dirs:
             include_dirs.append(include_dir_)
 
     return macros, cflags, ldflags, libs, lib_dirs, include_dirs
 
 
 # ========================================================================
-# Build
-# ========================================================================
-
-
-# ========================================================================
-# Extensions
+# Targets
 # ========================================================================
 
 CYTHON_DIRECTIVES = {
    'language_level': '3',
    'c_string_encoding': 'utf-8',
    'embedsignature': True,
 }
@@ -666,18 +710,15 @@
     ]
 
     pkg_cfg = {
         cfg_opt: globals()[cfg_opt]
         for cfg_opt in ['macros', 'cflags', 'include_dirs',]  # noqa: E231
     }
 
-    pkg_library = (
-        lib_name,
-        dict(sources=pkg_sources, **pkg_cfg)
-    )
+    pkg_library = (lib_name, dict(sources=pkg_sources, **pkg_cfg))
 
     return pkg_library
 
 
 def define_pkg_extension(ext_name,
                          auto_cpp_source=False, extra_cpp_sources=None,
                          **ext_kwargs):
@@ -762,15 +803,15 @@
     ldflags, libs, lib_dirs = parse_cli_ldflags()
     include_dirs = parse_cli_includes()
 
     # Adapt compilation options.
     macros, cflags, ldflags, libs, lib_dirs, include_dirs = add_options_nonomp(
         macros, cflags, ldflags, libs, lib_dirs, include_dirs
     )
-    macros, cflags, ldflags, libs, lib_dirs, include_dirs = add_options_openmp(
+    macros, cflags, ldflags, libs, lib_dirs, include_dirs = add_options_omp(
         macros, cflags, ldflags, libs, lib_dirs, include_dirs
     )
     macros, cflags, ldflags, libs, lib_dirs, include_dirs = add_options_pkgs(
         macros, cflags, ldflags, libs, lib_dirs, include_dirs
     )
 
     # Check compilation options.
```

### Comparing `Triumvirate-0.1.1/src/Triumvirate.egg-info/PKG-INFO` & `Triumvirate-0.1.2/src/Triumvirate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Triumvirate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Three-point clustering measurements in large-scale structure analyses.
 Home-page: https://mikeswang.github.io/Triumvirate
 Author: Mike S Wang, Naonori S Sugiyama
 Maintainer: Mike S Wang
 Maintainer-email: Mike S Wang <mikeshengbo.wang@ed.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -734,16 +734,16 @@
 =============
 
 Comprehensive documentation including the `scientific background
 <https://triumvirate.readthedocs.io/en/latest/background.html>`_,
 `installation instructions
 <https://triumvirate.readthedocs.io/en/latest/installation.html>`_,
 `tutorials
-<https://triumvirate.readthedocs.io/en/latest/tutorials.html>`_
-and `API reference
+<https://triumvirate.readthedocs.io/en/latest/tutorials.html>`_ and
+`API reference
 <https://triumvirate.readthedocs.io/en/latest/apiref.html>`_
 can be found at `triumvirate.readthedocs.io
 <https://triumvirate.readthedocs.io/en/latest/>`_.
 
 
 Installation
 ============
@@ -799,32 +799,33 @@
 
     $ make clean
     $ make [py|cpp]install [useomp=(true|1)]
 
 where ``cpplibinstall`` or ``cppappbuild`` respectively builds the C++
 static library or binary executable only, ``cppinstall`` builds both,
 ``pyinstall`` builds the Python package only, and ``install`` builds
-all of the above. To enable OpenMP parallelisation, append ``useomp=true`` or ``useomp=1`` to the end of the second line as shown above.
+all of the above. To enable OpenMP parallelisation, append ``useomp=true``
+or ``useomp=1`` to the end of the second line as shown above.
 
 .. note::
 
     The latest release is on the |main|_ branch. The default |Makefile|_
     (located at the repository directory root) should work in most
     build environments, but may need to be modified as appropriate.
 
 .. note::
 
     See the `Installation
     <https://triumvirate.readthedocs.io/en/latest/installation.html#dependencies>`__
     page in the documentation for more details about dependency requirements.
 
-.. warning::
+.. note::
 
-    Ensure your C++ compiler used supports OpenMP and is configured
-    accordingly. The default |Makefile|_ (located at the repository
+    If enabling OpenMP, ensure the C++ compiler used supports it and is
+    configured accordingly. The default |Makefile|_ (located at the repository
     directory root) assumes the GCC compiler and OpenMP library. See the
     `Installation
     <https://triumvirate.readthedocs.io/en/latest/installation.html#openmp-support>`__
     page in the documentation for more details.
 
 .. note::
 
@@ -833,20 +834,20 @@
     parallel jobs; see `GNU Make Manual
     <https://www.gnu.org/software/make/manual/html_node/Options-Summary.html>`_).
 
 
 Attribution
 ===========
 
-.. image:: https://img.shields.io/badge/JOSS-doi-brightgreen
-    :target: https://joss.theoj.org/papers/?/status.svg
+.. image:: https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f/status.svg
+    :target: https://joss.theoj.org/papers/a8325e3897dd726d9df42286bf72d19f
     :alt: JOSS
 
-.. image:: https://img.shields.io/badge/arXiv-yymm.%3F-b31b1b
-    :target: https://arxiv.org/abs/?.?
+.. image:: https://img.shields.io/badge/arXiv-2304.03643-b31b1b
+    :target: https://arxiv.org/abs/2304.03643
     :alt: arXiv
 
 .. image:: https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fsty3249-informational
     :target: https://doi.org/10.1093/mnras/sty3249
     :alt: MNRAS
 
 .. image:: https://img.shields.io/badge/doi-10.1093%2Fmnras%2Fstx2333-informational
@@ -899,15 +900,15 @@
 |Triumvirate| is made freely available under the `GPL-3.0 licence
 <https://www.gnu.org/licenses/gpl-3.0.en.html>`_. Please see |Licence|_
 (located at the repository directory root) for full terms and conditions.
 
 &copy; 2023 Mike S Wang & Naonori S Sugiyama
 
 
-.. |Triumvirate| replace:: Triumvirate
+.. |Triumvirate| replace:: ``Triumvirate``
 
 .. |hitomi| replace:: ``hitomi``
 .. _hitomi: https://github.com/naonori/hitomi
 
 .. |main| replace:: ``main``
 .. _main: https://github.com/MikeSWang/Triumvirate/tree/main
```

### Comparing `Triumvirate-0.1.1/src/Triumvirate.egg-info/SOURCES.txt` & `Triumvirate-0.1.2/src/Triumvirate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/__init__.py` & `Triumvirate-0.1.2/src/triumvirate/__init__.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/_bihankel.py` & `Triumvirate-0.1.2/src/triumvirate/_bihankel.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/_fftlog.pyx` & `Triumvirate-0.1.2/src/triumvirate/_fftlog.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 FFTLog algorithm (:mod:`~triumvirate._fftlog`)
 ==========================================================================
 
-Implementation of the FFTLog algorithm for Hankel-related transforms.
+Implement the FFTLog algorithm for Hankel-related transforms.
 
 """
 import numpy as np
 cimport numpy as np
 
 
 cdef extern from "include/fftlog.hpp":
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/_particles.pxd` & `Triumvirate-0.1.2/src/triumvirate/_particles.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Declaration of :cpp:class:`trv::ParticleCatalogue` and its
+"""Declare :cpp:class:`trv::ParticleCatalogue` and its
 data-loading method.
 
 """
 from libcpp.vector cimport vector
 
 
 cdef extern from "include/particles.hpp":
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/_particles.pyx` & `Triumvirate-0.1.2/src/triumvirate/_particles.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/_threept.pyx` & `Triumvirate-0.1.2/src/triumvirate/_threept.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Three-Point Correlator Algorithms (:mod:`~triumvirate._threept`)
 ==========================================================================
 
-Declaration and wrapping of three-point correlator algorithms.
+Declare and interface with three-point correlator algorithms.
 
 """
 from cython.operator cimport dereference as deref
 from libc.stdlib cimport free, malloc
 from libcpp cimport bool as bool_t
 
 import numpy as np
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/_twopt.pyx` & `Triumvirate-0.1.2/src/triumvirate/_twopt.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Two-Point Correlator Algorithms (:mod:`~triumvirate._twopt`)
 ==========================================================================
 
-Declaration and wrapping of two-point correlator algorithms.
+Declare and interface with two-point correlator algorithms.
 
 """
 from cython.operator cimport dereference as deref
 from libc.stdlib cimport free, malloc
 
 import numpy as np
 cimport numpy as np
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/_valid_install.py` & `Triumvirate-0.1.2/src/triumvirate/_valid_install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-"""Validate installation.
+"""
+Installation Validation (:mod:`~triumvirate._valid_install`)
+==========================================================================
+
+Check whether the Cython extensions have been compiled correctly by
+performing test computations.
 
-This private module checks whether the Cython extensions have been
-compiled correctly by performing test computations.  It is not meant to
-replace the full `pytest` suite, and does not check the correctness
-of the computed results.
+It is not meant to replace the full `pytest` suite, and does not check the
+correctness of the computed results.
 
 """
 import warnings
 
 import numpy as np
 
 from triumvirate.catalogue import ParticleCatalogue
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/_winconv.py` & `Triumvirate-0.1.2/src/triumvirate/_winconv.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/catalogue.py` & `Triumvirate-0.1.2/src/triumvirate/catalogue.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/dataobjs.pxd` & `Triumvirate-0.1.2/src/triumvirate/dataobjs.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Declaration of data objects.
+"""Declare data objects.
 
 """
 from libcpp.string cimport string
 from libcpp.vector cimport vector
 
 cimport numpy as np
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/dataobjs.pyx` & `Triumvirate-0.1.2/src/triumvirate/dataobjs.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/arrayops.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/arrayops.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/dataobjs.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/dataobjs.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/fftlog.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/fftlog.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/field.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/field.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/io.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/io.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/maths.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/maths.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/monitor.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/monitor.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/parameters.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/parameters.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/particles.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/particles.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/threept.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/threept.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/include/twopt.hpp` & `Triumvirate-0.1.2/src/triumvirate/include/twopt.hpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/logger.py` & `Triumvirate-0.1.2/src/triumvirate/logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/parameters.pxd` & `Triumvirate-0.1.2/src/triumvirate/parameters.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Declaration of :cpp:class:`trv::ParameterSet` and
-its members and methods.
+"""Declare :cpp:class:`trv::ParameterSet` and its members and methods.
 
 """
 from libcpp cimport bool as bool_t
 from libcpp.string cimport string
 
 
 cdef extern from "include/parameters.hpp":
```

### Comparing `Triumvirate-0.1.1/src/triumvirate/parameters.pyx` & `Triumvirate-0.1.2/src/triumvirate/parameters.pyx`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/resources/params_template.ini` & `Triumvirate-0.1.2/src/triumvirate/resources/params_template.ini`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/resources/params_template.yml` & `Triumvirate-0.1.2/src/triumvirate/resources/params_template.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/arrayops.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/arrayops.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/dataobjs.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/dataobjs.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/fftlog.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/fftlog.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/field.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/field.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/io.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/io.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/maths.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/maths.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/monitor.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/monitor.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/parameters.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/parameters.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/particles.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/particles.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/threept.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/threept.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/modules/twopt.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/modules/twopt.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/src/triumvirate.cpp` & `Triumvirate-0.1.2/src/triumvirate/src/triumvirate.cpp`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/threept.py` & `Triumvirate-0.1.2/src/triumvirate/threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/src/triumvirate/twopt.py` & `Triumvirate-0.1.2/src/triumvirate/twopt.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/conftest.py` & `Triumvirate-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_catalogue.py` & `Triumvirate-0.1.2/tests/test_catalogue.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_dataobjs.py` & `Triumvirate-0.1.2/tests/test_dataobjs.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/ctlgs/sample_catalogue.fits` & `Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.fits`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/ctlgs/sample_catalogue.h5` & `Triumvirate-0.1.2/tests/test_input/ctlgs/sample_catalogue.h5`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/ctlgs/test_rand_catalogue.txt` & `Triumvirate-0.1.2/tests/test_input/ctlgs/test_rand_catalogue.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/params/test_params.ini` & `Triumvirate-0.1.2/tests/test_input/params/test_params.ini`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/params/test_params.yml` & `Triumvirate-0.1.2/tests/test_input/params/test_params.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/params/tmpl_params.yml` & `Triumvirate-0.1.2/tests/test_input/params/tmpl_params.yml`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/bk000_bin0_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/bk000_bin0_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/bk000_bin0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/bk000_diag_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/bk000_diag_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/bk000_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/bk202_diag_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/bk202_diag_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/bk202_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/pk0_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/pk0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/pk0_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/pk0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/pk2_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/pk2_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/pk2_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/pk2_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/xi0_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/xi0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/xi0_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/xi0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/xi2_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/xi2_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/xi2_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/xi2_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/xiw0.txt` & `Triumvirate-0.1.2/tests/test_input/stats/xiw0.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/xiw2.txt` & `Triumvirate-0.1.2/tests/test_input/stats/xiw2.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zeta000_bin0_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zeta000_bin0_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zeta000_bin0_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zeta000_diag_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zeta000_diag_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zeta000_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zeta202_diag_gpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_gpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zeta202_diag_lpp.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zeta202_diag_lpp.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zetaw000_bin0.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zetaw000_bin0.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zetaw000_diag.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zetaw000_diag.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_input/stats/zetaw202_diag.txt` & `Triumvirate-0.1.2/tests/test_input/stats/zetaw202_diag.txt`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_logger.py` & `Triumvirate-0.1.2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_parameters.py` & `Triumvirate-0.1.2/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_threept.py` & `Triumvirate-0.1.2/tests/test_threept.py`

 * *Files identical despite different names*

### Comparing `Triumvirate-0.1.1/tests/test_twopt.py` & `Triumvirate-0.1.2/tests/test_twopt.py`

 * *Files identical despite different names*

