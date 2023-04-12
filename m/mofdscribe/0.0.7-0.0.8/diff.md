# Comparing `tmp/mofdscribe-0.0.7.tar.gz` & `tmp/mofdscribe-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mofdscribe-0.0.7.tar", last modified: Mon Dec 19 07:42:26 2022, max compression
+gzip compressed data, was "mofdscribe-0.0.8.tar", last modified: Wed Apr 12 13:53:58 2023, max compression
```

## Comparing `mofdscribe-0.0.7.tar` & `mofdscribe-0.0.8.tar`

### file list

```diff
@@ -1,316 +1,323 @@
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.093733 mofdscribe-0.0.7/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      610 2022-04-24 12:20:52.000000 mofdscribe-0.0.7/.cruft.json
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      193 2022-08-04 13:51:09.000000 mofdscribe-0.0.7/.deepsource.toml
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.991747 mofdscribe-0.0.7/.github/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.998355 mofdscribe-0.0.7/.github/workflows/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      609 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/.github/workflows/changelog.yml
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1912 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/.github/workflows/tests.yml
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7500 2022-06-14 20:20:46.000000 mofdscribe-0.0.7/.gitignore
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.998487 mofdscribe-0.0.7/.vscode/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       35 2022-04-15 08:00:12.000000 mofdscribe-0.0.7/.vscode/settings.json
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5235 2022-04-21 13:58:38.000000 mofdscribe-0.0.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1082 2022-03-18 08:16:05.000000 mofdscribe-0.0.7/LICENSE
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      347 2022-03-18 08:16:05.000000 mofdscribe-0.0.7/MANIFEST.in
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8146 2022-12-19 07:42:26.093847 mofdscribe-0.0.7/PKG-INFO
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6641 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/README.md
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.998957 mofdscribe-0.0.7/binder/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       34 2022-04-20 07:14:42.000000 mofdscribe-0.0.7/binder/postBuild
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       11 2022-04-20 07:14:42.000000 mofdscribe-0.0.7/binder/runtime.txt
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.999164 mofdscribe-0.0.7/dev_scripts/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5719 2022-08-10 07:47:47.000000 mofdscribe-0.0.7/dev_scripts/update_bench.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.999409 mofdscribe-0.0.7/docs/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      610 2022-04-20 07:14:42.000000 mofdscribe-0.0.7/docs/Makefile
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.002448 mofdscribe-0.0.7/docs/source/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.003905 mofdscribe-0.0.7/docs/source/api/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      693 2022-08-10 07:56:32.000000 mofdscribe-0.0.7/docs/source/api/bench.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      530 2022-12-12 17:03:24.000000 mofdscribe-0.0.7/docs/source/api/data.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2374 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/docs/source/api/featurizers.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       69 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/docs/source/api/helpers.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      139 2022-06-29 11:37:48.000000 mofdscribe-0.0.7/docs/source/api/metrics.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      143 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/docs/source/api/splitters.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      190 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/docs/source/api.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5420 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/docs/source/background.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10597 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/docs/source/conf.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3598 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/docs/source/contributing.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4907 2022-08-30 06:57:43.000000 mofdscribe-0.0.7/docs/source/dataleakage.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2929 2022-08-05 18:11:31.000000 mofdscribe-0.0.7/docs/source/datasets.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.992631 mofdscribe-0.0.7/docs/source/featurizers/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.004742 mofdscribe-0.0.7/docs/source/featurizers/atom_centered/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      703 2022-08-09 16:10:34.000000 mofdscribe-0.0.7/docs/source/featurizers/atom_centered/amd.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      580 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/docs/source/featurizers/atom_centered/ph.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1625 2022-08-02 22:12:21.000000 mofdscribe-0.0.7/docs/source/featurizers/atom_centered/racs.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.006168 mofdscribe-0.0.7/docs/source/featurizers/bu_centered/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      488 2022-08-12 10:52:46.000000 mofdscribe-0.0.7/docs/source/featurizers/bu_centered/distances.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      217 2022-08-12 10:52:50.000000 mofdscribe-0.0.7/docs/source/featurizers/bu_centered/flexibility.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      235 2022-08-12 10:52:53.000000 mofdscribe-0.0.7/docs/source/featurizers/bu_centered/lsop.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5170 2022-10-04 11:52:09.000000 mofdscribe-0.0.7/docs/source/featurizers/bu_centered/rdkit_derived.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      503 2022-08-12 10:53:00.000000 mofdscribe-0.0.7/docs/source/featurizers/bu_centered/sbu_match.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.008325 mofdscribe-0.0.7/docs/source/featurizers/global/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1047 2022-07-25 20:26:52.000000 mofdscribe-0.0.7/docs/source/featurizers/global/aprdf.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1212 2022-07-25 20:26:52.000000 mofdscribe-0.0.7/docs/source/featurizers/global/eqeq.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4505 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/docs/source/featurizers/global/ph.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3100 2022-07-25 20:26:52.000000 mofdscribe-0.0.7/docs/source/featurizers/global/pore.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      605 2022-08-03 06:11:38.000000 mofdscribe-0.0.7/docs/source/featurizers/global/price.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1550 2022-07-25 20:26:52.000000 mofdscribe-0.0.7/docs/source/featurizers/global/raspa.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      428 2022-07-25 20:26:52.000000 mofdscribe-0.0.7/docs/source/featurizers/global/voxel.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.008537 mofdscribe-0.0.7/docs/source/featurizers/host_guest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      756 2022-12-12 17:03:24.000000 mofdscribe-0.0.7/docs/source/featurizers/host_guest/host_guest_aprdf.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.019344 mofdscribe-0.0.7/docs/source/figures/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    85845 2022-04-21 07:47:07.000000 mofdscribe-0.0.7/docs/source/figures/ExamplePersistenceBalls3.svg
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   104828 2022-07-06 11:51:34.000000 mofdscribe-0.0.7/docs/source/figures/atomcentredph.png
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   508908 2022-04-23 19:09:21.000000 mofdscribe-0.0.7/docs/source/figures/energygrid.svg
--rw-rw-r--   0 kevinmaikjablonka   (501) staff       (20)   113956 2022-04-24 12:19:10.000000 mofdscribe-0.0.7/docs/source/figures/logo.png
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)  2189086 2022-07-06 15:57:35.000000 mofdscribe-0.0.7/docs/source/figures/persistent_image_chemistry.png
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    72244 2022-04-22 17:04:03.000000 mofdscribe-0.0.7/docs/source/figures/rays.png
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   276747 2022-08-04 20:27:55.000000 mofdscribe-0.0.7/docs/source/figures/show_structure.png
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   181216 2022-08-30 07:04:57.000000 mofdscribe-0.0.7/docs/source/figures/splits.png
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    13993 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/docs/source/getting_started.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1338 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/docs/source/index.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1538 2022-10-03 16:42:49.000000 mofdscribe-0.0.7/docs/source/installation.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1253 2022-08-10 07:34:33.000000 mofdscribe-0.0.7/docs/source/leaderboard.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.024031 mofdscribe-0.0.7/docs/source/leaderboards/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      891 2022-08-10 07:37:40.000000 mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.992908 mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.024967 mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9549 2022-08-10 07:51:28.000000 mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/R-RdedeuDkr20220810072203.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8920 2022-08-10 07:51:28.000000 mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNodu2d20220810070448.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8927 2022-08-10 07:51:28.000000 mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNoduJg20220810071815.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.993027 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.025877 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9551 2022-08-10 07:51:27.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RdedemHZA20220809154048.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8917 2022-08-10 07:51:27.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduVk20220809154016.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8928 2022-08-10 07:51:27.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduhB20220809154026.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.993147 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.026843 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9552 2022-08-10 07:51:27.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RdedeStm-20220809154539.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8930 2022-08-10 07:51:27.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduaC20220809154526.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8920 2022-08-10 07:51:27.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduww20220809154446.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8511 2022-08-09 18:19:53.000000 mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduzO20220809154518.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1174 2022-08-09 17:34:29.000000 mofdscribe-0.0.7/docs/source/leaderboards/logkH_CO2_id.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1139 2022-08-09 17:34:34.000000 mofdscribe-0.0.7/docs/source/leaderboards/logkH_CO2_ood.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      910 2022-08-10 07:42:42.000000 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.993270 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.027967 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9553 2022-08-10 07:51:28.000000 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RdedeLFjO20220809154725.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9615 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-Rden-CGnK20220817012931.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8928 2022-08-10 07:51:28.000000 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNodu9v20220809154701.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8919 2022-08-10 07:51:28.000000 mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNoduxg20220809154632.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      560 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/docs/source/maintaining.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7983 2022-12-12 17:03:24.000000 mofdscribe-0.0.7/docs/source/references.rst
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      791 2022-08-30 07:09:45.000000 mofdscribe-0.0.7/docs/source/splitters.rst
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.029301 mofdscribe-0.0.7/examples/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    43761 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/examples/add_model_to_leaderboard.ipynb
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   153919 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/examples/featurize.ipynb
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    80954 2022-08-05 18:11:31.000000 mofdscribe-0.0.7/examples/hyperparameter_optimization_in_bench.ipynb
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      365 2022-08-08 10:27:59.000000 mofdscribe-0.0.7/pyproject.toml
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3149 2022-12-19 07:42:26.094480 mofdscribe-0.0.7/setup.cfg
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      114 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/setup.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:25.993591 mofdscribe-0.0.7/src/
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.031035 mofdscribe-0.0.7/src/mofdscribe/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      113 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/src/mofdscribe/__init__.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.034327 mofdscribe-0.0.7/src/mofdscribe/bench/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      192 2022-08-10 08:17:18.000000 mofdscribe-0.0.7/src/mofdscribe/bench/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       75 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/src/mofdscribe/bench/bandgap.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2669 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/bench/ch4dc.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1433 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/bench/df_model.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2065 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/bench/dummy_models.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5211 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/bench/logkHCO2.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    12242 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/bench/mofbench.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2674 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/bench/pbegap.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1565 2022-08-09 14:52:14.000000 mofdscribe-0.0.7/src/mofdscribe/bench/watermark.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      176 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/constants.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.037421 mofdscribe-0.0.7/src/mofdscribe/datasets/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      230 2022-11-03 15:11:09.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9762 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/arabg_dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6364 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/arcmof_dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11044 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/bw_dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      789 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/checks.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11871 2022-12-12 17:03:24.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/core_dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5290 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    15653 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/qmof_dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    13069 2022-12-17 18:37:37.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/structuredataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10309 2022-12-12 17:03:24.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/thermal_stability_dataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2947 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/src/mofdscribe/datasets/utils.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.037955 mofdscribe-0.0.7/src/mofdscribe/featurizers/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1519 2022-08-12 11:12:22.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10226 2022-12-11 12:35:48.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/base.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.047426 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      804 2022-08-12 12:57:40.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9396 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/bu_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7762 2022-12-17 19:43:26.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/bu_matches.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2680 2022-10-03 16:42:49.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/compositionstats_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2795 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/distance_hist_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2139 2022-10-03 16:42:49.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/distance_stats_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4224 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/lsop_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5005 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/nconf20_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)  3088495 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/prototype_env.json
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4867 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/rdkitadaptor.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11262 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/shape_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4293 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/smarts_matches.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    27039 2022-12-17 22:08:21.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/utils.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.052610 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      471 2022-08-03 06:20:07.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5317 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/_fragment.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5875 2022-08-08 16:23:59.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/amd.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6298 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/aprdf.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.052900 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/data/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    16908 2022-08-04 12:36:21.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/data/elementprices.csv
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10727 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/energygrid.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8175 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/henry.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3614 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/partialchargehistogram.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3568 2022-10-04 11:52:09.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/partialchargestats.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4868 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/price.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11312 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/racs.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.053973 mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      208 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7396 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/guest_aprdf.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6933 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/host_guest_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2454 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/utils.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.055088 mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      348 2022-06-15 19:11:49.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10627 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/_voxelgrid.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    25605 2022-11-04 19:48:42.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/geometric_properties.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9585 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/voxelgrid.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.057052 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      320 2022-06-28 14:00:32.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11888 2022-12-17 21:45:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/_tda_helpers.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    12638 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/atom_centered_ph.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6995 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_hist.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11549 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_image.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6130 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_stats.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    13782 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_vect.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.060865 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1525 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3252 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/aggregators.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.061165 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/data/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    29477 2022-06-28 10:27:39.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/data/tuned_vesta.yml
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.061706 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/eqeq/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      931 2022-12-17 21:45:45.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/eqeq/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1168 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/extend.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1990 2022-12-12 07:38:47.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/histogram.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.064117 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-19 07:47:00.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    16816 2022-08-04 13:51:09.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/base_parser.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    12157 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/ff_builder.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    43624 2022-04-21 06:43:30.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/ff_data.yaml
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2182 2022-06-16 09:00:56.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/resize_uc.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3915 2022-11-08 09:54:40.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/run_raspa.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2326 2022-08-08 10:27:59.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/structure_graph.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2170 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/substructures.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      139 2022-08-04 12:39:04.000000 mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/tempdir.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      907 2022-12-19 07:41:05.000000 mofdscribe-0.0.7/src/mofdscribe/helpers.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.065445 mofdscribe-0.0.7/src/mofdscribe/metrics/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      226 2022-06-30 11:24:06.000000 mofdscribe-0.0.7/src/mofdscribe/metrics/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4055 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/src/mofdscribe/metrics/adverserial.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5046 2022-07-05 22:14:36.000000 mofdscribe-0.0.7/src/mofdscribe/metrics/metric_collection.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4010 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/src/mofdscribe/metrics/regression.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.067052 mofdscribe-0.0.7/src/mofdscribe/splitters/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      351 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/src/mofdscribe/splitters/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    49505 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/splitters/splitters.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    17851 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/src/mofdscribe/splitters/utils.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      190 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/src/mofdscribe/types.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1022 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/src/mofdscribe/version.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.031973 mofdscribe-0.0.7/src/mofdscribe.egg-info/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8146 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/src/mofdscribe.egg-info/PKG-INFO
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10490 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/src/mofdscribe.egg-info/SOURCES.txt
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        1 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/src/mofdscribe.egg-info/dependency_links.txt
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        1 2022-04-15 14:59:51.000000 mofdscribe-0.0.7/src/mofdscribe.egg-info/not-zip-safe
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      687 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/src/mofdscribe.egg-info/requires.txt
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       11 2022-12-19 07:42:25.000000 mofdscribe-0.0.7/src/mofdscribe.egg-info/top_level.txt
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.067930 mofdscribe-0.0.7/tests/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       60 2022-03-18 08:16:05.000000 mofdscribe-0.0.7/tests/__init__.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.068975 mofdscribe-0.0.7/tests/bench/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-07-05 12:29:02.000000 mofdscribe-0.0.7/tests/bench/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2795 2022-12-17 19:43:26.000000 mofdscribe-0.0.7/tests/bench/test_bench.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      637 2022-11-08 09:54:40.000000 mofdscribe-0.0.7/tests/bench/test_df_model.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      240 2022-08-09 13:55:19.000000 mofdscribe-0.0.7/tests/bench/test_watermark.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3424 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/conftest.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.071133 mofdscribe-0.0.7/tests/datasets/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-15 07:43:09.000000 mofdscribe-0.0.7/tests/datasets/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      827 2022-11-07 13:53:30.000000 mofdscribe-0.0.7/tests/datasets/test_arabg.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      812 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/datasets/test_arcmof.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      773 2022-08-08 10:27:59.000000 mofdscribe-0.0.7/tests/datasets/test_bw.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1107 2022-11-08 09:54:40.000000 mofdscribe-0.0.7/tests/datasets/test_core.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1259 2022-11-08 09:54:40.000000 mofdscribe-0.0.7/tests/datasets/test_qmof.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1720 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/tests/datasets/test_structuredataset.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1023 2022-12-12 17:03:24.000000 mofdscribe-0.0.7/tests/datasets/test_thermal_stability.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.072318 mofdscribe-0.0.7/tests/featurizers/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-29 09:20:30.000000 mofdscribe-0.0.7/tests/featurizers/__init__.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.076232 mofdscribe-0.0.7/tests/featurizers/bu/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-19 18:24:39.000000 mofdscribe-0.0.7/tests/featurizers/bu/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2416 2022-08-12 12:57:47.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_bu_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2387 2022-08-12 10:54:29.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_bu_matches.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      533 2022-08-12 10:54:50.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_composition_stats.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      636 2022-08-12 10:54:52.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_distance_hist_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      761 2022-08-12 10:54:54.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_distance_stats_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      526 2022-08-12 10:54:57.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_lsop_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      817 2022-08-12 10:54:59.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_nconf20_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      594 2022-08-12 10:55:02.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_rdkit_adaptor.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      433 2022-08-12 10:55:04.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_rdkit_converter.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      901 2022-10-04 11:52:09.000000 mofdscribe-0.0.7/tests/featurizers/bu/test_smarts_matches.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.078970 mofdscribe-0.0.7/tests/featurizers/chemistry/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       62 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      944 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_amd.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      538 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_aprdf.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      936 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_energygrid.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2596 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_fragment.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1088 2022-08-09 16:33:44.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_henry.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      686 2022-06-29 09:23:26.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_partialchargehistogram.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      741 2022-06-29 09:23:31.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_partialchargestats.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      597 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_price.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3480 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/tests/featurizers/chemistry/test_racs.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      243 2022-06-15 09:58:00.000000 mofdscribe-0.0.7/tests/featurizers/helpers.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.079568 mofdscribe-0.0.7/tests/featurizers/hostguest/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      386 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/tests/featurizers/hostguest/test_guest_aprdf.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      578 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/tests/featurizers/hostguest/test_host_guest_featurizer.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      587 2022-12-12 08:25:46.000000 mofdscribe-0.0.7/tests/featurizers/hostguest/test_utils.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.080092 mofdscribe-0.0.7/tests/featurizers/pore/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-15 07:53:47.000000 mofdscribe-0.0.7/tests/featurizers/pore/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5206 2022-08-08 13:16:08.000000 mofdscribe-0.0.7/tests/featurizers/pore/test_geometric_properties.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      347 2022-06-29 09:21:17.000000 mofdscribe-0.0.7/tests/featurizers/pore/test_voxelgrid.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1289 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/featurizers/test_aggregators.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2594 2022-08-08 11:38:41.000000 mofdscribe-0.0.7/tests/featurizers/test_base.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1395 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/featurizers/test_utils.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.081661 mofdscribe-0.0.7/tests/featurizers/topology/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-17 16:40:00.000000 mofdscribe-0.0.7/tests/featurizers/topology/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2794 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/featurizers/topology/test_atom_centered_ph.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1783 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/featurizers/topology/test_ph_hist.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1857 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/featurizers/topology/test_ph_image.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1783 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/featurizers/topology/test_ph_stats.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1936 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/featurizers/topology/test_ph_vect.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.082197 mofdscribe-0.0.7/tests/metrics/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-05-08 13:05:13.000000 mofdscribe-0.0.7/tests/metrics/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1913 2022-12-17 19:43:27.000000 mofdscribe-0.0.7/tests/metrics/test_adverserial.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1217 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/metrics/test_regression.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.082706 mofdscribe-0.0.7/tests/splitters/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-14 20:07:29.000000 mofdscribe-0.0.7/tests/splitters/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7208 2022-12-17 19:43:26.000000 mofdscribe-0.0.7/tests/splitters/test_splitters.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7450 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/splitters/test_utils.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.090269 mofdscribe-0.0.7/tests/test_files/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    20551 2022-06-10 16:23:28.000000 mofdscribe-0.0.7/tests/test_files/20450N2_ddec.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2671 2022-07-28 07:42:21.000000 mofdscribe-0.0.7/tests/test_files/ABACUF.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1963 2022-07-31 12:40:45.000000 mofdscribe-0.0.7/tests/test_files/BTC.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    39106 2022-08-29 19:29:26.000000 mofdscribe-0.0.7/tests/test_files/HKUST-1-La.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    30509 2022-07-29 13:49:12.000000 mofdscribe-0.0.7/tests/test_files/HKUST-1-linkers.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    39106 2022-04-16 13:37:53.000000 mofdscribe-0.0.7/tests/test_files/HKUST-1.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    16763 2022-04-16 16:38:00.000000 mofdscribe-0.0.7/tests/test_files/IRMOF-1.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)  1180643 2022-04-21 15:39:38.000000 mofdscribe-0.0.7/tests/test_files/asci_grid_C_co2.grid
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    26694 2022-04-26 05:42:36.000000 mofdscribe-0.0.7/tests/test_files/floating_check.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3171 2022-06-30 15:46:03.000000 mofdscribe-0.0.7/tests/test_files/linker_molecule.json
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.090599 mofdscribe-0.0.7/tests/test_files/test_dataset/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   257123 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/test_files/test_dataset/data.json
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.092406 mofdscribe-0.0.7/tests/test_files/test_dataset/structures/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4557 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ABAVIJ.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    26299 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ABAYIO.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    26293 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ABAYOU.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4904 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/test_files/test_dataset/structures/CUXJEM.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11955 2022-11-04 13:44:10.000000 mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ZUWXUM.cif
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2599 2022-06-28 11:12:21.000000 mofdscribe-0.0.7/tests/test_files/test_molecule.json
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7581 2022-06-28 11:08:34.000000 mofdscribe-0.0.7/tests/test_files/test_molecule_graph.json
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1231 2022-06-30 12:58:02.000000 mofdscribe-0.0.7/tests/test_files/triangle_structure.json
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      404 2022-06-15 09:58:06.000000 mofdscribe-0.0.7/tests/test_version.py
-drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2022-12-19 07:42:26.093490 mofdscribe-0.0.7/tests/utils/
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-17 08:58:20.000000 mofdscribe-0.0.7/tests/utils/__init__.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      335 2022-06-29 12:52:59.000000 mofdscribe-0.0.7/tests/utils/test_raspa.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      490 2022-07-30 10:59:11.000000 mofdscribe-0.0.7/tests/utils/test_structure_graph.py
--rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      762 2022-08-04 12:39:05.000000 mofdscribe-0.0.7/tests/utils/test_substructures.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.191926 mofdscribe-0.0.8/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      610 2022-04-24 12:20:52.000000 mofdscribe-0.0.8/.cruft.json
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      193 2022-08-04 13:51:09.000000 mofdscribe-0.0.8/.deepsource.toml
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.081494 mofdscribe-0.0.8/.github/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.090368 mofdscribe-0.0.8/.github/workflows/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      609 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/.github/workflows/changelog.yml
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1912 2022-12-19 07:41:05.000000 mofdscribe-0.0.8/.github/workflows/tests.yml
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7500 2022-06-14 20:20:46.000000 mofdscribe-0.0.8/.gitignore
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.090834 mofdscribe-0.0.8/.vscode/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       35 2022-04-15 08:00:12.000000 mofdscribe-0.0.8/.vscode/settings.json
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5235 2022-04-21 13:58:38.000000 mofdscribe-0.0.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1082 2022-03-18 08:16:05.000000 mofdscribe-0.0.8/LICENSE
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      347 2022-03-18 08:16:05.000000 mofdscribe-0.0.8/MANIFEST.in
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8146 2023-04-12 13:53:58.192060 mofdscribe-0.0.8/PKG-INFO
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6641 2022-12-19 07:41:05.000000 mofdscribe-0.0.8/README.md
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.091472 mofdscribe-0.0.8/binder/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       34 2022-04-20 07:14:42.000000 mofdscribe-0.0.8/binder/postBuild
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       11 2022-04-20 07:14:42.000000 mofdscribe-0.0.8/binder/runtime.txt
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.091909 mofdscribe-0.0.8/dev_scripts/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5719 2022-08-10 07:47:47.000000 mofdscribe-0.0.8/dev_scripts/update_bench.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.092212 mofdscribe-0.0.8/docs/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      610 2022-04-20 07:14:42.000000 mofdscribe-0.0.8/docs/Makefile
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.096027 mofdscribe-0.0.8/docs/source/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.098318 mofdscribe-0.0.8/docs/source/api/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      693 2022-08-10 07:56:32.000000 mofdscribe-0.0.8/docs/source/api/bench.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      530 2022-12-12 17:03:24.000000 mofdscribe-0.0.8/docs/source/api/data.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2500 2023-03-22 08:51:27.000000 mofdscribe-0.0.8/docs/source/api/featurizers.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       69 2022-12-19 07:41:05.000000 mofdscribe-0.0.8/docs/source/api/helpers.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      139 2022-06-29 11:37:48.000000 mofdscribe-0.0.8/docs/source/api/metrics.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      143 2022-07-31 12:40:45.000000 mofdscribe-0.0.8/docs/source/api/splitters.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      190 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/api.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5420 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/background.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10597 2023-04-12 13:53:57.000000 mofdscribe-0.0.8/docs/source/conf.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3598 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/contributing.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4907 2022-08-30 06:57:43.000000 mofdscribe-0.0.8/docs/source/dataleakage.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2929 2022-08-05 18:11:31.000000 mofdscribe-0.0.8/docs/source/datasets.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.082516 mofdscribe-0.0.8/docs/source/featurizers/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.099342 mofdscribe-0.0.8/docs/source/featurizers/atom_centered/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      703 2022-08-09 16:10:34.000000 mofdscribe-0.0.8/docs/source/featurizers/atom_centered/amd.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      580 2022-07-31 12:40:45.000000 mofdscribe-0.0.8/docs/source/featurizers/atom_centered/ph.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1625 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/featurizers/atom_centered/racs.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.100987 mofdscribe-0.0.8/docs/source/featurizers/bu_centered/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      488 2022-08-12 10:52:46.000000 mofdscribe-0.0.8/docs/source/featurizers/bu_centered/distances.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      217 2022-08-12 10:52:50.000000 mofdscribe-0.0.8/docs/source/featurizers/bu_centered/flexibility.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      235 2022-08-12 10:52:53.000000 mofdscribe-0.0.8/docs/source/featurizers/bu_centered/lsop.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5170 2022-10-04 11:52:09.000000 mofdscribe-0.0.8/docs/source/featurizers/bu_centered/rdkit_derived.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      503 2022-08-12 10:53:00.000000 mofdscribe-0.0.8/docs/source/featurizers/bu_centered/sbu_match.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.103533 mofdscribe-0.0.8/docs/source/featurizers/global/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1047 2022-07-25 20:26:52.000000 mofdscribe-0.0.8/docs/source/featurizers/global/aprdf.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1212 2022-07-25 20:26:52.000000 mofdscribe-0.0.8/docs/source/featurizers/global/eqeq.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4505 2022-08-29 19:29:26.000000 mofdscribe-0.0.8/docs/source/featurizers/global/ph.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3100 2022-07-25 20:26:52.000000 mofdscribe-0.0.8/docs/source/featurizers/global/pore.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      605 2022-08-03 06:11:38.000000 mofdscribe-0.0.8/docs/source/featurizers/global/price.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1550 2022-07-25 20:26:52.000000 mofdscribe-0.0.8/docs/source/featurizers/global/raspa.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      335 2023-03-22 08:51:27.000000 mofdscribe-0.0.8/docs/source/featurizers/global/text.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      428 2022-07-25 20:26:52.000000 mofdscribe-0.0.8/docs/source/featurizers/global/voxel.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.103922 mofdscribe-0.0.8/docs/source/featurizers/host_guest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      756 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/featurizers/host_guest/host_guest_aprdf.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.116102 mofdscribe-0.0.8/docs/source/figures/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    85845 2022-04-21 07:47:07.000000 mofdscribe-0.0.8/docs/source/figures/ExamplePersistenceBalls3.svg
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   104828 2022-07-06 11:51:34.000000 mofdscribe-0.0.8/docs/source/figures/atomcentredph.png
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   508908 2022-04-23 19:09:21.000000 mofdscribe-0.0.8/docs/source/figures/energygrid.svg
+-rw-rw-r--   0 kevinmaikjablonka   (501) staff       (20)   113956 2022-04-24 12:19:10.000000 mofdscribe-0.0.8/docs/source/figures/logo.png
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)  2189086 2022-07-06 15:57:35.000000 mofdscribe-0.0.8/docs/source/figures/persistent_image_chemistry.png
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    72244 2022-04-22 17:04:03.000000 mofdscribe-0.0.8/docs/source/figures/rays.png
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   276747 2022-08-04 20:27:55.000000 mofdscribe-0.0.8/docs/source/figures/show_structure.png
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   181216 2022-08-30 07:04:57.000000 mofdscribe-0.0.8/docs/source/figures/splits.png
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    13993 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/getting_started.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1338 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/index.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1538 2022-10-03 16:42:49.000000 mofdscribe-0.0.8/docs/source/installation.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1253 2022-08-10 07:34:33.000000 mofdscribe-0.0.8/docs/source/leaderboard.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.117884 mofdscribe-0.0.8/docs/source/leaderboards/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      891 2022-08-10 07:37:40.000000 mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.082876 mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.118861 mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9549 2022-08-10 07:51:28.000000 mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/R-RdedeuDkr20220810072203.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8920 2022-08-10 07:51:28.000000 mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNodu2d20220810070448.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8927 2022-08-10 07:51:28.000000 mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNoduJg20220810071815.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.083043 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.119781 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9551 2022-08-10 07:51:27.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RdedemHZA20220809154048.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8917 2022-08-10 07:51:27.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduVk20220809154016.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8928 2022-08-10 07:51:27.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduhB20220809154026.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.083234 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.121111 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9552 2022-08-10 07:51:27.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RdedeStm-20220809154539.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8930 2022-08-10 07:51:27.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduaC20220809154526.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8920 2022-08-10 07:51:27.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduww20220809154446.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8511 2022-08-09 18:19:53.000000 mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduzO20220809154518.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1174 2022-08-09 17:34:29.000000 mofdscribe-0.0.8/docs/source/leaderboards/logkH_CO2_id.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1139 2022-08-09 17:34:34.000000 mofdscribe-0.0.8/docs/source/leaderboards/logkH_CO2_ood.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      910 2022-08-10 07:42:42.000000 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.083432 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.122288 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9553 2022-08-10 07:51:28.000000 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RdedeLFjO20220809154725.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9615 2022-08-29 19:29:26.000000 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-Rden-CGnK20220817012931.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8928 2022-08-10 07:51:28.000000 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNodu9v20220809154701.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8919 2022-08-10 07:51:28.000000 mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNoduxg20220809154632.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      560 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/docs/source/maintaining.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7983 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/docs/source/references.rst
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      791 2022-08-30 07:09:45.000000 mofdscribe-0.0.8/docs/source/splitters.rst
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.123887 mofdscribe-0.0.8/examples/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    43761 2022-08-29 19:29:26.000000 mofdscribe-0.0.8/examples/add_model_to_leaderboard.ipynb
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   153919 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/examples/featurize.ipynb
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    80954 2022-08-05 18:11:31.000000 mofdscribe-0.0.8/examples/hyperparameter_optimization_in_bench.ipynb
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      365 2022-08-08 10:27:59.000000 mofdscribe-0.0.8/pyproject.toml
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3149 2023-04-12 13:53:58.193738 mofdscribe-0.0.8/setup.cfg
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      114 2022-08-04 12:39:04.000000 mofdscribe-0.0.8/setup.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.083811 mofdscribe-0.0.8/src/
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.126145 mofdscribe-0.0.8/src/mofdscribe/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      113 2022-12-19 07:41:05.000000 mofdscribe-0.0.8/src/mofdscribe/__init__.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.129892 mofdscribe-0.0.8/src/mofdscribe/bench/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      192 2022-08-10 08:17:18.000000 mofdscribe-0.0.8/src/mofdscribe/bench/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       75 2022-07-31 12:40:45.000000 mofdscribe-0.0.8/src/mofdscribe/bench/bandgap.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2669 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/src/mofdscribe/bench/ch4dc.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1433 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/bench/df_model.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2065 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/src/mofdscribe/bench/dummy_models.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5211 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/src/mofdscribe/bench/logkHCO2.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    12242 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/src/mofdscribe/bench/mofbench.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2674 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/src/mofdscribe/bench/pbegap.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1565 2022-08-09 14:52:14.000000 mofdscribe-0.0.8/src/mofdscribe/bench/watermark.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      176 2022-08-04 12:39:04.000000 mofdscribe-0.0.8/src/mofdscribe/constants.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.133164 mofdscribe-0.0.8/src/mofdscribe/datasets/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      230 2022-11-03 15:11:09.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9762 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/arabg_dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6364 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/arcmof_dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11044 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/bw_dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      789 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/checks.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11871 2022-12-12 17:03:24.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/core_dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5290 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    15653 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/qmof_dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    13069 2022-12-17 18:37:37.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/structuredataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10309 2022-12-12 17:03:24.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/thermal_stability_dataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2947 2022-08-29 19:29:26.000000 mofdscribe-0.0.8/src/mofdscribe/datasets/utils.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.133744 mofdscribe-0.0.8/src/mofdscribe/featurizers/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1519 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10226 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/base.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.141110 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      804 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9396 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/bu_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7762 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/bu_matches.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2680 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/compositionstats_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2795 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/distance_hist_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2139 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/distance_stats_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4224 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/lsop_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5005 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/nconf20_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)  3088495 2022-07-31 12:40:45.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/prototype_env.json
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4867 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/rdkitadaptor.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11262 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/shape_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4293 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/smarts_matches.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    27039 2022-12-17 22:08:21.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/utils.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.144772 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      471 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5317 2022-08-04 12:39:04.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/_fragment.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5875 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/amd.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6298 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/aprdf.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.144967 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/data/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    16908 2022-08-04 12:36:21.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/data/elementprices.csv
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10727 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/energygrid.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8175 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/henry.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3614 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/partialchargehistogram.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3568 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/partialchargestats.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4868 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/price.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11312 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/racs.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.146263 mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      208 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7396 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/guest_aprdf.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6933 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/host_guest_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2454 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/utils.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.147548 mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      348 2022-06-15 19:11:49.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10627 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/_voxelgrid.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    25605 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/geometric_properties.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     9585 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/voxelgrid.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.147999 mofdscribe-0.0.8/src/mofdscribe/featurizers/text/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2023-03-22 08:51:27.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/text/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5841 2023-04-12 13:53:39.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/text/mofdscriber.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.149663 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      320 2022-06-28 14:00:32.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11888 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/_tda_helpers.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    12638 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/atom_centered_ph.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6995 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_hist.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11549 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_image.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     6130 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_stats.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    13782 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_vect.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.151266 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1525 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3252 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/aggregators.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.151603 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/data/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    29477 2022-06-28 10:27:39.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/data/tuned_vesta.yml
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.152166 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/eqeq/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      931 2022-12-17 21:45:45.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/eqeq/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1168 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/extend.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1990 2022-12-12 07:38:47.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/histogram.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.154268 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-19 07:47:00.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    16816 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/base_parser.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    12157 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/ff_builder.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    43624 2022-04-21 06:43:30.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/ff_data.yaml
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2182 2022-06-16 09:00:56.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/resize_uc.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3915 2022-11-08 09:54:40.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/run_raspa.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2326 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/structure_graph.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2170 2022-08-04 12:39:04.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/substructures.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      139 2022-08-04 12:39:04.000000 mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/tempdir.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      907 2022-12-19 07:41:05.000000 mofdscribe-0.0.8/src/mofdscribe/helpers.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.155512 mofdscribe-0.0.8/src/mofdscribe/metrics/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      226 2022-06-30 11:24:06.000000 mofdscribe-0.0.8/src/mofdscribe/metrics/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4055 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/src/mofdscribe/metrics/adverserial.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5046 2022-07-05 22:14:36.000000 mofdscribe-0.0.8/src/mofdscribe/metrics/metric_collection.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4010 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/src/mofdscribe/metrics/regression.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.156997 mofdscribe-0.0.8/src/mofdscribe/splitters/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      351 2022-07-31 12:40:45.000000 mofdscribe-0.0.8/src/mofdscribe/splitters/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    49505 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/splitters/splitters.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    17851 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/src/mofdscribe/splitters/utils.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      190 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/src/mofdscribe/types.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1022 2023-04-12 13:53:57.000000 mofdscribe-0.0.8/src/mofdscribe/version.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.127359 mofdscribe-0.0.8/src/mofdscribe.egg-info/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     8146 2023-04-12 13:53:58.000000 mofdscribe-0.0.8/src/mofdscribe.egg-info/PKG-INFO
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    10699 2023-04-12 13:53:58.000000 mofdscribe-0.0.8/src/mofdscribe.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        1 2023-04-12 13:53:58.000000 mofdscribe-0.0.8/src/mofdscribe.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        1 2022-04-15 14:59:51.000000 mofdscribe-0.0.8/src/mofdscribe.egg-info/not-zip-safe
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      687 2023-04-12 13:53:58.000000 mofdscribe-0.0.8/src/mofdscribe.egg-info/requires.txt
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       11 2023-04-12 13:53:58.000000 mofdscribe-0.0.8/src/mofdscribe.egg-info/top_level.txt
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.157921 mofdscribe-0.0.8/tests/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       60 2022-03-18 08:16:05.000000 mofdscribe-0.0.8/tests/__init__.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.159045 mofdscribe-0.0.8/tests/bench/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-07-05 12:29:02.000000 mofdscribe-0.0.8/tests/bench/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2795 2022-12-17 19:43:26.000000 mofdscribe-0.0.8/tests/bench/test_bench.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      637 2022-11-08 09:54:40.000000 mofdscribe-0.0.8/tests/bench/test_df_model.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      240 2022-08-09 13:55:19.000000 mofdscribe-0.0.8/tests/bench/test_watermark.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3424 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/conftest.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.161394 mofdscribe-0.0.8/tests/datasets/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-15 07:43:09.000000 mofdscribe-0.0.8/tests/datasets/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      827 2022-11-07 13:53:30.000000 mofdscribe-0.0.8/tests/datasets/test_arabg.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      812 2022-08-29 19:29:26.000000 mofdscribe-0.0.8/tests/datasets/test_arcmof.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      773 2022-08-08 10:27:59.000000 mofdscribe-0.0.8/tests/datasets/test_bw.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1107 2022-11-08 09:54:40.000000 mofdscribe-0.0.8/tests/datasets/test_core.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1259 2022-11-08 09:54:40.000000 mofdscribe-0.0.8/tests/datasets/test_qmof.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1720 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/tests/datasets/test_structuredataset.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1023 2022-12-12 17:03:24.000000 mofdscribe-0.0.8/tests/datasets/test_thermal_stability.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.163333 mofdscribe-0.0.8/tests/featurizers/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-29 09:20:30.000000 mofdscribe-0.0.8/tests/featurizers/__init__.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.166987 mofdscribe-0.0.8/tests/featurizers/bu/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-19 18:24:39.000000 mofdscribe-0.0.8/tests/featurizers/bu/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2416 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_bu_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2387 2022-08-12 10:54:29.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_bu_matches.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      533 2022-08-12 10:54:50.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_composition_stats.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      636 2022-08-12 10:54:52.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_distance_hist_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      761 2022-08-12 10:54:54.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_distance_stats_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      526 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_lsop_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      817 2022-08-12 10:54:59.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_nconf20_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      594 2022-08-12 10:55:02.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_rdkit_adaptor.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      433 2022-08-12 10:55:04.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_rdkit_converter.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      901 2022-10-04 11:52:09.000000 mofdscribe-0.0.8/tests/featurizers/bu/test_smarts_matches.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.169623 mofdscribe-0.0.8/tests/featurizers/chemistry/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)       62 2022-07-31 12:40:45.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      944 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_amd.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      538 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_aprdf.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      936 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_energygrid.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2596 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_fragment.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1088 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_henry.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      686 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_partialchargehistogram.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      741 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_partialchargestats.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      597 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_price.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3480 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/chemistry/test_racs.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      243 2022-06-15 09:58:00.000000 mofdscribe-0.0.8/tests/featurizers/helpers.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.172049 mofdscribe-0.0.8/tests/featurizers/hostguest/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      386 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/hostguest/test_guest_aprdf.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      578 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/hostguest/test_host_guest_featurizer.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      587 2022-12-12 08:25:46.000000 mofdscribe-0.0.8/tests/featurizers/hostguest/test_utils.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.172585 mofdscribe-0.0.8/tests/featurizers/pore/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-15 07:53:47.000000 mofdscribe-0.0.8/tests/featurizers/pore/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     5206 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/pore/test_geometric_properties.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      347 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/pore/test_voxelgrid.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1289 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/featurizers/test_aggregators.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2594 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/test_base.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1395 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/tests/featurizers/test_utils.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.172896 mofdscribe-0.0.8/tests/featurizers/text/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2023-03-22 08:51:27.000000 mofdscribe-0.0.8/tests/featurizers/text/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      296 2023-03-22 08:51:27.000000 mofdscribe-0.0.8/tests/featurizers/text/test_mofdscriber.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.174040 mofdscribe-0.0.8/tests/featurizers/topology/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-17 16:40:00.000000 mofdscribe-0.0.8/tests/featurizers/topology/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2794 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/topology/test_atom_centered_ph.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1783 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/topology/test_ph_hist.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1857 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/topology/test_ph_image.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1783 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/topology/test_ph_stats.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1936 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/featurizers/topology/test_ph_vect.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.174716 mofdscribe-0.0.8/tests/metrics/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-05-08 13:05:13.000000 mofdscribe-0.0.8/tests/metrics/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1913 2022-12-17 19:43:27.000000 mofdscribe-0.0.8/tests/metrics/test_adverserial.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1217 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/tests/metrics/test_regression.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.175260 mofdscribe-0.0.8/tests/splitters/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-06-14 20:07:29.000000 mofdscribe-0.0.8/tests/splitters/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7208 2023-04-12 13:53:34.000000 mofdscribe-0.0.8/tests/splitters/test_splitters.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7450 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/tests/splitters/test_utils.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.186788 mofdscribe-0.0.8/tests/test_files/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    20551 2022-06-10 16:23:28.000000 mofdscribe-0.0.8/tests/test_files/20450N2_ddec.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2671 2022-07-28 07:42:21.000000 mofdscribe-0.0.8/tests/test_files/ABACUF.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1963 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/test_files/BTC.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    39106 2022-08-29 19:29:26.000000 mofdscribe-0.0.8/tests/test_files/HKUST-1-La.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    30509 2022-07-29 13:49:12.000000 mofdscribe-0.0.8/tests/test_files/HKUST-1-linkers.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    39106 2022-04-16 13:37:53.000000 mofdscribe-0.0.8/tests/test_files/HKUST-1.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    16763 2022-04-16 16:38:00.000000 mofdscribe-0.0.8/tests/test_files/IRMOF-1.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)  1180643 2022-04-21 15:39:38.000000 mofdscribe-0.0.8/tests/test_files/asci_grid_C_co2.grid
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    26694 2022-04-26 05:42:36.000000 mofdscribe-0.0.8/tests/test_files/floating_check.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     3171 2022-06-30 15:46:03.000000 mofdscribe-0.0.8/tests/test_files/linker_molecule.json
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.187214 mofdscribe-0.0.8/tests/test_files/test_dataset/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)   257123 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/test_files/test_dataset/data.json
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.190474 mofdscribe-0.0.8/tests/test_files/test_dataset/structures/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4557 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ABAVIJ.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    26299 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ABAYIO.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    26293 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ABAYOU.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     4904 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/test_files/test_dataset/structures/CUXJEM.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)    11955 2022-11-04 13:44:10.000000 mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ZUWXUM.cif
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     2599 2022-06-28 11:12:21.000000 mofdscribe-0.0.8/tests/test_files/test_molecule.json
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     7581 2022-06-28 11:08:34.000000 mofdscribe-0.0.8/tests/test_files/test_molecule_graph.json
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)     1231 2022-06-30 12:58:02.000000 mofdscribe-0.0.8/tests/test_files/triangle_structure.json
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      404 2022-06-15 09:58:06.000000 mofdscribe-0.0.8/tests/test_version.py
+drwxr-xr-x   0 kevinmaikjablonka   (501) staff       (20)        0 2023-04-12 13:53:58.191631 mofdscribe-0.0.8/tests/utils/
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)        0 2022-04-17 08:58:20.000000 mofdscribe-0.0.8/tests/utils/__init__.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      335 2022-06-29 12:52:59.000000 mofdscribe-0.0.8/tests/utils/test_raspa.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      490 2023-03-18 13:53:10.000000 mofdscribe-0.0.8/tests/utils/test_structure_graph.py
+-rw-r--r--   0 kevinmaikjablonka   (501) staff       (20)      762 2022-08-04 12:39:05.000000 mofdscribe-0.0.8/tests/utils/test_substructures.py
```

### Comparing `mofdscribe-0.0.7/.cruft.json` & `mofdscribe-0.0.8/.cruft.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/.github/workflows/changelog.yml` & `mofdscribe-0.0.8/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/.github/workflows/tests.yml` & `mofdscribe-0.0.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/.gitignore` & `mofdscribe-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/CODE_OF_CONDUCT.md` & `mofdscribe-0.0.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/LICENSE` & `mofdscribe-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/PKG-INFO` & `mofdscribe-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofdscribe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Ecosystem for digital reticular chemistry
 Home-page: https://github.com/kjappelbaum/mofdscribe
 Download-URL: https://github.com/kjappelbaum/mofdscribe/releases
 Author: Kevin M. Jablonka
 Author-email: mail@kjablonka.com
 Maintainer: Kevin M. Jablonka
 Maintainer-email: mail@kjablonka.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mofdscribe Version: 0.0.7 Summary: Ecosystem for
+Metadata-Version: 2.1 Name: mofdscribe Version: 0.0.8 Summary: Ecosystem for
 digital reticular chemistry Home-page: https://github.com/kjappelbaum/
 mofdscribe Download-URL: https://github.com/kjappelbaum/mofdscribe/releases
 Author: Kevin M. Jablonka Author-email: mail@kjablonka.com Maintainer: Kevin M.
 Jablonka Maintainer-email: mail@kjablonka.com License: MIT Project-URL: Bug
 Tracker, https://github.com/kjappelbaum/mofdscribe/issues Project-URL: Source
 Code, https://github.com/kjappelbaum/mofdscribe Keywords: mof,machine-
 learning,descriptors,featurization,reticular-chemistry Classifier: Development
```

### Comparing `mofdscribe-0.0.7/README.md` & `mofdscribe-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/dev_scripts/update_bench.py` & `mofdscribe-0.0.8/dev_scripts/update_bench.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/Makefile` & `mofdscribe-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/api/bench.rst` & `mofdscribe-0.0.8/docs/source/api/bench.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/api/data.rst` & `mofdscribe-0.0.8/docs/source/api/data.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/api/featurizers.rst` & `mofdscribe-0.0.8/docs/source/api/featurizers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -90,8 +90,15 @@
     :members:
 
 
 Host Guest featurization
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. automodule:: mofdscribe.featurizers.hostguest.host_guest_featurizer
+    :members:
+
+
+Text description
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. automodule:: mofdscribe.featurizers.text.mofdscriber
     :members:
```

### Comparing `mofdscribe-0.0.7/docs/source/background.rst` & `mofdscribe-0.0.8/docs/source/background.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/conf.py` & `mofdscribe-0.0.8/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "mofdscribe"
 copyright = f"{date.today().year}, Kevin M. Jablonka"
 author = "Kevin M. Jablonka"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.0.7"
+release = "0.0.8"
 
 # The short X.Y version.
 parsed_version = re.match(
     r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand(r"\g<major>.\g<minor>.\g<patch>")
```

### Comparing `mofdscribe-0.0.7/docs/source/contributing.rst` & `mofdscribe-0.0.8/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/dataleakage.rst` & `mofdscribe-0.0.8/docs/source/dataleakage.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/datasets.rst` & `mofdscribe-0.0.8/docs/source/datasets.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/atom_centered/amd.rst` & `mofdscribe-0.0.8/docs/source/featurizers/atom_centered/amd.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/atom_centered/ph.rst` & `mofdscribe-0.0.8/docs/source/featurizers/atom_centered/ph.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/atom_centered/racs.rst` & `mofdscribe-0.0.8/docs/source/featurizers/atom_centered/racs.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/bu_centered/rdkit_derived.rst` & `mofdscribe-0.0.8/docs/source/featurizers/bu_centered/rdkit_derived.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/global/aprdf.rst` & `mofdscribe-0.0.8/docs/source/featurizers/global/aprdf.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/global/eqeq.rst` & `mofdscribe-0.0.8/docs/source/featurizers/global/eqeq.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/global/ph.rst` & `mofdscribe-0.0.8/docs/source/featurizers/global/ph.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/global/pore.rst` & `mofdscribe-0.0.8/docs/source/featurizers/global/pore.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/global/price.rst` & `mofdscribe-0.0.8/docs/source/featurizers/global/price.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/global/raspa.rst` & `mofdscribe-0.0.8/docs/source/featurizers/global/raspa.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/featurizers/host_guest/host_guest_aprdf.rst` & `mofdscribe-0.0.8/docs/source/featurizers/host_guest/host_guest_aprdf.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/ExamplePersistenceBalls3.svg` & `mofdscribe-0.0.8/docs/source/figures/ExamplePersistenceBalls3.svg`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/atomcentredph.png` & `mofdscribe-0.0.8/docs/source/figures/atomcentredph.png`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/energygrid.svg` & `mofdscribe-0.0.8/docs/source/figures/energygrid.svg`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/logo.png` & `mofdscribe-0.0.8/docs/source/figures/logo.png`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/persistent_image_chemistry.png` & `mofdscribe-0.0.8/docs/source/figures/persistent_image_chemistry.png`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/rays.png` & `mofdscribe-0.0.8/docs/source/figures/rays.png`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/show_structure.png` & `mofdscribe-0.0.8/docs/source/figures/show_structure.png`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/figures/splits.png` & `mofdscribe-0.0.8/docs/source/figures/splits.png`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/getting_started.rst` & `mofdscribe-0.0.8/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/index.rst` & `mofdscribe-0.0.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/installation.rst` & `mofdscribe-0.0.8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboard.rst` & `mofdscribe-0.0.8/docs/source/leaderboard.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/R-RdedeuDkr20220810072203.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/R-RdedeuDkr20220810072203.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNodu2d20220810070448.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNodu2d20220810070448.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNoduJg20220810071815.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/ch4dc_id_models/latest/R-RduNoduJg20220810071815.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RdedemHZA20220809154048.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RdedemHZA20220809154048.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduVk20220809154016.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduVk20220809154016.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduhB20220809154026.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_id_models/latest/R-RduNoduhB20220809154026.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RdedeStm-20220809154539.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RdedeStm-20220809154539.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduaC20220809154526.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduaC20220809154526.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduww20220809154446.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduww20220809154446.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduzO20220809154518.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logKH_CO2_ood_models/latest/R-RduNoduzO20220809154518.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logkH_CO2_id.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logkH_CO2_id.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/logkH_CO2_ood.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/logkH_CO2_ood.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RdedeLFjO20220809154725.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RdedeLFjO20220809154725.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-Rden-CGnK20220817012931.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-Rden-CGnK20220817012931.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNodu9v20220809154701.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNodu9v20220809154701.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNoduxg20220809154632.rst` & `mofdscribe-0.0.8/docs/source/leaderboards/pbe_bandgap_id_models/latest/R-RduNoduxg20220809154632.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/maintaining.rst` & `mofdscribe-0.0.8/docs/source/maintaining.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/references.rst` & `mofdscribe-0.0.8/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/docs/source/splitters.rst` & `mofdscribe-0.0.8/docs/source/splitters.rst`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/examples/add_model_to_leaderboard.ipynb` & `mofdscribe-0.0.8/examples/add_model_to_leaderboard.ipynb`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/examples/featurize.ipynb` & `mofdscribe-0.0.8/examples/featurize.ipynb`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/examples/hyperparameter_optimization_in_bench.ipynb` & `mofdscribe-0.0.8/examples/hyperparameter_optimization_in_bench.ipynb`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/setup.cfg` & `mofdscribe-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mofdscribe
-version = 0.0.7
+version = 0.0.8
 description = Ecosystem for digital reticular chemistry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kjappelbaum/mofdscribe
 download_url = https://github.com/kjappelbaum/mofdscribe/releases
 project_urls = 
 	Bug Tracker = https://github.com/kjappelbaum/mofdscribe/issues
```

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/ch4dc.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/ch4dc.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/df_model.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/df_model.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/dummy_models.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/dummy_models.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/logkHCO2.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/logkHCO2.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/mofbench.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/mofbench.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/pbegap.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/pbegap.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/bench/watermark.py` & `mofdscribe-0.0.8/src/mofdscribe/bench/watermark.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/arabg_dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/arabg_dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/arcmof_dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/arcmof_dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/bw_dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/bw_dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/checks.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/checks.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/core_dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/core_dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/qmof_dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/qmof_dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/structuredataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/structuredataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/thermal_stability_dataset.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/thermal_stability_dataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/datasets/utils.py` & `mofdscribe-0.0.8/src/mofdscribe/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/__init__.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/base.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/base.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/__init__.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/__init__.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/bu_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/bu_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/bu_matches.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/bu_matches.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/compositionstats_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/compositionstats_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/distance_hist_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/distance_hist_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/distance_stats_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/distance_stats_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/lsop_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/lsop_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/nconf20_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/nconf20_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/prototype_env.json` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/prototype_env.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/rdkitadaptor.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/rdkitadaptor.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/shape_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/shape_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/smarts_matches.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/smarts_matches.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/bu/utils.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/bu/utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/_fragment.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/_fragment.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/amd.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/amd.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/aprdf.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/aprdf.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/data/elementprices.csv` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/data/elementprices.csv`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/energygrid.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/energygrid.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/henry.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/henry.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/partialchargehistogram.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/partialchargehistogram.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/partialchargestats.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/partialchargestats.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/price.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/price.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/chemistry/racs.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/chemistry/racs.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/guest_aprdf.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/guest_aprdf.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/host_guest_featurizer.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/host_guest_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/hostguest/utils.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/hostguest/utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/_voxelgrid.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/_voxelgrid.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/geometric_properties.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/geometric_properties.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/pore/voxelgrid.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/pore/voxelgrid.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/_tda_helpers.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/_tda_helpers.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/atom_centered_ph.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/atom_centered_ph.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_hist.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_hist.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_image.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_image.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_stats.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_stats.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/topology/ph_vect.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/topology/ph_vect.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/__init__.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/aggregators.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/aggregators.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/data/tuned_vesta.yml` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/data/tuned_vesta.yml`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/eqeq/__init__.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/eqeq/__init__.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/extend.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/extend.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/histogram.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/base_parser.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/base_parser.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/ff_builder.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/ff_builder.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/ff_data.yaml` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/ff_data.yaml`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/resize_uc.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/resize_uc.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/raspa/run_raspa.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/raspa/run_raspa.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/structure_graph.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/structure_graph.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/featurizers/utils/substructures.py` & `mofdscribe-0.0.8/src/mofdscribe/featurizers/utils/substructures.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/helpers.py` & `mofdscribe-0.0.8/src/mofdscribe/helpers.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/metrics/adverserial.py` & `mofdscribe-0.0.8/src/mofdscribe/metrics/adverserial.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/metrics/metric_collection.py` & `mofdscribe-0.0.8/src/mofdscribe/metrics/metric_collection.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/metrics/regression.py` & `mofdscribe-0.0.8/src/mofdscribe/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/splitters/splitters.py` & `mofdscribe-0.0.8/src/mofdscribe/splitters/splitters.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/splitters/utils.py` & `mofdscribe-0.0.8/src/mofdscribe/splitters/utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/src/mofdscribe/version.py` & `mofdscribe-0.0.8/src/mofdscribe/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`mofdscribe` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `mofdscribe-0.0.7/src/mofdscribe.egg-info/PKG-INFO` & `mofdscribe-0.0.8/src/mofdscribe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofdscribe
-Version: 0.0.7
+Version: 0.0.8
 Summary: Ecosystem for digital reticular chemistry
 Home-page: https://github.com/kjappelbaum/mofdscribe
 Download-URL: https://github.com/kjappelbaum/mofdscribe/releases
 Author: Kevin M. Jablonka
 Author-email: mail@kjablonka.com
 Maintainer: Kevin M. Jablonka
 Maintainer-email: mail@kjablonka.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mofdscribe Version: 0.0.7 Summary: Ecosystem for
+Metadata-Version: 2.1 Name: mofdscribe Version: 0.0.8 Summary: Ecosystem for
 digital reticular chemistry Home-page: https://github.com/kjappelbaum/
 mofdscribe Download-URL: https://github.com/kjappelbaum/mofdscribe/releases
 Author: Kevin M. Jablonka Author-email: mail@kjablonka.com Maintainer: Kevin M.
 Jablonka Maintainer-email: mail@kjablonka.com License: MIT Project-URL: Bug
 Tracker, https://github.com/kjappelbaum/mofdscribe/issues Project-URL: Source
 Code, https://github.com/kjappelbaum/mofdscribe Keywords: mof,machine-
 learning,descriptors,featurization,reticular-chemistry Classifier: Development
```

### Comparing `mofdscribe-0.0.7/src/mofdscribe.egg-info/SOURCES.txt` & `mofdscribe-0.0.8/src/mofdscribe.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 docs/source/featurizers/bu_centered/sbu_match.rst
 docs/source/featurizers/global/aprdf.rst
 docs/source/featurizers/global/eqeq.rst
 docs/source/featurizers/global/ph.rst
 docs/source/featurizers/global/pore.rst
 docs/source/featurizers/global/price.rst
 docs/source/featurizers/global/raspa.rst
+docs/source/featurizers/global/text.rst
 docs/source/featurizers/global/voxel.rst
 docs/source/featurizers/host_guest/host_guest_aprdf.rst
 docs/source/figures/ExamplePersistenceBalls3.svg
 docs/source/figures/atomcentredph.png
 docs/source/figures/energygrid.svg
 docs/source/figures/logo.png
 docs/source/figures/persistent_image_chemistry.png
@@ -140,14 +141,16 @@
 src/mofdscribe/featurizers/hostguest/guest_aprdf.py
 src/mofdscribe/featurizers/hostguest/host_guest_featurizer.py
 src/mofdscribe/featurizers/hostguest/utils.py
 src/mofdscribe/featurizers/pore/__init__.py
 src/mofdscribe/featurizers/pore/_voxelgrid.py
 src/mofdscribe/featurizers/pore/geometric_properties.py
 src/mofdscribe/featurizers/pore/voxelgrid.py
+src/mofdscribe/featurizers/text/__init__.py
+src/mofdscribe/featurizers/text/mofdscriber.py
 src/mofdscribe/featurizers/topology/__init__.py
 src/mofdscribe/featurizers/topology/_tda_helpers.py
 src/mofdscribe/featurizers/topology/atom_centered_ph.py
 src/mofdscribe/featurizers/topology/ph_hist.py
 src/mofdscribe/featurizers/topology/ph_image.py
 src/mofdscribe/featurizers/topology/ph_stats.py
 src/mofdscribe/featurizers/topology/ph_vect.py
@@ -216,14 +219,16 @@
 tests/featurizers/chemistry/test_racs.py
 tests/featurizers/hostguest/test_guest_aprdf.py
 tests/featurizers/hostguest/test_host_guest_featurizer.py
 tests/featurizers/hostguest/test_utils.py
 tests/featurizers/pore/__init__.py
 tests/featurizers/pore/test_geometric_properties.py
 tests/featurizers/pore/test_voxelgrid.py
+tests/featurizers/text/__init__.py
+tests/featurizers/text/test_mofdscriber.py
 tests/featurizers/topology/__init__.py
 tests/featurizers/topology/test_atom_centered_ph.py
 tests/featurizers/topology/test_ph_hist.py
 tests/featurizers/topology/test_ph_image.py
 tests/featurizers/topology/test_ph_stats.py
 tests/featurizers/topology/test_ph_vect.py
 tests/metrics/__init__.py
```

### Comparing `mofdscribe-0.0.7/src/mofdscribe.egg-info/requires.txt` & `mofdscribe-0.0.8/src/mofdscribe.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/bench/test_bench.py` & `mofdscribe-0.0.8/tests/bench/test_bench.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/bench/test_df_model.py` & `mofdscribe-0.0.8/tests/bench/test_df_model.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/conftest.py` & `mofdscribe-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_arabg.py` & `mofdscribe-0.0.8/tests/datasets/test_arabg.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_arcmof.py` & `mofdscribe-0.0.8/tests/datasets/test_arcmof.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_bw.py` & `mofdscribe-0.0.8/tests/datasets/test_bw.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_core.py` & `mofdscribe-0.0.8/tests/datasets/test_core.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_qmof.py` & `mofdscribe-0.0.8/tests/datasets/test_qmof.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_structuredataset.py` & `mofdscribe-0.0.8/tests/datasets/test_structuredataset.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/datasets/test_thermal_stability.py` & `mofdscribe-0.0.8/tests/datasets/test_thermal_stability.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_bu_featurizer.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_bu_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_bu_matches.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_bu_matches.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_composition_stats.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_composition_stats.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_distance_hist_featurizer.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_distance_hist_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_distance_stats_featurizer.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_distance_stats_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_lsop_featurizer.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_lsop_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_nconf20_featurizer.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_nconf20_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_rdkit_adaptor.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_rdkit_adaptor.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/bu/test_smarts_matches.py` & `mofdscribe-0.0.8/tests/featurizers/bu/test_smarts_matches.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_amd.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_amd.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_aprdf.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_aprdf.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_energygrid.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_energygrid.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_fragment.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_fragment.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_henry.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_henry.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_partialchargehistogram.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_partialchargehistogram.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_partialchargestats.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_partialchargestats.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_price.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_price.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/chemistry/test_racs.py` & `mofdscribe-0.0.8/tests/featurizers/chemistry/test_racs.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/hostguest/test_host_guest_featurizer.py` & `mofdscribe-0.0.8/tests/featurizers/hostguest/test_host_guest_featurizer.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/hostguest/test_utils.py` & `mofdscribe-0.0.8/tests/featurizers/hostguest/test_utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/pore/test_geometric_properties.py` & `mofdscribe-0.0.8/tests/featurizers/pore/test_geometric_properties.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/test_aggregators.py` & `mofdscribe-0.0.8/tests/featurizers/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/test_base.py` & `mofdscribe-0.0.8/tests/featurizers/test_base.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/test_utils.py` & `mofdscribe-0.0.8/tests/featurizers/test_utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/topology/test_atom_centered_ph.py` & `mofdscribe-0.0.8/tests/featurizers/topology/test_atom_centered_ph.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/topology/test_ph_hist.py` & `mofdscribe-0.0.8/tests/featurizers/topology/test_ph_hist.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/topology/test_ph_image.py` & `mofdscribe-0.0.8/tests/featurizers/topology/test_ph_image.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/topology/test_ph_stats.py` & `mofdscribe-0.0.8/tests/featurizers/topology/test_ph_stats.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/featurizers/topology/test_ph_vect.py` & `mofdscribe-0.0.8/tests/featurizers/topology/test_ph_vect.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/metrics/test_adverserial.py` & `mofdscribe-0.0.8/tests/metrics/test_adverserial.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/metrics/test_regression.py` & `mofdscribe-0.0.8/tests/metrics/test_regression.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/splitters/test_splitters.py` & `mofdscribe-0.0.8/tests/splitters/test_splitters.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/splitters/test_utils.py` & `mofdscribe-0.0.8/tests/splitters/test_utils.py`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/20450N2_ddec.cif` & `mofdscribe-0.0.8/tests/test_files/20450N2_ddec.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/ABACUF.cif` & `mofdscribe-0.0.8/tests/test_files/ABACUF.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/BTC.cif` & `mofdscribe-0.0.8/tests/test_files/BTC.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/HKUST-1-La.cif` & `mofdscribe-0.0.8/tests/test_files/HKUST-1-La.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/HKUST-1-linkers.cif` & `mofdscribe-0.0.8/tests/test_files/HKUST-1-linkers.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/HKUST-1.cif` & `mofdscribe-0.0.8/tests/test_files/HKUST-1.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/IRMOF-1.cif` & `mofdscribe-0.0.8/tests/test_files/IRMOF-1.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/asci_grid_C_co2.grid` & `mofdscribe-0.0.8/tests/test_files/asci_grid_C_co2.grid`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/floating_check.cif` & `mofdscribe-0.0.8/tests/test_files/floating_check.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/linker_molecule.json` & `mofdscribe-0.0.8/tests/test_files/linker_molecule.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_dataset/data.json` & `mofdscribe-0.0.8/tests/test_files/test_dataset/data.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ABAVIJ.cif` & `mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ABAVIJ.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ABAYIO.cif` & `mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ABAYIO.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ABAYOU.cif` & `mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ABAYOU.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_dataset/structures/CUXJEM.cif` & `mofdscribe-0.0.8/tests/test_files/test_dataset/structures/CUXJEM.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_dataset/structures/ZUWXUM.cif` & `mofdscribe-0.0.8/tests/test_files/test_dataset/structures/ZUWXUM.cif`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_molecule.json` & `mofdscribe-0.0.8/tests/test_files/test_molecule.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/test_molecule_graph.json` & `mofdscribe-0.0.8/tests/test_files/test_molecule_graph.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/test_files/triangle_structure.json` & `mofdscribe-0.0.8/tests/test_files/triangle_structure.json`

 * *Files identical despite different names*

### Comparing `mofdscribe-0.0.7/tests/utils/test_substructures.py` & `mofdscribe-0.0.8/tests/utils/test_substructures.py`

 * *Files identical despite different names*

