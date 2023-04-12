# Comparing `tmp/gwpy-3.0.3.tar.gz` & `tmp/gwpy-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwpy-3.0.3.tar", last modified: Sun Apr  9 14:51:14 2023, max compression
+gzip compressed data, was "gwpy-3.0.4.tar", last modified: Wed Apr 12 12:14:41 2023, max compression
```

## Comparing `gwpy-3.0.3.tar` & `gwpy-3.0.4.tar`

### file list

```diff
@@ -1,441 +1,441 @@
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2023-04-06 10:37:11.000000 gwpy-3.0.3/.codeclimate.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      498 2023-04-06 10:37:11.000000 gwpy-3.0.3/.codecov.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      483 2023-04-06 10:37:11.000000 gwpy-3.0.3/.flake8
--rw-r--r--   0 duncan    (1000) duncan    (1000)       30 2023-04-06 10:37:11.000000 gwpy-3.0.3/.gitattributes
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.974681 gwpy-3.0.3/.github/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/.github/workflows/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2023-04-09 14:36:48.000000 gwpy-3.0.3/.github/workflows/conda.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2920 2023-04-06 10:37:11.000000 gwpy-3.0.3/.github/workflows/dependencies.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3119 2023-04-06 10:37:11.000000 gwpy-3.0.3/.github/workflows/dist.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1415 2023-04-09 14:36:48.000000 gwpy-3.0.3/.github/workflows/lint.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      726 2023-04-06 10:37:11.000000 gwpy-3.0.3/.gitignore
--rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2023-04-06 10:37:11.000000 gwpy-3.0.3/.pep8speaks.yml
--rw-r--r--   0 duncan    (1000) duncan    (1000)      133 2023-04-06 10:37:11.000000 gwpy-3.0.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4481 2023-04-06 10:37:11.000000 gwpy-3.0.3/CONTRIBUTING.md
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2023-04-06 10:37:11.000000 gwpy-3.0.3/LICENSE
--rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2023-04-06 10:37:11.000000 gwpy-3.0.3/MANIFEST.in
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-09 14:51:14.064681 gwpy-3.0.3/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2023-04-06 10:37:11.000000 gwpy-3.0.3/README.md
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      788 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/Makefile
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_static/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_static/css/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_static/css/gwpy-sphinx.css
--rw-r--r--   0 duncan    (1000) duncan    (1000)    19634 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_static/favicon.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15166 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_static/gwpy_white_24.png
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.974681 gwpy-3.0.3/docs/_templates/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_templates/autoclass/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      860 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autoclass/class.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/_templates/autosummary/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      170 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autosummary/base.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1145 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      703 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/astro/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      735 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/astro/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2653 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/citing.rst.in
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/cli/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5295 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/cli/examples.ini
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2879 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/cli/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13301 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/conf.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/detector/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3245 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/detector/channel.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/dev/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3787 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/dev/release.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1624 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/env.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.974681 gwpy-3.0.3/docs/examples/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/examples/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/external/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/framecpp.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      990 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/framel.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3134 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/lalsuite.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1025 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/external/nds2.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    52297 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/gwpy-docs-logo.png
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2491 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1300 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/install.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2694 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/overview.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:13.994681 gwpy-3.0.3/docs/plot/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/colorbars.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2985 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/colors.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      772 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/filter.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2514 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/gps.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1838 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/legend.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1363 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/plot/log.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5072 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/references.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1513 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/dqsegdb.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6818 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6756 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2124 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/segments/thresholding.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4369 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/signal/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3771 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrogram/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/spectrum/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      505 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrum/filtering.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3732 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrum/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4986 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/spectrum/io.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/filter.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)      955 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/histogram.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1500 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    30445 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/table/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1756 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/plot.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2142 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/table/rate.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/time/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1085 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/time/index.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/docs/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11634 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/timeseries/datafind.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2722 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/timeseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10656 2023-04-09 14:36:48.000000 gwpy-3.0.3/docs/timeseries/io.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2744 2023-04-09 14:36:18.000000 gwpy-3.0.3/docs/timeseries/opendata.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3032 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/timeseries/plot.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8470 2023-04-06 10:37:11.000000 gwpy-3.0.3/docs/timeseries/statevector.rst
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/frequencyseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2584 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2065 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/hoff.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      258 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2585 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/inject.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/percentiles.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/rayleigh.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2203 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/transfer_function.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2630 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/frequencyseries/variance.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/miscellaneous/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      216 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3354 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/open-data-spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2366 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/range-spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/miscellaneous/range-timeseries.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      158 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/segments/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2411 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/segments/open-data.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.004681 gwpy-3.0.3/examples/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5642 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/signal/gw150914.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      179 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/signal/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3139 2023-04-09 14:36:48.000000 gwpy-3.0.3/examples/signal/qscan.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/examples/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2387 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2627 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2581 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/ratio.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2125 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/rayleigh.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2885 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/spectrogram/spectrogram2.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/examples/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1597 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/histogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      198 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2317 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/rate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2460 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/rate_binned.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2018 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/scatter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2287 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/table/tiles.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3734 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/test_examples.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/examples/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2644 2023-04-09 14:36:18.000000 gwpy-3.0.3/examples/timeseries/blrms.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4204 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/correlate.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2797 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/filter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/index.rst
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2641 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/inject.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2466 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/public.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3788 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/pycbc-snr.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/qscan.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2202 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/statevector.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2476 2023-04-06 10:37:11.000000 gwpy-3.0.3/examples/timeseries/whiten.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1533 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy/_version.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/astro/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1909 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/astro/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24880 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/astro/range.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/astro/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/astro/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6032 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/astro/tests/test_range.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/cli/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1404 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    34269 2023-04-09 14:36:18.000000 gwpy-3.0.3/gwpy/cli/cliproduct.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4048 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/coherencegram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5121 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/gwpy_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9140 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7131 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-04-09 14:36:18.000000 gwpy-3.0.3/gwpy/cli/spectrum.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy/cli/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      744 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10831 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/base.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1353 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_coherence.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1580 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_coherencegram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1718 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_gwpy_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2899 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1509 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_spectrogram.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1416 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_spectrum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1279 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1999 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/tests/test_transferfunction.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3891 2023-04-09 14:36:18.000000 gwpy-3.0.3/gwpy/cli/timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9784 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/cli/transferfunction.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1639 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/conftest.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/detector/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2252 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    26901 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/channel.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/detector/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1037 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3184 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/cis.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5689 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/clf.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5939 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/io/omega.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/detector/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    18473 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/detector/tests/test_channel.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2548 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/tests/test_units.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7113 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/detector/units.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/frequencyseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      995 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1943 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/_fdcommon.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14328 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/frequencyseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11947 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/hist.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/frequencyseries/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      907 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1071 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1036 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1149 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/io/ligolw.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/frequencyseries/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      756 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/frequencyseries/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11033 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/frequencyseries/tests/test_frequencyseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4005 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/frequencyseries/tests/test_hist.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      831 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4250 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/_framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14662 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/cache.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18462 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/datafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8399 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/ffldatafind.py
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18966 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5257 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6928 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    22182 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4116 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    19331 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3518 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/registry.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.024681 gwpy-3.0.3/gwpy/io/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      743 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8567 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_cache.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10606 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_datafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6277 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/tests/test_ffldatafind.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4228 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_kerberos.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10701 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3293 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12185 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3971 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/io/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7341 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/io/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/plot/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1641 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    23094 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/axes.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8733 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/bode.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7041 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/colorbar.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/colors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16720 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/gps.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1635 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/legend.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5030 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/log.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    21766 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4816 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/rc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    16943 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/plot/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      740 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11542 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/tests/test_axes.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3351 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_bode.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1881 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_colors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5456 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_gps.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2652 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_log.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4398 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_plot.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1252 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_rc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5442 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_segments.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2318 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/tests/test_tex.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_text.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1615 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/test_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1925 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/tests/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4783 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/plot/tex.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1989 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/text.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1383 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/units.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1670 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/plot/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/segments/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1194 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    52670 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/flag.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/segments/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1005 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11048 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3036 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/json.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4907 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5007 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/io/segwizard.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9042 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/segments/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    29683 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/segments/tests/test_flag.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5360 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/segments/tests/test_segments.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/signal/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      972 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1189 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/fft.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    20270 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/filter_design.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    24471 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/qtransform.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.034681 gwpy-3.0.3/gwpy/signal/spectral/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1818 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12000 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1851 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_median_mean.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3577 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2346 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_registry.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_scipy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14241 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1669 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/spectral/_utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/signal/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      747 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4349 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_filter_design.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4017 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_qtransform.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3543 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2195 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_median_mean.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2249 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1446 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_registry.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_scipy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3045 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_ui.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1453 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/signal/tests/test_spectral_utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2726 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/tests/test_window.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5927 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/signal/window.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/spectrogram/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      919 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5742 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/coherence.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/spectrogram/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      846 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)      963 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    22206 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/spectrogram.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/spectrogram/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      752 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/spectrogram/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6590 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/spectrogram/tests/test_spectrogram.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/table/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1418 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7918 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/filter.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2645 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/filters.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8173 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/gravityspy.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/table/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1564 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3809 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/cwb.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/fetch.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4663 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/gravityspy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8390 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/gstlal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5433 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/gwf.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/hacr.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13590 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4434 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2604 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/omega.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1333 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/omicron.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8894 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3318 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/root.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3857 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/snax.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3067 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/sql.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3183 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/io/utils.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    26330 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/table.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/table/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3392 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/table/tests/test_gravityspy.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7979 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/tests/test_io_gstlal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2848 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/table/tests/test_io_ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8313 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/table/tests/test_io_pycbc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    30399 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/table/tests/test_table.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.044681 gwpy-3.0.3/gwpy/testing/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/__init__.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/testing/data/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)   377295 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.gwf
--rw-r--r--   0 duncan    (1000) duncan    (1000)   382679 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.hdf
--rw-r--r--   0 duncan    (1000) duncan    (1000)       59 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      564 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2783 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/testing/errors.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3772 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/fixtures.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1480 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/marks.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4131 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/mocks.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    11726 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/testing/utils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/time/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1812 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2285 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/__main__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8975 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/time/_tconvert.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/time/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1362 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/time/tests/test_main.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5728 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/time/tests/test_time.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1134 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    57165 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/core.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      938 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1185 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/cache.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/core.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/io/gwf/
--rw-r--r--   0 duncan    (1000) duncan    (1000)    13156 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    17130 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4776 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/framel.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     6828 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/gwf/lalframe.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4214 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9345 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7811 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/nds2.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3595 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/io/wav.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    35787 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/statevector.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/timeseries/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      751 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    18215 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_core.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2265 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_framecpp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4969 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_lalframe.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1833 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_io_losc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12356 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_statevector.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    55164 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/tests/test_timeseries.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    87612 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/timeseries/timeseries.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/types/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1159 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    15282 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/array.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    12367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/array2d.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3074 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/index.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.054681 gwpy-3.0.3/gwpy/types/io/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      905 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2872 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/ascii.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8002 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/hdf5.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     7267 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/io/ligolw.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    36772 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/series.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3567 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/sliceutils.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/types/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8608 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/types/tests/test_array.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     9081 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/tests/test_array2d.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2044 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/tests/test_index.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)    14762 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/types/tests/test_series.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/utils/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      933 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3723 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/decorators.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1490 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/enum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1911 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     8507 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3284 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/misc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     5057 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     1367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/progress.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3396 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/shell.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/utils/sphinx/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      770 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3559 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/epydoc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4763 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/ex2rst.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3425 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/sphinx/zenodo.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.064681 gwpy-3.0.3/gwpy/utils/tests/
--rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/__init__.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2209 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_decorators.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2185 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_enum.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2000 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/test_env.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3478 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_lal.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2610 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_misc.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2062 2023-04-09 14:36:48.000000 gwpy-3.0.3/gwpy/utils/tests/test_mp.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2367 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/test_shell.py
--rw-r--r--   0 duncan    (1000) duncan    (1000)     2263 2023-04-06 10:37:11.000000 gwpy-3.0.3/gwpy/utils/tests/test_sphinx_ex2rst.py
-drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-09 14:51:14.014681 gwpy-3.0.3/gwpy.egg-info/
--rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/PKG-INFO
--rw-r--r--   0 duncan    (1000) duncan    (1000)    10040 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/SOURCES.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/dependency_links.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/entry_points.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)      793 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/requires.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)        5 2023-04-09 14:51:13.000000 gwpy-3.0.3/gwpy.egg-info/top_level.txt
--rw-r--r--   0 duncan    (1000) duncan    (1000)     4844 2023-04-09 14:36:48.000000 gwpy-3.0.3/pyproject.toml
--rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2023-04-09 14:51:14.064681 gwpy-3.0.3/setup.cfg
--rwxr-xr-x   0 duncan    (1000) duncan    (1000)     2989 2023-04-06 10:37:11.000000 gwpy-3.0.3/setup_utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      524 2023-04-06 10:37:11.000000 gwpy-3.0.4/.codeclimate.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      498 2023-04-06 10:37:11.000000 gwpy-3.0.4/.codecov.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      483 2023-04-06 10:37:11.000000 gwpy-3.0.4/.flake8
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       30 2023-04-06 10:37:11.000000 gwpy-3.0.4/.gitattributes
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.958642 gwpy-3.0.4/.github/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.978642 gwpy-3.0.4/.github/workflows/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5119 2023-04-12 09:57:39.000000 gwpy-3.0.4/.github/workflows/conda.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2920 2023-04-06 10:37:11.000000 gwpy-3.0.4/.github/workflows/dependencies.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3119 2023-04-06 10:37:11.000000 gwpy-3.0.4/.github/workflows/dist.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1415 2023-04-12 09:57:39.000000 gwpy-3.0.4/.github/workflows/lint.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      726 2023-04-06 10:37:11.000000 gwpy-3.0.4/.gitignore
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       44 2023-04-06 10:37:11.000000 gwpy-3.0.4/.pep8speaks.yml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      133 2023-04-06 10:37:11.000000 gwpy-3.0.4/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4481 2023-04-06 10:37:11.000000 gwpy-3.0.4/CONTRIBUTING.md
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35147 2023-04-06 10:37:11.000000 gwpy-3.0.4/LICENSE
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      176 2023-04-06 10:37:11.000000 gwpy-3.0.4/MANIFEST.in
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-12 12:14:41.108642 gwpy-3.0.4/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1800 2023-04-06 10:37:11.000000 gwpy-3.0.4/README.md
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      788 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/Makefile
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_static/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_static/css/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_static/css/gwpy-sphinx.css
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    19634 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_static/favicon.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15166 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_static/gwpy_white_24.png
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.958642 gwpy-3.0.4/docs/_templates/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_templates/autoclass/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      860 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autoclass/class.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/_templates/autosummary/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      170 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1145 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      703 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/astro/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      735 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/astro/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2653 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/citing.rst.in
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5295 2023-04-09 14:36:48.000000 gwpy-3.0.4/docs/cli/examples.ini
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2879 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/cli/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13301 2023-04-09 14:36:48.000000 gwpy-3.0.4/docs/conf.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/detector/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3245 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/detector/channel.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/dev/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3787 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/dev/release.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1624 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/env.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.958642 gwpy-3.0.4/docs/examples/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/examples/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.988642 gwpy-3.0.4/docs/external/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1162 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/framecpp.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      990 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/framel.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3134 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/lalsuite.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1025 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/external/nds2.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52297 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/gwpy-docs-logo.png
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2491 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1300 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/install.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2694 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/overview.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/plot/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2600 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/colorbars.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2985 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/colors.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      772 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/filter.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2514 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/gps.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3095 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1838 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/legend.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1363 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/plot/log.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5072 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/references.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1513 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/dqsegdb.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6818 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6756 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2124 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/segments/thresholding.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4369 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/signal/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3771 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrogram/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/spectrum/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      505 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrum/filtering.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3732 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrum/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4986 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/spectrum/io.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7364 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/filter.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      955 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/histogram.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1500 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30445 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/table/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1756 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/plot.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2142 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/table/rate.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/time/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1085 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/time/index.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/docs/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11634 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/timeseries/datafind.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2722 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/timeseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10656 2023-04-12 09:57:39.000000 gwpy-3.0.4/docs/timeseries/io.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2744 2023-04-12 12:10:00.000000 gwpy-3.0.4/docs/timeseries/opendata.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3032 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/timeseries/plot.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8470 2023-04-06 10:37:11.000000 gwpy-3.0.4/docs/timeseries/statevector.rst
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:40.998642 gwpy-3.0.4/examples/
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/frequencyseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2584 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2065 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/hoff.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      258 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2585 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/inject.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/percentiles.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2802 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/rayleigh.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2203 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/transfer_function.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2630 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/frequencyseries/variance.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/miscellaneous/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      216 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3354 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/open-data-spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2366 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/range-spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2490 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/miscellaneous/range-timeseries.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      158 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/segments/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2411 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/segments/open-data.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5642 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/signal/gw150914.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      179 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/signal/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3139 2023-04-09 14:36:48.000000 gwpy-3.0.4/examples/signal/qscan.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2387 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      209 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2627 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2581 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/ratio.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2125 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/rayleigh.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2885 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/spectrogram/spectrogram2.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1597 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/histogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      198 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2317 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/rate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2460 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/rate_binned.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2018 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/scatter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2287 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/table/tiles.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3734 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/test_examples.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/examples/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2644 2023-04-12 12:10:00.000000 gwpy-3.0.4/examples/timeseries/blrms.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4204 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/correlate.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2797 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/filter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      246 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/index.rst
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2641 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/inject.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2466 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/public.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3788 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/pycbc-snr.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/qscan.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2202 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/statevector.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2476 2023-04-06 10:37:11.000000 gwpy-3.0.4/examples/timeseries/whiten.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.008642 gwpy-3.0.4/gwpy/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1533 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      160 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy/_version.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/astro/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1909 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/astro/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24880 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/astro/range.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/astro/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/astro/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6032 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/astro/tests/test_range.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/cli/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1404 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    34269 2023-04-12 12:10:00.000000 gwpy-3.0.4/gwpy/cli/cliproduct.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4048 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3353 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/coherencegram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5121 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/gwpy_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9140 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7131 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4899 2023-04-12 12:10:00.000000 gwpy-3.0.4/gwpy/cli/spectrum.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy/cli/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      744 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10831 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/base.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1353 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_coherence.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1580 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_coherencegram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1718 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_gwpy_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2899 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1509 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_spectrogram.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1416 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_spectrum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1279 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1999 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/tests/test_transferfunction.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3891 2023-04-12 12:10:00.000000 gwpy-3.0.4/gwpy/cli/timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9784 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/cli/transferfunction.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1639 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/conftest.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/detector/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2252 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    26901 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/channel.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/detector/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1037 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3184 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/cis.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5689 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/clf.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     5939 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/io/omega.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/detector/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18473 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/detector/tests/test_channel.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2548 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/tests/test_units.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7113 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/detector/units.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/frequencyseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      995 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1943 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/_fdcommon.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14328 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/frequencyseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11947 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/hist.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/frequencyseries/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      907 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1071 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1036 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1149 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/io/ligolw.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.028642 gwpy-3.0.4/gwpy/frequencyseries/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      756 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/frequencyseries/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11033 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/frequencyseries/tests/test_frequencyseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4005 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/frequencyseries/tests/test_hist.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.038642 gwpy-3.0.4/gwpy/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      831 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4250 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/io/_framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14662 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/cache.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18462 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/datafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8399 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/ffldatafind.py
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)    18966 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/io/gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5257 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6928 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    22182 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4116 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    19331 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3518 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/registry.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.038642 gwpy-3.0.4/gwpy/io/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      743 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8567 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_cache.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10606 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_datafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6277 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/tests/test_ffldatafind.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4228 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_kerberos.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10701 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3293 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12185 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3971 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/io/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7341 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/io/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.048642 gwpy-3.0.4/gwpy/plot/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1641 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    23094 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/axes.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8733 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/bode.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7041 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/plot/colorbar.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/colors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16720 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/plot/gps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1635 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/legend.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5030 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/plot/log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    21766 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4816 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/rc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    16943 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.048642 gwpy-3.0.4/gwpy/plot/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      740 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11542 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/plot/tests/test_axes.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3351 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_bode.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1881 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_colors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5456 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_gps.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2652 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_log.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4398 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_plot.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1252 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_rc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5442 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_segments.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2318 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/plot/tests/test_tex.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1291 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_text.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1615 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/test_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1925 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/tests/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4783 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/plot/tex.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1989 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/text.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1383 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/units.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1670 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/plot/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.048642 gwpy-3.0.4/gwpy/segments/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1194 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    52670 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/flag.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/segments/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1005 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11048 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3036 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/json.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4907 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5007 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/io/segwizard.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9042 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/segments/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      749 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    29683 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/segments/tests/test_flag.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5360 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/segments/tests/test_segments.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/signal/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      972 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1189 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/fft.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    20270 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/filter_design.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    24471 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/qtransform.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/signal/spectral/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1818 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12000 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1851 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_median_mean.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3577 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2346 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_registry.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6492 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_scipy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14241 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1669 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/spectral/_utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.058642 gwpy-3.0.4/gwpy/signal/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      747 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4349 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_filter_design.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4017 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_qtransform.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3543 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2195 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_median_mean.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2249 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1446 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_registry.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1874 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_scipy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3045 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_ui.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1453 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/signal/tests/test_spectral_utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2726 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/tests/test_window.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5927 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/signal/window.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/spectrogram/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      919 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5742 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/coherence.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/spectrogram/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      846 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      963 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    22206 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/spectrogram.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/spectrogram/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      752 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/spectrogram/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6590 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/spectrogram/tests/test_spectrogram.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/table/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1418 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7918 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/filter.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2645 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/filters.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8173 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/gravityspy.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.068642 gwpy-3.0.4/gwpy/table/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1564 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3809 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/cwb.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/fetch.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4663 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/gravityspy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8390 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/gstlal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5433 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/gwf.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5205 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/hacr.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13590 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4434 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2604 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/omega.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1333 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/omicron.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8894 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3318 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/root.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3857 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/snax.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3067 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/sql.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3183 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/io/utils.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    26330 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/table.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.078642 gwpy-3.0.4/gwpy/table/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3392 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/table/tests/test_gravityspy.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7979 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/tests/test_io_gstlal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2848 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/table/tests/test_io_ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8313 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/table/tests/test_io_pycbc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    30399 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/table/tests/test_table.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.078642 gwpy-3.0.4/gwpy/testing/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/__init__.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/testing/data/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    58124 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   377295 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.gwf
+-rw-r--r--   0 duncan    (1000) duncan    (1000)   382679 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.hdf
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       59 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      564 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2783 2023-04-09 14:36:48.000000 gwpy-3.0.4/gwpy/testing/errors.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3772 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/fixtures.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1480 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/marks.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4131 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/mocks.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    11726 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/testing/utils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/time/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1812 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2285 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/__main__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8975 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/time/_tconvert.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/time/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      745 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1362 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/time/tests/test_main.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5728 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/time/tests/test_time.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.088642 gwpy-3.0.4/gwpy/timeseries/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1134 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    56990 2023-04-12 12:10:02.000000 gwpy-3.0.4/gwpy/timeseries/core.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/timeseries/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      938 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1185 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2602 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/cache.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4692 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/core.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/timeseries/io/gwf/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    13156 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    17130 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4776 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/framel.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     6828 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/gwf/lalframe.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4214 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9334 2023-04-12 12:10:02.000000 gwpy-3.0.4/gwpy/timeseries/io/losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7811 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/nds2.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3595 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/io/wav.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    35787 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/statevector.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/timeseries/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      751 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    18215 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_core.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2265 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_framecpp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4969 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_lalframe.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1833 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_io_losc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12356 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_statevector.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    55164 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/tests/test_timeseries.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    87612 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/timeseries/timeseries.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/types/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1159 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    15282 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/array.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    12367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/array2d.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3074 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/index.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.098642 gwpy-3.0.4/gwpy/types/io/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      905 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2872 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/ascii.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8002 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/hdf5.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     7267 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/io/ligolw.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    36772 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/series.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3567 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/sliceutils.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/types/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8608 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/types/tests/test_array.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     9081 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/tests/test_array2d.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2044 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/tests/test_index.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    14762 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/types/tests/test_series.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/utils/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      933 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3723 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/decorators.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1490 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/enum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1911 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     8507 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3284 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/misc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     5057 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     1367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/progress.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3396 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/shell.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/utils/sphinx/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      770 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3559 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/epydoc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4763 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/ex2rst.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3425 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/sphinx/zenodo.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.108642 gwpy-3.0.4/gwpy/utils/tests/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      746 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/__init__.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2209 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_decorators.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2185 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_enum.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2000 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/test_env.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3478 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_lal.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2610 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_misc.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2062 2023-04-12 09:57:39.000000 gwpy-3.0.4/gwpy/utils/tests/test_mp.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2367 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/test_shell.py
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     2263 2023-04-06 10:37:11.000000 gwpy-3.0.4/gwpy/utils/tests/test_sphinx_ex2rst.py
+drwxr-xr-x   0 duncan    (1000) duncan    (1000)        0 2023-04-12 12:14:41.018642 gwpy-3.0.4/gwpy.egg-info/
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     3146 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/PKG-INFO
+-rw-r--r--   0 duncan    (1000) duncan    (1000)    10040 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/SOURCES.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        1 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/dependency_links.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       54 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/entry_points.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)      793 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/requires.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)        5 2023-04-12 12:14:40.000000 gwpy-3.0.4/gwpy.egg-info/top_level.txt
+-rw-r--r--   0 duncan    (1000) duncan    (1000)     4844 2023-04-12 10:27:17.000000 gwpy-3.0.4/pyproject.toml
+-rw-r--r--   0 duncan    (1000) duncan    (1000)       38 2023-04-12 12:14:41.108642 gwpy-3.0.4/setup.cfg
+-rwxr-xr-x   0 duncan    (1000) duncan    (1000)     2989 2023-04-06 10:37:11.000000 gwpy-3.0.4/setup_utils.py
```

### Comparing `gwpy-3.0.3/.codeclimate.yml` & `gwpy-3.0.4/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/.github/workflows/conda.yml` & `gwpy-3.0.4/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/.github/workflows/dependencies.yml` & `gwpy-3.0.4/.github/workflows/dependencies.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/.github/workflows/dist.yml` & `gwpy-3.0.4/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/.github/workflows/lint.yml` & `gwpy-3.0.4/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/.gitignore` & `gwpy-3.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/CONTRIBUTING.md` & `gwpy-3.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/LICENSE` & `gwpy-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/PKG-INFO` & `gwpy-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpy
-Version: 3.0.3
+Version: 3.0.4
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwpy/issues
 Project-URL: Discussion Forum, https://gwpy.slack.com
 Project-URL: Documentation, https://gwpy.github.io/docs/
 Project-URL: Source Code, https://github.com/gwpy/gwpy
```

### Comparing `gwpy-3.0.3/README.md` & `gwpy-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/Makefile` & `gwpy-3.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/_static/css/gwpy-sphinx.css` & `gwpy-3.0.4/docs/_static/css/gwpy-sphinx.css`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/_static/favicon.png` & `gwpy-3.0.4/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/_static/gwpy_white_24.png` & `gwpy-3.0.4/docs/_static/gwpy_white_24.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/_templates/autoclass/class.rst` & `gwpy-3.0.4/docs/_templates/autoclass/class.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/_templates/autosummary/class.rst` & `gwpy-3.0.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/_templates/autosummary/module.rst` & `gwpy-3.0.4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/astro/index.rst` & `gwpy-3.0.4/docs/astro/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/citing.rst.in` & `gwpy-3.0.4/docs/citing.rst.in`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/cli/examples.ini` & `gwpy-3.0.4/docs/cli/examples.ini`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/cli/index.rst` & `gwpy-3.0.4/docs/cli/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/conf.py` & `gwpy-3.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/detector/channel.rst` & `gwpy-3.0.4/docs/detector/channel.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/dev/release.rst` & `gwpy-3.0.4/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/env.rst` & `gwpy-3.0.4/docs/env.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.4/docs/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/external/framecpp.rst` & `gwpy-3.0.4/docs/external/framecpp.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/external/framel.rst` & `gwpy-3.0.4/docs/external/framel.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/external/lalsuite.rst` & `gwpy-3.0.4/docs/external/lalsuite.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/external/nds2.rst` & `gwpy-3.0.4/docs/external/nds2.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/gwpy-docs-logo.png` & `gwpy-3.0.4/docs/gwpy-docs-logo.png`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/index.rst` & `gwpy-3.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/install.rst` & `gwpy-3.0.4/docs/install.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/overview.rst` & `gwpy-3.0.4/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/colorbars.rst` & `gwpy-3.0.4/docs/plot/colorbars.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/colors.rst` & `gwpy-3.0.4/docs/plot/colors.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/filter.rst` & `gwpy-3.0.4/docs/plot/filter.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/gps.rst` & `gwpy-3.0.4/docs/plot/gps.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/index.rst` & `gwpy-3.0.4/docs/plot/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/legend.rst` & `gwpy-3.0.4/docs/plot/legend.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/plot/log.rst` & `gwpy-3.0.4/docs/plot/log.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/references.rst` & `gwpy-3.0.4/docs/references.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/segments/dqsegdb.rst` & `gwpy-3.0.4/docs/segments/dqsegdb.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/segments/index.rst` & `gwpy-3.0.4/docs/segments/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/segments/io.rst` & `gwpy-3.0.4/docs/segments/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/segments/thresholding.rst` & `gwpy-3.0.4/docs/segments/thresholding.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/signal/index.rst` & `gwpy-3.0.4/docs/signal/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/spectrogram/index.rst` & `gwpy-3.0.4/docs/spectrogram/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/spectrum/index.rst` & `gwpy-3.0.4/docs/spectrum/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/spectrum/io.rst` & `gwpy-3.0.4/docs/spectrum/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.4/docs/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/filter.rst` & `gwpy-3.0.4/docs/table/filter.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/histogram.rst` & `gwpy-3.0.4/docs/table/histogram.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/index.rst` & `gwpy-3.0.4/docs/table/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/io.rst` & `gwpy-3.0.4/docs/table/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/plot.rst` & `gwpy-3.0.4/docs/table/plot.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/table/rate.rst` & `gwpy-3.0.4/docs/table/rate.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/time/index.rst` & `gwpy-3.0.4/docs/time/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/timeseries/datafind.rst` & `gwpy-3.0.4/docs/timeseries/datafind.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/timeseries/index.rst` & `gwpy-3.0.4/docs/timeseries/index.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/timeseries/io.rst` & `gwpy-3.0.4/docs/timeseries/io.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/timeseries/opendata.rst` & `gwpy-3.0.4/docs/timeseries/opendata.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/timeseries/plot.rst` & `gwpy-3.0.4/docs/timeseries/plot.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/docs/timeseries/statevector.rst` & `gwpy-3.0.4/docs/timeseries/statevector.rst`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/coherence.py` & `gwpy-3.0.4/examples/frequencyseries/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/hoff.py` & `gwpy-3.0.4/examples/frequencyseries/hoff.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/inject.py` & `gwpy-3.0.4/examples/frequencyseries/inject.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/percentiles.py` & `gwpy-3.0.4/examples/frequencyseries/percentiles.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/rayleigh.py` & `gwpy-3.0.4/examples/frequencyseries/rayleigh.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/transfer_function.py` & `gwpy-3.0.4/examples/frequencyseries/transfer_function.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/frequencyseries/variance.py` & `gwpy-3.0.4/examples/frequencyseries/variance.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/miscellaneous/open-data-spectrogram.py` & `gwpy-3.0.4/examples/miscellaneous/open-data-spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/miscellaneous/range-spectrogram.py` & `gwpy-3.0.4/examples/miscellaneous/range-spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/miscellaneous/range-timeseries.py` & `gwpy-3.0.4/examples/miscellaneous/range-timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/segments/open-data.py` & `gwpy-3.0.4/examples/segments/open-data.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/signal/gw150914.py` & `gwpy-3.0.4/examples/signal/gw150914.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/signal/qscan.py` & `gwpy-3.0.4/examples/signal/qscan.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/spectrogram/coherence.py` & `gwpy-3.0.4/examples/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/spectrogram/plot.py` & `gwpy-3.0.4/examples/spectrogram/plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/spectrogram/ratio.py` & `gwpy-3.0.4/examples/spectrogram/ratio.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/spectrogram/rayleigh.py` & `gwpy-3.0.4/examples/spectrogram/rayleigh.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/spectrogram/spectrogram2.py` & `gwpy-3.0.4/examples/spectrogram/spectrogram2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.4/examples/table/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/table/histogram.py` & `gwpy-3.0.4/examples/table/histogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/table/rate.py` & `gwpy-3.0.4/examples/table/rate.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/table/rate_binned.py` & `gwpy-3.0.4/examples/table/rate_binned.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/table/scatter.py` & `gwpy-3.0.4/examples/table/scatter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/table/tiles.py` & `gwpy-3.0.4/examples/table/tiles.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/test_examples.py` & `gwpy-3.0.4/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/blrms.py` & `gwpy-3.0.4/examples/timeseries/blrms.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/correlate.py` & `gwpy-3.0.4/examples/timeseries/correlate.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/filter.py` & `gwpy-3.0.4/examples/timeseries/filter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/inject.py` & `gwpy-3.0.4/examples/timeseries/inject.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/public.py` & `gwpy-3.0.4/examples/timeseries/public.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/pycbc-snr.py` & `gwpy-3.0.4/examples/timeseries/pycbc-snr.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/qscan.py` & `gwpy-3.0.4/examples/timeseries/qscan.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/statevector.py` & `gwpy-3.0.4/examples/timeseries/statevector.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/examples/timeseries/whiten.py` & `gwpy-3.0.4/examples/timeseries/whiten.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/__init__.py` & `gwpy-3.0.4/gwpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/astro/__init__.py` & `gwpy-3.0.4/gwpy/astro/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/astro/range.py` & `gwpy-3.0.4/gwpy/astro/range.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/astro/tests/__init__.py` & `gwpy-3.0.4/gwpy/astro/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/astro/tests/test_range.py` & `gwpy-3.0.4/gwpy/astro/tests/test_range.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/__init__.py` & `gwpy-3.0.4/gwpy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/cliproduct.py` & `gwpy-3.0.4/gwpy/cli/cliproduct.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/coherence.py` & `gwpy-3.0.4/gwpy/cli/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/coherencegram.py` & `gwpy-3.0.4/gwpy/cli/coherencegram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/gwpy_plot.py` & `gwpy-3.0.4/gwpy/cli/gwpy_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/qtransform.py` & `gwpy-3.0.4/gwpy/cli/qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/spectrogram.py` & `gwpy-3.0.4/gwpy/cli/spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/spectrum.py` & `gwpy-3.0.4/gwpy/cli/spectrum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/__init__.py` & `gwpy-3.0.4/gwpy/cli/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/base.py` & `gwpy-3.0.4/gwpy/cli/tests/base.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_coherence.py` & `gwpy-3.0.4/gwpy/cli/tests/test_coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_coherencegram.py` & `gwpy-3.0.4/gwpy/cli/tests/test_coherencegram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_gwpy_plot.py` & `gwpy-3.0.4/gwpy/cli/tests/test_gwpy_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_qtransform.py` & `gwpy-3.0.4/gwpy/cli/tests/test_qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_spectrogram.py` & `gwpy-3.0.4/gwpy/cli/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_spectrum.py` & `gwpy-3.0.4/gwpy/cli/tests/test_spectrum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_timeseries.py` & `gwpy-3.0.4/gwpy/cli/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/tests/test_transferfunction.py` & `gwpy-3.0.4/gwpy/cli/tests/test_transferfunction.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/timeseries.py` & `gwpy-3.0.4/gwpy/cli/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/cli/transferfunction.py` & `gwpy-3.0.4/gwpy/cli/transferfunction.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/conftest.py` & `gwpy-3.0.4/gwpy/conftest.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/__init__.py` & `gwpy-3.0.4/gwpy/detector/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/channel.py` & `gwpy-3.0.4/gwpy/detector/channel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/io/__init__.py` & `gwpy-3.0.4/gwpy/detector/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/io/cis.py` & `gwpy-3.0.4/gwpy/detector/io/cis.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/io/clf.py` & `gwpy-3.0.4/gwpy/detector/io/clf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/io/omega.py` & `gwpy-3.0.4/gwpy/detector/io/omega.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/tests/__init__.py` & `gwpy-3.0.4/gwpy/detector/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/tests/test_channel.py` & `gwpy-3.0.4/gwpy/detector/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/tests/test_units.py` & `gwpy-3.0.4/gwpy/detector/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/detector/units.py` & `gwpy-3.0.4/gwpy/detector/units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/__init__.py` & `gwpy-3.0.4/gwpy/frequencyseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/_fdcommon.py` & `gwpy-3.0.4/gwpy/frequencyseries/_fdcommon.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/frequencyseries.py` & `gwpy-3.0.4/gwpy/frequencyseries/frequencyseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/hist.py` & `gwpy-3.0.4/gwpy/frequencyseries/hist.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/io/__init__.py` & `gwpy-3.0.4/gwpy/frequencyseries/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/io/ascii.py` & `gwpy-3.0.4/gwpy/frequencyseries/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/io/hdf5.py` & `gwpy-3.0.4/gwpy/frequencyseries/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/io/ligolw.py` & `gwpy-3.0.4/gwpy/frequencyseries/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/tests/__init__.py` & `gwpy-3.0.4/gwpy/frequencyseries/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/tests/test_frequencyseries.py` & `gwpy-3.0.4/gwpy/frequencyseries/tests/test_frequencyseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/frequencyseries/tests/test_hist.py` & `gwpy-3.0.4/gwpy/frequencyseries/tests/test_hist.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/__init__.py` & `gwpy-3.0.4/gwpy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/_framecpp.py` & `gwpy-3.0.4/gwpy/io/_framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/cache.py` & `gwpy-3.0.4/gwpy/io/cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/datafind.py` & `gwpy-3.0.4/gwpy/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/ffldatafind.py` & `gwpy-3.0.4/gwpy/io/ffldatafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/gwf.py` & `gwpy-3.0.4/gwpy/io/gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/hdf5.py` & `gwpy-3.0.4/gwpy/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/kerberos.py` & `gwpy-3.0.4/gwpy/io/kerberos.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/ligolw.py` & `gwpy-3.0.4/gwpy/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/mp.py` & `gwpy-3.0.4/gwpy/io/mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/nds2.py` & `gwpy-3.0.4/gwpy/io/nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/registry.py` & `gwpy-3.0.4/gwpy/io/registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/__init__.py` & `gwpy-3.0.4/gwpy/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_cache.py` & `gwpy-3.0.4/gwpy/io/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_datafind.py` & `gwpy-3.0.4/gwpy/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_ffldatafind.py` & `gwpy-3.0.4/gwpy/io/tests/test_ffldatafind.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_gwf.py` & `gwpy-3.0.4/gwpy/io/tests/test_gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_kerberos.py` & `gwpy-3.0.4/gwpy/io/tests/test_kerberos.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_ligolw.py` & `gwpy-3.0.4/gwpy/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_mp.py` & `gwpy-3.0.4/gwpy/io/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_nds2.py` & `gwpy-3.0.4/gwpy/io/tests/test_nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/tests/test_utils.py` & `gwpy-3.0.4/gwpy/io/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/io/utils.py` & `gwpy-3.0.4/gwpy/io/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/__init__.py` & `gwpy-3.0.4/gwpy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/axes.py` & `gwpy-3.0.4/gwpy/plot/axes.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/bode.py` & `gwpy-3.0.4/gwpy/plot/bode.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/colorbar.py` & `gwpy-3.0.4/gwpy/plot/colorbar.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/colors.py` & `gwpy-3.0.4/gwpy/plot/colors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/gps.py` & `gwpy-3.0.4/gwpy/plot/gps.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/legend.py` & `gwpy-3.0.4/gwpy/plot/legend.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/log.py` & `gwpy-3.0.4/gwpy/plot/log.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/plot.py` & `gwpy-3.0.4/gwpy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/rc.py` & `gwpy-3.0.4/gwpy/plot/rc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/segments.py` & `gwpy-3.0.4/gwpy/plot/segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/__init__.py` & `gwpy-3.0.4/gwpy/plot/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_axes.py` & `gwpy-3.0.4/gwpy/plot/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_bode.py` & `gwpy-3.0.4/gwpy/plot/tests/test_bode.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_colors.py` & `gwpy-3.0.4/gwpy/plot/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_gps.py` & `gwpy-3.0.4/gwpy/plot/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_log.py` & `gwpy-3.0.4/gwpy/plot/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_plot.py` & `gwpy-3.0.4/gwpy/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_rc.py` & `gwpy-3.0.4/gwpy/plot/tests/test_rc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_segments.py` & `gwpy-3.0.4/gwpy/plot/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_tex.py` & `gwpy-3.0.4/gwpy/plot/tests/test_tex.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_text.py` & `gwpy-3.0.4/gwpy/plot/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/test_utils.py` & `gwpy-3.0.4/gwpy/plot/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tests/utils.py` & `gwpy-3.0.4/gwpy/plot/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/tex.py` & `gwpy-3.0.4/gwpy/plot/tex.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/text.py` & `gwpy-3.0.4/gwpy/plot/text.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/units.py` & `gwpy-3.0.4/gwpy/plot/units.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/plot/utils.py` & `gwpy-3.0.4/gwpy/plot/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/__init__.py` & `gwpy-3.0.4/gwpy/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/flag.py` & `gwpy-3.0.4/gwpy/segments/flag.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/io/__init__.py` & `gwpy-3.0.4/gwpy/segments/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/io/hdf5.py` & `gwpy-3.0.4/gwpy/segments/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/io/json.py` & `gwpy-3.0.4/gwpy/segments/io/json.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/io/ligolw.py` & `gwpy-3.0.4/gwpy/segments/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/io/segwizard.py` & `gwpy-3.0.4/gwpy/segments/io/segwizard.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/segments.py` & `gwpy-3.0.4/gwpy/segments/segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/tests/__init__.py` & `gwpy-3.0.4/gwpy/segments/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/tests/test_flag.py` & `gwpy-3.0.4/gwpy/segments/tests/test_flag.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/segments/tests/test_segments.py` & `gwpy-3.0.4/gwpy/segments/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/__init__.py` & `gwpy-3.0.4/gwpy/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/fft.py` & `gwpy-3.0.4/gwpy/signal/fft.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/filter_design.py` & `gwpy-3.0.4/gwpy/signal/filter_design.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/qtransform.py` & `gwpy-3.0.4/gwpy/signal/qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/__init__.py` & `gwpy-3.0.4/gwpy/signal/spectral/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_lal.py` & `gwpy-3.0.4/gwpy/signal/spectral/_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_median_mean.py` & `gwpy-3.0.4/gwpy/signal/spectral/_median_mean.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_pycbc.py` & `gwpy-3.0.4/gwpy/signal/spectral/_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_registry.py` & `gwpy-3.0.4/gwpy/signal/spectral/_registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_scipy.py` & `gwpy-3.0.4/gwpy/signal/spectral/_scipy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_ui.py` & `gwpy-3.0.4/gwpy/signal/spectral/_ui.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/spectral/_utils.py` & `gwpy-3.0.4/gwpy/signal/spectral/_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/__init__.py` & `gwpy-3.0.4/gwpy/signal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_filter_design.py` & `gwpy-3.0.4/gwpy/signal/tests/test_filter_design.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_qtransform.py` & `gwpy-3.0.4/gwpy/signal/tests/test_qtransform.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_lal.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_median_mean.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_median_mean.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_pycbc.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_registry.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_registry.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_scipy.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_scipy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_ui.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_ui.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_spectral_utils.py` & `gwpy-3.0.4/gwpy/signal/tests/test_spectral_utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/tests/test_window.py` & `gwpy-3.0.4/gwpy/signal/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/signal/window.py` & `gwpy-3.0.4/gwpy/signal/window.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/__init__.py` & `gwpy-3.0.4/gwpy/spectrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/coherence.py` & `gwpy-3.0.4/gwpy/spectrogram/coherence.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/io/__init__.py` & `gwpy-3.0.4/gwpy/spectrogram/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/io/hdf5.py` & `gwpy-3.0.4/gwpy/spectrogram/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/spectrogram.py` & `gwpy-3.0.4/gwpy/spectrogram/spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/tests/__init__.py` & `gwpy-3.0.4/gwpy/spectrogram/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/spectrogram/tests/test_spectrogram.py` & `gwpy-3.0.4/gwpy/spectrogram/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/__init__.py` & `gwpy-3.0.4/gwpy/table/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/filter.py` & `gwpy-3.0.4/gwpy/table/filter.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/filters.py` & `gwpy-3.0.4/gwpy/table/filters.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/gravityspy.py` & `gwpy-3.0.4/gwpy/table/gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/__init__.py` & `gwpy-3.0.4/gwpy/table/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/cwb.py` & `gwpy-3.0.4/gwpy/table/io/cwb.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/fetch.py` & `gwpy-3.0.4/gwpy/table/io/fetch.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/gravityspy.py` & `gwpy-3.0.4/gwpy/table/io/gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/gstlal.py` & `gwpy-3.0.4/gwpy/table/io/gstlal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/gwf.py` & `gwpy-3.0.4/gwpy/table/io/gwf.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/hacr.py` & `gwpy-3.0.4/gwpy/table/io/hacr.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/ligolw.py` & `gwpy-3.0.4/gwpy/table/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/losc.py` & `gwpy-3.0.4/gwpy/table/io/losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/omega.py` & `gwpy-3.0.4/gwpy/table/io/omega.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/omicron.py` & `gwpy-3.0.4/gwpy/table/io/omicron.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/pycbc.py` & `gwpy-3.0.4/gwpy/table/io/pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/root.py` & `gwpy-3.0.4/gwpy/table/io/root.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/snax.py` & `gwpy-3.0.4/gwpy/table/io/snax.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/sql.py` & `gwpy-3.0.4/gwpy/table/io/sql.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/io/utils.py` & `gwpy-3.0.4/gwpy/table/io/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/table.py` & `gwpy-3.0.4/gwpy/table/table.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/tests/__init__.py` & `gwpy-3.0.4/gwpy/table/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/tests/test_gravityspy.py` & `gwpy-3.0.4/gwpy/table/tests/test_gravityspy.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/tests/test_io_gstlal.py` & `gwpy-3.0.4/gwpy/table/tests/test_io_gstlal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/tests/test_io_ligolw.py` & `gwpy-3.0.4/gwpy/table/tests/test_io_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/tests/test_io_pycbc.py` & `gwpy-3.0.4/gwpy/table/tests/test_io_pycbc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/table/tests/test_table.py` & `gwpy-3.0.4/gwpy/table/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/__init__.py` & `gwpy-3.0.4/gwpy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz` & `gwpy-3.0.4/gwpy/testing/data/H1-LDAS_STRAIN-968654552-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.gwf` & `gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.gwf`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/data/HLV-HW100916-968654552-1.hdf` & `gwpy-3.0.4/gwpy/testing/data/HLV-HW100916-968654552-1.hdf`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz` & `gwpy-3.0.4/gwpy/testing/data/X1-GWPY_TEST_SEGMENTS-0-10.xml.gz`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/errors.py` & `gwpy-3.0.4/gwpy/testing/errors.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/fixtures.py` & `gwpy-3.0.4/gwpy/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/marks.py` & `gwpy-3.0.4/gwpy/testing/marks.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/mocks.py` & `gwpy-3.0.4/gwpy/testing/mocks.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/testing/utils.py` & `gwpy-3.0.4/gwpy/testing/utils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/time/__init__.py` & `gwpy-3.0.4/gwpy/time/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/time/__main__.py` & `gwpy-3.0.4/gwpy/time/__main__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/time/_tconvert.py` & `gwpy-3.0.4/gwpy/time/_tconvert.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/time/tests/__init__.py` & `gwpy-3.0.4/gwpy/time/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/time/tests/test_main.py` & `gwpy-3.0.4/gwpy/time/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/time/tests/test_time.py` & `gwpy-3.0.4/gwpy/time/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/__init__.py` & `gwpy-3.0.4/gwpy/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/core.py` & `gwpy-3.0.4/gwpy/timeseries/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,17 +376,17 @@
         return cls.DictClass.fetch(
             [channel], start, end, host=host, port=port, verbose=verbose,
             connection=connection, verify=verify, pad=pad, scaled=scaled,
             allow_tape=allow_tape, type=type, dtype=dtype)[str(channel)]
 
     @classmethod
     def fetch_open_data(cls, ifo, start, end, sample_rate=4096,
-                        tag=None, version=None,
-                        format='hdf5', host=GWOSC_DEFAULT_HOST,
-                        verbose=False, cache=None, **kwargs):
+                        version=None, format='hdf5',
+                        host=GWOSC_DEFAULT_HOST, verbose=False,
+                        cache=None, **kwargs):
         """Fetch open-access data from the LIGO Open Science Center
 
         Parameters
         ----------
         ifo : `str`
             the two-character prefix of the IFO in which you are interested,
             e.g. `'L1'`
@@ -400,18 +400,14 @@
             any input parseable by `~gwpy.time.to_gps` is fine
 
         sample_rate : `float`, optional,
             the sample rate of desired data; most data are stored
             by GWOSC at 4096 Hz, however there may be event-related
             data releases with a 16384 Hz rate, default: `4096`
 
-        tag : `str`, optional
-            file tag, e.g. ``'CLN'`` to select cleaned data, or ``'C00'``
-            for 'raw' calibrated data.
-
         version : `int`, optional
             version of files to download, defaults to highest discovered
             version
 
         format : `str`, optional
             the data format to download and parse, default: ``'h5py'``
 
@@ -474,15 +470,14 @@
         """
         from .io.losc import fetch_gwosc_data
         return fetch_gwosc_data(
             ifo,
             start,
             end,
             sample_rate=sample_rate,
-            tag=tag,
             version=version,
             format=format,
             verbose=verbose,
             cache=cache,
             host=host,
             cls=cls,
             **kwargs,
```

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/__init__.py` & `gwpy-3.0.4/gwpy/timeseries/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/ascii.py` & `gwpy-3.0.4/gwpy/timeseries/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/cache.py` & `gwpy-3.0.4/gwpy/timeseries/io/cache.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/core.py` & `gwpy-3.0.4/gwpy/timeseries/io/core.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/gwf/__init__.py` & `gwpy-3.0.4/gwpy/timeseries/io/gwf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/gwf/framecpp.py` & `gwpy-3.0.4/gwpy/timeseries/io/gwf/framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/gwf/framel.py` & `gwpy-3.0.4/gwpy/timeseries/io/gwf/framel.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/gwf/lalframe.py` & `gwpy-3.0.4/gwpy/timeseries/io/gwf/lalframe.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/hdf5.py` & `gwpy-3.0.4/gwpy/timeseries/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/losc.py` & `gwpy-3.0.4/gwpy/timeseries/io/losc.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 from ...utils.env import bool_env
 
 DQMASK_CHANNEL_REGEX = re.compile(r"\A[A-Z]\d:(GW|L)OSC-.*DQMASK\Z")
 STRAIN_CHANNEL_REGEX = re.compile(r"\A[A-Z]\d:(GW|L)OSC-.*STRAIN\Z")
 
 GWOSC_LOCATE_KWARGS = (
     'sample_rate',
-    'tag',
     'version',
     'host',
     'format',
     'dataset',
 )
```

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/nds2.py` & `gwpy-3.0.4/gwpy/timeseries/io/nds2.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/io/wav.py` & `gwpy-3.0.4/gwpy/timeseries/io/wav.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/statevector.py` & `gwpy-3.0.4/gwpy/timeseries/statevector.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/__init__.py` & `gwpy-3.0.4/gwpy/timeseries/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/test_core.py` & `gwpy-3.0.4/gwpy/timeseries/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_framecpp.py` & `gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_framecpp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/test_io_gwf_lalframe.py` & `gwpy-3.0.4/gwpy/timeseries/tests/test_io_gwf_lalframe.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/test_io_losc.py` & `gwpy-3.0.4/gwpy/timeseries/tests/test_io_losc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/test_statevector.py` & `gwpy-3.0.4/gwpy/timeseries/tests/test_statevector.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/tests/test_timeseries.py` & `gwpy-3.0.4/gwpy/timeseries/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/timeseries/timeseries.py` & `gwpy-3.0.4/gwpy/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/__init__.py` & `gwpy-3.0.4/gwpy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/array.py` & `gwpy-3.0.4/gwpy/types/array.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/array2d.py` & `gwpy-3.0.4/gwpy/types/array2d.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/index.py` & `gwpy-3.0.4/gwpy/types/index.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/io/__init__.py` & `gwpy-3.0.4/gwpy/types/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/io/ascii.py` & `gwpy-3.0.4/gwpy/types/io/ascii.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/io/hdf5.py` & `gwpy-3.0.4/gwpy/types/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/io/ligolw.py` & `gwpy-3.0.4/gwpy/types/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/series.py` & `gwpy-3.0.4/gwpy/types/series.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/sliceutils.py` & `gwpy-3.0.4/gwpy/types/sliceutils.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/tests/__init__.py` & `gwpy-3.0.4/gwpy/types/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/tests/test_array.py` & `gwpy-3.0.4/gwpy/types/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/tests/test_array2d.py` & `gwpy-3.0.4/gwpy/types/tests/test_array2d.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/tests/test_index.py` & `gwpy-3.0.4/gwpy/types/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/types/tests/test_series.py` & `gwpy-3.0.4/gwpy/types/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/__init__.py` & `gwpy-3.0.4/gwpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/decorators.py` & `gwpy-3.0.4/gwpy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/enum.py` & `gwpy-3.0.4/gwpy/utils/enum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/env.py` & `gwpy-3.0.4/gwpy/utils/env.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/lal.py` & `gwpy-3.0.4/gwpy/utils/lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/misc.py` & `gwpy-3.0.4/gwpy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/mp.py` & `gwpy-3.0.4/gwpy/utils/mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/progress.py` & `gwpy-3.0.4/gwpy/utils/progress.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/shell.py` & `gwpy-3.0.4/gwpy/utils/shell.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/sphinx/__init__.py` & `gwpy-3.0.4/gwpy/utils/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/sphinx/epydoc.py` & `gwpy-3.0.4/gwpy/utils/sphinx/epydoc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/sphinx/ex2rst.py` & `gwpy-3.0.4/gwpy/utils/sphinx/ex2rst.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/sphinx/zenodo.py` & `gwpy-3.0.4/gwpy/utils/sphinx/zenodo.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/__init__.py` & `gwpy-3.0.4/gwpy/utils/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_decorators.py` & `gwpy-3.0.4/gwpy/utils/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_enum.py` & `gwpy-3.0.4/gwpy/utils/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_env.py` & `gwpy-3.0.4/gwpy/utils/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_lal.py` & `gwpy-3.0.4/gwpy/utils/tests/test_lal.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_misc.py` & `gwpy-3.0.4/gwpy/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_mp.py` & `gwpy-3.0.4/gwpy/utils/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_shell.py` & `gwpy-3.0.4/gwpy/utils/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy/utils/tests/test_sphinx_ex2rst.py` & `gwpy-3.0.4/gwpy/utils/tests/test_sphinx_ex2rst.py`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy.egg-info/PKG-INFO` & `gwpy-3.0.4/gwpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwpy
-Version: 3.0.3
+Version: 3.0.4
 Summary: A python package for gravitational-wave astrophysics
 Author-email: Duncan Macleod <duncan.macleod@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwpy/gwpy/issues
 Project-URL: Discussion Forum, https://gwpy.slack.com
 Project-URL: Documentation, https://gwpy.github.io/docs/
 Project-URL: Source Code, https://github.com/gwpy/gwpy
```

### Comparing `gwpy-3.0.3/gwpy.egg-info/SOURCES.txt` & `gwpy-3.0.4/gwpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/gwpy.egg-info/requires.txt` & `gwpy-3.0.4/gwpy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/pyproject.toml` & `gwpy-3.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwpy-3.0.3/setup_utils.py` & `gwpy-3.0.4/setup_utils.py`

 * *Files identical despite different names*

