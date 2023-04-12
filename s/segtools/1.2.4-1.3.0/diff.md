# Comparing `tmp/segtools-1.2.4.tar.gz` & `tmp/segtools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/segtools-1.2.4.tar", last modified: Tue Oct  1 20:35:01 2019, max compression
+gzip compressed data, was "/home/runner/work/segtools/segtools/dist/.tmp-uetw3rav/segtools-1.3.0.tar", last modified: Wed Apr 12 15:39:26 2023, max compression
```

## Comparing `segtools-1.2.4.tar` & `segtools-1.3.0.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      806 2018-05-25 19:01:49.000000 segtools-1.2.4/README.rst
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    10285 2018-05-25 19:01:49.000000 segtools-1.2.4/ez_setup.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     7359 2019-10-01 20:34:17.000000 segtools-1.2.4/NEWS
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1263 2019-10-01 20:35:01.000000 segtools-1.2.4/PKG-INFO
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/R/
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/R/segtools/
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/R/segtools/man/
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1043 2018-05-25 19:01:49.000000 segtools-1.2.4/R/segtools/man/segtools-package.Rd
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)       31 2018-05-25 19:01:49.000000 segtools-1.2.4/R/segtools/NAMESPACE
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      420 2018-05-25 19:01:49.000000 segtools-1.2.4/R/segtools/Read-and-delete-me
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      281 2018-05-25 19:01:49.000000 segtools-1.2.4/R/segtools/DESCRIPTION
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      402 2018-05-25 19:01:49.000000 segtools-1.2.4/R/README
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)      280 2018-05-25 19:01:49.000000 segtools-1.2.4/R/build.sh
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      575 2018-05-25 19:01:49.000000 segtools-1.2.4/INSTALL
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      378 2019-10-01 20:34:17.000000 segtools-1.2.4/.hgtags
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools/
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    36740 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/aggregation.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    16486 2019-10-01 19:02:34.000000 segtools-1.2.4/segtools/html.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     1561 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/bed.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     2963 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/gff.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    18180 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/common.py
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools/resources/
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1304 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/signal_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      373 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/mnemonic_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1212 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/transition_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1094 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/aggregation_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1219 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/html_header.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     2686 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/gmtk_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)        0 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/__init__.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      244 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/html_footer.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      685 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/distance_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1481 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/length_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1756 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/aggregation_gene_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      873 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/nucleotide_div.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1658 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/resources/overlap_div.tmpl
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     8472 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/gmtk_parameters.py
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools/R/
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     3970 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/dinucleotide.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    14449 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/overlap.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     2911 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/distance.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    24934 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/track_statistics.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    13412 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/common.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)        0 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/__init__.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     9322 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/signal.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    18708 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/aggregation.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     6536 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/length.R
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     3924 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/R/transition.R
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    19447 2019-06-19 19:03:21.000000 segtools-1.2.4/segtools/overlap.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    24212 2019-10-01 20:03:52.000000 segtools-1.2.4/segtools/__init__.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    10283 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/nucleotide_frequency.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    12226 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/flatten.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     9059 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/length_distribution.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)       22 2019-10-01 20:34:17.000000 segtools-1.2.4/segtools/version.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     1584 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/mnemonics.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    15684 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/signal_distribution.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    13290 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/feature_distance.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     4228 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/relabel.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     5791 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/compare.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     2116 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/preprocess.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    13106 2018-05-25 19:01:49.000000 segtools-1.2.4/segtools/transition.py
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/doc/
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    35030 2019-07-15 15:59:33.000000 segtools-1.2.4/doc/segtools.rst
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     7231 2018-05-25 19:01:49.000000 segtools-1.2.4/doc/conf.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    74511 2018-05-25 19:01:49.000000 segtools-1.2.4/doc/flowchart.png
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     1430 2018-05-25 19:01:49.000000 segtools-1.2.4/doc/gethelp.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     4110 2018-05-25 19:01:49.000000 segtools-1.2.4/doc/make.bat
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     5273 2018-05-25 19:01:49.000000 segtools-1.2.4/doc/Makefile
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      440 2018-05-25 19:01:49.000000 segtools-1.2.4/doc/index.rst
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    44230 2018-05-25 19:01:49.000000 segtools-1.2.4/install.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     3927 2019-06-19 19:03:21.000000 segtools-1.2.4/setup.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     7068 2018-05-25 19:01:49.000000 segtools-1.2.4/install.tmpl
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)       35 2018-05-25 19:01:49.000000 segtools-1.2.4/.hgignore
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    17987 2018-05-25 19:01:49.000000 segtools-1.2.4/COPYING
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)      117 2019-10-01 20:35:01.000000 segtools-1.2.4/setup.cfg
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)    18092 2018-05-25 19:01:49.000000 segtools-1.2.4/LICENSE
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/test/
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)      894 2018-05-25 19:01:49.000000 segtools-1.2.4/test/run_all.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)    11235 2018-05-25 19:01:49.000000 segtools-1.2.4/test/test_overlap.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     4927 2018-05-25 19:01:49.000000 segtools-1.2.4/test/test_feature_distance.py
--rwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)     2842 2018-05-25 19:01:49.000000 segtools-1.2.4/test/test_bed_compare.py
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      472 2018-05-25 19:01:49.000000 segtools-1.2.4/TODO
-drwxr-xr-x   0 eroberts (18659) mhoffma1  (9365)        0 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)        1 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/dependency_links.txt
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1263 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/PKG-INFO
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)        1 2018-05-25 19:38:50.000000 segtools-1.2.4/segtools.egg-info/not-zip-safe
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)        9 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/top_level.txt
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)      337 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/entry_points.txt
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)     1823 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/SOURCES.txt
--rw-r--r--   0 eroberts (18659) mhoffma1  (9365)       62 2019-10-01 20:35:01.000000 segtools-1.2.4/segtools.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 15:39:08.000000 segtools-1.3.0/.github/workflows/continuous-integration-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 15:39:08.000000 segtools-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 15:39:08.000000 segtools-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-12 15:39:08.000000 segtools-1.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-12 15:39:08.000000 segtools-1.3.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-04-12 15:39:08.000000 segtools-1.3.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-12 15:39:08.000000 segtools-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-12 15:39:08.000000 segtools-1.3.0/NEWS
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-12 15:39:26.000000 segtools-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/R/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-12 15:39:08.000000 segtools-1.3.0/R/README
+-rwxr-xr-x   0 runner    (1001) docker     (123)      280 2023-04-12 15:39:08.000000 segtools-1.3.0/R/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/R/segtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-12 15:39:08.000000 segtools-1.3.0/R/segtools/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 15:39:08.000000 segtools-1.3.0/R/segtools/NAMESPACE
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 15:39:08.000000 segtools-1.3.0/R/segtools/Read-and-delete-me
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/R/segtools/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 15:39:08.000000 segtools-1.3.0/R/segtools/man/segtools-package.Rd
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-12 15:39:08.000000 segtools-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-12 15:39:08.000000 segtools-1.3.0/TODO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74511 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/flowchart.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1192 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/gethelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    33050 2023-04-12 15:39:08.000000 segtools-1.3.0/doc/segtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 15:39:08.000000 segtools-1.3.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-12 15:39:08.000000 segtools-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools/R/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/aggregation.R
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/common.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/dinucleotide.R
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/distance.R
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/length.R
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/overlap.R
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/signal.R
+-rw-r--r--   0 runner    (1001) docker     (123)    24934 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/track_statistics.R
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/R/transition.R
+-rw-r--r--   0 runner    (1001) docker     (123)    24713 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36740 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/aggregation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1561 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18317 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5789 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13290 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/feature_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12249 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/flatten.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2963 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/gff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8454 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/gmtk_parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16513 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/html.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9041 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/length_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1584 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/mnemonics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10433 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/nucleotide_frequency.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19447 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/overlap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2116 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/preprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4209 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/relabel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/aggregation_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/aggregation_gene_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/distance_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/gmtk_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/html_footer.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/html_header.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/length_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/mnemonic_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/nucleotide_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/overlap_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/signal_div.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/resources/transition_div.tmpl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15670 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/signal_distribution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13021 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 15:39:08.000000 segtools-1.3.0/segtools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 15:39:26.000000 segtools-1.3.0/segtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 15:39:26.000000 segtools-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:39:26.000000 segtools-1.3.0/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      859 2023-04-12 15:39:08.000000 segtools-1.3.0/test/run_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2983 2023-04-12 15:39:08.000000 segtools-1.3.0/test/test_bed_compare.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4716 2023-04-12 15:39:08.000000 segtools-1.3.0/test/test_feature_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11713 2023-04-12 15:39:08.000000 segtools-1.3.0/test/test_overlap.py
```

### Comparing `segtools-1.2.4/NEWS` & `segtools-1.3.0/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-1.2.4:
-* fix rpy2 version 3 errors on Python 2
-* fix html output for Python 3
+1.3.0:
+* dropped official python 2 support
+* all tools are now supported on python 3
+* updated build system and removed legacy installation scripts
+* added support for wheel distributions
+* latest docs now available on segtools.readthedocs.org
+* updated existing test cases
+* added runtime checks for genomedata in segtools-nucleotide-frequency and segtools-signal-distribution
+* added CITATION.cff for aiding in citation
 
 1.2.3:
 * add support for rpy2 version 3
 
 1.2.2:
 * segtools-overlap: added compatibility with python 3
```

### Comparing `segtools-1.2.4/R/segtools/man/segtools-package.Rd` & `segtools-1.3.0/R/segtools/man/segtools-package.Rd`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/aggregation.py` & `segtools-1.3.0/segtools/aggregation.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/html.py` & `segtools-1.3.0/segtools/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pkg_resources import resource_string
 from shutil import copy
 from string import Template
 
 from . import log, Segmentation, die, add_common_options
 from .common import check_clobber, get_ordered_labels, make_divfilename, \
      make_id, make_filename, make_tabfilename, map_mnemonics, NICE_EXTS, \
-     PKG_RESOURCE, PY3_COMPAT_ERROR
+     PKG_RESOURCE
 from .version import __version__
 
 MNEMONIC_TEMPLATE_FILENAME = "mnemonic_div.tmpl"
 HEADER_TEMPLATE_FILENAME = "html_header.tmpl"
 FOOTER_TEMPLATE_FILENAME = "html_footer.tmpl"
 GENOMEBROWSER_URL = "http://genome.ucsc.edu/cgi-bin/hgTracks?org=human&hgt.customText=track"
 GENOMEBROWSER_OPTIONS = {"autoScale":"off",
@@ -40,24 +40,23 @@
 <li>Link to view this segmentation in the UCSC genome browser:<br />
 <script type="text/javascript">print_genomebrowser_link("%s");</script>
 </li>"""
 
 DESCRIPTION_MODULE = ("description", "Segmentation information")
 MNEMONIC_MODULE = ("mnemonics", "Mnemonics")
 
-HTML_TEMPLATE_ENCODING = "ascii"
+# resource_string returns bytes
+# Ref: https://importlib-resources.readthedocs.io/en/latest/migration.html#pkg-resources-resource-string
+template_bytes = partial(resource_string, PKG_RESOURCE)
 
 def template_substitute(filename):
     """
     Simplify import resource strings in the package
     """
-    template_string = resource_string(PKG_RESOURCE,
-                                      filename).decode(HTML_TEMPLATE_ENCODING)
-
-    return Template(template_string).safe_substitute
+    return Template(template_bytes(filename).decode()).safe_substitute
 
 def tuple2link(entry):
     """entry should be a (url, text) tuple"""
     return '<a href="%s">%s</a>' % entry
 
 def list2html(list, code=False, link=False):
     """
@@ -223,15 +222,14 @@
 
 def save_html_div(template_filename, dirpath, namebase,
                   clobber=False, verbose=True, **kwargs):
     """Save an HTML div file for a module run by subsituting a template file"""
     fields = form_template_dict(dirpath, namebase, **kwargs)
     div_filename = make_divfilename(dirpath, namebase)
     log("Saving html data to file: %s" % div_filename, verbose)
-
     try:
         html = template_substitute(template_filename)(fields)
     except KeyError as e:
         log("Error: Missing data: %s. Skipping HTML output." % e)
         return
 
     write_html_div(dirpath, namebase, html, clobber=clobber)
```

### Comparing `segtools-1.2.4/segtools/bed.py` & `segtools-1.3.0/segtools/bed.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/gff.py` & `segtools-1.3.0/segtools/gff.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/common.py` & `segtools-1.3.0/segtools/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,27 +33,29 @@
 EXT_DOT = "dot"
 EXT_HTML = "html"
 EXT_DIV = "div"
 EXT_SLIDE = os.extsep.join(["slide", EXT_PNG])
 EXT_THUMB = os.extsep.join(["thumb", EXT_PNG])  # for thumbnails
 EXT_SUMMARY = os.extsep.join(["summary", EXT_TAB])
 
+GENOMEDATA_INSTALL_ERROR_MSG = "Genomedata is required for this tool. " \
+                               "Please install the 'genomedata' package " \
+                               "for this python environment"
+
 IMG_EXTS = [EXT_PNG, EXT_PDF, EXT_SLIDE, EXT_THUMB]
 NICE_EXTS = dict(tab=EXT_TAB, pdf=EXT_PDF, png=EXT_PNG, html=EXT_HTML,
                  div=EXT_DIV, slide=EXT_SLIDE, thumb=EXT_THUMB,
                  summary=EXT_SUMMARY, dot=EXT_DOT)
 
 SUFFIX_GZ = os.extsep + EXT_GZ
 
 LABEL_ALL = "all"
 
 THUMB_SIZE = 100
 
-PY3_COMPAT_ERROR = "{} is not yet compatible with this version of Python"
-
 class OutputMasker(object):
     """Class to mask the output of a stream.
 
     Suggested usage:
       sys.stout = OutputMasker(sys.stdout)  # Start masking
       <commands with stout masked>  # Masked commands
       sys.stdout = sys.stdout.restore()  # Stop masking
```

### Comparing `segtools-1.2.4/segtools/resources/signal_div.tmpl` & `segtools-1.3.0/segtools/resources/signal_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/transition_div.tmpl` & `segtools-1.3.0/segtools/resources/transition_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/aggregation_div.tmpl` & `segtools-1.3.0/segtools/resources/aggregation_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/html_header.tmpl` & `segtools-1.3.0/segtools/resources/html_header.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/gmtk_div.tmpl` & `segtools-1.3.0/segtools/resources/gmtk_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/distance_div.tmpl` & `segtools-1.3.0/segtools/resources/distance_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/length_div.tmpl` & `segtools-1.3.0/segtools/resources/length_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/aggregation_gene_div.tmpl` & `segtools-1.3.0/segtools/resources/aggregation_gene_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/nucleotide_div.tmpl` & `segtools-1.3.0/segtools/resources/nucleotide_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/resources/overlap_div.tmpl` & `segtools-1.3.0/segtools/resources/overlap_div.tmpl`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/gmtk_parameters.py` & `segtools-1.3.0/segtools/gmtk_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 import sys
 
 from numpy import array
 
 from . import log, die, RInterface, add_common_options, open_transcript
-from .common import setup_directory, PY3_COMPAT_ERROR
+from .common import setup_directory
 from .html import save_html_div
 from .transition import save_plot, save_graph
 from .mnemonics import create_mnemonic_file
 from .signal_distribution import SignalStats
 from .version import __version__
 
 NAMEBASE = "%s" % MODULE
```

### Comparing `segtools-1.2.4/segtools/R/dinucleotide.R` & `segtools-1.3.0/segtools/R/dinucleotide.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/overlap.R` & `segtools-1.3.0/segtools/R/overlap.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/distance.R` & `segtools-1.3.0/segtools/R/distance.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/track_statistics.R` & `segtools-1.3.0/segtools/R/track_statistics.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/common.R` & `segtools-1.3.0/segtools/R/common.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/signal.R` & `segtools-1.3.0/segtools/R/signal.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/aggregation.R` & `segtools-1.3.0/segtools/R/aggregation.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/length.R` & `segtools-1.3.0/segtools/R/length.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/R/transition.R` & `segtools-1.3.0/segtools/R/transition.R`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/overlap.py` & `segtools-1.3.0/segtools/overlap.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/__init__.py` & `segtools-1.3.0/segtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from functools import partial
 from logging import basicConfig, critical, INFO, info
 from numpy import array, int64, uint32
 from time import time
 
 from pkg_resources import resource_filename
 
+import rpy2.robjects.packages as r_packages
+from rpy2.robjects.vectors import StrVector
+
 from .bed import read_native as read_bed
 from .gff import read_native as read_gff
 
 from .version import __version__
 
 try:
     PKG = __package__  # Python 2.6
@@ -47,14 +50,17 @@
 
 _READERS=dict(bed=read_bed, narrowpeak=read_bed,
               gff=read_gff, gtf=partial(read_gff, gtf=True))
 
 GFF_FORMATS = frozenset(["gff", "gtf"])
 BED_FORMATS = frozenset(["bed", "narrowpeak"])
 
+# List of R package pre-requisites
+R_PACKAGES = ["latticeExtra", "reshape"]
+
 # Determine rpy2 version and get correct imports
 # Get the correct write console callback function between Rpy2 versions
 try:
     from rpy2.rinterface import set_writeconsole_regular
     RPY2_MAJOR_VERSION = 2
 except ImportError:
     from rpy2.rinterface_lib.callbacks import consolewrite_print
@@ -74,14 +80,22 @@
         set_writeconsole_regular(callback)
 
 
 def get_r_dirname():
     return resource_filename(PKG_R, "")
 
 
+def install_r_dependencies() -> None:
+    # Ref: https://rpy2.github.io/doc/latest/html/robjects_rpackages.html#installing-removing-r-packages
+
+    utils = r_packages.importr('utils')
+    utils.chooseCRANmirror(ind=1) # Select first mirror
+    utils.install_packages(StrVector(R_PACKAGES))
+
+
 class Annotation(object):
     """Base class for representing annotation files (BED/GFF/GTF files)
 
     chromosomes: a dict
       key: chromosome name
       val: segments, a numpy.ndarray,
            (each row is a (start, end, key, [strand, ...]) struct)
@@ -557,14 +571,15 @@
         try:
             result = self.call(func, *args, **kwargs)
         except self.RError:
             die("Encoundered error within R:\n%s" % "\n  ".join(r_log))
 
         # Return console back to stderr
         set_r_writeconsole(self._r_console)
+        self._rinterface._post_initr_setup
 
         log("Plotting completed in %.1f seconds" % (time() - start),
             self.verbose)
         return result
 
 
 class ProgressBar(object):
```

### Comparing `segtools-1.2.4/segtools/nucleotide_frequency.py` & `segtools-1.3.0/segtools/nucleotide_frequency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 #!/usr/bin/env python
-from __future__ import division, with_statement
+
 
 """
 Provides command-line and package entry points for analyzing nucleotide
 and dinucleotide frequencies for each label in the segmentation or annotation
 file.
 
 """
 
 import numpy
 import os
 import sys
 import warnings
 
 from collections import defaultdict
-from genomedata import Genome
+
+# Detect runtime genomedata dependency
+try:
+    from genomedata import Genome
+except ModuleNotFoundError:
+    from .common import GENOMEDATA_INSTALL_ERROR_MSG
+    raise ModuleNotFoundError(GENOMEDATA_INSTALL_ERROR_MSG) from None
+
 from numpy import zeros, bincount, array
 
 from . import log, Annotation, die, RInterface, open_transcript, \
      add_common_options, ProgressBar
 from .common import make_tabfilename, setup_directory, tab_saver
 
 from .html import save_html_div
@@ -96,15 +103,15 @@
 
     # Store counts of each (di)nucleotide observed
     # separated by label
     nuc_counts = defaultdict(dict)
     dinuc_counts = defaultdict(dict)
 
     labels = annotation.labels
-    for label_key in labels.iterkeys():
+    for label_key in labels.keys():
         nuc_counts[label_key] = zeros(len(nuc_categories)+1, dtype=numpy.long)
         dinuc_counts[label_key] = zeros(len(dinuc_categories)+1,
                                         dtype=numpy.long)
 
     # Count (di)nucleotides over annotation
     for chromosome in genome:
         chrom = chromosome.name
```

### Comparing `segtools-1.2.4/segtools/flatten.py` & `segtools-1.3.0/segtools/flatten.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 that describes the generated labels (use -m to change).
 """
 
 # Author: Orion Buske <stasis@uw.edu>
 # Date:   02.02.2010
 
 
-from __future__ import division, with_statement
+
 
 import os
 import sys
 
 from numpy import concatenate
 
 from . import log, Segmentation, die, add_common_options
@@ -186,21 +186,21 @@
     files = sorted(segmentations.keys())  # Constant file order
 
     chroms = set()
     label_offsets = {}  # file -> label_offset
     shifted_labels = {}  # shifted_key -> label_string
     for file in files:
         segmentation = segmentations[file]
-        chroms.update(segmentation.chromosomes.keys())
+        chroms.update(list(segmentation.chromosomes.keys()))
         labels = segmentation.labels
 
         # Shift labels of file to be unique
         label_offset = len(shifted_labels)
         label_offsets[file] = label_offset
-        for key, label in labels.iteritems():
+        for key, label in iter(list(labels.items())):
             shifted_labels[key + label_offset] = "%s:%s" % (file, label)
 
     signature_labels = {}  # (shifted_key, ...) -> flat_key
     flat_labels = {}  # flat_key -> label_string
     new_segments = []
     for chrom in chroms:
         segments = join_chrom_segments(chrom, files, segmentations,
@@ -228,39 +228,39 @@
     if filter is None or filter == 0:
         return labels, segments
 
     if (not isinstance(filter, float) or filter < 0 or filter > 1):
         raise ValueError("Invalid value of filter: %s" % str(filter))
 
     # Find span of labels and whole segmentation
-    print >>sys.stderr, "Calculating span of labels and segmentation...",
+    print("Calculating span of labels and segmentation...", end=' ', file=sys.stderr)
     n_seg = 0
-    n_keys = dict([(key, 0) for key in labels.iterkeys()])
+    n_keys = dict([(key, 0) for key in iter(list(labels.keys()))])
     for segment in segments:
         key = segment[3]
         length = segment[2] - segment[1]
         n_keys[key] += length
         n_seg += length
-    print >>sys.stderr, "done"
+    print("done", file=sys.stderr)
 
     # Find segment labels that need to be filtered
     filtered_labels = dict(labels)  # Copy of original labels
     thresh = n_seg * filter
-    for key, n_key in n_keys.iteritems():
+    for key, n_key in iter(list(n_keys.items())):
         if n_key < thresh:
             del filtered_labels[key]
 
     # Remove segments not in filtered segment labels
-    print >>sys.stderr, "Filtering segment labels below threshold...",
+    print("Filtering segment labels below threshold...", end=' ', file=sys.stderr)
     filtered_segments = []
     for segment in segments:
         key = segment[3]
         if key in filtered_labels:
             filtered_segments.append(segment)
-    print >>sys.stderr, "done"
+    print("done", file=sys.stderr)
 
     return filtered_labels, filtered_segments
 
 def print_bed(segments, filename=None):
     """Print segments in BED format to file (or stdout if None)"""
     if filename is None:
         outfile = sys.stdout
@@ -278,15 +278,15 @@
 
 def print_readme(labels, filename=DEFAULT_HELPFILE):
     if os.path.isfile(filename):
         log("Warning: overwriting file: %s" % filename)
 
     with open(filename, "w") as ofp:
         ofp.write("%s\n" % "\t".join(["old", "new", "description"]))
-        for key, label in labels.iteritems():
+        for key, label in iter(list(labels.items())):
             ofp.write("%s\n" % "\t".join([str(key), str(key), label]))
 
 def flatten(files, outfile=None, helpfile=DEFAULT_HELPFILE,
             filter=None, verbose=True):
     segmentations = {}
     for file in files:
         assert os.path.isfile(file)
```

### Comparing `segtools-1.2.4/segtools/length_distribution.py` & `segtools-1.3.0/segtools/length_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from collections import defaultdict
 from numpy import concatenate, median
 
 from . import Annotation, die, RInterface, open_transcript, \
      add_common_options, log
 from .common import get_ordered_labels, LABEL_ALL, make_tabfilename, \
-     setup_directory, tab_saver, PY3_COMPAT_ERROR
+     setup_directory, tab_saver
 
 from .html import save_html_div
 from .version import __version__
 
 FIELDNAMES_SUMMARY = ["label", "num.segs", "mean.len", "median.len",
                      "stdev.len", "num.bp", "frac.bp"]
 FIELDNAMES = ["label", "length"]
```

### Comparing `segtools-1.2.4/segtools/mnemonics.py` & `segtools-1.3.0/segtools/mnemonics.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/signal_distribution.py` & `segtools-1.3.0/segtools/signal_distribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,24 +20,26 @@
 
 from functools import partial
 from numpy import arcsinh, isfinite, isnan, longdouble, sqrt, square, zeros
 
 from . import log, Segmentation, die, RInterface, add_common_options, \
      open_transcript, ProgressBar
 from .common import iter_segments_continuous,  \
-     make_tabfilename, setup_directory, tab_reader, tab_saver, PY3_COMPAT_ERROR
+     make_tabfilename, setup_directory, tab_reader, tab_saver
 from .html import save_html_div
 from .mnemonics import create_mnemonic_file
 from .version import __version__
 
-# XXX: Port Genomedata to Python 3
+# Detect runtime genomedata dependency
 try:
     from genomedata import Genome
-except ImportError:
-    log(PY3_COMPAT_ERROR.format("Genomedata"))
+except ModuleNotFoundError:
+    from .common import GENOMEDATA_INSTALL_ERROR_MSG
+    raise ModuleNotFoundError(GENOMEDATA_INSTALL_ERROR_MSG) from None
+
 
 FIELDNAMES = ["label", "trackname", "mean", "sd", "n"]
 NAMEBASE = str(MODULE)
 
 HTML_TITLE = "Signal value statistics"
 HTML_TEMPLATE_FILENAME = "signal_div.tmpl"
 
@@ -370,17 +372,14 @@
                 parser.error("Output directory cannot be an input directory")
 
     return (options, args)
 
 ## Command-line entry point
 def main(args=sys.argv[1:]):
 
-    if sys.version_info[0] == 3:
-        die(PY3_COMPAT_ERROR.format("Genomedata"))
-
     from genomedata import Genome
 
     (options, args) = parse_options(args)
     bedfilename = args[0]
     genomedatadir = args[1]
 
     kwargs = dict(options.__dict__)
```

### Comparing `segtools-1.2.4/segtools/feature_distance.py` & `segtools-1.3.0/segtools/feature_distance.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/relabel.py` & `segtools-1.3.0/segtools/relabel.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 merging overlapping segments with the same final label.
 Outputs the new segmentation in bed format to stdout (-o to change).
 """
 
 # Author: Orion Buske <stasis@uw.edu>
 # Date:   05.16.2011
 
-from __future__ import division, with_statement
+
 
 import os
 import sys
 
 from . import log, Segmentation, die, add_common_options
 from .common import map_mnemonics, get_ordered_labels
 from .version import __version__
@@ -27,16 +27,16 @@
 
 SCORE_DEFAULT = 0
 STRAND_UNKNOWN = StrandUnknown()
 
 def get_strand(segment):
     try:
         return segment['strand']
-    # IndexError, not KeyError, because segment is a NumPy struct
-    except IndexError:
+    # IndexError or ValueError, not KeyError, because segment is a NumPy struct
+    except (IndexError, ValueError):
         return STRAND_UNKNOWN
 
 def relabel(segfilename, mnemonicfilename, outfile=None, verbose=True):
     assert os.path.isfile(segfilename)
     segmentation = Segmentation(segfilename, verbose=verbose)
 
     labels = segmentation.labels
@@ -56,28 +56,28 @@
 
     if outfile is None:
         out = sys.stdout
     else:
         out = open(outfile, "w")
 
     try:
-        for chrom, segments in segmentation.chromosomes.iteritems():
+        for chrom, segments in segmentation.chromosomes.items():
             def print_segment(segment, label):
                 start = segment['start']
                 end = segment['end']
                 old = segment['key']
                 tokens = [chrom, start, end, mnemonics[old]]
 
                 strand = get_strand(segment)
                 if strand != STRAND_UNKNOWN or colors:
                     tokens.extend([SCORE_DEFAULT, str(strand)])
 
                 if colors:
                     tokens.extend([start, end, colors[old]])
-                print >>out, "\t".join(map(str, tokens))
+                print("\t".join(map(str, tokens)), file=out)
 
             prev_segment = segments[0]
             prev_label = mnemonics[prev_segment['key']]
             for segment in segments[1:]:
                 # Merge adjacent segments of same label
                 label = mnemonics[segment['key']]
                 if (label == prev_label and
```

### Comparing `segtools-1.2.4/segtools/compare.py` & `segtools-1.3.0/segtools/compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 def edit_distance(bedfile1, bedfile2, quick=False, verbose=True):
     """Given two segmentations, returns the edit distance (bp) between them"""
     segmentations = [Segmentation(bedfile, verbose=verbose)
                      for bedfile in [bedfile1, bedfile2]]
 
     for segmentation in segmentations:
-        for segments in segmentation.chromosomes.itervalues():
+        for segments in iter(segmentation.chromosomes.values()):
             if not (segments['start'][1:] >= segments['end'][:-1]).all():
                 raise SyntaxError("Overlapping segments found in: %s" % \
                                       segmentation.name)
 
     chroms = set()
     for segmentation in segmentations:
         chroms.update(segmentation.chromosomes.keys())
@@ -62,17 +62,17 @@
                 bases_missing1 += bases_in_segments(segs2)
             elif segs2 is None:
                 bases_missing2 += bases_in_segments(segs1)
             continue
 
         # Segments in both segmentations
         segs1_iter = iter(segs1)
-        start1, end1, key1 = segs1_iter.next()
+        start1, end1, key1 = next(segs1_iter)
         segs2_iter = iter(segs2)
-        start2, end2, key2 = segs2_iter.next()
+        start2, end2, key2 = next(segs2_iter)
         while True:
             advance1 = False
             advance2 = False
             if start1 < start2:  # move up segment 1
                 stop = min(start2, end1)
                 bases_missing2 += stop - start1
                 start1 = stop
@@ -107,24 +107,24 @@
                 # Advance both
                 start1 = stop
                 start2 = stop
 
             # Carry out any pending advances
             if advance1:
                 try:
-                    start1, end1, key1 = segs1_iter.next()
+                    start1, end1, key1 = next(segs1_iter)
                 except StopIteration:
                     bases_missing1 += end2 - start2
                     for start2, end2, key2 in segs2_iter:
                         bases_missing1 += end2 - start2
                     break
 
             if advance2:
                 try:
-                    start2, end2, key2 = segs2_iter.next()
+                    start2, end2, key2 = next(segs2_iter)
                 except StopIteration:
                     bases_missing2 += end1 - start1
                     for start1, end1, key1 in segs1_iter:
                         bases_missing2 += end1 - start1
                     break
 
         if quick: break
```

### Comparing `segtools-1.2.4/segtools/preprocess.py` & `segtools-1.3.0/segtools/preprocess.py`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/segtools/transition.py` & `segtools-1.3.0/segtools/transition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
-from __future__ import absolute_import
-from __future__ import division, with_statement
+
+
 import six
 from six.moves import zip
 
 """
 Provides command-line and package entry points for analyzing the observed
 segmentation label transitions in the given BED-formatted segmentation.
```

### Comparing `segtools-1.2.4/doc/segtools.rst` & `segtools-1.3.0/doc/segtools.rst`

 * *Files 6% similar despite different names*

```diff
@@ -36,31 +36,29 @@
 
     conda install segtools
 
 .. _Bioconda: https://bioconda.github.io/
 
 Otherwise, Segtools requires the following prerequisites:
 
-- Python 2.7 *or* Python 3.6+, with Rpy2 2.1.3+
+- Python 3.7+, with Rpy2 2.1.3+
 - Zlib
 - Numpy 1.3+
 - R 2.10.0+, with latticeExtra and reshape packages
 
 
 Once these prerequisites are properly installed, Segtools can be
 installed with::
 
   pip install segtools
 
 To use :ref:`segtools-signal-distribution <segtools-signal-distribution>`
 or :ref:`segtools-nucleotide-frequency <segtools-nucleotide-frequency>`,
 the Python package, Genomedata, is also required.
 
-To know what tools are compatible for Python 2 and 3 see the
-:ref:`Python compatibility table<python-compatibility-by-tool>`.
 
 Segmentations versus annotations
 ================================
 A segmentation is a division of a genome (or part of a genome) into
 non-overlapping segments, each of which is assigned one of a fixed set
 of labels.  Ideally, segments that share a common label are somehow
 similar to one another, and vice versa.  Segtools helps you identify
@@ -114,54 +112,14 @@
    :alt: Flowchart of basic Segtools command workflow
 
 Segtools commands can be run through their
 :ref:`command-line <command-line-interface>`
 or :ref:`Python <python-interface>`
 interfaces.
 
-
-.. _`python-compatibility-by-tool`:
-
-Python 2/3 compatibility status
--------------------------------
-
-Segtools is available for both Python 2 and Python 3.
-This table shows the compatibility of each tool for both Python versions:
-
-+-------------------------+------------+------------+
-|           Tool          |  Python 2  |  Python 3  |
-+=========================+============+============+
-|       aggregation       |     ✓      |     ✓      |
-+-------------------------+------------+------------+
-|         compare         |     ✓      |            |
-+-------------------------+------------+------------+
-|    feature-distance     |     ✓      |     ✓      |
-+-------------------------+------------+------------+
-|         flatten         |     ✓      |            |
-+-------------------------+------------+------------+
-|      html-report        |     ✓      |            |
-+-------------------------+------------+------------+
-|   length-distribution   |     ✓      |     ✓      |
-+-------------------------+------------+------------+
-|   nucleotide-frequency  |     ✓      |            |
-+-------------------------+------------+------------+
-|         overlap         |     ✓      |     ✓      |
-+-------------------------+------------+------------+
-|       preprocess        |     ✓      |     ✓      |
-+-------------------------+------------+------------+
-|         relabel         |     ✓      |            |
-+-------------------------+------------+------------+
-|   signal-distribution   |     ✓      |            |
-+-------------------------+------------+------------+
-|       transition        |     ✓      |            |
-+-------------------------+------------+------------+
-|     gmtk-parameters     |     ✓      |     ✓      |
-+-------------------------+------------+------------+
-
-
 .. _`command-line-interface`:
 
 Command-line interface
 ----------------------
 
 Commands that analyze a single segmentation:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `segtools-1.2.4/doc/conf.py` & `segtools-1.3.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 from __future__ import absolute_import
+from importlib.metadata import version
+
 import sys
 
 sys.path.append("..")
 
-from segtools.version import __version__ as release
-
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.imgmath', 'sphinx.ext.viewcode']
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.imgmath', 'sphinx.ext.viewcode', 'sphinx_rtd_theme']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
@@ -49,14 +49,16 @@
 copyright = u'2009-2011, Orion J. Buske, 2010-2011 Michael M. Hoffman'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
+# Ref: https://github.com/pypa/setuptools_scm#usage-from-sphinx
+release = version('segtools')
 version = release.rsplit(".", 1)[0]
 # The full version, including alpha/beta/rc tags.
 #release = '1.1.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `segtools-1.2.4/doc/flowchart.png` & `segtools-1.3.0/doc/flowchart.png`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/doc/make.bat` & `segtools-1.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/doc/Makefile` & `segtools-1.3.0/doc/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	@echo "  doctest    to run all doctests embedded in the documentation (if enabled)"
 
 clean:
 	-rm -rf $(BUILDDIR)/*
 
 $(CMDLINEHELPDIR)/%.help.txt:
 	@mkdir -p $(@D)
-	python gethelp.py $* > $@
+	python3 gethelp.py $* > $@
 
 cmdline-help: $(addprefix $(CMDLINEHELPDIR)/segtools-,compare.help.txt preprocess.help.txt aggregation.help.txt feature-distance.help.txt flatten.help.txt gmtk-parameters.help.txt html-report.help.txt transition.help.txt length-distribution.help.txt nucleotide-frequency.help.txt overlap.help.txt signal-distribution.help.txt relabel.help.txt)
 
 html: $(PREREQS)
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
```

### Comparing `segtools-1.2.4/COPYING` & `segtools-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/LICENSE` & `segtools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segtools-1.2.4/test/run_all.py` & `segtools-1.3.0/test/run_all.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python
-from __future__ import division, with_statement
 
 import os
 import re
 import sys
 import unittest
 
 def main(verbose=True):
     # Move to test directory to allow imports
     os.chdir(os.path.dirname(__file__) or ".")
 
     # Gather a list of unittest modules
     filenames = os.listdir(os.getcwd())
     regex = re.compile("^test_.*\.py$", re.IGNORECASE)
-    module_filenames = filter(regex.search, filenames)
+    module_filenames = list(filter(regex.search, filenames))
     make_module_name = lambda filename: filename[:-3]
-    modulenames = map(make_module_name, module_filenames)
+    modulenames = list(map(make_module_name, module_filenames))
     if verbose:
-        print "Found test modules: %r" % modulenames
+        print("Found test modules: %r" % modulenames)
 
     # Run the test suite for each
     suite = unittest.defaultTestLoader.loadTestsFromNames(modulenames)
     if verbose:
         verbosity = 2
     else:
         verbosity = 1
```

### Comparing `segtools-1.2.4/test/test_overlap.py` & `segtools-1.3.0/test/test_overlap.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,194 +23,195 @@
     strings = []
     for line in lines:
         chr, start, end, label = line
         strings.append("chr%s\t%s\t%s\t%d\t%d" % \
                            (chr, "source", label, start+1, end))
     return "\n".join(strings)
 
-class OverlapTester(unittest.TestCase):
-    def init(self):
-        pass
-
-    def setUp(self):
-        self.kwargs = {"verbose": False}
-        self.init()
-
-        # Set self.features from self.subject, self.query
-        self.features = []
-        self._open_files = []
-        for type, data in [self.subject, self.query]:
-            if type == "bed":
-                new_file = NamedTemporaryFile(suffix=".bed")
-                new_file.write(data2bed(data))
-            elif type == "gff":
-                new_file = NamedTemporaryFile(suffix=".gff")
-                new_file.write(data2gff(data))
-            elif type == "gtf":
-                new_file = NamedTemporaryFile(suffix=".gtf")
-                new_file.write(data2gff(data))
-
-            new_file.flush()
-            self._open_files.append(new_file)
-            features = Annotation(new_file.name, verbose=False)
-
-            if features:
-                self.features.append(features)
-
-    def tearDown(self):
-        for file in self._open_files:
-            file.close()
-
-    def test(self):
-        stats = calc_overlap(*self.features, **self.kwargs)
-        self.assertValuesEqual(stats, self.answer)
-
-    def assertArraysEqual(self, arr1, arr2):
-        not_equal = (arr1 != arr2)
-        if not_equal.any():
-            self.fail("%r != %r" % (arr1, arr2))
-
-    def assertValuesEqual(self, observed, expected):
-        # counts, totals, nones
-        for val1, val2 in zip(observed, expected):
-            self.assertArraysEqual(val1, array(val2))
+class OverlapTestCases:
+    class OverlapTester(unittest.TestCase):
+        def init(self):
+            pass
+
+        def setUp(self):
+            self.kwargs = {"verbose": False}
+            self.init()
+
+            # Set self.features from self.subject, self.query
+            self.features = []
+            self._open_files = []
+            for type, data in [self.subject, self.query]:
+                if type == "bed":
+                    new_file = NamedTemporaryFile(mode="w", suffix=".bed")
+                    new_file.write(data2bed(data))
+                elif type == "gff":
+                    new_file = NamedTemporaryFile(mode="w", suffix=".gff")
+                    new_file.write(data2gff(data))
+                elif type == "gtf":
+                    new_file = NamedTemporaryFile(mode="w", suffix=".gtf")
+                    new_file.write(data2gff(data))
+
+                new_file.flush()
+                self._open_files.append(new_file)
+                features = Annotation(new_file.name, verbose=False)
+
+                if features:
+                    self.features.append(features)
+
+        def tearDown(self):
+            for file in self._open_files:
+                file.close()
+
+        def test(self):
+            stats = calc_overlap(*self.features, **self.kwargs)
+            self.assertValuesEqual(stats, self.answer)
+
+        def assertArraysEqual(self, arr1, arr2):
+            not_equal = (arr1 != arr2)
+            if not_equal.any():
+                self.fail("%r != %r" % (arr1, arr2))
+
+        def assertValuesEqual(self, observed, expected):
+            # counts, totals, nones
+            for val1, val2 in zip(observed, expected):
+                self.assertArraysEqual(val1, array(val2))
 
-class TestSegmentPerfectOverlap(OverlapTester):
+class TestSegmentPerfectOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 0, 50, 1),  # chrom, start, end, label
                                 (1, 50, 100, 2)])
         self.query = ("bed", [(1, 0, 50, 1),
                               (1, 50, 100, 2)])
         self.answer = ([[1, 0], [0, 1]],  # subi vs qryj
                        (1, 1),  # total
                        (0, 0))  # none
 
-class TestBasePerfectOverlap(OverlapTester):
+class TestBasePerfectOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 0, 50, 1),
                                 (1, 50, 100, 2)])
         self.query = ("bed", [(1, 0, 50, 1),
                               (1, 50, 100, 2)])
         self.answer = ([[50, 0], [0, 50]],
                        (50, 50),
                        (0, 0))
 
-class TestSegmentNoOverlap(OverlapTester):
+class TestSegmentNoOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 10, 20, 1)])
         self.query = ("bed", [(1, 20, 35, 6)])
         self.answer = ([0],
                        (1),
                        (1))
 
-class TestBaseNoOverlap(OverlapTester):
+class TestBaseNoOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 10, 20, 1)])
         self.query = ("bed", [(1, 20, 35, 6)])
         self.answer = ([0],
                        (10),
                        (10))
 
-class TestSegmentNoOverlapChrom(OverlapTester):
+class TestSegmentNoOverlapChrom(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 10, 20, 1)])
         self.query = ("bed", [(9, 20, 35, 6)])
         self.answer = ([0],
                        (1),
                        (1))
 
-class TestBaseNoOverlapChrom(OverlapTester):
+class TestBaseNoOverlapChrom(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 10, 20, 1)])
         self.query = ("bed", [(9, 20, 35, 6)])
         self.answer = ([0],
                        (10),
                        (10))
 
-class TestSegmentSimpleOverlap(OverlapTester):
+class TestSegmentSimpleOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 11, 20, 1),
                                 (1, 25, 35, 2),
                                 (1, 37, 40, 3)])
         self.query = ("gff", [(1, 15, 37, 2)])
         self.answer = ([[1], [1], [0]],
                        (1, 1, 1),
                        (0, 0, 1))
 
-class TestBaseSimpleOverlap(OverlapTester):
+class TestBaseSimpleOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 11, 20, 1),
                                 (1, 25, 35, 2),
                                 (1, 37, 40, 3)])
         self.query = ("bed", [(1, 15, 37, 2)])
         self.answer = ([[5], [10], [0]],
                        (9, 10, 3),
                        (4, 0, 3))
 
-class TestSegmentStackedFeatures(OverlapTester):
+class TestSegmentStackedFeatures(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 0, 10, 1)])
         self.query = ("gff", [(1, 2, 9, 2),
                               (1, 3, 12, 3),
                               (1, 4, 7, 4),
                               (1, 5, 6, 5)])
         self.answer = ([1, 1, 1, 1],
                        (1),
                        (0))
 
-class TestBaseStackedFeatures(OverlapTester):
+class TestBaseStackedFeatures(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 0, 10, 1)])
         self.query = ("gff", [(1, 2, 9, 2),
                               (1, 3, 12, 3),
                               (1, 4, 7, 4),
                               (1, 5, 6, 5)])
         self.answer = ([7, 7, 3, 1],
                        (10),
                        (2))
 
-class TestSegmentOverlappingFeatures(OverlapTester):
+class TestSegmentOverlappingFeatures(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 0, 10, 1),
                                 (1, 10, 20, 2),
                                 (1, 20, 30, 1)])
         self.query = ("gff", [(1, 0, 30, 1),
                               (1, 2, 15, 1),
                               (1, 5, 20, 2),
                               (1, 10, 12, 1)])
         self.answer = ([[2, 1], [1, 1]],
                        (2, 1),
                        (0, 0))
 
-class TestBaseOverlappingFeatures(OverlapTester):
+class TestBaseOverlappingFeatures(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 0, 10, 1),
                                 (1, 10, 20, 2),
                                 (1, 20, 30, 1)])
         self.query = ("gff", [(1, 0, 30, 1),
                               (1, 2, 15, 1),
                               (1, 5, 20, 2),
                               (1, 10, 12, 1)])
         self.answer = ([[20, 5], [10, 10]],
                        (20, 10),
                        (0, 0))
 
-class TestSegmentComplexOverlap(OverlapTester):
+class TestSegmentComplexOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 0, 4, 1),
                                 (1, 10, 15, 2),
                                 (1, 15, 21, 3),
                                 (1, 26, 27, 1),
                                 (1, 30, 31, 2),
@@ -224,15 +225,15 @@
                               (1, 25, 30, 3),
                               (2, 5, 10, 1),
                               (2, 10, 15, 3)])
         self.answer = ([[2, 1, 1], [0, 1, 1], [1, 1, 0]],
                        (2, 3, 2),
                        (0, 1, 1))
 
-class TestBaseComplexOverlap(OverlapTester):
+class TestBaseComplexOverlap(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 0, 4, 1),
                                 (1, 10, 15, 2),
                                 (1, 15, 21, 3),
                                 (1, 26, 27, 1),
                                 (1, 30, 31, 2),
@@ -246,15 +247,15 @@
                               (1, 25, 30, 3),
                               (2, 5, 10, 1),
                               (2, 10, 15, 3)])
         self.answer = ([[5, 1, 1], [0, 5, 1], [6, 1, 0]],
                        (5, 8, 105),
                        (0, 2, 99))
 
-class TestSegmentComplexOverlapReversed(OverlapTester):
+class TestSegmentComplexOverlapReversed(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "segments"
         self.subject = ("bed", [(1, 0, 10, 1),
                                 (1, 5, 15, 2),
                                 (1, 15, 25, 1),
                                 (1, 20, 30, 1),
                                 (1, 20, 30, 2),
@@ -269,15 +270,15 @@
                               (2, 14, 16, 2),
                               (3, 1, 100, 3)])
         self.answer = ([[2, 0, 2], [1, 1, 1], [1, 1, 0]],
                        (4, 2, 2),
                        (1, 0, 0))
 
 
-class TestBaseComplexOverlapReversed(OverlapTester):
+class TestBaseComplexOverlapReversed(OverlapTestCases.OverlapTester):
     def init(self):
         self.kwargs["mode"] = "bases"
         self.subject = ("bed", [(1, 0, 10, 1),
                                 (1, 5, 15, 2),
                                 (1, 15, 25, 1),
                                 (1, 20, 30, 1),
                                 (1, 20, 30, 2),
```

### Comparing `segtools-1.2.4/test/test_feature_distance.py` & `segtools-1.3.0/test/test_feature_distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 from __future__ import with_statement
 
 import inspect
 import os
 import sys
 import unittest
 
-from tempfile import NamedTemporaryFile
+from shutil import rmtree
+from tempfile import mkdtemp, NamedTemporaryFile
+
+from segtools.feature_distance import DELIM, feature_distance, PRINT_FIELDS
 
-from segtools.feature_distance import DELIM, feature_distance, STANDARD_FIELDS
 
 def data2bed(lines):
     # Input lines should each be a tuple of (chrom, start, end, label)
     strings = []
     for line in lines:
         strings.append("chr%s\t%d\t%d\t%s" % line)
     return "\n".join(strings)
@@ -57,92 +59,87 @@
     def writelines(self, lines):
         self._log.extend(lines)
     def restore(self):
         sys.stdout = self._stdout
     def log(self):
         return "".join(self._log)
 
-class MainTester(unittest.TestCase):
-    def init(self):
-        pass
+class FeatureDistanceTestCases:
+    class MainTester(unittest.TestCase):
+        def init(self):
+            pass
+
+        def setUp(self):
+            self.kwargs = {"verbose": False}
+            self.init()
+
+            # Set self.features from self.segments, self.features_list
+            self.feature_file = None
+            self.segment_file = None
+            self._open_files = []
+            
+            self.output_path = mkdtemp()
 
-    def setUp(self):
-        self.kwargs = {"verbose": False}
-        self.init()
-
-        # Set self.features from self.segments, self.features_list
-        self.feature_files = []
-        self.segment_file = None
-        self._open_files = []
-
-        new_file = NamedTemporaryFile(suffix=".bed")
-        new_file.write(data2bed(self.segments))
-        new_file.flush()
-        self._open_files.append(new_file)
-        self.segment_file = new_file.name
+            new_file = NamedTemporaryFile(mode="w",suffix=".bed")
+            new_file.write(data2bed(self.segments))
+            new_file.flush()
+            self._open_files.append(new_file)
+            self.segment_file = new_file.name
+
+            type, data = self.features
 
-        for type, data in self.features_list:
             if type == "bed":
-                new_file = NamedTemporaryFile(suffix=".bed")
+                new_file = NamedTemporaryFile(mode="w", suffix=".bed")
                 new_file.write(data2bed(data))
             elif type == "gff":
-                new_file = NamedTemporaryFile(suffix=".gff")
+                new_file = NamedTemporaryFile(mode="w",suffix=".gff")
                 new_file.write(data2gff(data))
             elif type == "gtf":
-                new_file = NamedTemporaryFile(suffix=".gtf")
+                new_file = NamedTemporaryFile(mode="w",suffix=".gtf")
                 new_file.write(data2gff(data))
 
             new_file.flush()
             self._open_files.append(new_file)
-            self.feature_files.append(new_file.name)
+            self.feature_file = new_file.name
 
-    def tearDown(self):
-        for file in self._open_files:
-            file.close()
-
-    def test(self):
-        # Run function, logging stdout
-        self._saver = OutputSaver()
-        stats = feature_distance(self.segment_file, self.feature_files,
-                                 **self.kwargs)
-        self._saver.restore()
-        log_lines = self._saver.log().strip("\n").split("\n")
-        log_header = log_lines.pop(0).split(DELIM)
-
-        # Check header
-        header_answer = STANDARD_FIELDS + \
-            [os.path.basename(filename) for filename in self.feature_files]
-        self.assertEqual(log_header, header_answer)
-
-        # Check values
-        observed_strs = [line.split(DELIM)[len(STANDARD_FIELDS):]
-                         for line in log_lines]
-        answer_strs = [[str(val) for val in line] for line in self.answer]
+        def tearDown(self):
+            for file in self._open_files:
+                file.close()
+            
+            rmtree(self.output_path)
+
+        def test(self):
+            # Run function, logging stdout
+            self._saver = OutputSaver()
+            _ = feature_distance(self.segment_file, self.feature_file,
+                                 self.output_path, **self.kwargs)
+            self._saver.restore()
+            log_lines = self._saver.log().strip("\n").split("\n")
+            log_header = log_lines.pop(0).split(DELIM)
+
+            # Check header
+            header_answer = PRINT_FIELDS
+            self.assertEqual(log_header, header_answer)
+
+            # Check values
+            observed_strs = [[line.split(DELIM)[-1]]
+                            for line in log_lines]
+            answer_strs = [[str(val) for val in line] for line in self.answer]
 
-        self.assertEqual(observed_strs, answer_strs)
+            self.assertEqual(observed_strs, answer_strs)
 
-class TestSimple(MainTester):
+class TestSimple(FeatureDistanceTestCases.MainTester):
     def init(self):
         self.segments = [(1, 5, 6, 1),
                          (1, 10, 15, 1),
                          (1, 15, 20, 1)]
-        self.features_list = [("bed", [(1, 6, 11, 1),
-                                       (1, 11, 12, 1)])]
+        self.features = ("bed", [(1, 6, 11, 1),
+                                 (1, 11, 12, 1)])
         self.answer = [[1], [0], [4]]
 
-class TestStrandCorrect(MainTester):
-    def init(self):
-        self.kwargs["correct_strands"] = [0]
-        self.segments = [(1, 60, 90, 0),
-                         (1, 130, 140, 0)]
-        self.features_list = [("gtf", [(1, 1, 10, 1, "+"),
-                                       (1, 2, 3, 2, "-"),
-                                       (1, 3, 50, 4, "+"),
-                                       (1, 120, 125, 1, "-")])]
-        self.answer = [[-11], [6]]
 
 def suite():
     classes = []
     members = inspect.getmembers(sys.modules[__name__])
     for name, value in members:
         if inspect.isclass(value) and name.startswith("Test"):
             classes.append(value)
```

### Comparing `segtools-1.2.4/test/test_bed_compare.py` & `segtools-1.3.0/test/test_bed_compare.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,43 +4,45 @@
 import inspect
 import sys
 import unittest
 
 from tempfile import NamedTemporaryFile
 
 from segtools import Segmentation
-from segtools.bed_compare import edit_distance
+from segtools.compare import edit_distance
 
 def beddata2bed(lines):
     # Input lines should each be a tuple of (chrom, start, end, label)
     strings = []
     for line in lines:
         strings.append("chr%s\t%d\t%d\t%s" % line)
     return "\n".join(strings)
 
+@unittest.skip("No data for base BED Generation tests")
 class BedGenerator(unittest.TestCase):
     def init(self):
         pass
 
     def setUp(self):
         self.init()
 
         # Create fake bed files
-        self._open_bedfiles = [NamedTemporaryFile(suffix=".bed"),
-                               NamedTemporaryFile(suffix=".bed")]
+        self._open_bedfiles = [NamedTemporaryFile(mode="w", suffix=".bed"),
+                               NamedTemporaryFile(mode="w",  suffix=".bed")]
         for file, data in zip(self._open_bedfiles, self.beddata):
             file.write(beddata2bed(data))
         for file in self._open_bedfiles:
             file.flush()
         self.bedfiles = [file.name for file in self._open_bedfiles]
 
     def tearDown(self):
         for file in self._open_bedfiles:
             file.close()
-
+            
+@unittest.skip("No data for base BED Generation tests")
 class EditDistanceTester(BedGenerator):
     def test(self):
         stats = edit_distance(self.bedfiles[0], self.bedfiles[1], verbose=False)
         self.assertValuesEqual(stats, self.answer)
 
     def assertValuesEqual(self, observed, expected):
         for val1, val2 in zip(observed, expected):
```

### Comparing `segtools-1.2.4/segtools.egg-info/SOURCES.txt` & `segtools-1.3.0/segtools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-.hgignore
-.hgtags
+.gitignore
+.readthedocs.yaml
+CITATION.cff
 COPYING
-INSTALL
 LICENSE
 NEWS
 README.rst
 TODO
-ez_setup.py
-install.py
-install.tmpl
-setup.cfg
-setup.py
+environment.yml
+pyproject.toml
+.github/workflows/continuous-integration-workflow.yml
+.github/workflows/python-publish.yml
 R/README
 R/build.sh
 R/segtools/DESCRIPTION
 R/segtools/NAMESPACE
 R/segtools/R
 R/segtools/Read-and-delete-me
 R/segtools/man/segtools-package.Rd
@@ -44,15 +43,14 @@
 segtools/signal_distribution.py
 segtools/transition.py
 segtools/version.py
 segtools.egg-info/PKG-INFO
 segtools.egg-info/SOURCES.txt
 segtools.egg-info/dependency_links.txt
 segtools.egg-info/entry_points.txt
-segtools.egg-info/not-zip-safe
 segtools.egg-info/requires.txt
 segtools.egg-info/top_level.txt
 segtools/R/__init__.py
 segtools/R/aggregation.R
 segtools/R/common.R
 segtools/R/dinucleotide.R
 segtools/R/distance.R
```

