# Comparing `tmp/qp-prob-0.8.0.tar.gz` & `tmp/qp-prob-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qp-prob-0.8.0.tar", last modified: Tue Apr 11 01:52:12 2023, max compression
+gzip compressed data, was "qp-prob-0.8.1.tar", last modified: Wed Apr 12 20:45:53 2023, max compression
```

## Comparing `qp-prob-0.8.0.tar` & `qp-prob-0.8.1.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-11 01:52:01.000000 qp-prob-0.8.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-11 01:52:01.000000 qp-prob-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-04-11 01:52:12.003129 qp-prob-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-11 01:52:01.000000 qp-prob-0.8.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)       52 2023-04-11 01:52:01.000000 qp-prob-0.8.0/do_cover.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)   861344 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/demo.html
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (122)   757141 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/practical_example.html
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/qp.rst
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-11 01:52:01.000000 qp-prob-0.8.0/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/nb/
--rw-r--r--   0 runner    (1001) docker     (122)    32323 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/iterator_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    15156 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/metrics_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/mixmod_examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    11839 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/practical_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    37404 2023-04-11 01:52:01.000000 qp-prob-0.8.0/nb/quantile_parameterization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-04-11 01:52:01.000000 qp-prob-0.8.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (122)      326 2023-04-11 01:52:01.000000 qp-prob-0.8.0/render_nb.sh
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-11 01:52:01.000000 qp-prob-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 01:52:12.003129 qp-prob-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-11 01:52:01.000000 qp-prob-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/src/qp/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    11413 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/conversion_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/src/qp/data/
--rw-r--r--   0 runner    (1001) docker     (122)   161680 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/data/CFHTLens_sample.P.npy
--rw-r--r--   0 runner    (1001) docker     (122)    16848 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/data/test.hdf5
--rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/dict_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    21140 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)    11359 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/hist_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    12842 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/interp_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.999129 qp-prob-0.8.0/src/qp/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/array_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/brier.py
--rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/goodness_of_fit.py
--rw-r--r--   0 runner    (1001) docker     (122)    17889 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7560 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/metrics/pit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6155 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/mixmod_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/packed_interp_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/packing_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14160 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/pdf_gen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quant_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
--rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
--rw-r--r--   0 runner    (1001) docker     (122)     6796 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/dual_spline_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/piecewise_constant.py
--rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/quantile_pdf_constructors/piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/scipy_pdfs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/sparse_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)    10121 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/sparse_rep.py
--rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/spline_pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)    23972 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-11 01:52:01.000000 qp-prob-0.8.0/src/qp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/src/qp_prob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        3 2023-04-11 01:52:11.000000 qp-prob-0.8.0/src/qp_prob.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:11.995129 qp-prob-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/tests/qp/
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/fidelity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:12.003129 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
--rw-r--r--   0 runner    (1001) docker     (122)     4145 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (122)     4607 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_brier.py
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_eval_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_flex_coefs.npy
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (122)    15872 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_pit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5816 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_scipy_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-11 01:52:01.000000 qp-prob-0.8.0/tests/qp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.777543 qp-prob-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.757542 qp-prob-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.761542 qp-prob-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1749 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-12 20:45:40.000000 qp-prob-0.8.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-12 20:45:40.000000 qp-prob-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-12 20:45:53.777543 qp-prob-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-12 20:45:40.000000 qp-prob-0.8.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)       52 2023-04-12 20:45:40.000000 qp-prob-0.8.1/do_cover.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.765542 qp-prob-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1192 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6764 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9914 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   861344 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/demo.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (122)   757141 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/practical_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/qp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-12 20:45:40.000000 qp-prob-0.8.1/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.765542 qp-prob-0.8.1/nb/
+-rw-r--r--   0 runner    (1001) docker     (122)    32323 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/iterator_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    15156 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/metrics_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4917 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/mixmod_examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    11839 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/practical_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    37404 2023-04-12 20:45:40.000000 qp-prob-0.8.1/nb/quantile_parameterization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2036 2023-04-12 20:45:40.000000 qp-prob-0.8.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      326 2023-04-12 20:45:40.000000 qp-prob-0.8.1/render_nb.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-04-12 20:45:40.000000 qp-prob-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 20:45:53.777543 qp-prob-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-12 20:45:40.000000 qp-prob-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.757542 qp-prob-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.769542 qp-prob-0.8.1/src/qp/
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-12 20:45:52.000000 qp-prob-0.8.1/src/qp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11419 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/conversion_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.769542 qp-prob-0.8.1/src/qp/data/
+-rw-r--r--   0 runner    (1001) docker     (122)   161680 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/data/CFHTLens_sample.P.npy
+-rw-r--r--   0 runner    (1001) docker     (122)    16848 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/data/test.hdf5
+-rw-r--r--   0 runner    (1001) docker     (122)     5697 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/dict_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21140 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6521 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/hist_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12842 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/lazy_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/src/qp/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/array_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3322 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/brier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/goodness_of_fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17889 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7560 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/metrics/pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6155 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/mixmod_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9400 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/packed_interp_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4298 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/packing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14160 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/pdf_gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9099 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quant_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4535 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6796 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4251 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3952 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1464 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/scipy_pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/sparse_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10121 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/sparse_rep.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10537 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/spline_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1130 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7824 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23972 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-12 20:45:40.000000 qp-prob-0.8.1/src/qp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/src/qp_prob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        3 2023-04-12 20:45:53.000000 qp-prob-0.8.1/src/qp_prob.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.757542 qp-prob-0.8.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.773543 qp-prob-0.8.1/tests/qp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/fidelity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:53.777543 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4854 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4145 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4607 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_brier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_eval_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4448 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_flex_coefs.npy
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15872 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_pit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5816 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_scipy_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2894 2023-04-12 20:45:40.000000 qp-prob-0.8.1/tests/qp/test_utils.py
```

### Comparing `qp-prob-0.8.0/.github/workflows/pypi.yaml` & `qp-prob-0.8.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/.github/workflows/python-package.yml` & `qp-prob-0.8.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/.gitignore` & `qp-prob-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/.travis.yml` & `qp-prob-0.8.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/LICENSE` & `qp-prob-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/PKG-INFO` & `qp-prob-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.8.0
+Version: 0.8.1
 License: MIT License
         
         Copyright (c) 2016 Alex Malz & Phil Marshall
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,14 +26,16 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 # qp
 
 Quantile parametrization for probability distribution functions.
```

### Comparing `qp-prob-0.8.0/README.md` & `qp-prob-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/.gitignore` & `qp-prob-0.8.1/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/Makefile` & `qp-prob-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/conf.py` & `qp-prob-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/contributing.rst` & `qp-prob-0.8.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/demo.html` & `qp-prob-0.8.1/docs/demo.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/index.rst` & `qp-prob-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/install.rst` & `qp-prob-0.8.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/practical_example.html` & `qp-prob-0.8.1/docs/practical_example.html`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/docs/qp.rst` & `qp-prob-0.8.1/docs/qp.rst`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/nb/demo.ipynb` & `qp-prob-0.8.1/nb/demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/nb/iterator_demo.ipynb` & `qp-prob-0.8.1/nb/iterator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/nb/metrics_examples.ipynb` & `qp-prob-0.8.1/nb/metrics_examples.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/nb/mixmod_examples.ipynb` & `qp-prob-0.8.1/nb/mixmod_examples.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/nb/practical_example.ipynb` & `qp-prob-0.8.1/nb/practical_example.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/nb/quantile_parameterization_demo.ipynb` & `qp-prob-0.8.1/nb/quantile_parameterization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/pyproject.toml` & `qp-prob-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,17 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
 ]
 dynamic = ["version"]
 dependencies = [
-    "matplotlib",
     "numpy",
     "scipy >= 1.9.0",
-    "scikit-learn",
-    "tables_io >= 0.7.7",
+    "tables-io >= 0.8.0",
     "deprecated",
 ]
 
 
 [metadata]
 author = "Alex Malz, Phil Marshall, Eric Charles"
 author_email = "aimalz@nyu.edu, pjm@slac.stanford.edu, echarles@slac.stanford.edu"
@@ -41,25 +39,35 @@
 [tool.setuptools.package-data]
 "qp.data" = ["*.npy"]
 
 [tool.setuptools_scm]
 write_to = "src/qp/_version.py"
 
 [project.optional-dependencies]
+full = [
+    "tables-io[full]",
+]
+all = [
+    "tables-io[full]",
+    "matplotlib",
+    "scikit-learn",
+]
 dev = [
+    "tables-io[full]",
+    "matplotlib",
+    "scikit-learn",
     "pytest",
     "pytest-cov",
     "packaging",
     "pillow",
     "cycler",
     "python-dateutil",
     "kiwisolver",
     "joblib",
     "threadpoolctl",
-    "h5py",
     "pylint",
     "mpi4py",
     "coverage",
 ]
 
 [tool.coverage.run]
 source = ["qp"]
```

### Comparing `qp-prob-0.8.0/src/qp/__init__.py` & `qp-prob-0.8.1/src/qp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 from .quant_pdf import *
 from .mixmod_pdf import *
 from .sparse_pdf import *
 from .scipy_pdfs import *
 from .packed_interp_pdf import *
 from .ensemble import Ensemble
 from .factory import instance, add_class, create, read, convert, concatenate, iterator, data_length, from_tables
+from .lazy_modules import *
 
 from . import utils
 
 from . import packing_utils
 
 from . import test_funcs
```

### Comparing `qp-prob-0.8.0/src/qp/conversion_funcs.py` & `qp-prob-0.8.1/src/qp/conversion_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """This module implements functions to convert distributions between various representations
 These functions should then be registered with the `qp.ConversionDict` using `qp_add_mapping`.
 That will allow the automated conversion mechanisms to work.
 """
 import numpy as np
 
-from sklearn import mixture
 from scipy import integrate as sciint
 from scipy import interpolate as sciinterp
 
 from .sparse_rep import indices2shapes, build_sparse_representation, decode_sparse_indices
+from .lazy_modules import mixture
 
 def extract_vals_at_x(in_dist, **kwargs):
     """Convert using a set of x and y values.
 
     Parameters
     ----------
     in_dist : `qp.Ensemble`
```

### Comparing `qp-prob-0.8.0/src/qp/data/CFHTLens_sample.P.npy` & `qp-prob-0.8.1/src/qp/data/CFHTLens_sample.P.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/data/test.hdf5` & `qp-prob-0.8.1/src/qp/data/test.hdf5`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/dict_utils.py` & `qp-prob-0.8.1/src/qp/dict_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/ensemble.py` & `qp-prob-0.8.1/src/qp/ensemble.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/factory.py` & `qp-prob-0.8.1/src/qp/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,18 +118,18 @@
             raise KeyError("Class nameed %s is not in factory" % class_name)
         the_class = self[class_name]
         ctor_func = the_class.creation_method(method)
         return Ensemble(ctor_func, data)
 
     def from_tables(self, tables):
         """Build this ensemble from a tables
-        
+
         Parameters
         ----------
-        tables: `dict` 
+        tables: `dict`
 
         Notes
         -----
         This will use information in the meta data table to figure out how to construct the data
         need to build the ensemble.
         """
         md_table = tables['meta']
@@ -145,15 +145,15 @@
 
         the_class = self[pdf_name]
         reader_convert = the_class.reader_method(pdf_version)
         ctor_func = the_class.creation_method(None)
         if reader_convert is not None: #pragma: no cover
             data = reader_convert(data)
         return Ensemble(ctor_func, data=data, ancil=ancil_table)
-       
+
     def read(self, filename):
         """Read this ensemble from a file
 
         Parameters
         ----------
         filename : `str`
```

### Comparing `qp-prob-0.8.0/src/qp/hist_pdf.py` & `qp-prob-0.8.1/src/qp/hist_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/interp_pdf.py` & `qp-prob-0.8.1/src/qp/interp_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/metrics/array_metrics.py` & `qp-prob-0.8.1/src/qp/metrics/array_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/metrics/brier.py` & `qp-prob-0.8.1/src/qp/metrics/brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/metrics/goodness_of_fit.py` & `qp-prob-0.8.1/src/qp/metrics/goodness_of_fit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/metrics/metrics.py` & `qp-prob-0.8.1/src/qp/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/metrics/pit.py` & `qp-prob-0.8.1/src/qp/metrics/pit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/mixmod_pdf.py` & `qp-prob-0.8.1/src/qp/mixmod_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/packed_interp_pdf.py` & `qp-prob-0.8.1/src/qp/packed_interp_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/packing_utils.py` & `qp-prob-0.8.1/src/qp/packing_utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/pdf_gen.py` & `qp-prob-0.8.1/src/qp/pdf_gen.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/plotting.py` & `qp-prob-0.8.1/src/qp/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Functions to plot PDFs"""
 
 import numpy as np
 
-import matplotlib as mpl
-import matplotlib.pyplot as plt
+from .lazy_modules import mpl, plt
 
 
 def init_matplotlib():
     """Initialize matplotlib parameters"""
     # Comment out usetex and serif, as these sometimes
     # cause issues on cori with no LaTex installed by
     # default
```

### Comparing `qp-prob-0.8.0/src/qp/quant_pdf.py` & `qp-prob-0.8.1/src/qp/quant_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py` & `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/abstract_pdf_constructor.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py` & `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/cdf_spline_derivative.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/quantile_pdf_constructors/dual_spline_average.py` & `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/dual_spline_average.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/quantile_pdf_constructors/piecewise_constant.py` & `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/quantile_pdf_constructors/piecewise_linear.py` & `qp-prob-0.8.1/src/qp/quantile_pdf_constructors/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/scipy_pdfs.py` & `qp-prob-0.8.1/src/qp/scipy_pdfs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/sparse_pdf.py` & `qp-prob-0.8.1/src/qp/sparse_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/sparse_rep.py` & `qp-prob-0.8.1/src/qp/sparse_rep.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/spline_pdf.py` & `qp-prob-0.8.1/src/qp/spline_pdf.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/test_data.py` & `qp-prob-0.8.1/src/qp/test_data.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/test_funcs.py` & `qp-prob-0.8.1/src/qp/test_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp/utils.py` & `qp-prob-0.8.1/src/qp/utils.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/src/qp_prob.egg-info/PKG-INFO` & `qp-prob-0.8.1/src/qp_prob.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qp-prob
-Version: 0.8.0
+Version: 0.8.1
 License: MIT License
         
         Copyright (c) 2016 Alex Malz & Phil Marshall
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,14 +26,16 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+Provides-Extra: full
+Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 # qp
 
 Quantile parametrization for probability distribution functions.
```

### Comparing `qp-prob-0.8.0/src/qp_prob.egg-info/SOURCES.txt` & `qp-prob-0.8.1/src/qp_prob.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/qp/_version.py
 src/qp/conversion_funcs.py
 src/qp/dict_utils.py
 src/qp/ensemble.py
 src/qp/factory.py
 src/qp/hist_pdf.py
 src/qp/interp_pdf.py
+src/qp/lazy_modules.py
 src/qp/mixmod_pdf.py
 src/qp/packed_interp_pdf.py
 src/qp/packing_utils.py
 src/qp/pdf_gen.py
 src/qp/plotting.py
 src/qp/quant_pdf.py
 src/qp/scipy_pdfs.py
```

### Comparing `qp-prob-0.8.0/tests/qp/.gitignore` & `qp-prob-0.8.1/tests/qp/.gitignore`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/benchmark.py` & `qp-prob-0.8.1/tests/qp/benchmark.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/fidelity.py` & `qp-prob-0.8.1/tests/qp/fidelity.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py` & `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_cdf_spline_derivative.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py` & `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_dual_spline_average.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py` & `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_constant.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py` & `qp-prob-0.8.1/tests/qp/quantile_pdf_constructors/test_piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_auto.py` & `qp-prob-0.8.1/tests/qp/test_auto.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_brier.py` & `qp-prob-0.8.1/tests/qp/test_brier.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_ensemble.py` & `qp-prob-0.8.1/tests/qp/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_eval_funcs.py` & `qp-prob-0.8.1/tests/qp/test_eval_funcs.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_flex_coefs.npy` & `qp-prob-0.8.1/tests/qp/test_flex_coefs.npy`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_infrastructure.py` & `qp-prob-0.8.1/tests/qp/test_infrastructure.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_metrics.py` & `qp-prob-0.8.1/tests/qp/test_metrics.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_parallel.py` & `qp-prob-0.8.1/tests/qp/test_parallel.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_pit.py` & `qp-prob-0.8.1/tests/qp/test_pit.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_scipy_vectorization.py` & `qp-prob-0.8.1/tests/qp/test_scipy_vectorization.py`

 * *Files identical despite different names*

### Comparing `qp-prob-0.8.0/tests/qp/test_utils.py` & `qp-prob-0.8.1/tests/qp/test_utils.py`

 * *Files identical despite different names*

