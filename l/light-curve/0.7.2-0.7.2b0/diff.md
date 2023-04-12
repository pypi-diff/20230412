# Comparing `tmp/light_curve-0.7.2.tar.gz` & `tmp/light_curve-0.7.2b0.tar.gz`

## Comparing `light_curve-0.7.2.tar` & `light_curve-0.7.2b0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1675 1970-01-01 00:00:00.000000 light_curve-0.7.2/Cargo.toml
--rw-r--r--   0     1001      122       91 2023-04-12 14:50:44.000000 light_curve-0.7.2/.gitignore
--rw-r--r--   0     1001      122    75073 2023-04-12 14:50:44.000000 light_curve-0.7.2/.readme/benchplot.png
--rw-r--r--   0     1001      122    21785 2023-04-12 14:50:44.000000 light_curve-0.7.2/README.md
--rw-r--r--   0     1001      122        7 2023-04-12 14:50:44.000000 light_curve-0.7.2/docs/.gitignore
--rw-r--r--   0     1001      122      634 2023-04-12 14:50:44.000000 light_curve-0.7.2/docs/Makefile
--rw-r--r--   0     1001      122     2028 2023-04-12 14:50:44.000000 light_curve-0.7.2/docs/conf.py
--rw-r--r--   0     1001      122      697 2023-04-12 14:50:44.000000 light_curve-0.7.2/docs/index.rst
--rw-r--r--   0     1001      122      795 2023-04-12 14:50:44.000000 light_curve-0.7.2/docs/make.bat
--rw-r--r--   0     1001      122       14 2023-04-12 14:50:44.000000 light_curve-0.7.2/docs/requirements.txt
--rw-r--r--   0     1001      122      271 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/__init__.py
--rw-r--r--   0     1001      122      288 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_ext.py
--rw-r--r--   0     1001      122     1011 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/__init__.py
--rw-r--r--   0     1001      122        0 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/__init__.py
--rw-r--r--   0     1001      122     2482 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/_base.py
--rw-r--r--   0     1001      122     1136 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/_base_meta.py
--rw-r--r--   0     1001      122      303 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/_lstsq.py
--rw-r--r--   0     1001      122      321 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/adnormal.py
--rw-r--r--   0     1001      122      232 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/amplitude.py
--rw-r--r--   0     1001      122      409 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/beyondnstd.py
--rw-r--r--   0     1001      122     1309 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/bins.py
--rw-r--r--   0     1001      122      365 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/cusum.py
--rw-r--r--   0     1001      122      329 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/eta.py
--rw-r--r--   0     1001      122      382 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/etae.py
--rw-r--r--   0     1001      122      365 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/excvar.py
--rw-r--r--   0     1001      122     1081 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/extractor.py
--rw-r--r--   0     1001      122     1998 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py
--rw-r--r--   0     1001      122      414 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/intpercrange.py
--rw-r--r--   0     1001      122      476 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/kurtosis.py
--rw-r--r--   0     1001      122      618 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/linfit.py
--rw-r--r--   0     1001      122      455 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/lintrend.py
--rw-r--r--   0     1001      122     2099 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py
--rw-r--r--   0     1001      122      531 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/magnpratio.py
--rw-r--r--   0     1001      122      371 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/maxslope.py
--rw-r--r--   0     1001      122      217 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/mean.py
--rw-r--r--   0     1001      122      253 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/meanvar.py
--rw-r--r--   0     1001      122      282 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/medabsdev.py
--rw-r--r--   0     1001      122      435 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/medbufrperc.py
--rw-r--r--   0     1001      122      223 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/median.py
--rw-r--r--   0     1001      122     2641 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/otsusplit.py
--rw-r--r--   0     1001      122      506 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/pdiffmperc.py
--rw-r--r--   0     1001      122      309 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/percampl.py
--rw-r--r--   0     1001      122      377 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/redchi2.py
--rw-r--r--   0     1001      122      236 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/skew.py
--rw-r--r--   0     1001      122      250 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/stdev.py
--rw-r--r--   0     1001      122      419 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/stetsonk.py
--rw-r--r--   0     1001      122      265 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/features/weightmean.py
--rw-r--r--   0     1001      122      596 2023-04-12 14:50:44.000000 light_curve-0.7.2/light_curve/light_curve_py/warnings.py
--rw-r--r--   0     1001      122     6305 2023-04-12 14:50:44.000000 light_curve-0.7.2/pyproject.toml
--rw-r--r--   0     1001      122     1395 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/check.rs
--rw-r--r--   0     1001      122     2245 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/cont_array.rs
--rw-r--r--   0     1001      122    50948 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/dmdt.rs
--rw-r--r--   0     1001      122     1504 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/errors.rs
--rw-r--r--   0     1001      122    63506 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/features.rs
--rw-r--r--   0     1001      122     3528 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/lib.rs
--rw-r--r--   0     1001      122     4269 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/ln_prior.rs
--rw-r--r--   0     1001      122     3600 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/np_array.rs
--rw-r--r--   0     1001      122     4450 2023-04-12 14:50:44.000000 light_curve-0.7.2/src/transform.rs
--rw-r--r--   0     1001      122        0 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/__init__.py
--rw-r--r--   0     1001      122        0 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_ext/__init__.py
--rw-r--r--   0     1001      122    12272 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_ext/test_dmdt.py
--rw-r--r--   0     1001      122     9675 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_ext/test_feature.py
--rw-r--r--   0     1001      122      786 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_ext/test_ln_prior.py
--rw-r--r--   0     1001      122        0 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/__init__.py
--rw-r--r--   0     1001      122      304 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_adnormal.py
--rw-r--r--   0     1001      122      289 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_amplitude.py
--rw-r--r--   0     1001      122      516 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_beyondnstd.py
--rw-r--r--   0     1001      122     2058 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_bins.py
--rw-r--r--   0     1001      122      964 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_call.py
--rw-r--r--   0     1001      122      302 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_cusum.py
--rw-r--r--   0     1001      122      311 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_eta.py
--rw-r--r--   0     1001      122      562 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_etae.py
--rw-r--r--   0     1001      122      359 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_excvar.py
--rw-r--r--   0     1001      122     1905 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_extractor.py
--rw-r--r--   0     1001      122      478 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_intpercrange.py
--rw-r--r--   0     1001      122      497 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_kurtosis.py
--rw-r--r--   0     1001      122      702 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_linfit.py
--rw-r--r--   0     1001      122      939 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_lintrend.py
--rw-r--r--   0     1001      122      608 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_magnpratio.py
--rw-r--r--   0     1001      122      297 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_maxslope.py
--rw-r--r--   0     1001      122      450 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_mean.py
--rw-r--r--   0     1001      122      326 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_meanvar.py
--rw-r--r--   0     1001      122      335 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_medabsdev.py
--rw-r--r--   0     1001      122      317 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_medbufrperc.py
--rw-r--r--   0     1001      122      509 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_median.py
--rw-r--r--   0     1001      122     1579 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_n_not_det_before_fd.py
--rw-r--r--   0     1001      122     1307 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_otsusplit.py
--rw-r--r--   0     1001      122      336 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_pdiffmperc.py
--rw-r--r--   0     1001      122      321 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_percampl.py
--rw-r--r--   0     1001      122      650 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_redchi2.py
--rw-r--r--   0     1001      122      302 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_skew.py
--rw-r--r--   0     1001      122      348 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_stdev.py
--rw-r--r--   0     1001      122      673 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_stetsonk.py
--rw-r--r--   0     1001      122      351 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/light_curve_py/test_weightmean.py
--rw-r--r--   0     1001      122    23632 2023-04-12 14:50:44.000000 light_curve-0.7.2/tests/test_w_bench.py
--rw-r--r--   0     1001      122    48843 2023-04-12 14:50:44.000000 light_curve-0.7.2/Cargo.lock
--rw-r--r--   0        0        0    23563 1970-01-01 00:00:00.000000 light_curve-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 light_curve-0.7.2b0/Cargo.toml
+-rw-r--r--   0     1001      122       91 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/.gitignore
+-rw-r--r--   0     1001      122    75073 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/.readme/benchplot.png
+-rw-r--r--   0     1001      122    21785 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/README.md
+-rw-r--r--   0     1001      122        7 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/.gitignore
+-rw-r--r--   0     1001      122      634 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/Makefile
+-rw-r--r--   0     1001      122     2028 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/conf.py
+-rw-r--r--   0     1001      122      697 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/index.rst
+-rw-r--r--   0     1001      122      795 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/make.bat
+-rw-r--r--   0     1001      122       14 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/requirements.txt
+-rw-r--r--   0     1001      122      271 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/__init__.py
+-rw-r--r--   0     1001      122      288 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_ext.py
+-rw-r--r--   0     1001      122     1011 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/__init__.py
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/__init__.py
+-rw-r--r--   0     1001      122     2482 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/_base.py
+-rw-r--r--   0     1001      122     1136 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/_base_meta.py
+-rw-r--r--   0     1001      122      303 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/_lstsq.py
+-rw-r--r--   0     1001      122      321 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/adnormal.py
+-rw-r--r--   0     1001      122      232 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/amplitude.py
+-rw-r--r--   0     1001      122      409 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/beyondnstd.py
+-rw-r--r--   0     1001      122     1309 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/bins.py
+-rw-r--r--   0     1001      122      365 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/cusum.py
+-rw-r--r--   0     1001      122      329 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/eta.py
+-rw-r--r--   0     1001      122      382 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/etae.py
+-rw-r--r--   0     1001      122      365 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/excvar.py
+-rw-r--r--   0     1001      122     1081 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/extractor.py
+-rw-r--r--   0     1001      122     1998 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py
+-rw-r--r--   0     1001      122      414 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/intpercrange.py
+-rw-r--r--   0     1001      122      476 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/kurtosis.py
+-rw-r--r--   0     1001      122      618 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/linfit.py
+-rw-r--r--   0     1001      122      455 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/lintrend.py
+-rw-r--r--   0     1001      122     2099 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py
+-rw-r--r--   0     1001      122      531 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/magnpratio.py
+-rw-r--r--   0     1001      122      371 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/maxslope.py
+-rw-r--r--   0     1001      122      217 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/mean.py
+-rw-r--r--   0     1001      122      253 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/meanvar.py
+-rw-r--r--   0     1001      122      282 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/medabsdev.py
+-rw-r--r--   0     1001      122      435 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/medbufrperc.py
+-rw-r--r--   0     1001      122      223 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/median.py
+-rw-r--r--   0     1001      122     2641 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/otsusplit.py
+-rw-r--r--   0     1001      122      506 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/pdiffmperc.py
+-rw-r--r--   0     1001      122      309 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/percampl.py
+-rw-r--r--   0     1001      122      377 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/redchi2.py
+-rw-r--r--   0     1001      122      236 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/skew.py
+-rw-r--r--   0     1001      122      250 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/stdev.py
+-rw-r--r--   0     1001      122      419 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/stetsonk.py
+-rw-r--r--   0     1001      122      265 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/weightmean.py
+-rw-r--r--   0     1001      122      596 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/warnings.py
+-rw-r--r--   0     1001      122     6058 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/pyproject.toml
+-rw-r--r--   0     1001      122     1395 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/check.rs
+-rw-r--r--   0     1001      122     2245 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/cont_array.rs
+-rw-r--r--   0     1001      122    50948 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/dmdt.rs
+-rw-r--r--   0     1001      122     1504 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/errors.rs
+-rw-r--r--   0     1001      122    63506 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/features.rs
+-rw-r--r--   0     1001      122     3528 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/lib.rs
+-rw-r--r--   0     1001      122     4269 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/ln_prior.rs
+-rw-r--r--   0     1001      122     3600 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/np_array.rs
+-rw-r--r--   0     1001      122     4450 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/transform.rs
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/__init__.py
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/__init__.py
+-rw-r--r--   0     1001      122    12272 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/test_dmdt.py
+-rw-r--r--   0     1001      122     9675 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/test_feature.py
+-rw-r--r--   0     1001      122      786 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/test_ln_prior.py
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/__init__.py
+-rw-r--r--   0     1001      122      304 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_adnormal.py
+-rw-r--r--   0     1001      122      289 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_amplitude.py
+-rw-r--r--   0     1001      122      516 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_beyondnstd.py
+-rw-r--r--   0     1001      122     2058 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_bins.py
+-rw-r--r--   0     1001      122      964 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_call.py
+-rw-r--r--   0     1001      122      302 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_cusum.py
+-rw-r--r--   0     1001      122      311 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_eta.py
+-rw-r--r--   0     1001      122      562 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_etae.py
+-rw-r--r--   0     1001      122      359 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_excvar.py
+-rw-r--r--   0     1001      122     1905 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_extractor.py
+-rw-r--r--   0     1001      122      478 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_intpercrange.py
+-rw-r--r--   0     1001      122      497 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_kurtosis.py
+-rw-r--r--   0     1001      122      702 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_linfit.py
+-rw-r--r--   0     1001      122      939 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_lintrend.py
+-rw-r--r--   0     1001      122      608 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_magnpratio.py
+-rw-r--r--   0     1001      122      297 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_maxslope.py
+-rw-r--r--   0     1001      122      450 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_mean.py
+-rw-r--r--   0     1001      122      326 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_meanvar.py
+-rw-r--r--   0     1001      122      335 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_medabsdev.py
+-rw-r--r--   0     1001      122      317 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_medbufrperc.py
+-rw-r--r--   0     1001      122      509 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_median.py
+-rw-r--r--   0     1001      122     1579 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_n_not_det_before_fd.py
+-rw-r--r--   0     1001      122     1307 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_otsusplit.py
+-rw-r--r--   0     1001      122      336 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_pdiffmperc.py
+-rw-r--r--   0     1001      122      321 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_percampl.py
+-rw-r--r--   0     1001      122      650 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_redchi2.py
+-rw-r--r--   0     1001      122      302 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_skew.py
+-rw-r--r--   0     1001      122      348 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_stdev.py
+-rw-r--r--   0     1001      122      673 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_stetsonk.py
+-rw-r--r--   0     1001      122      351 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_weightmean.py
+-rw-r--r--   0     1001      122    23632 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/test_w_bench.py
+-rw-r--r--   0     1001      122    48850 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/Cargo.lock
+-rw-r--r--   0        0        0    23378 1970-01-01 00:00:00.000000 light_curve-0.7.2b0/PKG-INFO
```

### Comparing `light_curve-0.7.2/Cargo.toml` & `light_curve-0.7.2b0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "light-curve-python"
-version = "0.7.2"
+version = "0.7.2-beta.0"
 authors = ["Konstantin Malanchev <hombit@gmail.com>", "Anastasia Lavrukhina <lavrukhina.ad@gmail.com>"]
 description = "Feature extractor from noisy time series"
 readme = "README.md"
 repository = "https://github.com/light-curve/light-curve-python"
 license = "GPL-3.0-or-later"
 edition = "2021"
 rust-version = "1.62"
```

### Comparing `light_curve-0.7.2/.readme/benchplot.png` & `light_curve-0.7.2b0/.readme/benchplot.png`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/README.md` & `light_curve-0.7.2b0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 | ----------- |-------------|--------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
 | **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | wheel (no Ceres, no GSL)                                             |
 | **i686**    | src         | src                            | —                                                              | not tested                                                           |
 | **aarch64** | wheel       | wheel                          | src https://github.com/light-curve/light-curve-python/issues/5 | not tested                                                           |
 | **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                    |
 
 - "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram performance, which is not a default build option. For Windows x86-64 we provide wheel with no Ceres and no GSL support, which is not a default build option.
-- "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.62+ to install it via `pip install`.
+- "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.57+ to install it via `pip install`.
 - "not tested": building from the source code is not tested, please report us building status via issue/PR/email.
 
 We build aarch64 macOS 12.0+ Python 3.8+ wheels locally and submit them running this command in `light-curve` directory:
 ```
 rm -rf ./wheelhouse
 CIBW_BUILD='cp3*-macosx_arm64' CIBW_ENVIRONMENT="MACOSX_DEPLOYMENT_TARGET=12.0 MATURIN_PEP517_ARGS='--locked --no-default-features --features ceres-source,fftw-source,gsl'" CIBW_BEFORE_ALL='curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y; brew install gsl' python3 -mcibuildwheel --platform macos
 twine upload wheelhouse/*.whl
```

### Comparing `light_curve-0.7.2/docs/Makefile` & `light_curve-0.7.2b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/docs/conf.py` & `light_curve-0.7.2b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/docs/index.rst` & `light_curve-0.7.2b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/docs/make.bat` & `light_curve-0.7.2b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/__init__.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/__init__.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/_base.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/_base.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/_base_meta.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/_base_meta.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/bins.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/bins.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/extractor.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/extractor.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/linfit.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/linfit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/magnpratio.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/magnpratio.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/features/otsusplit.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/otsusplit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/light_curve/light_curve_py/warnings.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/warnings.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/pyproject.toml` & `light_curve-0.7.2b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,23 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Rust",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 
 [project.optional-dependencies]
-test-no-bench = [
-    "pytest",
-    "markdown-pytest",
-    "pytest-benchmark",  # We need it here because we use benchmark-specific command line options
-    "pytest-subtests>=0.10",
-    "numpy",
-    "scipy",
-]
 test = [
-    "light-curve[test-no-bench]",
     "feets",
     "joblib",
+    "numpy",
     "pandas",
+    "pytest",
+    "pytest-benchmark",
+    "markdown-pytest",
+    "pytest-subtests",
 ]
 dev = [
     "light-curve[test]",
     "black",
     "ruff",
 ]
 
@@ -102,18 +98,14 @@
 minversion = "6.0"
 # requires pytest-benchmark
 addopts = "-ra --import-mode=append --benchmark-min-time=0.1 --benchmark-max-time=5.0 --benchmark-sort=mean --benchmark-disable"
 testpaths = [
     "tests/",
     "README.md", # requires markdown-pytest
 ]
-markers = [
-    "nobs: marks benchmarks for different numbers of observations (deselect with '-m \"not nobs\"')",
-    "multi: marks multiprocessing benchmarks (deselect with '-m \"not multi\"')",
-]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37,py38,py39,py310,py311
 isolated_build = True
 
@@ -121,14 +113,30 @@
 extras = dev
 commands =
     pytest README.md tests/ light_curve/
     ruff .
 """
 
 
+# Test
+# We skip benchmark tests, because it requires feets and its transitive
+# dependencies, which are tricky and slow to compile on marginal platforms.
+# For testing we use only platforms for which scipy binary wheels are available
+[[tool.cibuildwheel.overrides]]
+select = "cp*-manylinux_x86_64 cp*-manylinux_aarch64 cp*-macosx*"
+test-command = "pytest {package}/README.md {package}/light_curve/ {package}/tests/ --ignore {package}/tests/test_w_bench.py"
+test-requires = [
+    "pytest",
+    "pytest-benchmark",
+    "markdown-pytest",
+    "pytest-subtests",
+    "numpy",
+    "scipy",
+]
+
 [tool.cibuildwheel]
 # We use our own images which include Rust, GSL and platform-optimised FFTW
 # Manylinux CPython
 manylinux-aarch64-image = "ghcr.io/light-curve/base-docker-images/manylinux2014_aarch64"
 # not supported
 #manylinux-i686-image = "ghcr.io/light-curve/base-docker-images/manylinux2014_i686"
 manylinux-ppc64le-image = "ghcr.io/light-curve/base-docker-images/manylinux2014_ppc64le"
@@ -175,16 +183,7 @@
 environment = { "MATURIN_PEP517_ARGS" = "--locked --no-default-features --features fftw-source" }
 
 # Build with Intel MKL on Linux x86_64
 [[tool.cibuildwheel.overrides]]
 select = "*linux_x86_64"
 # We use system Ceres because it is available as a static library in our build environment
 environment = { "PATH" = "$PATH:$HOME/.cargo/bin", "MATURIN_PEP517_ARGS" = "--locked --no-default-features --features ceres-system,fftw-mkl,gsl" }
-
-# Test
-# We skip benchmark tests, because it requires feets and its transitive
-# dependencies, which are tricky and slow to compile on marginal platforms.
-# For testing we use only platforms for which scipy binary wheels are available
-[[tool.cibuildwheel.overrides]]
-select = "cp*-manylinux_x86_64 cp*-manylinux_aarch64 cp*-macosx*"
-test-command = "pytest {package}/README.md {package}/light_curve/ {package}/tests/ --ignore {package}/tests/test_w_bench.py"
-test-extras = ["test-no-bench"]
```

### Comparing `light_curve-0.7.2/src/check.rs` & `light_curve-0.7.2b0/src/check.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/cont_array.rs` & `light_curve-0.7.2b0/src/cont_array.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/dmdt.rs` & `light_curve-0.7.2b0/src/dmdt.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/errors.rs` & `light_curve-0.7.2b0/src/errors.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/features.rs` & `light_curve-0.7.2b0/src/features.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/lib.rs` & `light_curve-0.7.2b0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/ln_prior.rs` & `light_curve-0.7.2b0/src/ln_prior.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/np_array.rs` & `light_curve-0.7.2b0/src/np_array.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/src/transform.rs` & `light_curve-0.7.2b0/src/transform.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_ext/test_dmdt.py` & `light_curve-0.7.2b0/tests/light_curve_ext/test_dmdt.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_ext/test_feature.py` & `light_curve-0.7.2b0/tests/light_curve_ext/test_feature.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_ext/test_ln_prior.py` & `light_curve-0.7.2b0/tests/light_curve_ext/test_ln_prior.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_beyondnstd.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_beyondnstd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_bins.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_bins.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_call.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_call.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_etae.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_etae.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_extractor.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_extractor.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_linfit.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_linfit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_lintrend.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_lintrend.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_magnpratio.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_magnpratio.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_n_not_det_before_fd.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_otsusplit.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_otsusplit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_redchi2.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_redchi2.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/light_curve_py/test_stetsonk.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_stetsonk.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/tests/test_w_bench.py` & `light_curve-0.7.2b0/tests/test_w_bench.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.2/Cargo.lock` & `light_curve-0.7.2b0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
  "thiserror",
  "thread_local 1.1.4",
  "unzip3",
 ]
 
 [[package]]
 name = "light-curve-python"
-version = "0.7.2"
+version = "0.7.2-beta.0"
 dependencies = [
  "anyhow",
  "const_format",
  "conv",
  "enum-iterator",
  "enumflags2",
  "itertools 0.10.5",
```

### Comparing `light_curve-0.7.2/PKG-INFO` & `light_curve-0.7.2b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
 Name: light-curve
-Version: 0.7.2
+Version: 0.7.2b0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Dist: numpy
 Requires-Dist: scipy
-Requires-Dist: pytest; extra == 'test-no-bench'
-Requires-Dist: markdown-pytest; extra == 'test-no-bench'
-Requires-Dist: pytest-benchmark; extra == 'test-no-bench'
-Requires-Dist: pytest-subtests>=0.10; extra == 'test-no-bench'
-Requires-Dist: numpy; extra == 'test-no-bench'
-Requires-Dist: scipy; extra == 'test-no-bench'
-Requires-Dist: light-curve[test]; extra == 'dev'
-Requires-Dist: black; extra == 'dev'
-Requires-Dist: ruff; extra == 'dev'
-Requires-Dist: light-curve[test-no-bench]; extra == 'test'
 Requires-Dist: feets; extra == 'test'
 Requires-Dist: joblib; extra == 'test'
+Requires-Dist: numpy; extra == 'test'
 Requires-Dist: pandas; extra == 'test'
-Provides-Extra: test-no-bench
-Provides-Extra: dev
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-benchmark; extra == 'test'
+Requires-Dist: markdown-pytest; extra == 'test'
+Requires-Dist: pytest-subtests; extra == 'test'
+Requires-Dist: light-curve[test]; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: test
+Provides-Extra: dev
 Summary: Feature extractor from noisy time series
 Author: Konstantin Malanchev <hombit@gmail.com>, Anastasia Lavrukhina <lavrukhina.ad@gmail.com>
 Author-email: Konstantin Malanchev <hombit@gmail.com>, Anastasia Lavrukhina <lavrukhina.ad@gmail.com>
 License: GPL-3.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/light-curve/light-curve-python
@@ -63,15 +60,15 @@
 | ----------- |-------------|--------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
 | **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | wheel (no Ceres, no GSL)                                             |
 | **i686**    | src         | src                            | —                                                              | not tested                                                           |
 | **aarch64** | wheel       | wheel                          | src https://github.com/light-curve/light-curve-python/issues/5 | not tested                                                           |
 | **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                    |
 
 - "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram performance, which is not a default build option. For Windows x86-64 we provide wheel with no Ceres and no GSL support, which is not a default build option.
-- "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.62+ to install it via `pip install`.
+- "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.57+ to install it via `pip install`.
 - "not tested": building from the source code is not tested, please report us building status via issue/PR/email.
 
 We build aarch64 macOS 12.0+ Python 3.8+ wheels locally and submit them running this command in `light-curve` directory:
 ```
 rm -rf ./wheelhouse
 CIBW_BUILD='cp3*-macosx_arm64' CIBW_ENVIRONMENT="MACOSX_DEPLOYMENT_TARGET=12.0 MATURIN_PEP517_ARGS='--locked --no-default-features --features ceres-source,fftw-source,gsl'" CIBW_BEFORE_ALL='curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y; brew install gsl' python3 -mcibuildwheel --platform macos
 twine upload wheelhouse/*.whl
```

