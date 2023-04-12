# Comparing `tmp/foldedleastsquares-1.0.38.tar.gz` & `tmp/foldedleastsquares-1.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foldedleastsquares-1.0.38.tar", last modified: Wed Apr 12 15:32:52 2023, max compression
+gzip compressed data, was "dist/foldedleastsquares-1.0.39.tar", last modified: Wed Apr 12 16:01:56 2023, max compression
```

## Comparing `foldedleastsquares-1.0.38.tar` & `foldedleastsquares-1.0.39.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/tutorials/
--rwxrwxrwx   0 martin    (1000) martin    (1000)   205928 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/07 The influence of limb darkening values.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   272427 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/10 Measurement uncertainties.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   277149 2021-01-23 08:20:50.000000 foldedleastsquares-1.0.38/tutorials/12 A comet-like transit from Kepler KIC 12557548 with TLS.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   614539 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/11 A planet from TESS with TLS.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)    56339 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/data_per_t14.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)   333163 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/02 Starter's guide - K2-3b, a red dwarf with a planet.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   229894 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/04 Exploring the TLS spectra and statistics.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)  1116963 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/01 Quick start with synthetic data.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   553194 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/03 Multiple planets - K2-3, a red dwarf with 3 Super-Earths.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)    42518 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/08 Edge effect jitter correction.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   199436 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/06 Comparison between TLS and BLS.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)    99387 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/05 Custom transit shapes - Example of the grazing planet WASP-75.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   124754 2021-01-23 08:28:23.000000 foldedleastsquares-1.0.38/tutorials/13 Flares detection from TESS Proxima Centauri data.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   568511 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/tutorials/09 Optimal period grid and optimal duration grid.ipynb
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     5220 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       79 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     3263 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      107 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     5220 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/PKG-INFO
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/.github/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 martin    (1000) martin    (1000)      635 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/documentation.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)      604 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/feature_request.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)      530 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1622 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/CONTRIBUTING.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1071 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/LICENSE
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4846 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/docs/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/docs/source/
--rwxrwxrwx   0 martin    (1000) martin    (1000)      906 2020-12-29 16:17:32.000000 foldedleastsquares-1.0.38/docs/source/Installation.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)    22976 2021-01-23 08:21:36.000000 foldedleastsquares-1.0.38/docs/source/Python interface.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)      863 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/conf.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    86868 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/animation.gif
--rwxrwxrwx   0 martin    (1000) martin    (1000)   136291 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/faq_2.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)   144986 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/faq_1.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4608 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/Changelog.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1413 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/Command.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)    41253 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/fig_histo_teff.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)   115484 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/logo.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)      412 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/index.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)     9943 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/FAQ.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)    68827 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/docs/source/frontpage_rescaled.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)      747 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/.travis.yml
--rwxrwxrwx   0 martin    (1000) martin    (1000)      132 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/.directory
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1619 2022-05-09 09:54:48.000000 foldedleastsquares-1.0.38/setup.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      101 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/.gitignore
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3332 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/CODE_OF_CONDUCT.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/setup.cfg
--rwxrwxrwx   0 martin    (1000) martin    (1000)      349 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/PULL_REQUEST_TEMPLATE.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)       33 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/MANIFEST.in
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares/template_generator/
--rwxrwxrwx   0 martin    (1000) martin    (1000)        0 2020-12-30 08:11:56.000000 foldedleastsquares-1.0.38/foldedleastsquares/template_generator/__init__.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     6202 2022-06-18 12:59:13.000000 foldedleastsquares-1.0.38/foldedleastsquares/template_generator/tailed_transit_template_generator.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    13158 2023-04-12 15:31:36.000000 foldedleastsquares-1.0.38/foldedleastsquares/template_generator/transit_template_generator.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    17706 2022-06-18 12:58:51.000000 foldedleastsquares-1.0.38/foldedleastsquares/template_generator/default_transit_template_generator.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1171 2021-04-18 15:50:51.000000 foldedleastsquares-1.0.38/foldedleastsquares/__init__.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     6891 2022-02-20 09:11:20.000000 foldedleastsquares-1.0.38/foldedleastsquares/core.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    12386 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/JAA546A14limb1-4.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     6392 2021-05-13 09:09:02.000000 foldedleastsquares-1.0.38/foldedleastsquares/catalog.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 15:32:52.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/
--rwxrwxrwx   0 martin    (1000) martin    (1000)    90800 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/EPIC201367065.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3224 2021-05-13 09:02:58.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_transit_depth_min.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      507 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_validation.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     2014 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_period_grid.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     2051 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_uncertainties.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      352 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/tls_config.cfg
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3450 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_catalog_data.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)       35 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/run_tests.sh
--rwxrwxrwx   0 martin    (1000) martin    (1000)    80075 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/EPIC206154641.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)      890 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_duration_grid.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1847 2023-03-31 07:39:45.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_multi_planet.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      326 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/run_tests.bat
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3051 2023-03-31 09:25:29.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_shapes.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4964 2023-03-31 09:41:53.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_stats_gap.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      362 2021-05-13 09:02:58.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_FAP.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      769 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_cleaned_array.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1372 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_resample.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     7433 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/test_synthetic.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    94432 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/tests/EPIC201367065_detrended.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1973 2021-01-23 18:43:31.000000 foldedleastsquares-1.0.38/foldedleastsquares/results.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     8204 2022-12-07 19:16:32.000000 foldedleastsquares-1.0.38/foldedleastsquares/main.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    15976 2022-06-18 12:58:43.000000 foldedleastsquares-1.0.38/foldedleastsquares/stats.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    23488 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/fap.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4206 2021-05-13 09:09:38.000000 foldedleastsquares-1.0.38/foldedleastsquares/command_line.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     8098 2021-05-13 09:08:34.000000 foldedleastsquares-1.0.38/foldedleastsquares/validate.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1052 2021-05-13 09:08:43.000000 foldedleastsquares-1.0.38/foldedleastsquares/grid.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4800 2021-08-19 15:36:24.000000 foldedleastsquares-1.0.38/foldedleastsquares/tls_constants.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3844 2021-05-13 09:09:22.000000 foldedleastsquares-1.0.38/foldedleastsquares/helpers.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    12620 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/ld_claret_tess.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)       53 2023-04-12 15:32:31.000000 foldedleastsquares-1.0.38/foldedleastsquares/version.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1611 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.38/foldedleastsquares/interpolation.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/tutorials/
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   205928 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/07 The influence of limb darkening values.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   272427 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/10 Measurement uncertainties.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   277149 2021-01-23 08:20:50.000000 foldedleastsquares-1.0.39/tutorials/12 A comet-like transit from Kepler KIC 12557548 with TLS.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   614539 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/11 A planet from TESS with TLS.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    56339 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/data_per_t14.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   333163 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/02 Starter's guide - K2-3b, a red dwarf with a planet.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   229894 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/04 Exploring the TLS spectra and statistics.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)  1116963 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/01 Quick start with synthetic data.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   553194 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/03 Multiple planets - K2-3, a red dwarf with 3 Super-Earths.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    42518 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/08 Edge effect jitter correction.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   199436 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/06 Comparison between TLS and BLS.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    99387 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/05 Custom transit shapes - Example of the grazing planet WASP-75.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   124754 2021-01-23 08:28:23.000000 foldedleastsquares-1.0.39/tutorials/13 Flares detection from TESS Proxima Centauri data.ipynb
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   568511 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/09 Optimal period grid and optimal duration grid.ipynb
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5220 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       79 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3263 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      107 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5220 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/PKG-INFO
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/.github/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      635 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/documentation.md
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      604 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      530 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1622 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/CONTRIBUTING.md
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1071 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/LICENSE
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     4846 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/docs/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/docs/source/
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      906 2020-12-29 16:17:32.000000 foldedleastsquares-1.0.39/docs/source/Installation.rst
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    22976 2021-01-23 08:21:36.000000 foldedleastsquares-1.0.39/docs/source/Python interface.rst
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      863 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/conf.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    86868 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/animation.gif
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   136291 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/faq_2.png
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   144986 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/faq_1.png
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     4608 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/Changelog.rst
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1413 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/Command.rst
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    41253 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/fig_histo_teff.png
+-rwxrwxrwx   0 martin    (1000) martin    (1000)   115484 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/logo.png
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      412 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/index.rst
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     9943 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/FAQ.rst
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    68827 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/frontpage_rescaled.png
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      747 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.travis.yml
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      132 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.directory
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1619 2022-05-09 09:54:48.000000 foldedleastsquares-1.0.39/setup.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      101 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.gitignore
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     3332 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/setup.cfg
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      349 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/PULL_REQUEST_TEMPLATE.md
+-rwxrwxrwx   0 martin    (1000) martin    (1000)       33 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/MANIFEST.in
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/
+-rwxrwxrwx   0 martin    (1000) martin    (1000)        0 2020-12-30 08:11:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/__init__.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     6202 2022-06-18 12:59:13.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/tailed_transit_template_generator.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    13229 2023-04-12 15:52:28.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/transit_template_generator.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    17706 2022-06-18 12:58:51.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/default_transit_template_generator.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1171 2021-04-18 15:50:51.000000 foldedleastsquares-1.0.39/foldedleastsquares/__init__.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     6891 2022-02-20 09:11:20.000000 foldedleastsquares-1.0.39/foldedleastsquares/core.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    12386 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/JAA546A14limb1-4.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     6392 2021-05-13 09:09:02.000000 foldedleastsquares-1.0.39/foldedleastsquares/catalog.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    90800 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC201367065.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     3224 2021-05-13 09:02:58.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_transit_depth_min.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      507 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_validation.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     2427 2023-04-12 16:01:05.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_period_grid.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     2051 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_uncertainties.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      352 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/tls_config.cfg
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     3450 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_catalog_data.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)       35 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/run_tests.sh
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    80075 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC206154641.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      890 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_duration_grid.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1847 2023-03-31 07:39:45.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_multi_planet.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      326 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/run_tests.bat
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     3051 2023-03-31 09:25:29.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_shapes.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     4964 2023-03-31 09:41:53.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_stats_gap.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      362 2021-05-13 09:02:58.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_FAP.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)      769 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_cleaned_array.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1372 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_resample.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     7433 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_synthetic.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    94432 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC201367065_detrended.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1973 2021-01-23 18:43:31.000000 foldedleastsquares-1.0.39/foldedleastsquares/results.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     8204 2022-12-07 19:16:32.000000 foldedleastsquares-1.0.39/foldedleastsquares/main.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    15976 2022-06-18 12:58:43.000000 foldedleastsquares-1.0.39/foldedleastsquares/stats.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    23488 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/fap.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     4206 2021-05-13 09:09:38.000000 foldedleastsquares-1.0.39/foldedleastsquares/command_line.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     8098 2021-05-13 09:08:34.000000 foldedleastsquares-1.0.39/foldedleastsquares/validate.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1052 2021-05-13 09:08:43.000000 foldedleastsquares-1.0.39/foldedleastsquares/grid.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     4800 2021-08-19 15:36:24.000000 foldedleastsquares-1.0.39/foldedleastsquares/tls_constants.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     3844 2021-05-13 09:09:22.000000 foldedleastsquares-1.0.39/foldedleastsquares/helpers.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)    12620 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/ld_claret_tess.csv
+-rwxrwxrwx   0 martin    (1000) martin    (1000)       53 2023-04-12 15:52:28.000000 foldedleastsquares-1.0.39/foldedleastsquares/version.py
+-rwxrwxrwx   0 martin    (1000) martin    (1000)     1611 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/interpolation.py
```

### Comparing `foldedleastsquares-1.0.38/tutorials/07 The influence of limb darkening values.ipynb` & `foldedleastsquares-1.0.39/tutorials/07 The influence of limb darkening values.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/10 Measurement uncertainties.ipynb` & `foldedleastsquares-1.0.39/tutorials/10 Measurement uncertainties.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/12 A comet-like transit from Kepler KIC 12557548 with TLS.ipynb` & `foldedleastsquares-1.0.39/tutorials/12 A comet-like transit from Kepler KIC 12557548 with TLS.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/11 A planet from TESS with TLS.ipynb` & `foldedleastsquares-1.0.39/tutorials/11 A planet from TESS with TLS.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/data_per_t14.csv` & `foldedleastsquares-1.0.39/tutorials/data_per_t14.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/02 Starter's guide - K2-3b, a red dwarf with a planet.ipynb` & `foldedleastsquares-1.0.39/tutorials/02 Starter's guide - K2-3b, a red dwarf with a planet.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/04 Exploring the TLS spectra and statistics.ipynb` & `foldedleastsquares-1.0.39/tutorials/04 Exploring the TLS spectra and statistics.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/01 Quick start with synthetic data.ipynb` & `foldedleastsquares-1.0.39/tutorials/01 Quick start with synthetic data.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/03 Multiple planets - K2-3, a red dwarf with 3 Super-Earths.ipynb` & `foldedleastsquares-1.0.39/tutorials/03 Multiple planets - K2-3, a red dwarf with 3 Super-Earths.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/08 Edge effect jitter correction.ipynb` & `foldedleastsquares-1.0.39/tutorials/08 Edge effect jitter correction.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/06 Comparison between TLS and BLS.ipynb` & `foldedleastsquares-1.0.39/tutorials/06 Comparison between TLS and BLS.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/05 Custom transit shapes - Example of the grazing planet WASP-75.ipynb` & `foldedleastsquares-1.0.39/tutorials/05 Custom transit shapes - Example of the grazing planet WASP-75.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/13 Flares detection from TESS Proxima Centauri data.ipynb` & `foldedleastsquares-1.0.39/tutorials/13 Flares detection from TESS Proxima Centauri data.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/tutorials/09 Optimal period grid and optimal duration grid.ipynb` & `foldedleastsquares-1.0.39/tutorials/09 Optimal period grid and optimal duration grid.ipynb`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares.egg-info/PKG-INFO` & `foldedleastsquares-1.0.39/foldedleastsquares.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.0.38
+Version: 1.0.39
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/hippke/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares.egg-info/SOURCES.txt` & `foldedleastsquares-1.0.39/foldedleastsquares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/PKG-INFO` & `foldedleastsquares-1.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.0.38
+Version: 1.0.39
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/hippke/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/documentation.md` & `foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/feature_request.md` & `foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/.github/ISSUE_TEMPLATE/bug_report.md` & `foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/CONTRIBUTING.md` & `foldedleastsquares-1.0.39/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/LICENSE` & `foldedleastsquares-1.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/README.md` & `foldedleastsquares-1.0.39/README.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/Installation.rst` & `foldedleastsquares-1.0.39/docs/source/Installation.rst`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/Python interface.rst` & `foldedleastsquares-1.0.39/docs/source/Python interface.rst`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/conf.py` & `foldedleastsquares-1.0.39/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/animation.gif` & `foldedleastsquares-1.0.39/docs/source/animation.gif`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/faq_2.png` & `foldedleastsquares-1.0.39/docs/source/faq_2.png`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/faq_1.png` & `foldedleastsquares-1.0.39/docs/source/faq_1.png`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/Changelog.rst` & `foldedleastsquares-1.0.39/docs/source/Changelog.rst`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/Command.rst` & `foldedleastsquares-1.0.39/docs/source/Command.rst`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/fig_histo_teff.png` & `foldedleastsquares-1.0.39/docs/source/fig_histo_teff.png`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/logo.png` & `foldedleastsquares-1.0.39/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/FAQ.rst` & `foldedleastsquares-1.0.39/docs/source/FAQ.rst`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/docs/source/frontpage_rescaled.png` & `foldedleastsquares-1.0.39/docs/source/frontpage_rescaled.png`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/.travis.yml` & `foldedleastsquares-1.0.39/.travis.yml`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/setup.py` & `foldedleastsquares-1.0.39/setup.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/CODE_OF_CONDUCT.md` & `foldedleastsquares-1.0.39/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/template_generator/tailed_transit_template_generator.py` & `foldedleastsquares-1.0.39/foldedleastsquares/template_generator/tailed_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/template_generator/transit_template_generator.py` & `foldedleastsquares-1.0.39/foldedleastsquares/template_generator/transit_template_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
         effective_time_span = effective_time_span * tls_constants.SECONDS_PER_DAY
         # boundary conditions
         f_min = n_transits_min / time_span
         f_max = 1.0 / (2 * pi) * sqrt(tls_constants.G * M_star / (3 * R_star) ** 3)
         P_min = 1 / f_max / tls_constants.SECONDS_PER_DAY
         if 0 < period_min < P_min:
             warnings.warn("You selected a `period_min` shorter than the Roche Limit period of " + str(numpy.round(P_min, 2)))
+            f_max = 1.0 / (period_min * tls_constants.SECONDS_PER_DAY)
         # optimal frequency sampling, Equations (5), (6), (7)
         A = (
                 (2 * pi) ** (2.0 / 3)
                 / pi
                 * R_star
                 / (tls_constants.G * M_star) ** (1.0 / 3)
                 / (effective_time_span * oversampling_factor)
```

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/template_generator/default_transit_template_generator.py` & `foldedleastsquares-1.0.39/foldedleastsquares/template_generator/default_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/__init__.py` & `foldedleastsquares-1.0.39/foldedleastsquares/__init__.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/core.py` & `foldedleastsquares-1.0.39/foldedleastsquares/core.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/JAA546A14limb1-4.csv` & `foldedleastsquares-1.0.39/foldedleastsquares/JAA546A14limb1-4.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/catalog.py` & `foldedleastsquares-1.0.39/foldedleastsquares/catalog.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/EPIC201367065.csv` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC201367065.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_transit_depth_min.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_transit_depth_min.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_period_grid.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_period_grid.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,8 +45,20 @@
         M_star=1,  # M_sun
         time_span=1000,  # days
         period_min=0,
         period_max=999,
         oversampling_factor=3,
     )
     numpy.testing.assert_equal(len(periods), 4308558)
+
+    periods = default_transit_template_generator.period_grid(
+        R_star=1,  # R_sun
+        M_star=1,  # M_sun
+        time_span=20,  # days
+        period_min=0.5,
+        period_max=999,
+        oversampling_factor=3,
+    )
+    numpy.testing.assert_almost_equal(max(periods), 10)
+    numpy.testing.assert_almost_equal(min(periods), 0.500, 3)
+    numpy.testing.assert_equal(len(periods), 1895)
     print("passed")
```

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_uncertainties.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_uncertainties.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_catalog_data.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_catalog_data.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/EPIC206154641.csv` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC206154641.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_duration_grid.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_duration_grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_multi_planet.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_multi_planet.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_shapes.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_stats_gap.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_stats_gap.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_cleaned_array.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_cleaned_array.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_resample.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/test_synthetic.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tests/EPIC201367065_detrended.csv` & `foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC201367065_detrended.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/results.py` & `foldedleastsquares-1.0.39/foldedleastsquares/results.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/main.py` & `foldedleastsquares-1.0.39/foldedleastsquares/main.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/stats.py` & `foldedleastsquares-1.0.39/foldedleastsquares/stats.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/fap.csv` & `foldedleastsquares-1.0.39/foldedleastsquares/fap.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/command_line.py` & `foldedleastsquares-1.0.39/foldedleastsquares/command_line.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/validate.py` & `foldedleastsquares-1.0.39/foldedleastsquares/validate.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/grid.py` & `foldedleastsquares-1.0.39/foldedleastsquares/grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/tls_constants.py` & `foldedleastsquares-1.0.39/foldedleastsquares/tls_constants.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/helpers.py` & `foldedleastsquares-1.0.39/foldedleastsquares/helpers.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/ld_claret_tess.csv` & `foldedleastsquares-1.0.39/foldedleastsquares/ld_claret_tess.csv`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.38/foldedleastsquares/interpolation.py` & `foldedleastsquares-1.0.39/foldedleastsquares/interpolation.py`

 * *Files identical despite different names*

