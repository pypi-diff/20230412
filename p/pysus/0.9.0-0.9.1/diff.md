# Comparing `tmp/pysus-0.9.0.tar.gz` & `tmp/pysus-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysus-0.9.0.tar", max compression
+gzip compressed data, was "pysus-0.9.1.tar", max compression
```

## Comparing `pysus-0.9.0.tar` & `pysus-0.9.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    35149 2023-03-28 18:39:09.918351 pysus-0.9.0/LICENSE
--rw-r--r--   0        0        0     1204 2023-03-28 18:41:12.385499 pysus-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     8421 2023-03-28 18:39:09.958351 pysus-0.9.0/pysus/Notebooks/Analyzing SIH.ipynb
--rw-r--r--   0        0        0  1092118 2023-03-28 18:39:09.962351 pysus-0.9.0/pysus/Notebooks/Analyzing SIM.ipynb
--rw-r--r--   0        0        0    14877 2023-03-28 18:39:09.962351 pysus-0.9.0/pysus/Notebooks/Analyzing SINASC Data.ipynb
--rw-r--r--   0        0        0    47374 2023-03-28 18:39:09.962351 pysus-0.9.0/pysus/Notebooks/Getting_CNES_Data.ipynb
--rw-r--r--   0        0        0     5309 2023-03-28 18:39:09.962351 pysus-0.9.0/pysus/Notebooks/Processing SIM with municipality.ipynb
--rw-r--r--   0        0        0    30724 2023-03-28 18:39:09.962351 pysus-0.9.0/pysus/Notebooks/Processing SIM.ipynb
--rw-r--r--   0        0        0    59869 2023-03-28 18:39:09.962351 pysus-0.9.0/pysus/Notebooks/SINAN.ipynb
--rw-r--r--   0        0        0      422 2023-03-28 18:41:12.385499 pysus-0.9.0/pysus/__init__.py
--rw-r--r--   0        0        0   165526 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/dataset/geocode_by_cities.json
--rw-r--r--   0        0        0     3931 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/ANIM.tar.gz
--rw-r--r--   0        0        0     7064 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/BOTU.tar.gz
--rw-r--r--   0        0        0     5341 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/CHAG.tar.gz
--rw-r--r--   0        0        0     5439 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/CHIK.tar.gz
--rw-r--r--   0        0        0     5290 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/COLE.tar.gz
--rw-r--r--   0        0        0     4496 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/COQU.tar.gz
--rw-r--r--   0        0        0     5439 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/DENG.tar.gz
--rw-r--r--   0        0        0     5093 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/DIFT.tar.gz
--rw-r--r--   0        0        0     2953 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/ESQU.tar.gz
--rw-r--r--   0        0        0     5257 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/FAMA.tar.gz
--rw-r--r--   0        0        0     4638 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/FMAC.tar.gz
--rw-r--r--   0        0        0     6354 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/FTIF.tar.gz
--rw-r--r--   0        0        0     4247 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/HANS.tar.gz
--rw-r--r--   0        0        0     6202 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/HANT.tar.gz
--rw-r--r--   0        0        0     5603 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/HEPA.tar.gz
--rw-r--r--   0        0        0     4554 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/IEXO.tar.gz
--rw-r--r--   0        0        0     4214 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/LEIV.tar.gz
--rw-r--r--   0        0        0     4958 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/LEPT.tar.gz
--rw-r--r--   0        0        0     4293 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/LTAN.tar.gz
--rw-r--r--   0        0        0     3614 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/MALA.tar.gz
--rw-r--r--   0        0        0     5652 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/MENI.tar.gz
--rw-r--r--   0        0        0     3114 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/PEST.tar.gz
--rw-r--r--   0        0        0     5404 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/RAIV.tar.gz
--rw-r--r--   0        0        0     5439 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/SIFC.tar.gz
--rw-r--r--   0        0        0     1952 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/SIFG.tar.gz
--rw-r--r--   0        0        0     4189 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/TETA.tar.gz
--rw-r--r--   0        0        0     5518 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/TETN.tar.gz
--rw-r--r--   0        0        0     5659 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/TUBE.tar.gz
--rw-r--r--   0        0        0    35103 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/metadata/SINAN/typecast.py
--rw-r--r--   0        0        0      766 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/CIHA.py
--rw-r--r--   0        0        0     2277 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/CNES.py
--rw-r--r--   0        0        0     3074 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/ESUS.py
--rw-r--r--   0        0        0    13567 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/IBGE.py
--rw-r--r--   0        0        0     3171 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/Infodengue.py
--rw-r--r--   0        0        0      695 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/Infogripe.py
--rw-r--r--   0        0        0     1016 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/PNI.py
--rw-r--r--   0        0        0     2382 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/SIA.py
--rw-r--r--   0        0        0      847 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/SIH.py
--rw-r--r--   0        0        0     6675 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/SIM.py
--rw-r--r--   0        0        0     1688 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/SINAN.py
--rw-r--r--   0        0        0    24446 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/__init__.py
--rw-r--r--   0        0        0      790 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/sinasc.py
--rw-r--r--   0        0        0     3677 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/online_data/vaccine.py
--rw-r--r--   0        0        0     1922 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/preprocessing/ESUS.py
--rw-r--r--   0        0        0     6289 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/preprocessing/SIM.py
--rw-r--r--   0        0        0      128 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/preprocessing/__init__.py
--rw-r--r--   0        0        0    10129 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/preprocessing/decoders.py
--rw-r--r--   0        0        0     2402 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/preprocessing/geodata.py
--rw-r--r--   0        0        0     3878 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/preprocessing/sinan.py
--rw-r--r--   0        0        0      128 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/tests/__init__.py
--rw-r--r--   0        0        0      505 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/tests/test_SIA.py
--rw-r--r--   0        0        0      722 2023-03-28 18:39:09.966351 pysus-0.9.0/pysus/tests/test_cnes.py
--rw-r--r--   0        0        0  9175254 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/EPR-2016-06-01-2016.dbf
--rw-r--r--   0        0        0       66 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/__init__.py
--rw-r--r--   0        0        0     3126 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_Infodengue.py
--rw-r--r--   0        0        0      330 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_Infogripe.py
--rw-r--r--   0        0        0      640 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_PNI.py
--rw-r--r--   0        0        0      795 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_ciha.py
--rw-r--r--   0        0        0     2265 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_sia.py
--rw-r--r--   0        0        0      547 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_sih.py
--rw-r--r--   0        0        0     1249 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_sim.py
--rw-r--r--   0        0        0     4622 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_sinan.py
--rw-r--r--   0        0        0      785 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_sinasc.py
--rw-r--r--   0        0        0      419 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_data/test_vaccine.py
--rw-r--r--   0        0        0     6975 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_decoders.py
--rw-r--r--   0        0        0      304 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_esus.py
--rw-r--r--   0        0        0     1382 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_ibge.py
--rw-r--r--   0        0        0      741 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_init.py
--rw-r--r--   0        0        0      642 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_sih.py
--rw-r--r--   0        0        0     2123 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_sim.py
--rw-r--r--   0        0        0      758 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/tests/test_utilities.py
--rw-r--r--   0        0        0        0 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/utilities/__init__.py
--rw-r--r--   0        0        0     2766 2023-03-28 18:39:09.994351 pysus-0.9.0/pysus/utilities/readdbc.py
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 pysus-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 20:41:44.705570 pysus-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1372 2023-04-12 20:43:37.110119 pysus-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8421 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Analyzing SIH.ipynb
+-rw-r--r--   0        0        0    15450 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Analyzing SIM.ipynb
+-rw-r--r--   0        0        0    14877 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Analyzing SINASC Data.ipynb
+-rw-r--r--   0        0        0    47374 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Getting_CNES_Data.ipynb
+-rw-r--r--   0        0        0     3057 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Processing SIM with municipality.ipynb
+-rw-r--r--   0        0        0    27870 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/Processing SIM.ipynb
+-rw-r--r--   0        0        0    59869 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/Notebooks/SINAN.ipynb
+-rw-r--r--   0        0        0      422 2023-04-12 20:43:37.106119 pysus-0.9.1/pysus/__init__.py
+-rw-r--r--   0        0        0   165526 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/dataset/geocode_by_cities.json
+-rw-r--r--   0        0        0     3931 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/ANIM.tar.gz
+-rw-r--r--   0        0        0     7064 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/BOTU.tar.gz
+-rw-r--r--   0        0        0     5341 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/CHAG.tar.gz
+-rw-r--r--   0        0        0     5439 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/CHIK.tar.gz
+-rw-r--r--   0        0        0     5290 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/COLE.tar.gz
+-rw-r--r--   0        0        0     4496 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/COQU.tar.gz
+-rw-r--r--   0        0        0     5439 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/DENG.tar.gz
+-rw-r--r--   0        0        0     5093 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/DIFT.tar.gz
+-rw-r--r--   0        0        0     2953 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/ESQU.tar.gz
+-rw-r--r--   0        0        0     5257 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/FAMA.tar.gz
+-rw-r--r--   0        0        0     4638 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/FMAC.tar.gz
+-rw-r--r--   0        0        0     6354 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/FTIF.tar.gz
+-rw-r--r--   0        0        0     4247 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/HANS.tar.gz
+-rw-r--r--   0        0        0     6202 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/HANT.tar.gz
+-rw-r--r--   0        0        0     5603 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/HEPA.tar.gz
+-rw-r--r--   0        0        0     4554 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/IEXO.tar.gz
+-rw-r--r--   0        0        0     4214 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/LEIV.tar.gz
+-rw-r--r--   0        0        0     4958 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/LEPT.tar.gz
+-rw-r--r--   0        0        0     4293 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/LTAN.tar.gz
+-rw-r--r--   0        0        0     3614 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/MALA.tar.gz
+-rw-r--r--   0        0        0     5652 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/MENI.tar.gz
+-rw-r--r--   0        0        0     3114 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/PEST.tar.gz
+-rw-r--r--   0        0        0     5404 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/RAIV.tar.gz
+-rw-r--r--   0        0        0     5439 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/SIFC.tar.gz
+-rw-r--r--   0        0        0     1952 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/SIFG.tar.gz
+-rw-r--r--   0        0        0     4189 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/TETA.tar.gz
+-rw-r--r--   0        0        0     5518 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/TETN.tar.gz
+-rw-r--r--   0        0        0     5659 2023-04-12 20:41:44.749570 pysus-0.9.1/pysus/metadata/SINAN/TUBE.tar.gz
+-rw-r--r--   0        0        0    35103 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/metadata/SINAN/typecast.py
+-rw-r--r--   0        0        0      766 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/CIHA.py
+-rw-r--r--   0        0        0     2277 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/CNES.py
+-rw-r--r--   0        0        0     3074 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/ESUS.py
+-rw-r--r--   0        0        0    13567 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/IBGE.py
+-rw-r--r--   0        0        0     3170 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/Infodengue.py
+-rw-r--r--   0        0        0      695 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/Infogripe.py
+-rw-r--r--   0        0        0     1016 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/PNI.py
+-rw-r--r--   0        0        0     2382 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SIA.py
+-rw-r--r--   0        0        0      847 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SIH.py
+-rw-r--r--   0        0        0     6675 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SIM.py
+-rw-r--r--   0        0        0     1688 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/SINAN.py
+-rw-r--r--   0        0        0    24424 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/__init__.py
+-rw-r--r--   0        0        0      790 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/sinasc.py
+-rw-r--r--   0        0        0     3677 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/online_data/vaccine.py
+-rw-r--r--   0        0        0     1922 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/ESUS.py
+-rw-r--r--   0        0        0     6289 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/SIM.py
+-rw-r--r--   0        0        0      128 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/__init__.py
+-rw-r--r--   0        0        0    10109 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/decoders.py
+-rw-r--r--   0        0        0     2402 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/geodata.py
+-rw-r--r--   0        0        0     3878 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/preprocessing/sinan.py
+-rw-r--r--   0        0        0      128 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/tests/__init__.py
+-rw-r--r--   0        0        0      505 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/tests/test_SIA.py
+-rw-r--r--   0        0        0      722 2023-04-12 20:41:44.753570 pysus-0.9.1/pysus/tests/test_cnes.py
+-rw-r--r--   0        0        0  9175254 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/EPR-2016-06-01-2016.dbf
+-rw-r--r--   0        0        0       66 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     3126 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_Infodengue.py
+-rw-r--r--   0        0        0      330 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_Infogripe.py
+-rw-r--r--   0        0        0      640 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_PNI.py
+-rw-r--r--   0        0        0      795 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_ciha.py
+-rw-r--r--   0        0        0     2265 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sia.py
+-rw-r--r--   0        0        0      547 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sih.py
+-rw-r--r--   0        0        0     1249 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sim.py
+-rw-r--r--   0        0        0     4624 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sinan.py
+-rw-r--r--   0        0        0      785 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_sinasc.py
+-rw-r--r--   0        0        0      419 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_data/test_vaccine.py
+-rw-r--r--   0        0        0     6975 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_decoders.py
+-rw-r--r--   0        0        0      304 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_esus.py
+-rw-r--r--   0        0        0     1382 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_ibge.py
+-rw-r--r--   0        0        0      741 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_init.py
+-rw-r--r--   0        0        0      642 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_sih.py
+-rw-r--r--   0        0        0     2123 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_sim.py
+-rw-r--r--   0        0        0      758 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/tests/test_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/utilities/__init__.py
+-rw-r--r--   0        0        0     2766 2023-04-12 20:41:44.781571 pysus-0.9.1/pysus/utilities/readdbc.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 pysus-0.9.1/PKG-INFO
```

### Comparing `pysus-0.9.0/LICENSE` & `pysus-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pyproject.toml` & `pysus-0.9.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "pysus"
-version = "0.9.0"  # changed by semantic-release
+version = "0.9.1"  # changed by semantic-release
 description = "Tools for dealing with Brazil's Public health data"
 authors = ["Flavio Codeco Coelho <fccoelho@gmail.com>"]
 license = "GPL"
 
 packages = [{include='pysus'}]
 
 [tool.poetry.dependencies]
 cffi = "1.15.1"
 dbfread = "2.0.7"
-elasticsearch = "^8.3.3"
 fastparquet = "^0.8.1"
 geocoder = "^1.38.1"
 jupyterlab = "^3.4.5"
 numpy = "1.23.2"
 pandas = "1.4.3"
 pyarrow = ">=11.0.0"
 pycparser = "2.21"
@@ -24,22 +23,31 @@
 pytz = "2022.2.1"
 six = "1.16.0"
 tqdm = "4.64.0"
 wget = "^3.2"
 loguru = "^0.6.0"
 Unidecode = "^1.3.6"
 sqlalchemy = "<2.0.0"
+elasticsearch = "7.16.2"
+ipykernel = "^6.22.0"
+geobr = "^0.2.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pytest = ">=6.1.0"
 black = "^22.6.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 pre-commit = "^2.20.0"
-pytest = "^5.2"
 sphinx = "^5.1.1"
+nbmake = "^1.4.1"
+matplotlib = "^3.7.1"
+folium = "^0.14.0"
+seaborn = "^0.12.2"
+descartes = "^1.1.0"
+keplergl = "^0.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `pysus-0.9.0/pysus/Notebooks/Analyzing SIH.ipynb` & `pysus-0.9.1/pysus/Notebooks/Analyzing SIH.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/Notebooks/Analyzing SINASC Data.ipynb` & `pysus-0.9.1/pysus/Notebooks/Analyzing SINASC Data.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/Notebooks/Getting_CNES_Data.ipynb` & `pysus-0.9.1/pysus/Notebooks/Getting_CNES_Data.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/Notebooks/Processing SIM.ipynb` & `pysus-0.9.1/pysus/Notebooks/Processing SIM.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9713649068825493%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1}, 2: {'execution_count': 2, 'outputs': {0: {'data': "*

 * *            "{'text/plain': {insert: [(0, '      contador  ORIGEM  TIPOBITO   DTOBITO  HORAOBITO  "*

 * *            "NATURAL    DTNASC  \\\\\\n'), (1, '0     1         1       2         06082010  "*

 * *            "2000       831      09041945   \\n'), (2, '1     2         1       2         "*

 * *            "06082010  1300       812      20011912   \\n'), (3, '2     3         1       "*

 * *            "2         02102010  1700     […]*

```diff
@@ -5,26 +5,26 @@
             "metadata": {},
             "source": [
                 "## Processin SIM data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from pysus.online_data import SIM, parquets_to_dataframe\n",
                 "from pysus.preprocessing.decoders import translate_variables_SIM\n",
                 "from pysus.preprocessing.SIM import group_and_count, redistribute_missing, redistribute_cid_chapter"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -334,229 +334,122 @@
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>3009 rows \u00d7 59 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "     contador ORIGEM TIPOBITO   DTOBITO HORAOBITO NATURAL    DTNASC IDADE  \\\n",
-                            "0           1      1        2  06082010      2000     831  09041945   465   \n",
-                            "1           2      1        2  06082010      1300     812  20011912   498   \n",
-                            "2           3      1        2  02102010      1700     812  17032010   306   \n",
-                            "3           4      1        2  07042010      2300          07042010   005   \n",
-                            "4           5      1        2  13052010      0030     812  04081971   438   \n",
-                            "...       ...    ...      ...       ...       ...     ...       ...   ...   \n",
-                            "3004     3005      1        2  28092010      0100          20041958   452   \n",
-                            "3005     3006      1        2  14102010      1015          24031928   482   \n",
-                            "3006     3007      1        2  21112010      0650          11121955   454   \n",
-                            "3007     3008      1        2  10112010      0500          07071955   455   \n",
-                            "3008     3009      1        2  10102010      1240          07051976   434   \n",
-                            "\n",
-                            "     SEXO RACACOR  ... DTCADASTRO ATESTANTE FONTEINV DTRECEBIM UFINFORM  \\\n",
-                            "0       2          ...   19082010                     20092010            \n",
-                            "1       1          ...   19082010                  2  01102010            \n",
-                            "2       2       4  ...   05012011         3           10022011            \n",
-                            "3       2       1  ...   06052010         1           20072010            \n",
-                            "4       1       1  ...   21062010         5           20072010            \n",
-                            "...   ...     ...  ...        ...       ...      ...       ...      ...   \n",
-                            "3004    2       4  ...   20102010                     11112010            \n",
-                            "3005    1       1  ...   06122010         2           19012011            \n",
-                            "3006    2       1  ...   09122010         5           17012011            \n",
-                            "3007    1       1  ...   04012011         2           19012011            \n",
-                            "3008    2       4  ...   28122010         2           26112010            \n",
-                            "\n",
-                            "     CB_PRE MORTEPARTO DTCADINF TPOBITOCOR DTCADINV  \n",
-                            "0       R98                                          \n",
-                            "1       R98                                          \n",
-                            "2       R98                                          \n",
-                            "3      O689                                          \n",
-                            "4      X999                                          \n",
-                            "...     ...        ...      ...        ...      ...  \n",
-                            "3004   I619                                          \n",
-                            "3005   I219                                          \n",
-                            "3006   C349                                          \n",
-                            "3007   C787                                          \n",
-                            "3008   I739                                          \n",
+                            "      contador  ORIGEM  TIPOBITO   DTOBITO  HORAOBITO  NATURAL    DTNASC  \\\n",
+                            "0     1         1       2         06082010  2000       831      09041945   \n",
+                            "1     2         1       2         06082010  1300       812      20011912   \n",
+                            "2     3         1       2         02102010  1700       812      17032010   \n",
+                            "3     4         1       2         07042010  2300                07042010   \n",
+                            "4     5         1       2         13052010  0030       812      04081971   \n",
+                            "...        ...     ...       ...       ...        ...      ...       ...   \n",
+                            "3004  3005      1       2         28092010  0100                20041958   \n",
+                            "3005  3006      1       2         14102010  1015                24031928   \n",
+                            "3006  3007      1       2         21112010  0650                11121955   \n",
+                            "3007  3008      1       2         10112010  0500                07071955   \n",
+                            "3008  3009      1       2         10102010  1240                07051976   \n",
+                            "\n",
+                            "      IDADE  SEXO  RACACOR  ...  DTCADASTRO  ATESTANTE  FONTEINV  DTRECEBIM  \\\n",
+                            "0     465       2           ...  19082010                         20092010    \n",
+                            "1     498       1           ...  19082010               2         01102010    \n",
+                            "2     306       2  4        ...  05012011    3                    10022011    \n",
+                            "3     005       2  1        ...  06052010    1                    20072010    \n",
+                            "4     438       1  1        ...  21062010    5                    20072010    \n",
+                            "...     ...   ...      ...  ...         ...        ...       ...        ...   \n",
+                            "3004  452       2  4        ...  20102010                         11112010    \n",
+                            "3005  482       1  1        ...  06122010    2                    19012011    \n",
+                            "3006  454       2  1        ...  09122010    5                    17012011    \n",
+                            "3007  455       1  1        ...  04012011    2                    19012011    \n",
+                            "3008  434       2  4        ...  28122010    2                    26112010    \n",
+                            "\n",
+                            "     UFINFORM  CB_PRE MORTEPARTO DTCADINF TPOBITOCOR DTCADINV  \n",
+                            "0              R98                                             \n",
+                            "1              R98                                             \n",
+                            "2              R98                                             \n",
+                            "3              O689                                            \n",
+                            "4              X999                                            \n",
+                            "...       ...     ...        ...      ...        ...      ...  \n",
+                            "3004           I619                                            \n",
+                            "3005           I219                                            \n",
+                            "3006           C349                                            \n",
+                            "3007           C787                                            \n",
+                            "3008           I739                                            \n",
                             "\n",
                             "[3009 rows x 59 columns]"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = parquets_to_dataframe(SIM.download('ac',2010))\n",
                 "df"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 3,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "df['SEXO'] = df['SEXO'].astype('object')"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>CODMUNRES</th>\n",
-                            "      <th>SEXO</th>\n",
-                            "      <th>IDADE_ANOS</th>\n",
-                            "      <th>CID10_CHAPTER</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[65.0, 66.0)</td>\n",
-                            "      <td>18</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[90.0, inf)</td>\n",
-                            "      <td>9</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[0.0, 1.0)</td>\n",
-                            "      <td>18</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>1200427</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[0.0, 1.0)</td>\n",
-                            "      <td>16</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>1200203</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[38.0, 39.0)</td>\n",
-                            "      <td>20</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3004</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[52.0, 53.0)</td>\n",
-                            "      <td>9</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3005</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[82.0, 83.0)</td>\n",
-                            "      <td>9</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3006</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[54.0, 55.0)</td>\n",
-                            "      <td>2</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3007</th>\n",
-                            "      <td>missing</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[55.0, 56.0)</td>\n",
-                            "      <td>2</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3008</th>\n",
-                            "      <td>1200401</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[34.0, 35.0)</td>\n",
-                            "      <td>9</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "<p>3009 rows \u00d7 4 columns</p>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "     CODMUNRES       SEXO    IDADE_ANOS CID10_CHAPTER\n",
-                            "0      1200401   Feminino  [65.0, 66.0)            18\n",
-                            "1      1200401  Masculino   [90.0, inf)             9\n",
-                            "2      1200401   Feminino    [0.0, 1.0)            18\n",
-                            "3      1200427   Feminino    [0.0, 1.0)            16\n",
-                            "4      1200203  Masculino  [38.0, 39.0)            20\n",
-                            "...        ...        ...           ...           ...\n",
-                            "3004   1200401   Feminino  [52.0, 53.0)             9\n",
-                            "3005   1200401  Masculino  [82.0, 83.0)             9\n",
-                            "3006   1200401   Feminino  [54.0, 55.0)             2\n",
-                            "3007   missing  Masculino  [55.0, 56.0)             2\n",
-                            "3008   1200401   Feminino  [34.0, 35.0)             9\n",
-                            "\n",
-                            "[3009 rows x 4 columns]"
-                        ]
-                    },
-                    "execution_count": 14,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "2023-04-11 14:08:10.623 | DEBUG    | pysus.online_data.SIM:get_municipios:180 - Stablishing connection with ftp.datasus.gov.br.\n",
+                        "220 Microsoft FTP Service\n",
+                        "2023-04-11 14:08:10.659 | DEBUG    | pysus.online_data.SIM:get_municipios:184 - Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS\n",
+                        "2023-04-11 14:08:10.661 | INFO     | pysus.online_data.SIM:get_municipios:194 - Local parquet file found at /home/luabida/pysus/SIM_CADMUN_.parquet\n",
+                        "/home/luabida/Projetos/InfoDengue/PySUS/pysus/preprocessing/decoders.py:122: FutureWarning: The series.append method is deprecated and will be removed from pandas in a future version. Use pandas.concat instead.\n",
+                        "  return df[\"MUNCODDV\"].append(df[\"MUNCOD\"]).astype(\"int64\").values\n",
+                        "2023-04-11 14:08:10.920 | DEBUG    | pysus.online_data.SIM:get_CID10_chapters_table:42 - Stablishing connection with ftp.datasus.gov.br.\n",
+                        "220 Microsoft FTP Service\n",
+                        "2023-04-11 14:08:10.955 | DEBUG    | pysus.online_data.SIM:get_CID10_chapters_table:46 - Changing FTP work dir to: /dissemin/publicos/SIM/CID10/TABELAS\n",
+                        "2023-04-11 14:08:10.956 | INFO     | pysus.online_data.SIM:get_CID10_chapters_table:56 - Local parquet file found at /home/luabida/pysus/SIM_CIDCAP10_.parquet\n"
+                    ]
                 }
             ],
             "source": [
                 "variables = ['CODMUNRES','SEXO','IDADE_ANOS','CID10_CHAPTER']\n",
-                "nan_string = 'missing'\n",
                 "\n",
                 "df = translate_variables_SIM(\n",
                 "                                df,\n",
                 "                                age_classes=True,\n",
                 "                                classify_cid10_chapters=True,\n",
-                "                                nan_string=nan_string\n",
                 "                            )\n",
                 "df = df[variables]\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "counts = group_and_count(df,variables)\n",
-                "counts[\"COUNTS_ORIGINAL\"] = counts[\"COUNTS\"]"
+                "counts[\"COUNTS_ORIGINAL\"] = counts[\"COUNTS\"]\n",
+                "nan_string = 'missing'"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 6,
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
@@ -589,155 +482,155 @@
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>13</th>\n",
                             "      <td>1200013</td>\n",
                             "      <td>Feminino</td>\n",
                             "      <td>[0.0, 1.0)</td>\n",
                             "      <td>16</td>\n",
-                            "      <td>2.000000</td>\n",
                             "      <td>2.0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>7191</th>\n",
-                            "      <td>1200054</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[55.0, 56.0)</td>\n",
-                            "      <td>1</td>\n",
-                            "      <td>1.032258</td>\n",
-                            "      <td>1.0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>7318</th>\n",
-                            "      <td>1200054</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[62.0, 63.0)</td>\n",
-                            "      <td>11</td>\n",
-                            "      <td>1.041667</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>9397</th>\n",
                             "      <td>1200104</td>\n",
                             "      <td>Feminino</td>\n",
                             "      <td>[0.0, 1.0)</td>\n",
                             "      <td>16</td>\n",
-                            "      <td>2.000000</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>10615</th>\n",
                             "      <td>1200104</td>\n",
                             "      <td>Feminino</td>\n",
                             "      <td>[72.0, 73.0)</td>\n",
                             "      <td>10</td>\n",
-                            "      <td>2.000000</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>10961</th>\n",
+                            "      <td>1200104</td>\n",
+                            "      <td>Masculino</td>\n",
+                            "      <td>[0.0, 1.0)</td>\n",
+                            "      <td>16</td>\n",
+                            "      <td>3.0</td>\n",
+                            "      <td>3.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>11423</th>\n",
+                            "      <td>1200104</td>\n",
+                            "      <td>Masculino</td>\n",
+                            "      <td>[27.0, 28.0)</td>\n",
+                            "      <td>20</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>98545</th>\n",
-                            "      <td>1200807</td>\n",
-                            "      <td>Feminino</td>\n",
-                            "      <td>[0.0, 1.0)</td>\n",
-                            "      <td>16</td>\n",
-                            "      <td>4.000000</td>\n",
-                            "      <td>4.0</td>\n",
+                            "      <th>96787</th>\n",
+                            "      <td>1200708</td>\n",
+                            "      <td>Masculino</td>\n",
+                            "      <td>[81.0, 82.0)</td>\n",
+                            "      <td>9</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>100129</th>\n",
+                            "      <th>98539</th>\n",
                             "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[1.0, 2.0)</td>\n",
-                            "      <td>20</td>\n",
-                            "      <td>1.071429</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>Feminino</td>\n",
+                            "      <td>[0.0, 1.0)</td>\n",
+                            "      <td>10</td>\n",
+                            "      <td>2.0</td>\n",
+                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>101037</th>\n",
+                            "      <th>98545</th>\n",
                             "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[55.0, 56.0)</td>\n",
-                            "      <td>9</td>\n",
-                            "      <td>1.032258</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>Feminino</td>\n",
+                            "      <td>[0.0, 1.0)</td>\n",
+                            "      <td>16</td>\n",
+                            "      <td>4.0</td>\n",
+                            "      <td>4.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>101420</th>\n",
                             "      <td>1200807</td>\n",
                             "      <td>Masculino</td>\n",
                             "      <td>[77.0, 78.0)</td>\n",
                             "      <td>18</td>\n",
-                            "      <td>2.000000</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>101539</th>\n",
                             "      <td>1200807</td>\n",
                             "      <td>Masculino</td>\n",
                             "      <td>[84.0, 85.0)</td>\n",
                             "      <td>18</td>\n",
-                            "      <td>2.000000</td>\n",
+                            "      <td>2.0</td>\n",
                             "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>503 rows \u00d7 6 columns</p>\n",
+                            "<p>466 rows \u00d7 6 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "       CODMUNRES       SEXO    IDADE_ANOS CID10_CHAPTER    COUNTS  \\\n",
-                            "13       1200013   Feminino    [0.0, 1.0)            16  2.000000   \n",
-                            "7191     1200054  Masculino  [55.0, 56.0)             1  1.032258   \n",
-                            "7318     1200054  Masculino  [62.0, 63.0)            11  1.041667   \n",
-                            "9397     1200104   Feminino    [0.0, 1.0)            16  2.000000   \n",
-                            "10615    1200104   Feminino  [72.0, 73.0)            10  2.000000   \n",
-                            "...          ...        ...           ...           ...       ...   \n",
-                            "98545    1200807   Feminino    [0.0, 1.0)            16  4.000000   \n",
-                            "100129   1200807  Masculino    [1.0, 2.0)            20  1.071429   \n",
-                            "101037   1200807  Masculino  [55.0, 56.0)             9  1.032258   \n",
-                            "101420   1200807  Masculino  [77.0, 78.0)            18  2.000000   \n",
-                            "101539   1200807  Masculino  [84.0, 85.0)            18  2.000000   \n",
+                            "       CODMUNRES       SEXO    IDADE_ANOS CID10_CHAPTER  COUNTS  \\\n",
+                            "13       1200013   Feminino    [0.0, 1.0)            16     2.0   \n",
+                            "9397     1200104   Feminino    [0.0, 1.0)            16     2.0   \n",
+                            "10615    1200104   Feminino  [72.0, 73.0)            10     2.0   \n",
+                            "10961    1200104  Masculino    [0.0, 1.0)            16     3.0   \n",
+                            "11423    1200104  Masculino  [27.0, 28.0)            20     2.0   \n",
+                            "...          ...        ...           ...           ...     ...   \n",
+                            "96787    1200708  Masculino  [81.0, 82.0)             9     2.0   \n",
+                            "98539    1200807   Feminino    [0.0, 1.0)            10     2.0   \n",
+                            "98545    1200807   Feminino    [0.0, 1.0)            16     4.0   \n",
+                            "101420   1200807  Masculino  [77.0, 78.0)            18     2.0   \n",
+                            "101539   1200807  Masculino  [84.0, 85.0)            18     2.0   \n",
                             "\n",
                             "        COUNTS_ORIGINAL  \n",
                             "13                  2.0  \n",
-                            "7191                1.0  \n",
-                            "7318                1.0  \n",
                             "9397                2.0  \n",
                             "10615               2.0  \n",
+                            "10961               3.0  \n",
+                            "11423               2.0  \n",
                             "...                 ...  \n",
+                            "96787               2.0  \n",
+                            "98539               2.0  \n",
                             "98545               4.0  \n",
-                            "100129              1.0  \n",
-                            "101037              1.0  \n",
                             "101420              2.0  \n",
                             "101539              2.0  \n",
                             "\n",
-                            "[503 rows x 6 columns]"
+                            "[466 rows x 6 columns]"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "counts = redistribute_missing(counts,['CODMUNRES','SEXO','IDADE_ANOS'],nan_string=nan_string)\n",
                 "counts[counts[\"COUNTS\"] > 1]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -817,109 +710,102 @@
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>101558</th>\n",
-                            "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[86.0, 87.0)</td>\n",
+                            "      <th>107831</th>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>[87.0, 88.0)</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>101575</th>\n",
-                            "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[87.0, 88.0)</td>\n",
+                            "      <th>107848</th>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>[88.0, 89.0)</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>101592</th>\n",
-                            "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[88.0, 89.0)</td>\n",
+                            "      <th>107865</th>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>[89.0, 90.0)</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>101609</th>\n",
-                            "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[89.0, 90.0)</td>\n",
+                            "      <th>107882</th>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>[90.0, inf)</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>101626</th>\n",
-                            "      <td>1200807</td>\n",
-                            "      <td>Masculino</td>\n",
-                            "      <td>[90.0, inf)</td>\n",
+                            "      <th>107899</th>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>NA</td>\n",
+                            "      <td>NA</td>\n",
                             "      <td>1</td>\n",
                             "      <td>0.0</td>\n",
                             "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>4004 rows \u00d7 6 columns</p>\n",
+                            "<p>6348 rows \u00d7 6 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "       CODMUNRES       SEXO    IDADE_ANOS CID10_CHAPTER  COUNTS  \\\n",
-                            "0        1200013   Feminino    [0.0, 1.0)             1     1.0   \n",
-                            "17       1200013   Feminino    [1.0, 2.0)             1     0.0   \n",
-                            "34       1200013   Feminino    [2.0, 3.0)             1     0.0   \n",
-                            "51       1200013   Feminino    [3.0, 4.0)             1     0.0   \n",
-                            "68       1200013   Feminino    [4.0, 5.0)             1     0.0   \n",
-                            "...          ...        ...           ...           ...     ...   \n",
-                            "101558   1200807  Masculino  [86.0, 87.0)             1     0.0   \n",
-                            "101575   1200807  Masculino  [87.0, 88.0)             1     0.0   \n",
-                            "101592   1200807  Masculino  [88.0, 89.0)             1     0.0   \n",
-                            "101609   1200807  Masculino  [89.0, 90.0)             1     0.0   \n",
-                            "101626   1200807  Masculino   [90.0, inf)             1     0.0   \n",
+                            "       CODMUNRES      SEXO    IDADE_ANOS CID10_CHAPTER  COUNTS  \\\n",
+                            "0        1200013  Feminino    [0.0, 1.0)             1     1.0   \n",
+                            "17       1200013  Feminino    [1.0, 2.0)             1     0.0   \n",
+                            "34       1200013  Feminino    [2.0, 3.0)             1     0.0   \n",
+                            "51       1200013  Feminino    [3.0, 4.0)             1     0.0   \n",
+                            "68       1200013  Feminino    [4.0, 5.0)             1     0.0   \n",
+                            "...          ...       ...           ...           ...     ...   \n",
+                            "107831        NA        NA  [87.0, 88.0)             1     0.0   \n",
+                            "107848        NA        NA  [88.0, 89.0)             1     0.0   \n",
+                            "107865        NA        NA  [89.0, 90.0)             1     0.0   \n",
+                            "107882        NA        NA   [90.0, inf)             1     0.0   \n",
+                            "107899        NA        NA            NA             1     0.0   \n",
                             "\n",
                             "        COUNTS_ORIGINAL  \n",
                             "0                   1.0  \n",
                             "17                  0.0  \n",
                             "34                  0.0  \n",
                             "51                  0.0  \n",
                             "68                  0.0  \n",
                             "...                 ...  \n",
-                            "101558              0.0  \n",
-                            "101575              0.0  \n",
-                            "101592              0.0  \n",
-                            "101609              0.0  \n",
-                            "101626              0.0  \n",
+                            "107831              0.0  \n",
+                            "107848              0.0  \n",
+                            "107865              0.0  \n",
+                            "107882              0.0  \n",
+                            "107899              0.0  \n",
                             "\n",
-                            "[4004 rows x 6 columns]"
+                            "[6348 rows x 6 columns]"
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "counts = redistribute_cid_chapter(counts,['CODMUNRES','SEXO','IDADE_ANOS'])\n",
                 "counts[counts['CID10_CHAPTER'] == 1]"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `pysus-0.9.0/pysus/Notebooks/SINAN.ipynb` & `pysus-0.9.1/pysus/Notebooks/SINAN.ipynb`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/dataset/geocode_by_cities.json` & `pysus-0.9.1/pysus/dataset/geocode_by_cities.json`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/ANIM.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/ANIM.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/BOTU.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/BOTU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/CHAG.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/CHAG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/CHIK.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/CHIK.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/COLE.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/COLE.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/COQU.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/COQU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/DENG.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/DENG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/DIFT.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/DIFT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/ESQU.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/ESQU.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/FAMA.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/FAMA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/FMAC.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/FMAC.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/FTIF.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/FTIF.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/HANS.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/HANS.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/HANT.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/HANT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/HEPA.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/HEPA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/IEXO.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/IEXO.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/LEIV.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/LEIV.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/LEPT.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/LEPT.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/LTAN.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/LTAN.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/MALA.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/MALA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/MENI.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/MENI.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/PEST.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/PEST.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/RAIV.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/RAIV.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/SIFC.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/SIFC.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/SIFG.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/SIFG.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/TETA.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/TETA.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/TETN.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/TETN.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/TUBE.tar.gz` & `pysus-0.9.1/pysus/metadata/SINAN/TUBE.tar.gz`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/metadata/SINAN/typecast.py` & `pysus-0.9.1/pysus/metadata/SINAN/typecast.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/CIHA.py` & `pysus-0.9.1/pysus/online_data/CIHA.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/CNES.py` & `pysus-0.9.1/pysus/online_data/CNES.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/ESUS.py` & `pysus-0.9.1/pysus/online_data/ESUS.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/IBGE.py` & `pysus-0.9.1/pysus/online_data/IBGE.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/Infodengue.py` & `pysus-0.9.1/pysus/online_data/Infodengue.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,9 +107,8 @@
             + "&ey_start="
             + f"{ey_start}"
             + "&ey_end="
             + f"{ey_end}"
         )
 
         url_resp = "?".join([url, params])
-
         return pd.read_csv(url_resp, index_col="SE").T
```

### Comparing `pysus-0.9.0/pysus/online_data/Infogripe.py` & `pysus-0.9.1/pysus/online_data/Infogripe.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/PNI.py` & `pysus-0.9.1/pysus/online_data/PNI.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/SIA.py` & `pysus-0.9.1/pysus/online_data/SIA.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/SIH.py` & `pysus-0.9.1/pysus/online_data/SIH.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/SIM.py` & `pysus-0.9.1/pysus/online_data/SIM.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/SINAN.py` & `pysus-0.9.1/pysus/online_data/SINAN.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/__init__.py` & `pysus-0.9.1/pysus/online_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,36 +181,38 @@
         if self.database not in DB_PATHS:
             print(
                 f"Database {self.database} not supported try one of these"
                 "{list(DB_PATHS.keys())}"
             )
             return pd.DataFrame()
 
-        with self.ftp_server.login() as ftp:
-            response = {
-                "folder": [],
-                "date": [],
-                "file_size": [],
-                "file_name": [],
-            }
-
-            def parse(line):
-                data = line.strip().split()
-                response["folder"].append(pth)
-                response["date"].append(
-                    pd.to_datetime(" ".join([data[0], data[1]]))
-                )
-                response["file_size"].append(
-                    0 if data[2] == "<DIR>" else int(data[2])
-                )
-                response["file_name"].append(data[3])
+        ftp = FTP_datasus()
+        response = {
+            "folder": [],
+            "date": [],
+            "file_size": [],
+            "file_name": [],
+        }
+
+        def parse(line):
+            data = line.strip().split()
+            response["folder"].append(pth)
+            response["date"].append(
+                pd.to_datetime(" ".join([data[0], data[1]]))
+            )
+            response["file_size"].append(
+                0 if data[2] == "<DIR>" else int(data[2])
+            )
+            response["file_name"].append(data[3])
 
-            for pth in DB_PATHS[self.database]:
-                ftp.cwd(pth)
-                flist = ftp.retrlines("LIST", parse)
+        for pth in DB_PATHS[self.database]:
+            ftp.cwd(pth)
+            flist = ftp.retrlines("LIST", parse)
+        
+        ftp.close()
         return pd.DataFrame(response)
 
     def list_available_years(
         self,
         UF: str = None,
         SINAN_disease: str = None,
         CNES_group: str = None,
@@ -349,14 +351,15 @@
                 # SIM, SINASC
                 else:
                     available_dbs.extend(
                         ftp.nlst(f"{path}/*.DBC")  # case insensitive
                     )
             except Exception as e:
                 raise e
+        ftp.close()
         return available_dbs
 
 
 class FTP_Downloader:
     """
     Databases: "SINAN", "SIM", "SINASC", "SIH", "SIA", "PNI", "CNES", "CIHA"
     FTP_Downloader will be responsible for fetching DBF and DBC files
@@ -423,15 +426,14 @@
                 downloaded_parquets.append(str(parquet_dir))
             else:
                 local_filepath = self._extract_dbc(path, local_dir=local_dir)
                 parquet_dir = self._dbfc_to_parquets(
                     local_filepath, local_dir=local_dir
                 )
                 downloaded_parquets.append(str(parquet_dir))
-
         return (
             downloaded_parquets[0] 
             if len(downloaded_parquets) == 1 
             else tuple(downloaded_parquets)
         )
 
     def _get_dbc_paths(
@@ -510,15 +512,14 @@
                     rf"{CNES_group}/{CNES_group}{UF}{year}{month}.dbc", re.I
                 )
             elif db == "CIHA":
                 if not year or not month or not UF:
                     raise ValueError("Missing year(s), month(s) or UF(s)")
                 file_pattern = re.compile(rf"CIHA{UF}{year}{month}.dbc", re.I)
             return file_pattern
-
         files = list()
         for y, m, uf in product(
             years or [], months or [], UFs or []
         ):  # Allows None
             norm = lambda y: str(y)[-2:].zfill(2)
             regex = url_regex(year=norm(y), month=norm(m), UF=str(uf))
             filtered = list(filter(regex.search, all_dbcs))
@@ -540,14 +541,15 @@
             ftp = ftp = FTP("ftp.datasus.gov.br")
             ftp.login()
             ftp.cwd(filedir)
             ftp.retrbinary(
                 f"RETR {filename}",
                 open(f"{filepath}", "wb").write,
             )
+            ftp.close()
             return str(filepath)
         except error_perm as e:
             logging.error(f"Not able to download {filename}")
             raise e
 
     def _dbfc_to_parquets(self, fpath: str, local_dir: str) -> str(PosixPath):
         """DBC/DBF files to parquets using Pandas & PyArrow"""
```

### Comparing `pysus-0.9.0/pysus/online_data/sinasc.py` & `pysus-0.9.1/pysus/online_data/sinasc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/online_data/vaccine.py` & `pysus-0.9.1/pysus/online_data/vaccine.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/preprocessing/ESUS.py` & `pysus-0.9.1/pysus/preprocessing/ESUS.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/preprocessing/SIM.py` & `pysus-0.9.1/pysus/preprocessing/SIM.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/preprocessing/decoders.py` & `pysus-0.9.1/pysus/preprocessing/decoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,16 +174,16 @@
             df[column_name] = classify_age(df[column_name], **classify_args)
             df[column_name] = df[column_name].astype("category")
             df[column_name] = df[column_name].cat.add_categories(["NA"])
             df[column_name] = df[column_name].fillna("NA")
 
     # SEXO
     if "SEXO" in variables_names:
-        df['SEXO'] = df.SEXO.str.strip().replace(
-            {"0": None, "9": None, "1": "Masculino", "2": "Feminino"}
+        df['SEXO'] = df.SEXO.replace(
+            {0: None, 9: None, 1: "Masculino", 2: "Feminino"}
         )
         df["SEXO"] = df["SEXO"].astype("category")
         df["SEXO"] = df["SEXO"].cat.add_categories(["NA"])
         df["SEXO"] = df["SEXO"].fillna("NA")
 
     # MUNRES
     if "MUNIRES" in variables_names:
```

### Comparing `pysus-0.9.0/pysus/preprocessing/geodata.py` & `pysus-0.9.1/pysus/preprocessing/geodata.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/preprocessing/sinan.py` & `pysus-0.9.1/pysus/preprocessing/sinan.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_cnes.py` & `pysus-0.9.1/pysus/tests/test_cnes.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/EPR-2016-06-01-2016.dbf` & `pysus-0.9.1/pysus/tests/test_data/EPR-2016-06-01-2016.dbf`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_Infodengue.py` & `pysus-0.9.1/pysus/tests/test_data/test_Infodengue.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_PNI.py` & `pysus-0.9.1/pysus/tests/test_data/test_PNI.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_ciha.py` & `pysus-0.9.1/pysus/tests/test_data/test_ciha.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_sia.py` & `pysus-0.9.1/pysus/tests/test_data/test_sia.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_sih.py` & `pysus-0.9.1/pysus/tests/test_data/test_sih.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_sim.py` & `pysus-0.9.1/pysus/tests/test_data/test_sim.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_sinan.py` & `pysus-0.9.1/pysus/tests/test_data/test_sinan.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def test_download(self):
         files = download(self.d1, [7,8,9], data_path=self.data_path)
         self.assertEqual(len(files), 3)
 
     def test_read_dataframe(self):
         df = parquets_to_dataframe(Path(self.data_path)/self.r1[0])
         self.assertIsInstance(df, pd.DataFrame)
-        self.assertEqual(df.shape, (1, 89))
+        self.assertEqual(df.shape, (110, 94))
     
     def test_metadata_dataframe(self):
         df = metadata_df('Raiva Humana')
         self.assertIsInstance(df, pd.DataFrame)
         self.assertEqual(df.shape, (68, 7))
```

### Comparing `pysus-0.9.0/pysus/tests/test_data/test_sinasc.py` & `pysus-0.9.1/pysus/tests/test_data/test_sinasc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_decoders.py` & `pysus-0.9.1/pysus/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_ibge.py` & `pysus-0.9.1/pysus/tests/test_ibge.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_init.py` & `pysus-0.9.1/pysus/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_sih.py` & `pysus-0.9.1/pysus/tests/test_sih.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_sim.py` & `pysus-0.9.1/pysus/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/tests/test_utilities.py` & `pysus-0.9.1/pysus/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/pysus/utilities/readdbc.py` & `pysus-0.9.1/pysus/utilities/readdbc.py`

 * *Files identical despite different names*

### Comparing `pysus-0.9.0/PKG-INFO` & `pysus-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pysus
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for dealing with Brazil's Public health data
 License: GPL
 Author: Flavio Codeco Coelho
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Unidecode (>=1.3.6,<2.0.0)
 Requires-Dist: cffi (==1.15.1)
 Requires-Dist: dbfread (==2.0.7)
-Requires-Dist: elasticsearch (>=8.3.3,<9.0.0)
+Requires-Dist: elasticsearch (==7.16.2)
 Requires-Dist: fastparquet (>=0.8.1,<0.9.0)
+Requires-Dist: geobr (>=0.2.0,<0.3.0)
 Requires-Dist: geocoder (>=1.38.1,<2.0.0)
+Requires-Dist: ipykernel (>=6.22.0,<7.0.0)
 Requires-Dist: jupyterlab (>=3.4.5,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: pandas (==1.4.3)
 Requires-Dist: pyarrow (>=11.0.0)
 Requires-Dist: pycparser (==2.21)
 Requires-Dist: pyreaddbc (==1.0.0)
```

