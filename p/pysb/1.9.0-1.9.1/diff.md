# Comparing `tmp/pysb-1.9.0.tar.gz` & `tmp/pysb-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysb-1.9.0.tar", last modified: Fri May 10 18:31:49 2019, max compression
+gzip compressed data, was "dist/pysb-1.9.1.tar", last modified: Fri Jun 28 17:36:38 2019, max compression
```

## Comparing `pysb-1.9.0.tar` & `pysb-1.9.1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/
--rw-r--r--   0 alex       (501) staff       (20)     1313 2016-09-28 20:53:31.000000 pysb-1.9.0/LICENSE.txt
--rw-r--r--   0 alex       (501) staff       (20)      133 2019-04-02 19:50:13.000000 pysb-1.9.0/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)     2306 2019-05-10 18:31:49.000000 pysb-1.9.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1138 2019-03-05 19:13:57.000000 pysb-1.9.0/README.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/
--rw-r--r--   0 alex       (501) staff       (20)     4582 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/Makefile
--rw-r--r--   0 alex       (501) staff       (20)     8427 2019-05-10 16:06:49.000000 pysb-1.9.0/doc/conf.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/examples/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/examples/__pycache__/
--rw-r--r--   0 alex       (501) staff       (20)      726 2019-03-05 19:01:13.000000 pysb-1.9.0/doc/examples/__pycache__/mymodel4.cpython-37.pyc
--rw-r--r--   0 alex       (501) staff       (20)    22808 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/fig_mymodel4.png
--rw-r--r--   0 alex       (501) staff       (20)     1238 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/examples/mymodel.dot
--rw-r--r--   0 alex       (501) staff       (20)      109 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/examples/mymodel0.py
--rw-r--r--   0 alex       (501) staff       (20)      198 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/mymodel1.py
--rw-r--r--   0 alex       (501) staff       (20)      300 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/mymodel2.py
--rw-r--r--   0 alex       (501) staff       (20)      500 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/mymodel3.py
--rw-r--r--   0 alex       (501) staff       (20)      765 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/mymodel4.py
--rw-r--r--   0 alex       (501) staff       (20)     1806 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/mymodel5.py
--rw-r--r--   0 alex       (501) staff       (20)     2397 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/examples/mymodel_fxns.py
--rw-r--r--   0 alex       (501) staff       (20)     4761 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/examples/robertson_standalone.py
--rw-r--r--   0 alex       (501) staff       (20)    17774 2017-10-31 21:34:46.000000 pysb-1.9.0/doc/examples/test.png
--rw-r--r--   0 alex       (501) staff       (20)     3553 2019-03-05 21:03:02.000000 pysb-1.9.0/doc/faq.rst
--rw-r--r--   0 alex       (501) staff       (20)     1228 2019-03-05 21:03:02.000000 pysb-1.9.0/doc/index.rst
--rw-r--r--   0 alex       (501) staff       (20)     8561 2019-04-11 00:10:23.000000 pysb-1.9.0/doc/installation.rst
--rw-r--r--   0 alex       (501) staff       (20)     4507 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/make.bat
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/modules/
--rw-r--r--   0 alex       (501) staff       (20)      126 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/bng.rst
--rw-r--r--   0 alex       (501) staff       (20)      105 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/core.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/modules/export/
--rw-r--r--   0 alex       (501) staff       (20)      160 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/bng_net.rst
--rw-r--r--   0 alex       (501) staff       (20)      135 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/bngl.rst
--rw-r--r--   0 alex       (501) staff       (20)      144 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/index.rst
--rw-r--r--   0 alex       (501) staff       (20)      141 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/kappa.rst
--rw-r--r--   0 alex       (501) staff       (20)      187 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/mathematica.rst
--rw-r--r--   0 alex       (501) staff       (20)      162 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/matlab.rst
--rw-r--r--   0 alex       (501) staff       (20)      192 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/potterswheel.rst
--rw-r--r--   0 alex       (501) staff       (20)      175 2019-03-05 19:13:57.000000 pysb-1.9.0/doc/modules/export/pysb_flat.rst
--rw-r--r--   0 alex       (501) staff       (20)      168 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/python.rst
--rw-r--r--   0 alex       (501) staff       (20)      148 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/export/sbml.rst
--rw-r--r--   0 alex       (501) staff       (20)      156 2019-03-05 21:03:02.000000 pysb-1.9.0/doc/modules/export/stochkit.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/modules/importers/
--rw-r--r--   0 alex       (501) staff       (20)      283 2019-03-05 19:13:57.000000 pysb-1.9.0/doc/modules/importers/index.rst
--rw-r--r--   0 alex       (501) staff       (20)      291 2019-04-24 19:00:36.000000 pysb-1.9.0/doc/modules/index.rst
--rw-r--r--   0 alex       (501) staff       (20)      130 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/integrate.rst
--rw-r--r--   0 alex       (501) staff       (20)      124 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/kappa.rst
--rw-r--r--   0 alex       (501) staff       (20)      105 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/macros.rst
--rw-r--r--   0 alex       (501) staff       (20)      165 2019-03-05 21:03:02.000000 pysb-1.9.0/doc/modules/modeltests.rst
--rw-r--r--   0 alex       (501) staff       (20)      166 2019-03-05 21:03:02.000000 pysb-1.9.0/doc/modules/pattern.rst
--rw-r--r--   0 alex       (501) staff       (20)      132 2019-03-05 19:13:57.000000 pysb-1.9.0/doc/modules/simulator.rst
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/doc/modules/tools/
--rw-r--r--   0 alex       (501) staff       (20)      373 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/tools/render.rst
--rw-r--r--   0 alex       (501) staff       (20)      207 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/tools/render_reactions.rst
--rw-r--r--   0 alex       (501) staff       (20)      183 2016-09-28 20:53:31.000000 pysb-1.9.0/doc/modules/tools/render_species.rst
--rw-r--r--   0 alex       (501) staff       (20)    14418 2017-10-31 21:34:51.000000 pysb-1.9.0/doc/modules/tools/robertson_reactions.png
--rw-r--r--   0 alex       (501) staff       (20)      191 2019-04-24 19:00:36.000000 pysb-1.9.0/doc/modules/tools/sensitivity_analysis.rst
--rw-r--r--   0 alex       (501) staff       (20)      164 2019-03-05 19:13:57.000000 pysb-1.9.0/doc/requirements.txt
--rw-r--r--   0 alex       (501) staff       (20)    65129 2018-03-09 23:20:56.000000 pysb-1.9.0/doc/tutorial.ipynb
--rw-r--r--   0 alex       (501) staff       (20)    43542 2018-03-09 22:34:49.000000 pysb-1.9.0/doc/tutorial.md
--rw-r--r--   0 alex       (501) staff       (20)    42923 2019-04-10 17:22:19.000000 pysb-1.9.0/doc/tutorial.rst
--rw-r--r--   0 alex       (501) staff       (20)     1366 2019-03-05 19:13:57.000000 pysb-1.9.0/doc/useful_references.rst
--rw-r--r--   0 alex       (501) staff       (20)    11434 2019-02-04 18:19:13.000000 pysb-1.9.0/ez_setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/
--rw-r--r--   0 alex       (501) staff       (20)      709 2019-05-10 16:06:49.000000 pysb-1.9.0/pysb/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      471 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/_version.py
--rw-r--r--   0 alex       (501) staff       (20)    11205 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/anneal_mod.py
--rw-r--r--   0 alex       (501) staff       (20)     1415 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/annotation.py
--rw-r--r--   0 alex       (501) staff       (20)    32754 2019-05-10 16:06:49.000000 pysb-1.9.0/pysb/bng.py
--rw-r--r--   0 alex       (501) staff       (20)     7563 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/builder.py
--rw-r--r--   0 alex       (501) staff       (20)    89225 2019-05-10 18:04:00.000000 pysb-1.9.0/pysb/core.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/examples/
--rw-r--r--   0 alex       (501) staff       (20)        0 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/examples/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2560 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/bax_pore.py
--rw-r--r--   0 alex       (501) staff       (20)     2205 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/examples/bax_pore_sequential.py
--rw-r--r--   0 alex       (501) staff       (20)     3294 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/bngwiki_egfr_simple.py
--rw-r--r--   0 alex       (501) staff       (20)     1960 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/examples/bngwiki_enzymatic_cycle_mm.py
--rw-r--r--   0 alex       (501) staff       (20)     1221 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/bngwiki_simple.py
--rw-r--r--   0 alex       (501) staff       (20)     8715 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/earm_1_0.py
--rw-r--r--   0 alex       (501) staff       (20)     6696 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/examples/earm_1_3.py
--rw-r--r--   0 alex       (501) staff       (20)      930 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/examples/explicit.py
--rw-r--r--   0 alex       (501) staff       (20)      651 2018-06-08 02:41:36.000000 pysb-1.9.0/pysb/examples/expression_observables.py
--rw-r--r--   0 alex       (501) staff       (20)     1022 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/examples/fixed_initial.py
--rw-r--r--   0 alex       (501) staff       (20)    10821 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/fricker_2010_apoptosis.py
--rw-r--r--   0 alex       (501) staff       (20)     1087 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/hello_pysb.py
--rw-r--r--   0 alex       (501) staff       (20)     3732 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/examples/kinase_cascade.py
--rw-r--r--   0 alex       (501) staff       (20)      645 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/michment.py
--rw-r--r--   0 alex       (501) staff       (20)     1291 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/examples/move_connected.py
--rw-r--r--   0 alex       (501) staff       (20)     3174 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/examples/robertson.py
--rw-r--r--   0 alex       (501) staff       (20)      432 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_bax_pore.py
--rw-r--r--   0 alex       (501) staff       (20)     1074 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_bax_pore_sequential.py
--rw-r--r--   0 alex       (501) staff       (20)      408 2019-04-02 23:40:18.000000 pysb-1.9.0/pysb/examples/run_bng_ssa_example.py
--rw-r--r--   0 alex       (501) staff       (20)     3152 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_earm_1_0.py
--rw-r--r--   0 alex       (501) staff       (20)     2377 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_earm_hpp.py
--rw-r--r--   0 alex       (501) staff       (20)     1151 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_earm_stochkit.py
--rw-r--r--   0 alex       (501) staff       (20)     1083 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_fixed_initial.py
--rw-r--r--   0 alex       (501) staff       (20)      426 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_kinase_cascade.py
--rw-r--r--   0 alex       (501) staff       (20)      903 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/examples/run_michment.py
--rw-r--r--   0 alex       (501) staff       (20)      722 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_robertson.py
--rw-r--r--   0 alex       (501) staff       (20)      244 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/examples/run_tutorial_a.py
--rw-r--r--   0 alex       (501) staff       (20)      484 2019-03-05 19:13:57.000000 pysb-1.9.0/pysb/examples/run_tyson_oscillator.py
--rw-r--r--   0 alex       (501) staff       (20)     1051 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/examples/run_tyson_oscillator_stochkit.py
--rw-r--r--   0 alex       (501) staff       (20)      570 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/examples/synth_deg.py
--rw-r--r--   0 alex       (501) staff       (20)       98 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/examples/tutorial_a.py
--rw-r--r--   0 alex       (501) staff       (20)      154 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/examples/tutorial_b.py
--rw-r--r--   0 alex       (501) staff       (20)      224 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/examples/tutorial_c.py
--rw-r--r--   0 alex       (501) staff       (20)     2259 2019-03-05 19:13:57.000000 pysb-1.9.0/pysb/examples/tyson_oscillator.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/export/
--rw-r--r--   0 alex       (501) staff       (20)     4991 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/export/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1636 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/export/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)     1147 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/export/bng_net.py
--rw-r--r--   0 alex       (501) staff       (20)     1041 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/export/bngl.py
--rw-r--r--   0 alex       (501) staff       (20)     1455 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/export/kappa.py
--rw-r--r--   0 alex       (501) staff       (20)     9329 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/mathematica.py
--rw-r--r--   0 alex       (501) staff       (20)    18070 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/matlab.py
--rw-r--r--   0 alex       (501) staff       (20)     5706 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/potterswheel.py
--rw-r--r--   0 alex       (501) staff       (20)     2773 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/pysb_flat.py
--rw-r--r--   0 alex       (501) staff       (20)    10066 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/python.py
--rw-r--r--   0 alex       (501) staff       (20)    11113 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/sbml.py
--rw-r--r--   0 alex       (501) staff       (20)    12045 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/export/stochkit.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/generator/
--rw-r--r--   0 alex       (501) staff       (20)        0 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/generator/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    12268 2019-05-10 16:06:49.000000 pysb-1.9.0/pysb/generator/bng.py
--rw-r--r--   0 alex       (501) staff       (20)    12947 2019-05-10 16:06:49.000000 pysb-1.9.0/pysb/generator/kappa.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/importers/
--rw-r--r--   0 alex       (501) staff       (20)        0 2019-03-05 19:13:57.000000 pysb-1.9.0/pysb/importers/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    18798 2019-05-10 16:06:49.000000 pysb-1.9.0/pysb/importers/bngl.py
--rw-r--r--   0 alex       (501) staff       (20)     2056 2018-09-11 02:13:31.000000 pysb-1.9.0/pysb/importers/kappa.py
--rw-r--r--   0 alex       (501) staff       (20)     9384 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/importers/sbml.py
--rw-r--r--   0 alex       (501) staff       (20)    10512 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/integrate.py
--rw-r--r--   0 alex       (501) staff       (20)     4629 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/jacobian.py
--rw-r--r--   0 alex       (501) staff       (20)    16215 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/kappa.py
--rw-r--r--   0 alex       (501) staff       (20)     7016 2019-03-05 19:13:57.000000 pysb-1.9.0/pysb/logging.py
--rw-r--r--   0 alex       (501) staff       (20)   107027 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/macros.py
--rw-r--r--   0 alex       (501) staff       (20)     2175 2018-09-18 02:09:21.000000 pysb-1.9.0/pysb/merge.py
--rw-r--r--   0 alex       (501) staff       (20)     8896 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/pathfinder.py
--rw-r--r--   0 alex       (501) staff       (20)    38058 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/pattern.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/simulator/
--rw-r--r--   0 alex       (501) staff       (20)      356 2019-04-26 20:34:16.000000 pysb-1.9.0/pysb/simulator/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    55659 2019-05-10 16:35:31.000000 pysb-1.9.0/pysb/simulator/base.py
--rw-r--r--   0 alex       (501) staff       (20)    11652 2019-05-10 16:35:31.000000 pysb-1.9.0/pysb/simulator/bng.py
--rw-r--r--   0 alex       (501) staff       (20)    27616 2019-04-24 18:04:24.000000 pysb-1.9.0/pysb/simulator/cupsoda.py
--rw-r--r--   0 alex       (501) staff       (20)    28096 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/simulator/scipyode.py
--rw-r--r--   0 alex       (501) staff       (20)    13878 2019-04-25 20:41:55.000000 pysb-1.9.0/pysb/simulator/stochkit.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/testing/
--rw-r--r--   0 alex       (501) staff       (20)     2734 2019-03-05 19:13:57.000000 pysb-1.9.0/pysb/testing/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    13280 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/testing/modeltests.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/tests/
--rw-r--r--   0 alex       (501) staff       (20)      191 2019-03-05 19:13:57.000000 pysb-1.9.0/pysb/tests/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1146 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/tests/jacobian_runtimes.py
--rw-r--r--   0 alex       (501) staff       (20)     8350 2019-04-24 19:00:36.000000 pysb-1.9.0/pysb/tests/test_bng.py
--rw-r--r--   0 alex       (501) staff       (20)    14551 2019-05-10 18:04:00.000000 pysb-1.9.0/pysb/tests/test_core.py
--rw-r--r--   0 alex       (501) staff       (20)     1960 2019-04-02 23:40:18.000000 pysb-1.9.0/pysb/tests/test_examples.py
--rw-r--r--   0 alex       (501) staff       (20)     3846 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/tests/test_exporters.py
--rw-r--r--   0 alex       (501) staff       (20)     2067 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/tests/test_expressions.py
--rw-r--r--   0 alex       (501) staff       (20)      141 2018-11-29 22:01:06.000000 pysb-1.9.0/pysb/tests/test_importer_kappa.py
--rw-r--r--   0 alex       (501) staff       (20)     7288 2019-05-10 16:06:49.000000 pysb-1.9.0/pysb/tests/test_importers.py
--rw-r--r--   0 alex       (501) staff       (20)     4835 2019-04-25 19:40:00.000000 pysb-1.9.0/pysb/tests/test_integrate.py
--rw-r--r--   0 alex       (501) staff       (20)    10127 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/tests/test_kappa.py
--rw-r--r--   0 alex       (501) staff       (20)      327 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/tests/test_macros.py
--rw-r--r--   0 alex       (501) staff       (20)      575 2018-09-16 23:30:20.000000 pysb-1.9.0/pysb/tests/test_merge.py
--rw-r--r--   0 alex       (501) staff       (20)     2455 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/tests/test_pattern.py
--rw-r--r--   0 alex       (501) staff       (20)     7937 2019-04-24 19:00:36.000000 pysb-1.9.0/pysb/tests/test_sensitivity_analysis.py
--rw-r--r--   0 alex       (501) staff       (20)     8583 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/tests/test_simulationresult.py
--rw-r--r--   0 alex       (501) staff       (20)     6815 2019-05-10 16:35:31.000000 pysb-1.9.0/pysb/tests/test_simulator_bng.py
--rw-r--r--   0 alex       (501) staff       (20)     4329 2019-04-11 00:10:23.000000 pysb-1.9.0/pysb/tests/test_simulator_cupsoda.py
--rw-r--r--   0 alex       (501) staff       (20)    19220 2019-04-26 01:53:18.000000 pysb-1.9.0/pysb/tests/test_simulator_scipy.py
--rw-r--r--   0 alex       (501) staff       (20)     1565 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/tests/test_simulator_stochkit.py
--rw-r--r--   0 alex       (501) staff       (20)     1211 2019-02-04 18:19:13.000000 pysb-1.9.0/pysb/tests/test_util.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb/tools/
--rw-r--r--   0 alex       (501) staff       (20)        0 2016-09-28 20:53:31.000000 pysb-1.9.0/pysb/tools/__init__.py
--rwxr-xr-x   0 alex       (501) staff       (20)     5596 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/tools/render_reactions.py
--rwxr-xr-x   0 alex       (501) staff       (20)     5583 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/tools/render_species.py
--rw-r--r--   0 alex       (501) staff       (20)    29666 2019-04-24 19:00:36.000000 pysb-1.9.0/pysb/tools/sensitivity_analysis.py
--rw-r--r--   0 alex       (501) staff       (20)     4011 2019-04-10 17:22:19.000000 pysb-1.9.0/pysb/tools/species_graph.py
--rw-r--r--   0 alex       (501) staff       (20)     6472 2019-03-05 21:03:02.000000 pysb-1.9.0/pysb/util.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/pysb.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     2306 2019-05-10 18:31:48.000000 pysb-1.9.0/pysb.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4354 2019-05-10 18:31:48.000000 pysb-1.9.0/pysb.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2019-05-10 18:31:48.000000 pysb-1.9.0/pysb.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       68 2019-05-10 18:31:48.000000 pysb-1.9.0/pysb.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        5 2019-05-10 18:31:48.000000 pysb-1.9.0/pysb.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-05-10 18:31:49.000000 pysb-1.9.0/scripts/
--rw-r--r--   0 alex       (501) staff       (20)      565 2019-02-04 18:19:13.000000 pysb-1.9.0/scripts/pysb_export
--rw-r--r--   0 alex       (501) staff       (20)      255 2019-05-10 18:31:49.000000 pysb-1.9.0/setup.cfg
--rwxr-xr-x   0 alex       (501) staff       (20)     2105 2019-04-25 20:41:55.000000 pysb-1.9.0/setup.py
--rw-r--r--   0 alex       (501) staff       (20)    62475 2019-02-04 18:19:13.000000 pysb-1.9.0/versioneer.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/
+-rw-r--r--   0 alex       (501) staff       (20)     1313 2016-09-28 20:53:31.000000 pysb-1.9.1/LICENSE.txt
+-rw-r--r--   0 alex       (501) staff       (20)      133 2019-04-02 19:50:13.000000 pysb-1.9.1/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)     2306 2019-06-28 17:36:38.000000 pysb-1.9.1/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1138 2019-03-05 19:13:57.000000 pysb-1.9.1/README.rst
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/
+-rw-r--r--   0 alex       (501) staff       (20)     4582 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/Makefile
+-rw-r--r--   0 alex       (501) staff       (20)     8427 2019-06-28 16:44:37.000000 pysb-1.9.1/doc/conf.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/examples/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/examples/__pycache__/
+-rw-r--r--   0 alex       (501) staff       (20)      726 2019-03-05 19:01:13.000000 pysb-1.9.1/doc/examples/__pycache__/mymodel4.cpython-37.pyc
+-rw-r--r--   0 alex       (501) staff       (20)    22808 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/fig_mymodel4.png
+-rw-r--r--   0 alex       (501) staff       (20)     1238 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/examples/mymodel.dot
+-rw-r--r--   0 alex       (501) staff       (20)      109 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/examples/mymodel0.py
+-rw-r--r--   0 alex       (501) staff       (20)      198 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/mymodel1.py
+-rw-r--r--   0 alex       (501) staff       (20)      300 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/mymodel2.py
+-rw-r--r--   0 alex       (501) staff       (20)      500 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/mymodel3.py
+-rw-r--r--   0 alex       (501) staff       (20)      765 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/mymodel4.py
+-rw-r--r--   0 alex       (501) staff       (20)     1806 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/mymodel5.py
+-rw-r--r--   0 alex       (501) staff       (20)     2397 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/examples/mymodel_fxns.py
+-rw-r--r--   0 alex       (501) staff       (20)     4761 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/examples/robertson_standalone.py
+-rw-r--r--   0 alex       (501) staff       (20)    17774 2017-10-31 21:34:46.000000 pysb-1.9.1/doc/examples/test.png
+-rw-r--r--   0 alex       (501) staff       (20)     3553 2019-03-05 21:03:02.000000 pysb-1.9.1/doc/faq.rst
+-rw-r--r--   0 alex       (501) staff       (20)     1228 2019-03-05 21:03:02.000000 pysb-1.9.1/doc/index.rst
+-rw-r--r--   0 alex       (501) staff       (20)     8561 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/installation.rst
+-rw-r--r--   0 alex       (501) staff       (20)     4507 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/make.bat
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/modules/
+-rw-r--r--   0 alex       (501) staff       (20)      126 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/bng.rst
+-rw-r--r--   0 alex       (501) staff       (20)      105 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/core.rst
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/modules/export/
+-rw-r--r--   0 alex       (501) staff       (20)      160 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/bng_net.rst
+-rw-r--r--   0 alex       (501) staff       (20)      135 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/bngl.rst
+-rw-r--r--   0 alex       (501) staff       (20)      144 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/index.rst
+-rw-r--r--   0 alex       (501) staff       (20)      141 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/kappa.rst
+-rw-r--r--   0 alex       (501) staff       (20)      187 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/mathematica.rst
+-rw-r--r--   0 alex       (501) staff       (20)      162 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/matlab.rst
+-rw-r--r--   0 alex       (501) staff       (20)      192 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/potterswheel.rst
+-rw-r--r--   0 alex       (501) staff       (20)      175 2019-03-05 19:13:57.000000 pysb-1.9.1/doc/modules/export/pysb_flat.rst
+-rw-r--r--   0 alex       (501) staff       (20)      168 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/python.rst
+-rw-r--r--   0 alex       (501) staff       (20)      148 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/export/sbml.rst
+-rw-r--r--   0 alex       (501) staff       (20)      156 2019-03-05 21:03:02.000000 pysb-1.9.1/doc/modules/export/stochkit.rst
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/modules/importers/
+-rw-r--r--   0 alex       (501) staff       (20)      283 2019-03-05 19:13:57.000000 pysb-1.9.1/doc/modules/importers/index.rst
+-rw-r--r--   0 alex       (501) staff       (20)      291 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/modules/index.rst
+-rw-r--r--   0 alex       (501) staff       (20)      130 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/integrate.rst
+-rw-r--r--   0 alex       (501) staff       (20)      124 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/kappa.rst
+-rw-r--r--   0 alex       (501) staff       (20)      105 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/macros.rst
+-rw-r--r--   0 alex       (501) staff       (20)      165 2019-03-05 21:03:02.000000 pysb-1.9.1/doc/modules/modeltests.rst
+-rw-r--r--   0 alex       (501) staff       (20)      166 2019-03-05 21:03:02.000000 pysb-1.9.1/doc/modules/pattern.rst
+-rw-r--r--   0 alex       (501) staff       (20)      132 2019-03-05 19:13:57.000000 pysb-1.9.1/doc/modules/simulator.rst
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/doc/modules/tools/
+-rw-r--r--   0 alex       (501) staff       (20)      373 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/tools/render.rst
+-rw-r--r--   0 alex       (501) staff       (20)      207 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/tools/render_reactions.rst
+-rw-r--r--   0 alex       (501) staff       (20)      183 2016-09-28 20:53:31.000000 pysb-1.9.1/doc/modules/tools/render_species.rst
+-rw-r--r--   0 alex       (501) staff       (20)    14418 2017-10-31 21:34:51.000000 pysb-1.9.1/doc/modules/tools/robertson_reactions.png
+-rw-r--r--   0 alex       (501) staff       (20)      191 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/modules/tools/sensitivity_analysis.rst
+-rw-r--r--   0 alex       (501) staff       (20)      164 2019-03-05 19:13:57.000000 pysb-1.9.1/doc/requirements.txt
+-rw-r--r--   0 alex       (501) staff       (20)    65129 2018-03-09 23:20:56.000000 pysb-1.9.1/doc/tutorial.ipynb
+-rw-r--r--   0 alex       (501) staff       (20)    43542 2018-03-09 22:34:49.000000 pysb-1.9.1/doc/tutorial.md
+-rw-r--r--   0 alex       (501) staff       (20)    42923 2019-05-10 20:37:48.000000 pysb-1.9.1/doc/tutorial.rst
+-rw-r--r--   0 alex       (501) staff       (20)     1366 2019-03-05 19:13:57.000000 pysb-1.9.1/doc/useful_references.rst
+-rw-r--r--   0 alex       (501) staff       (20)    11434 2019-02-04 18:19:13.000000 pysb-1.9.1/ez_setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/
+-rw-r--r--   0 alex       (501) staff       (20)      709 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      471 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/_version.py
+-rw-r--r--   0 alex       (501) staff       (20)    11205 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/anneal_mod.py
+-rw-r--r--   0 alex       (501) staff       (20)     1415 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/annotation.py
+-rw-r--r--   0 alex       (501) staff       (20)    32754 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/bng.py
+-rw-r--r--   0 alex       (501) staff       (20)     7563 2019-05-21 19:43:39.000000 pysb-1.9.1/pysb/builder.py
+-rw-r--r--   0 alex       (501) staff       (20)    89225 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/core.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/examples/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/examples/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2560 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/bax_pore.py
+-rw-r--r--   0 alex       (501) staff       (20)     2205 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/examples/bax_pore_sequential.py
+-rw-r--r--   0 alex       (501) staff       (20)     3294 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/bngwiki_egfr_simple.py
+-rw-r--r--   0 alex       (501) staff       (20)     1960 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/examples/bngwiki_enzymatic_cycle_mm.py
+-rw-r--r--   0 alex       (501) staff       (20)     1221 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/bngwiki_simple.py
+-rw-r--r--   0 alex       (501) staff       (20)     8715 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/earm_1_0.py
+-rw-r--r--   0 alex       (501) staff       (20)     6696 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/examples/earm_1_3.py
+-rw-r--r--   0 alex       (501) staff       (20)      930 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/explicit.py
+-rw-r--r--   0 alex       (501) staff       (20)      651 2018-06-08 02:41:36.000000 pysb-1.9.1/pysb/examples/expression_observables.py
+-rw-r--r--   0 alex       (501) staff       (20)     1022 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/fixed_initial.py
+-rw-r--r--   0 alex       (501) staff       (20)    10821 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/fricker_2010_apoptosis.py
+-rw-r--r--   0 alex       (501) staff       (20)     1087 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/hello_pysb.py
+-rw-r--r--   0 alex       (501) staff       (20)     3732 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/examples/kinase_cascade.py
+-rw-r--r--   0 alex       (501) staff       (20)      645 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/michment.py
+-rw-r--r--   0 alex       (501) staff       (20)     1291 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/examples/move_connected.py
+-rw-r--r--   0 alex       (501) staff       (20)     3174 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/examples/robertson.py
+-rw-r--r--   0 alex       (501) staff       (20)      432 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_bax_pore.py
+-rw-r--r--   0 alex       (501) staff       (20)     1074 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_bax_pore_sequential.py
+-rw-r--r--   0 alex       (501) staff       (20)      408 2019-04-02 23:40:18.000000 pysb-1.9.1/pysb/examples/run_bng_ssa_example.py
+-rw-r--r--   0 alex       (501) staff       (20)     3152 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_earm_1_0.py
+-rw-r--r--   0 alex       (501) staff       (20)     2377 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_earm_hpp.py
+-rw-r--r--   0 alex       (501) staff       (20)     1151 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_earm_stochkit.py
+-rw-r--r--   0 alex       (501) staff       (20)     1083 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_fixed_initial.py
+-rw-r--r--   0 alex       (501) staff       (20)      426 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_kinase_cascade.py
+-rw-r--r--   0 alex       (501) staff       (20)      903 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_michment.py
+-rw-r--r--   0 alex       (501) staff       (20)      722 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_robertson.py
+-rw-r--r--   0 alex       (501) staff       (20)      244 2019-04-10 17:22:19.000000 pysb-1.9.1/pysb/examples/run_tutorial_a.py
+-rw-r--r--   0 alex       (501) staff       (20)      484 2019-03-05 19:13:57.000000 pysb-1.9.1/pysb/examples/run_tyson_oscillator.py
+-rw-r--r--   0 alex       (501) staff       (20)     1051 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/examples/run_tyson_oscillator_stochkit.py
+-rw-r--r--   0 alex       (501) staff       (20)      570 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/examples/synth_deg.py
+-rw-r--r--   0 alex       (501) staff       (20)       98 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/examples/tutorial_a.py
+-rw-r--r--   0 alex       (501) staff       (20)      154 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/examples/tutorial_b.py
+-rw-r--r--   0 alex       (501) staff       (20)      224 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/examples/tutorial_c.py
+-rw-r--r--   0 alex       (501) staff       (20)     2259 2019-03-05 19:13:57.000000 pysb-1.9.1/pysb/examples/tyson_oscillator.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/export/
+-rw-r--r--   0 alex       (501) staff       (20)     4991 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/export/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1636 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/export/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1147 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/export/bng_net.py
+-rw-r--r--   0 alex       (501) staff       (20)     1041 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/export/bngl.py
+-rw-r--r--   0 alex       (501) staff       (20)     1455 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/export/kappa.py
+-rw-r--r--   0 alex       (501) staff       (20)     9329 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/export/mathematica.py
+-rw-r--r--   0 alex       (501) staff       (20)    18070 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/export/matlab.py
+-rw-r--r--   0 alex       (501) staff       (20)     5706 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/export/potterswheel.py
+-rw-r--r--   0 alex       (501) staff       (20)     2773 2019-05-21 19:43:39.000000 pysb-1.9.1/pysb/export/pysb_flat.py
+-rw-r--r--   0 alex       (501) staff       (20)    10066 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/export/python.py
+-rw-r--r--   0 alex       (501) staff       (20)    11113 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/export/sbml.py
+-rw-r--r--   0 alex       (501) staff       (20)    12045 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/export/stochkit.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/generator/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/generator/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    12268 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/generator/bng.py
+-rw-r--r--   0 alex       (501) staff       (20)    12947 2019-06-28 17:33:12.000000 pysb-1.9.1/pysb/generator/kappa.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/importers/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2019-03-05 19:13:57.000000 pysb-1.9.1/pysb/importers/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    18798 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/importers/bngl.py
+-rw-r--r--   0 alex       (501) staff       (20)     2056 2018-09-11 02:13:31.000000 pysb-1.9.1/pysb/importers/kappa.py
+-rw-r--r--   0 alex       (501) staff       (20)     9384 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/importers/sbml.py
+-rw-r--r--   0 alex       (501) staff       (20)    10512 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/integrate.py
+-rw-r--r--   0 alex       (501) staff       (20)     4629 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/jacobian.py
+-rw-r--r--   0 alex       (501) staff       (20)    16215 2019-06-28 17:17:07.000000 pysb-1.9.1/pysb/kappa.py
+-rw-r--r--   0 alex       (501) staff       (20)     7016 2019-03-05 19:13:57.000000 pysb-1.9.1/pysb/logging.py
+-rw-r--r--   0 alex       (501) staff       (20)   107027 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/macros.py
+-rw-r--r--   0 alex       (501) staff       (20)     2175 2018-09-18 02:09:21.000000 pysb-1.9.1/pysb/merge.py
+-rw-r--r--   0 alex       (501) staff       (20)     8896 2019-04-10 17:22:19.000000 pysb-1.9.1/pysb/pathfinder.py
+-rw-r--r--   0 alex       (501) staff       (20)    38058 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/pattern.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/simulator/
+-rw-r--r--   0 alex       (501) staff       (20)      356 2019-06-28 17:33:12.000000 pysb-1.9.1/pysb/simulator/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    54148 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/simulator/base.py
+-rw-r--r--   0 alex       (501) staff       (20)    11652 2019-06-09 18:44:52.000000 pysb-1.9.1/pysb/simulator/bng.py
+-rw-r--r--   0 alex       (501) staff       (20)    27616 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/simulator/cupsoda.py
+-rw-r--r--   0 alex       (501) staff       (20)    28096 2019-05-21 19:43:39.000000 pysb-1.9.1/pysb/simulator/scipyode.py
+-rw-r--r--   0 alex       (501) staff       (20)    13878 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/simulator/stochkit.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/testing/
+-rw-r--r--   0 alex       (501) staff       (20)     2734 2019-03-05 19:13:57.000000 pysb-1.9.1/pysb/testing/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)    13280 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/testing/modeltests.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/tests/
+-rw-r--r--   0 alex       (501) staff       (20)      191 2019-03-05 19:13:57.000000 pysb-1.9.1/pysb/tests/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1146 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/tests/jacobian_runtimes.py
+-rw-r--r--   0 alex       (501) staff       (20)     8350 2019-05-21 19:43:39.000000 pysb-1.9.1/pysb/tests/test_bng.py
+-rw-r--r--   0 alex       (501) staff       (20)    14551 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/tests/test_core.py
+-rw-r--r--   0 alex       (501) staff       (20)     1960 2019-04-02 23:40:18.000000 pysb-1.9.1/pysb/tests/test_examples.py
+-rw-r--r--   0 alex       (501) staff       (20)     3846 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tests/test_exporters.py
+-rw-r--r--   0 alex       (501) staff       (20)     2067 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/tests/test_expressions.py
+-rw-r--r--   0 alex       (501) staff       (20)      141 2018-11-29 22:01:06.000000 pysb-1.9.1/pysb/tests/test_importer_kappa.py
+-rw-r--r--   0 alex       (501) staff       (20)     7288 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/tests/test_importers.py
+-rw-r--r--   0 alex       (501) staff       (20)     4835 2019-04-25 19:40:00.000000 pysb-1.9.1/pysb/tests/test_integrate.py
+-rw-r--r--   0 alex       (501) staff       (20)    10127 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/tests/test_kappa.py
+-rw-r--r--   0 alex       (501) staff       (20)      327 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/tests/test_macros.py
+-rw-r--r--   0 alex       (501) staff       (20)      575 2018-09-16 23:30:20.000000 pysb-1.9.1/pysb/tests/test_merge.py
+-rw-r--r--   0 alex       (501) staff       (20)     2455 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/tests/test_pattern.py
+-rw-r--r--   0 alex       (501) staff       (20)     7937 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tests/test_sensitivity_analysis.py
+-rw-r--r--   0 alex       (501) staff       (20)     8583 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tests/test_simulationresult.py
+-rw-r--r--   0 alex       (501) staff       (20)     8245 2019-06-28 16:44:37.000000 pysb-1.9.1/pysb/tests/test_simulator_bng.py
+-rw-r--r--   0 alex       (501) staff       (20)     4329 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tests/test_simulator_cupsoda.py
+-rw-r--r--   0 alex       (501) staff       (20)    19220 2019-06-13 21:25:47.000000 pysb-1.9.1/pysb/tests/test_simulator_scipy.py
+-rw-r--r--   0 alex       (501) staff       (20)     1565 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/tests/test_simulator_stochkit.py
+-rw-r--r--   0 alex       (501) staff       (20)     1211 2019-02-04 18:19:13.000000 pysb-1.9.1/pysb/tests/test_util.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb/tools/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2016-09-28 20:53:31.000000 pysb-1.9.1/pysb/tools/__init__.py
+-rwxr-xr-x   0 alex       (501) staff       (20)     5596 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tools/render_reactions.py
+-rwxr-xr-x   0 alex       (501) staff       (20)     5583 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/tools/render_species.py
+-rw-r--r--   0 alex       (501) staff       (20)    29666 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tools/sensitivity_analysis.py
+-rw-r--r--   0 alex       (501) staff       (20)     4011 2019-05-10 20:37:48.000000 pysb-1.9.1/pysb/tools/species_graph.py
+-rw-r--r--   0 alex       (501) staff       (20)     6472 2019-03-05 21:03:02.000000 pysb-1.9.1/pysb/util.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     2306 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4354 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       68 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        5 2019-06-28 17:36:38.000000 pysb-1.9.1/pysb.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2019-06-28 17:36:38.000000 pysb-1.9.1/scripts/
+-rw-r--r--   0 alex       (501) staff       (20)      565 2019-02-04 18:19:13.000000 pysb-1.9.1/scripts/pysb_export
+-rw-r--r--   0 alex       (501) staff       (20)      255 2019-06-28 17:36:38.000000 pysb-1.9.1/setup.cfg
+-rwxr-xr-x   0 alex       (501) staff       (20)     2105 2019-05-10 20:37:48.000000 pysb-1.9.1/setup.py
+-rw-r--r--   0 alex       (501) staff       (20)    62475 2019-02-04 18:19:13.000000 pysb-1.9.1/versioneer.py
```

### Comparing `pysb-1.9.0/LICENSE.txt` & `pysb-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/PKG-INFO` & `pysb-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysb
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python Systems Biology modeling framework
 Home-page: http://pysb.org/
 Author: Jeremy Muhlich
 Author-email: jmuhlich@bitflood.org
 License: UNKNOWN
 Description: PySB
         ====
```

### Comparing `pysb-1.9.0/README.rst` & `pysb-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/Makefile` & `pysb-1.9.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/conf.py` & `pysb-1.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/__pycache__/mymodel4.cpython-37.pyc` & `pysb-1.9.1/doc/examples/__pycache__/mymodel4.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/fig_mymodel4.png` & `pysb-1.9.1/doc/examples/fig_mymodel4.png`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/mymodel.dot` & `pysb-1.9.1/doc/examples/mymodel.dot`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/mymodel4.py` & `pysb-1.9.1/doc/examples/mymodel4.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/mymodel5.py` & `pysb-1.9.1/doc/examples/mymodel5.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/mymodel_fxns.py` & `pysb-1.9.1/doc/examples/mymodel_fxns.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/robertson_standalone.py` & `pysb-1.9.1/doc/examples/robertson_standalone.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/examples/test.png` & `pysb-1.9.1/doc/examples/test.png`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/faq.rst` & `pysb-1.9.1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/index.rst` & `pysb-1.9.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/installation.rst` & `pysb-1.9.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/make.bat` & `pysb-1.9.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/modules/tools/robertson_reactions.png` & `pysb-1.9.1/doc/modules/tools/robertson_reactions.png`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/tutorial.ipynb` & `pysb-1.9.1/doc/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/tutorial.md` & `pysb-1.9.1/doc/tutorial.md`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/tutorial.rst` & `pysb-1.9.1/doc/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/doc/useful_references.rst` & `pysb-1.9.1/doc/useful_references.rst`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/ez_setup.py` & `pysb-1.9.1/ez_setup.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/__init__.py` & `pysb-1.9.1/pysb/__init__.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/anneal_mod.py` & `pysb-1.9.1/pysb/anneal_mod.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/annotation.py` & `pysb-1.9.1/pysb/annotation.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/bng.py` & `pysb-1.9.1/pysb/bng.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/builder.py` & `pysb-1.9.1/pysb/builder.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/core.py` & `pysb-1.9.1/pysb/core.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/bax_pore.py` & `pysb-1.9.1/pysb/examples/bax_pore.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/bax_pore_sequential.py` & `pysb-1.9.1/pysb/examples/bax_pore_sequential.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/bngwiki_egfr_simple.py` & `pysb-1.9.1/pysb/examples/bngwiki_egfr_simple.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/bngwiki_enzymatic_cycle_mm.py` & `pysb-1.9.1/pysb/examples/bngwiki_enzymatic_cycle_mm.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/bngwiki_simple.py` & `pysb-1.9.1/pysb/examples/bngwiki_simple.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/earm_1_0.py` & `pysb-1.9.1/pysb/examples/earm_1_0.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/earm_1_3.py` & `pysb-1.9.1/pysb/examples/earm_1_3.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/explicit.py` & `pysb-1.9.1/pysb/examples/explicit.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/expression_observables.py` & `pysb-1.9.1/pysb/examples/expression_observables.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/fixed_initial.py` & `pysb-1.9.1/pysb/examples/fixed_initial.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/fricker_2010_apoptosis.py` & `pysb-1.9.1/pysb/examples/fricker_2010_apoptosis.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/hello_pysb.py` & `pysb-1.9.1/pysb/examples/hello_pysb.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/kinase_cascade.py` & `pysb-1.9.1/pysb/examples/kinase_cascade.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/michment.py` & `pysb-1.9.1/pysb/examples/michment.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/move_connected.py` & `pysb-1.9.1/pysb/examples/move_connected.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/robertson.py` & `pysb-1.9.1/pysb/examples/robertson.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_bax_pore_sequential.py` & `pysb-1.9.1/pysb/examples/run_bax_pore_sequential.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_earm_1_0.py` & `pysb-1.9.1/pysb/examples/run_earm_1_0.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_earm_hpp.py` & `pysb-1.9.1/pysb/examples/run_earm_hpp.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_earm_stochkit.py` & `pysb-1.9.1/pysb/examples/run_earm_stochkit.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_fixed_initial.py` & `pysb-1.9.1/pysb/examples/run_fixed_initial.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_michment.py` & `pysb-1.9.1/pysb/examples/run_michment.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_robertson.py` & `pysb-1.9.1/pysb/examples/run_robertson.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/run_tyson_oscillator_stochkit.py` & `pysb-1.9.1/pysb/examples/run_tyson_oscillator_stochkit.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/synth_deg.py` & `pysb-1.9.1/pysb/examples/synth_deg.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/examples/tyson_oscillator.py` & `pysb-1.9.1/pysb/examples/tyson_oscillator.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/__init__.py` & `pysb-1.9.1/pysb/export/__init__.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/__main__.py` & `pysb-1.9.1/pysb/export/__main__.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/bng_net.py` & `pysb-1.9.1/pysb/export/bng_net.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/bngl.py` & `pysb-1.9.1/pysb/export/bngl.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/kappa.py` & `pysb-1.9.1/pysb/export/kappa.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/mathematica.py` & `pysb-1.9.1/pysb/export/mathematica.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/matlab.py` & `pysb-1.9.1/pysb/export/matlab.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/potterswheel.py` & `pysb-1.9.1/pysb/export/potterswheel.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/pysb_flat.py` & `pysb-1.9.1/pysb/export/pysb_flat.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/python.py` & `pysb-1.9.1/pysb/export/python.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/sbml.py` & `pysb-1.9.1/pysb/export/sbml.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/export/stochkit.py` & `pysb-1.9.1/pysb/export/stochkit.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/generator/bng.py` & `pysb-1.9.1/pysb/generator/bng.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/generator/kappa.py` & `pysb-1.9.1/pysb/generator/kappa.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/importers/bngl.py` & `pysb-1.9.1/pysb/importers/bngl.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/importers/kappa.py` & `pysb-1.9.1/pysb/importers/kappa.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/importers/sbml.py` & `pysb-1.9.1/pysb/importers/sbml.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/integrate.py` & `pysb-1.9.1/pysb/integrate.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/jacobian.py` & `pysb-1.9.1/pysb/jacobian.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/kappa.py` & `pysb-1.9.1/pysb/kappa.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/logging.py` & `pysb-1.9.1/pysb/logging.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/macros.py` & `pysb-1.9.1/pysb/macros.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/merge.py` & `pysb-1.9.1/pysb/merge.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/pathfinder.py` & `pysb-1.9.1/pysb/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/pattern.py` & `pysb-1.9.1/pysb/pattern.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/simulator/base.py` & `pysb-1.9.1/pysb/simulator/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,53 +158,89 @@
             if self._initials:
                 return len(list(self._initials.values())[0])
             elif self._run_initials:
                 return len(list(self._run_initials.values())[0])
             else:
                 return len(self.param_values)
 
-    def _update_initials_dict(self, initials_dict, initials_source):
+    def _update_initials_dict(self, initials_dict, initials_source, subs=None):
         if isinstance(initials_source, collections.Mapping):
             # Can't just use .update() as we need to test
             # equality with .is_equivalent_to()
-            for cp, val in initials_source.items():
-                found = False
-                for existing_cp in initials_dict.keys():
-                    if existing_cp.is_equivalent_to(as_complex_pattern(cp)):
-                        initials_dict[existing_cp] = val
-                        found = True
-                        break
-                if not found:
-                    initials_dict[cp] = val
+            for cp, value_obj in initials_source.items():
+                cp = as_complex_pattern(cp)
+                if any(existing_cp.is_equivalent_to(cp)
+                       for existing_cp in initials_dict):
+                    continue
+
+                if isinstance(value_obj, (collections.Sequence, np.ndarray))\
+                        and all(isinstance(v, numbers.Number) for v in value_obj):
+                    value = value_obj
+                elif isinstance(value_obj, Expression):
+                    value = [value_obj.expand_expr().evalf(subs=subs[sim]) for sim in range(len(subs))]
+                elif isinstance(value_obj, Parameter):
+                    # Set parameter using param_values
+                    pi = self._model.parameters.index(value_obj)
+                    value = [self.param_values[sim][pi] for sim in range(len(self.param_values))]
+                else:
+                    raise TypeError("Unexpected initial condition "
+                                    "value type: %s" % type(value_obj))
+
+                initials_dict[cp] = value
         elif initials_source is not None:
             # Update from array-like structure, which we can only do if we
             # have the species available (e.g. not in network-free simulations)
             if not self.model.species:
                 raise ValueError(
                     'Cannot update initials from an array-like source without '
-                    'model species. ')
-            initials_dict = {}
+                    'model species.')
             for cp_idx, cp in enumerate(self.model.species):
-                initials_dict[cp] = [initials_source[n][cp_idx] for n in
-                                     range(len(initials_source))]
+                if any(existing_cp.is_equivalent_to(cp) for existing_cp in
+                       initials_dict):
+                    continue
+                initials_dict[cp] = [initials_source[n][cp_idx]
+                                     for n in range(len(initials_source))]
         return initials_dict
 
     @property
     def initials_dict(self):
         n_sims = self._check_run_initials_vs_base_initials_length()
         if n_sims == 1:
             n_sims = len(self.param_values)
-        initials_dict = {ic.pattern: [ic.value.value] * n_sims
-                         for ic in self.model.initials}
+
+        # Apply any per-run initial overrides
+        initials_dict = self._update_initials_dict({}, self._run_initials)
+
         # Apply any base initial overrides
         initials_dict = self._update_initials_dict(initials_dict,
                                                    self._initials)
-        # Apply any per-run initial overrides
-        initials_dict = self._update_initials_dict(initials_dict,
-                                                   self._run_initials)
+
+        model_initials = {ic.pattern: ic.value
+                          for ic in self.model.initials}
+
+        # Otherwise, populate initials from the model
+        n_sims_params = len(self.param_values)
+        n_sims_actual = max(n_sims_params, n_sims)
+
+        # Get remaining initials from the model itself and
+        # self.param_values, if necessary
+        subs = None
+        if any(isinstance(v, Expression) for v in model_initials.values()):
+            # Only need parameter substitutions if model initials include
+            # expressions
+            subs = [
+                dict((p, pv[i]) for i, p in
+                     enumerate(self._model.parameters))
+                for pv in self.param_values]
+            if len(subs) == 1 and n_sims_actual > 1:
+                subs = list(itertools.repeat(subs[0], n_sims_actual))
+
+        initials_dict = self._update_initials_dict(
+            initials_dict, model_initials, subs=subs
+        )
 
         return initials_dict
 
     def _check_run_initials_vs_base_initials_length(self):
         # Otherwise, build the list from the model, and any overrides
         # specified in self._initials and self._run_initials
         n_sims_initials = self._num_sims_calc(self._initials)
@@ -239,100 +275,29 @@
             if not isinstance(self._run_initials, collections.Mapping) and \
                     self._initials is None:
                 return self._run_initials
         elif not isinstance(self._initials, collections.Mapping) and \
                 self._initials is not None:
             return self._initials
 
-        n_sims_initials = self._check_run_initials_vs_base_initials_length()
-
         # At this point (after dimensionality check), we can return
         # self._run_initials if it's not a dictionary and not None
         if self._run_initials is not None and not isinstance(
                 self._run_initials, collections.Mapping):
             return self._run_initials
 
+        n_sims_initials = self._check_run_initials_vs_base_initials_length()
         n_sims_params = len(self.param_values)
         n_sims_actual = max(n_sims_params, n_sims_initials)
 
-        y0 = np.full((n_sims_actual, len(self.model.species)), np.nan)
-
-        # Process any overrides
-        y0 = self._update_y0(y0, self._run_initials)
-        y0 = self._update_y0(y0, self._initials)
-
-        # Fast NaN check with short circuit
-        if np.isnan(np.sum(y0)):
-            # Get remaining initials from the model itself and
-            # self.param_values, if necessary
-            subs = None
-            if self._model.expressions:
-                # Only need parameter substitutions if model has expressions
-                subs = [
-                    dict((p, pv[i]) for i, p in
-                         enumerate(self._model.parameters))
-                    for pv in self.param_values]
-                if len(subs) == 1 and n_sims_actual > 1:
-                    subs = list(itertools.repeat(subs[0], n_sims_actual))
-            ic_tuples = [(ic.pattern, ic.value) for ic in self._model.initials]
-            y0 = self._update_y0(y0, ic_tuples, subs, n_sims_params)
-
-        # Any remaining unset initials should be set to zero
-        y0 = np.nan_to_num(y0)
-
-        return y0
-
-    def _update_y0(self, y0, initials_source, subs=None, n_sims_params=None):
-        """ Update the initial conditions list y0 using initials_source """
-        if initials_source is None:
-            return y0
-
-        if isinstance(initials_source, np.ndarray) and \
-                initials_source.shape != 1:
-            # If initials_source is a multi-dimensional array, we can set
-            # the y0 values directly
-            nan_pos = np.isnan(y0)
-            y0[nan_pos] = initials_source[nan_pos]
-            return y0
-
-        if isinstance(initials_source, collections.Mapping):
-            initials_source = initials_source.items()
-
-        for cp, value_obj in initials_source:
-            cp = as_complex_pattern(cp)
-            si = self._model.get_species_index(cp)
-            if si is None:
-                raise IndexError("Species not found in model: %s" % repr(cp))
-
-            # Loop over all simulations
-            for sim in range(len(y0)):
-                # If this initial condition has already been set, skip it
-                if not np.isnan(y0[sim][si]):
-                    continue
-
-                if isinstance(value_obj, (collections.Sequence, np.ndarray))\
-                        and isinstance(value_obj[sim], numbers.Number):
-                    value = value_obj[sim]
-                elif isinstance(value_obj, Expression):
-                    value = value_obj.expand_expr().evalf(subs=subs[sim])
-                elif isinstance(value_obj, Parameter):
-                    if sim > 0 and n_sims_params == 1:
-                        # Parameters can be copied from previous
-                        # simulation if they have not been specified
-                        # explicitly in self.param_values
-                        value = y0[sim - 1][si]
-                    else:
-                        # Set parameter using param_values
-                        pi = self._model.parameters.index(value_obj)
-                        value = self.param_values[sim][pi]
-                else:
-                    raise TypeError("Unexpected initial condition "
-                                    "value type: %s" % type(value_obj))
+        y0 = np.full((n_sims_actual, len(self.model.species)), 0.0)
 
-                y0[sim][si] = value
+        for species, vals in self.initials_dict.items():
+            species_index = self._model.get_species_index(species)
+            y0[:, species_index] = vals
 
         return y0
 
     @initials.setter
     def initials(self, new_initials):
         self._initials = self._process_incoming_initials(new_initials)
```

### Comparing `pysb-1.9.0/pysb/simulator/bng.py` & `pysb-1.9.1/pysb/simulator/bng.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/simulator/cupsoda.py` & `pysb-1.9.1/pysb/simulator/cupsoda.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/simulator/scipyode.py` & `pysb-1.9.1/pysb/simulator/scipyode.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/simulator/stochkit.py` & `pysb-1.9.1/pysb/simulator/stochkit.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/testing/__init__.py` & `pysb-1.9.1/pysb/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/testing/modeltests.py` & `pysb-1.9.1/pysb/testing/modeltests.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/jacobian_runtimes.py` & `pysb-1.9.1/pysb/tests/jacobian_runtimes.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_bng.py` & `pysb-1.9.1/pysb/tests/test_bng.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_core.py` & `pysb-1.9.1/pysb/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_examples.py` & `pysb-1.9.1/pysb/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_exporters.py` & `pysb-1.9.1/pysb/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_expressions.py` & `pysb-1.9.1/pysb/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_importers.py` & `pysb-1.9.1/pysb/tests/test_importers.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_integrate.py` & `pysb-1.9.1/pysb/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_kappa.py` & `pysb-1.9.1/pysb/tests/test_kappa.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_merge.py` & `pysb-1.9.1/pysb/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_pattern.py` & `pysb-1.9.1/pysb/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_sensitivity_analysis.py` & `pysb-1.9.1/pysb/tests/test_sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_simulationresult.py` & `pysb-1.9.1/pysb/tests/test_simulationresult.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_simulator_cupsoda.py` & `pysb-1.9.1/pysb/tests/test_simulator_cupsoda.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_simulator_scipy.py` & `pysb-1.9.1/pysb/tests/test_simulator_scipy.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_simulator_stochkit.py` & `pysb-1.9.1/pysb/tests/test_simulator_stochkit.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tests/test_util.py` & `pysb-1.9.1/pysb/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tools/render_reactions.py` & `pysb-1.9.1/pysb/tools/render_reactions.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tools/render_species.py` & `pysb-1.9.1/pysb/tools/render_species.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tools/sensitivity_analysis.py` & `pysb-1.9.1/pysb/tools/sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/tools/species_graph.py` & `pysb-1.9.1/pysb/tools/species_graph.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb/util.py` & `pysb-1.9.1/pysb/util.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/pysb.egg-info/PKG-INFO` & `pysb-1.9.1/pysb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysb
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python Systems Biology modeling framework
 Home-page: http://pysb.org/
 Author: Jeremy Muhlich
 Author-email: jmuhlich@bitflood.org
 License: UNKNOWN
 Description: PySB
         ====
```

### Comparing `pysb-1.9.0/pysb.egg-info/SOURCES.txt` & `pysb-1.9.1/pysb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/scripts/pysb_export` & `pysb-1.9.1/scripts/pysb_export`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/setup.py` & `pysb-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pysb-1.9.0/versioneer.py` & `pysb-1.9.1/versioneer.py`

 * *Files identical despite different names*

