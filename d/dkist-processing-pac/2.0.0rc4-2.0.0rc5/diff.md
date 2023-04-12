# Comparing `tmp/dkist-processing-pac-2.0.0rc4.tar.gz` & `tmp/dkist-processing-pac-2.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-pac-2.0.0rc4.tar", last modified: Wed Mar 15 19:29:29 2023, max compression
+gzip compressed data, was "dkist-processing-pac-2.0.0rc5.tar", last modified: Tue Mar 21 21:39:14 2023, max compression
```

## Comparing `dkist-processing-pac-2.0.0rc4.tar` & `dkist-processing-pac-2.0.0rc5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3042 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/16.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/17.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/18.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/19.bugfix.rst
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/20.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/changelog/21.bugfix.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/CS_files/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/CS_files/aggressive_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/CS_files/asp16_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/CS_files/efficient_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/CS_files/may_CS.txt
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/constants.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/M12_fitUV.yml
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/baseline.yml
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/fit_QUV.yml
--rw-rw-rw-   0 root         (0) root         (0)      379 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/no_T.yml
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/use_M12.yml
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/use_M12_I_sys_per_step.yml
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/fit_modes/use_M12_globalRet_globalTrans.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/init_values/
--rw-rw-rw-   0 root         (0) root         (0)   284469 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf
--rw-rw-rw-   0 root         (0) root         (0)   192191 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf
--rw-rw-rw-   0 root         (0) root         (0)    32177 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/py_table.txt
--rw-rw-rw-   0 root         (0) root         (0)   306602 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/telescope_db.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14749 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/fitter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     5017 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/fitting_core.py
--rw-rw-rw-   0 root         (0) root         (0)     8831 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/polcal_fitter.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/input_data/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/input_data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10286 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/input_data/drawer.py
--rw-rw-rw-   0 root         (0) root         (0)     6161 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/input_data/dresser.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11414 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/calibration_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     3383 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/mueller_matrices.py
--rw-rw-rw-   0 root         (0) root         (0)    12300 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/telescope.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15374 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     7793 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_calibration_unit.py
--rw-rw-rw-   0 root         (0) root         (0)     7639 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_drawer.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_dresser.py
--rw-rw-rw-   0 root         (0) root         (0)     8460 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_fitter_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_mueller_matrices.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_nd_parameter_array.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_polcal_fitter.py
--rw-rw-rw-   0 root         (0) root         (0)    15571 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_telescope.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.965934 dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-03-15 19:29:29.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-03-15 19:29:29.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-15 19:29:29.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-03-15 19:29:29.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-15 19:29:29.000000 dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     5571 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/background.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1831 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     8458 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/layout.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-15 19:29:29.969934 dkist-processing-pac-2.0.0rc4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      102 2023-03-15 19:29:24.000000 dkist-processing-pac-2.0.0rc4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3547 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/16.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/17.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/18.bugfix.rst
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/19.bugfix.rst
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/20.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/changelog/21.bugfix.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/aggressive_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      763 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/asp16_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/efficient_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/may_CS.txt
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/constants.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/M12_fitUV.yml
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/baseline.yml
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/fit_QUV.yml
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/no_T.yml
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/use_M12.yml
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/use_M12_I_sys_per_step.yml
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/fit_modes/use_M12_globalRet_globalTrans.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/
+-rw-rw-rw-   0 root         (0) root         (0)   284469 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf
+-rw-rw-rw-   0 root         (0) root         (0)   192191 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf
+-rw-rw-rw-   0 root         (0) root         (0)    32177 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/py_table.txt
+-rw-rw-rw-   0 root         (0) root         (0)   306602 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/telescope_db.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15220 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     5017 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitting_core.py
+-rw-rw-rw-   0 root         (0) root         (0)     9110 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/polcal_fitter.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10286 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/drawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/dresser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11414 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/calibration_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/mueller_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    12300 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/telescope.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15374 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     7793 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_calibration_unit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7639 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_drawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_dresser.py
+-rw-rw-rw-   0 root         (0) root         (0)     9205 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_fitter_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_mueller_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_nd_parameter_array.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_polcal_fitter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15571 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_telescope.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.338895 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3547 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-21 21:39:14.000000 dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5571 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/background.rst
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1831 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8458 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-21 21:39:14.342896 dkist-processing-pac-2.0.0rc5/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-21 21:39:14.346896 dkist-processing-pac-2.0.0rc5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      102 2023-03-21 21:39:07.000000 dkist-processing-pac-2.0.0rc5/setup.py
```

### Comparing `dkist-processing-pac-2.0.0rc4/.gitignore` & `dkist-processing-pac-2.0.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/.pre-commit-config.yaml` & `dkist-processing-pac-2.0.0rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/CHANGELOG.rst` & `dkist-processing-pac-2.0.0rc5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/PKG-INFO` & `dkist-processing-pac-2.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-pac
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: PA&C Pipeline
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-pac/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: unknown
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/pac
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-pac-2.0.0rc4/README.rst` & `dkist-processing-pac-2.0.0rc5/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/bitbucket-pipelines.yml` & `dkist-processing-pac-2.0.0rc5/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/check_changelog_updated.sh` & `dkist-processing-pac-2.0.0rc5/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/CS_files/asp16_CS.txt` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/CS_files/asp16_CS.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_cu_pars.asdf`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/init_values/OCCal_VIS_tm_pars.asdf`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/py_table.txt` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/py_table.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/data/telescope_db.txt` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/data/telescope_db.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/fitter_parameters.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitter_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -294,25 +294,34 @@
         for m in range(O.shape[0]):
             for i, s in enumerate(["I", "Q", "U", "V"]):
                 params["modmat_{}{}".format(m, s)].set(value=O[m, i])
 
         # Just in case
         params["modmat_0I"].set(value=1)
 
-    def fix_global_CU_params(self, global_fit_params: Parameters):
-        """Fix."""
-        global_par_dict = global_fit_params.valuesdict()
+    def apply_global_CU_params(
+        self, global_fit_params: Parameters, inherit_global_vary: bool = False
+    ):
+        """Update local parameter values with results from a global parameter fit.
+
+        If `inherit_global_vary` is False then all global parameters will fixed in the local parameters. If it is True
+        then the fixed/free-ness of each global parameter will carry over to the local parameters.
+        """
         num_points = np.prod(self.fov_shape)
         for i in range(num_points):
             idx = np.unravel_index(i, self.fov_shape)
             params = self.init_params[idx]
             for par in CU_PARAMS:
                 for d in range(self.dresser.numdrawers):
                     par_name = f"{par}_CS{d:02n}"
-                    params[par_name].set(value=global_par_dict[par_name], vary=False)
+                    value = global_fit_params[par_name].value
+                    vary = False
+                    if inherit_global_vary:
+                        vary = global_fit_params[par_name].vary
+                    params[par_name].set(value=value, vary=vary)
 
 
 class NdParameterArray:
     """Store single lmfit `Parameters` objects for an N-dimensional set of points.
 
     This is basically a normal python list, but with some sneaky indexing to make it look like it has the same shape
     as the fit FOV.
```

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/fitting_core.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/fitting_core.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/fitter/polcal_fitter.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/fitter/polcal_fitter.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         local_dresser: Dresser,
         global_dresser: Dresser,
         fit_mode: str,
         init_set: str,
         fit_TM: bool = False,
         threads: int = 1,
         super_name: str = "",
+        inherit_global_vary_in_local_fit: bool = False,
         _dont_fit: bool = False,
         suppress_local_starting_values: bool = False,
         **fit_kwargs,
     ):
 
         self.fit_mode = fit_mode
         self.init_set = init_set
@@ -99,17 +100,21 @@
             self.run_fits(
                 fit_container=self.global_objects,
                 threads=threads,
                 super_name=super_name,
                 **fit_kwargs,
             )
 
-            logger.info("Fixing global CU parameters in local fits")
+            logger.info("Applying global CU parameters in local fits")
+            if not inherit_global_vary_in_local_fit:
+                logging.info("Global CU parameters will be fixed in local fits.")
             global_fit_pars = self.global_objects.fit_parameters.first_parameters
-            self.local_objects.full_parameters.fix_global_CU_params(global_fit_pars)
+            self.local_objects.full_parameters.apply_global_CU_params(
+                global_fit_pars, inherit_global_vary=inherit_global_vary_in_local_fit
+            )
 
             logger.info("Fitting local modulation matrices")
             self.run_fits(
                 fit_container=self.local_objects,
                 threads=threads,
                 super_name=super_name,
                 suppress_point_starting_values=suppress_local_starting_values,
```

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/input_data/drawer.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/drawer.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/input_data/dresser.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/input_data/dresser.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/calibration_unit.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/calibration_unit.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/mueller_matrices.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/mueller_matrices.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/optics/telescope.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/optics/telescope.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/conftest.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_calibration_unit.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_calibration_unit.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_drawer.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_drawer.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_dresser.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_dresser.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_fitter_parameters.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_fitter_parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,34 +147,47 @@
     params.init_params[0, 0, 0]["ret0h_CS00"].set(value=999.0)
     params.init_params[0, 0, 0]["ret045_CS00"].set(value=999.0)
     params.init_params[0, 0, 0]["ret0r_CS00"].set(value=999.0)
 
     return params
 
 
-def test_fix_global_CU_params(session_full_params, weird_local_params):
+@pytest.mark.parametrize(
+    "inherit_global_vary",
+    [pytest.param(True, id="inherit global vary"), pytest.param(False, id="fix local CU params")],
+)
+def test_apply_global_CU_params(session_full_params, weird_local_params, inherit_global_vary):
     """
     Given: two PolcalDresserParameters; one global and one local
-    When: fixing the local parameter's CU params with the global parameters
-    Then: the correct values are assinged and the CU params are fixed
+    When: applying the global parameter's CU params to the local parameters
+    Then: the correct values are assigned and the CU params are fixed unless the vary carries through
     """
     global_params = session_full_params.fit_params[0, 0, 0]
-    weird_local_params.fix_global_CU_params(global_params)
+    weird_local_params.apply_global_CU_params(
+        global_params, inherit_global_vary=inherit_global_vary
+    )
     local_params = weird_local_params.init_params[0, 0, 0]
 
     assert local_params["t_ret_CS00"].value == global_params["t_ret_CS00"].value
-    assert local_params["t_ret_CS00"].vary is False
     assert local_params["t_pol_CS00"].value == global_params["t_pol_CS00"].value
-    assert local_params["t_pol_CS00"].vary is False
     assert local_params["ret0h_CS00"].value == global_params["ret0h_CS00"].value
-    assert local_params["ret0h_CS00"].vary is False
     assert local_params["ret045_CS00"].value == global_params["ret045_CS00"].value
-    assert local_params["ret045_CS00"].vary is False
     assert local_params["ret0r_CS00"].value == global_params["ret0r_CS00"].value
-    assert local_params["ret0r_CS00"].vary is False
+    if not inherit_global_vary:
+        assert local_params["ret0r_CS00"].vary is False
+        assert local_params["ret045_CS00"].vary is False
+        assert local_params["ret0h_CS00"].vary is False
+        assert local_params["t_pol_CS00"].vary is False
+        assert local_params["t_ret_CS00"].vary is False
+    else:
+        assert local_params["ret0r_CS00"].vary is global_params["ret0r_CS00"].vary
+        assert local_params["ret045_CS00"].vary is global_params["ret045_CS00"].vary
+        assert local_params["ret0h_CS00"].vary is global_params["ret0h_CS00"].vary
+        assert local_params["t_pol_CS00"].vary is global_params["t_pol_CS00"].vary
+        assert local_params["t_ret_CS00"].vary is global_params["t_ret_CS00"].vary
 
 
 def test_demodulation_matrix(session_full_params):
     """
     Given: DresserParameters
     When: accessing the *de*modulation matrices
     Then: the correct matrix is returned
```

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_nd_parameter_array.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_nd_parameter_array.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_polcal_fitter.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_polcal_fitter.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac/tests/test_telescope.py` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac/tests/test_telescope.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/PKG-INFO` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-pac
-Version: 2.0.0rc4
+Version: 2.0.0rc5
 Summary: PA&C Pipeline
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-pac/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: unknown
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/pac
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-pac-2.0.0rc4/dkist_processing_pac.egg-info/SOURCES.txt` & `dkist-processing-pac-2.0.0rc5/dkist_processing_pac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/docs/Makefile` & `dkist-processing-pac-2.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/docs/background.rst` & `dkist-processing-pac-2.0.0rc5/docs/background.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/docs/conf.py` & `dkist-processing-pac-2.0.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/docs/layout.rst` & `dkist-processing-pac-2.0.0rc5/docs/layout.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/docs/make.bat` & `dkist-processing-pac-2.0.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/licenses/LICENSE.rst` & `dkist-processing-pac-2.0.0rc5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/pyproject.toml` & `dkist-processing-pac-2.0.0rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-pac-2.0.0rc4/setup.cfg` & `dkist-processing-pac-2.0.0rc5/setup.cfg`

 * *Files identical despite different names*

