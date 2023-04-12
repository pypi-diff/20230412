# Comparing `tmp/pypath_omnipath-0.14.44.tar.gz` & `tmp/pypath_omnipath-0.14.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypath_omnipath-0.14.44.tar", max compression
+gzip compressed data, was "pypath_omnipath-0.14.48.tar", max compression
```

## Comparing `pypath_omnipath-0.14.44.tar` & `pypath_omnipath-0.14.48.tar`

### file list

```diff
@@ -1,327 +1,329 @@
--rw-r--r--   0        0        0    35141 2016-11-05 19:50:35.500333 pypath_omnipath-0.14.44/LICENSE
--rw-r--r--   0        0        0    11484 2023-03-28 22:00:59.866728 pypath_omnipath-0.14.44/README.rst
--rw-r--r--   0        0        0     2743 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/__init__.py
--rw-r--r--   0        0        0     2057 2023-03-28 21:50:04.559745 pypath_omnipath-0.14.44/pypath/_metadata.py
--rw-r--r--   0        0        0      666 2022-12-05 01:12:34.011729 pypath_omnipath-0.14.44/pypath/biocypher/__init__.py
--rw-r--r--   0        0        0     7863 2022-12-05 01:12:34.011729 pypath_omnipath-0.14.44/pypath/biocypher/adapter.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.502224 pypath_omnipath-0.14.44/pypath/core/__init__.py
--rw-r--r--   0        0        0   174368 2023-03-28 21:42:43.136035 pypath_omnipath-0.14.44/pypath/core/annot.py
--rw-r--r--   0        0        0     4327 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.44/pypath/core/attrs.py
--rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/core/common.py
--rw-r--r--   0        0        0    18572 2023-01-16 16:04:45.973912 pypath_omnipath-0.14.44/pypath/core/complex.py
--rw-r--r--   0        0        0    13362 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/core/entity.py
--rw-r--r--   0        0        0    37353 2022-11-29 10:17:12.502224 pypath_omnipath-0.14.44/pypath/core/enz_sub.py
--rw-r--r--   0        0        0    20612 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.44/pypath/core/evidence.py
--rw-r--r--   0        0        0    95812 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.44/pypath/core/interaction.py
--rw-r--r--   0        0        0    30155 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.44/pypath/core/intercell.py
--rw-r--r--   0        0        0   230647 2022-11-29 10:17:12.505557 pypath_omnipath-0.14.44/pypath/core/intercell_annot.py
--rw-r--r--   0        0        0   140284 2023-03-22 23:04:06.734552 pypath_omnipath-0.14.44/pypath/core/network.py
--rw-r--r--   0        0        0      138 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.44/pypath/data/__init__.py
--rw-r--r--   0        0        0     1300 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/embl_colors
--rw-r--r--   0        0        0      271 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/ensembl_biomart_query.xml
--rw-r--r--   0        0        0      227 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/goose_ancestors.sql
--rw-r--r--   0        0        0      712 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/goose_annotations.sql
--rw-r--r--   0        0        0      120 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/goose_terms.sql
--rw-r--r--   0        0        0      186 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/apache_2.0.json
--rw-r--r--   0        0        0      190 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/artistic_2.0.json
--rw-r--r--   0        0        0      199 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/biocarta.json
--rw-r--r--   0        0        0      188 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/bsd.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_2.5.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_3.0.json
--rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_4.0.json
--rw-r--r--   0        0        0      242 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc-nd_3.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc-nd_4.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc_2.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc_3.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc_4.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc_sa_3.0.json
--rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nc_sa_4.0.json
--rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nd_3.0.json
--rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_nd_4.0.json
--rw-r--r--   0        0        0      224 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_sa_2.5.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_sa_3.0.json
--rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_by_sa_4.0.json
--rw-r--r--   0        0        0      233 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cc_zero.json
--rw-r--r--   0        0        0      196 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cellcellinteractions.json
--rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/composite.json
--rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/cosmic.json
--rw-r--r--   0        0        0      194 2022-03-18 18:18:43.477819 pypath_omnipath-0.14.44/pypath/data/licenses/cytosig.json
--rw-r--r--   0        0        0      182 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/dsl.json
--rw-r--r--   0        0        0      185 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/elm.json
--rw-r--r--   0        0        0      174 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.44/pypath/data/licenses/embl-ebi.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/gnu_gpl_v2.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/gnu_gpl_v3.json
--rw-r--r--   0        0        0      200 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/gnu_lgpl_v3.json
--rw-r--r--   0        0        0      311 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/hgnc.json
--rw-r--r--   0        0        0      150 2022-09-15 18:20:39.089511 pypath_omnipath-0.14.44/pypath/data/licenses/hpo.json
--rw-r--r--   0        0        0      139 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/hprd.json
--rw-r--r--   0        0        0      168 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/i2d.json
--rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/informal.json
--rw-r--r--   0        0        0      175 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/kegg.json
--rw-r--r--   0        0        0      174 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/kinase-com.json
--rw-r--r--   0        0        0      268 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/mirecords.json
--rw-r--r--   0        0        0      184 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/mirtarbase.json
--rw-r--r--   0        0        0      154 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/mit.json
--rw-r--r--   0        0        0      165 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/mppi.json
--rw-r--r--   0        0        0      360 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/nar.json
--rw-r--r--   0        0        0      179 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/no_license.json
--rw-r--r--   0        0        0      177 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/pathwaycommons.json
--rw-r--r--   0        0        0      351 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/pdb.json
--rw-r--r--   0        0        0      363 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/phosphonetworks.json
--rw-r--r--   0        0        0      464 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/licenses/unspecified.json
--rw-r--r--   0        0        0     5462 2023-03-28 13:01:46.148225 pypath_omnipath-0.14.44/pypath/data/settings.yaml
--rw-r--r--   0        0        0     1150 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/www/favicon.ico
--rw-r--r--   0        0        0      486 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/www/http500.html
--rw-r--r--   0        0        0      324 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.44/pypath/data/www/index.html
--rw-r--r--   0        0        0     5815 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.44/pypath/formats/obo.py
--rw-r--r--   0        0        0     8624 2023-03-09 00:29:38.782357 pypath_omnipath-0.14.44/pypath/formats/sqldump.py
--rw-r--r--   0        0        0     1358 2023-03-09 17:12:37.914407 pypath_omnipath-0.14.44/pypath/formats/sqlite.py
--rw-r--r--   0        0        0     7508 2023-03-13 13:39:42.775048 pypath_omnipath-0.14.44/pypath/formats/xml.py
--rw-r--r--   0        0        0     2204 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/__init__.py
--rw-r--r--   0        0        0     1075 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/abs.py
--rw-r--r--   0        0        0     3155 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/acsn.py
--rw-r--r--   0        0        0     2422 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/adhesome.py
--rw-r--r--   0        0        0     2343 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/almen2009.py
--rw-r--r--   0        0        0     5340 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/baccin2019.py
--rw-r--r--   0        0        0     6319 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.44/pypath/inputs/biogps.py
--rw-r--r--   0        0        0     5016 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/biogrid.py
--rw-r--r--   0        0        0    10223 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/biomart.py
--rw-r--r--   0        0        0     5365 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/biomodels.py
--rw-r--r--   0        0        0     1794 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/ca1.py
--rw-r--r--   0        0        0     2760 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/cancercellmap.py
--rw-r--r--   0        0        0     5541 2023-03-23 11:43:45.220378 pypath_omnipath-0.14.44/pypath/inputs/cancerdrugsdb.py
--rw-r--r--   0        0        0     1907 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/cancersea.py
--rw-r--r--   0        0        0     3358 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/cell.py
--rw-r--r--   0        0        0     6338 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/cellcall.py
--rw-r--r--   0        0        0     1551 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/cellcellinteractions.py
--rw-r--r--   0        0        0     9191 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/cellchatdb.py
--rw-r--r--   0        0        0    15036 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/cellinker.py
--rw-r--r--   0        0        0     9174 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/cellphonedb.py
--rw-r--r--   0        0        0     5398 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/celltalkdb.py
--rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/celltypist.py
--rw-r--r--   0        0        0    13899 2023-03-09 16:16:55.198353 pypath_omnipath-0.14.44/pypath/inputs/chembl.py
--rw-r--r--   0        0        0     3430 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.44/pypath/inputs/clinvar.py
--rw-r--r--   0        0        0     5528 2023-03-27 19:35:18.140054 pypath_omnipath-0.14.44/pypath/inputs/collectri.py
--rw-r--r--   0        0        0     7920 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/common.py
--rw-r--r--   0        0        0     2656 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/compleat.py
--rw-r--r--   0        0        0     4509 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/complexportal.py
--rw-r--r--   0        0        0     4036 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/comppi.py
--rw-r--r--   0        0        0     2788 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/connectomedb.py
--rw-r--r--   0        0        0     2793 2023-03-23 12:55:34.154293 pypath_omnipath-0.14.44/pypath/inputs/corum.py
--rw-r--r--   0        0        0     4779 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/cosmic.py
--rw-r--r--   0        0        0     4234 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/cpad.py
--rw-r--r--   0        0        0     1989 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/cpdb.py
--rw-r--r--   0        0        0     3412 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.44/pypath/inputs/credentials.py
--rw-r--r--   0        0        0     3344 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/csa.py
--rw-r--r--   0        0        0     3547 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/cspa.py
--rw-r--r--   0        0        0     5114 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.44/pypath/inputs/ctdbase.py
--rw-r--r--   0        0        0     3343 2023-03-22 17:05:50.626476 pypath_omnipath-0.14.44/pypath/inputs/cytosig.py
--rw-r--r--   0        0        0     4765 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/dbptm.py
--rw-r--r--   0        0        0     2833 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/deathdomain.py
--rw-r--r--   0        0        0     4384 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/depod.py
--rw-r--r--   0        0        0     3721 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.44/pypath/inputs/dgidb.py
--rw-r--r--   0        0        0     4921 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/dip.py
--rw-r--r--   0        0        0    68257 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.44/pypath/inputs/disgenet.py
--rw-r--r--   0        0        0    17135 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/domino.py
--rw-r--r--   0        0        0    12715 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/dorothea.py
--rw-r--r--   0        0        0    20676 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.44/pypath/inputs/drugbank.py
--rw-r--r--   0        0        0     4706 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/drugcentral.py
--rw-r--r--   0        0        0     4803 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/ebi.py
--rw-r--r--   0        0        0     4929 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/elm.py
--rw-r--r--   0        0        0     2523 2023-03-28 12:11:30.004207 pypath_omnipath-0.14.44/pypath/inputs/embopress.py
--rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/embrace.py
--rw-r--r--   0        0        0     1220 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/encode.py
--rw-r--r--   0        0        0     1856 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/ensembl.py
--rw-r--r--   0        0        0     3152 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/exocarta.py
--rw-r--r--   0        0        0     3425 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/genecards.py
--rw-r--r--   0        0        0    26086 2023-03-28 21:26:09.280054 pypath_omnipath-0.14.44/pypath/inputs/go.py
--rw-r--r--   0        0        0     2356 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/gpcrdb.py
--rw-r--r--   0        0        0     1937 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/graphviz.py
--rw-r--r--   0        0        0     8093 2023-03-28 11:43:53.797828 pypath_omnipath-0.14.44/pypath/inputs/guide2pharma.py
--rw-r--r--   0        0        0     1597 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/havugimana.py
--rw-r--r--   0        0        0     1628 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/hgnc.py
--rw-r--r--   0        0        0     3763 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/hippie.py
--rw-r--r--   0        0        0    12568 2023-03-20 14:49:33.714166 pypath_omnipath-0.14.44/pypath/inputs/hmdb.py
--rw-r--r--   0        0        0     4862 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/homologene.py
--rw-r--r--   0        0        0    10335 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/hpmr.py
--rw-r--r--   0        0        0     4781 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/hpo.py
--rw-r--r--   0        0        0     2748 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/hprd.py
--rw-r--r--   0        0        0     1491 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/htri.py
--rw-r--r--   0        0        0     1773 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/humancellmap.py
--rw-r--r--   0        0        0     2048 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/humap.py
--rw-r--r--   0        0        0     8093 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/huri.py
--rw-r--r--   0        0        0     2665 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/i3d.py
--rw-r--r--   0        0        0     6713 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/icellnet.py
--rw-r--r--   0        0        0     8076 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/ielm.py
--rw-r--r--   0        0        0     3914 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/imweb.py
--rw-r--r--   0        0        0     2242 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/innatedb.py
--rw-r--r--   0        0        0     3005 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/instruct.py
--rw-r--r--   0        0        0     5688 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/intact.py
--rw-r--r--   0        0        0     1741 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/integrins.py
--rw-r--r--   0        0        0     8866 2023-03-28 21:43:59.156468 pypath_omnipath-0.14.44/pypath/inputs/interpro.py
--rw-r--r--   0        0        0     2405 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/intogen.py
--rw-r--r--   0        0        0     1708 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/ipi.py
--rw-r--r--   0        0        0     3630 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/iptmnet.py
--rw-r--r--   0        0        0     3192 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/italk.py
--rw-r--r--   0        0        0     2557 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/kea.py
--rw-r--r--   0        0        0    20507 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/kegg.py
--rw-r--r--   0        0        0    14746 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/kegg_api.py
--rw-r--r--   0        0        0     1932 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/kinasedotcom.py
--rw-r--r--   0        0        0     2522 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/kirouac2010.py
--rw-r--r--   0        0        0     4327 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/lambert2018.py
--rw-r--r--   0        0        0     2174 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/laudanna.py
--rw-r--r--   0        0        0     5633 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/li2012.py
--rw-r--r--   0        0        0     2625 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/lincs.py
--rw-r--r--   0        0        0     2926 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/lmpid.py
--rw-r--r--   0        0        0     1549 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/lncdisease.py
--rw-r--r--   0        0        0     2026 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/lncrnadb.py
--rw-r--r--   0        0        0     7887 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/locate.py
--rw-r--r--   0        0        0     3648 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/lrdb.py
--rw-r--r--   0        0        0     2907 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/macrophage.py
--rw-r--r--   0        0        0      568 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/main.py
--rw-r--r--   0        0        0     2334 2023-03-28 17:55:35.707415 pypath_omnipath-0.14.44/pypath/inputs/matrisome.py
--rw-r--r--   0        0        0     4171 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/matrixdb.py
--rw-r--r--   0        0        0     1107 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/mcam.py
--rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/membranome.py
--rw-r--r--   0        0        0     4296 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/mimp.py
--rw-r--r--   0        0        0     1365 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/mir2disease.py
--rw-r--r--   0        0        0     3865 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/mirbase.py
--rw-r--r--   0        0        0     1742 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/mirdeathdb.py
--rw-r--r--   0        0        0     1651 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/mirecords.py
--rw-r--r--   0        0        0     2177 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/mirtarbase.py
--rw-r--r--   0        0        0     1069 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/mitab.py
--rw-r--r--   0        0        0     3166 2023-03-23 12:55:18.904569 pypath_omnipath-0.14.44/pypath/inputs/mppi.py
--rw-r--r--   0        0        0    11420 2023-03-28 13:11:27.070439 pypath_omnipath-0.14.44/pypath/inputs/msigdb.py
--rw-r--r--   0        0        0     2100 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/ncrdeathdb.py
--rw-r--r--   0        0        0     1830 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/negatome.py
--rw-r--r--   0        0        0     1758 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/netbiol.py
--rw-r--r--   0        0        0     6376 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/netpath.py
--rw-r--r--   0        0        0     2994 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.44/pypath/inputs/oma.py
--rw-r--r--   0        0        0     3600 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/ontology.py
--rw-r--r--   0        0        0     2845 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/opm.py
--rw-r--r--   0        0        0     2313 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/oreganno.py
--rw-r--r--   0        0        0     4003 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/panglaodb.py
--rw-r--r--   0        0        0     3558 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.44/pypath/inputs/pathophenodb.py
--rw-r--r--   0        0        0     4593 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/pathwaycommons.py
--rw-r--r--   0        0        0     1071 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/pazar.py
--rw-r--r--   0        0        0     6333 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/pdb.py
--rw-r--r--   0        0        0     2411 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/pdzbase.py
--rw-r--r--   0        0        0     6660 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.44/pypath/inputs/pepcyber.py
--rw-r--r--   0        0        0     9162 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/pfam.py
--rw-r--r--   0        0        0     6669 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.44/pypath/inputs/pharos.py
--rw-r--r--   0        0        0     1673 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/phobius.py
--rw-r--r--   0        0        0     2299 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/phosphatome.py
--rw-r--r--   0        0        0     3433 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/phosphoelm.py
--rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/phosphonetworks.py
--rw-r--r--   0        0        0     1299 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.44/pypath/inputs/phosphopoint.py
--rw-r--r--   0        0        0    37326 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/phosphosite.py
--rw-r--r--   0        0        0     9976 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/pisa.py
--rw-r--r--   0        0        0     1850 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/pro.py
--rw-r--r--   0        0        0     3189 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/progeny.py
--rw-r--r--   0        0        0     7531 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/proteinatlas.py
--rw-r--r--   0        0        0     3573 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/proteins.py
--rw-r--r--   0        0        0     3808 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/protmapper.py
--rw-r--r--   0        0        0     2463 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/pubchem.py
--rw-r--r--   0        0        0     4224 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/pubmed.py
--rw-r--r--   0        0        0     4418 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/ramilowski2015.py
--rw-r--r--   0        0        0     5426 2023-03-22 21:01:49.738609 pypath_omnipath-0.14.44/pypath/inputs/ramp.py
--rw-r--r--   0        0        0     6496 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/rdata.py
--rw-r--r--   0        0        0    40102 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/reaction.py
--rw-r--r--   0        0        0     7539 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/scconnect.py
--rw-r--r--   0        0        0     2455 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/science.py
--rw-r--r--   0        0        0     5578 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/signalink.py
--rw-r--r--   0        0        0    11727 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/signor.py
--rw-r--r--   0        0        0     5681 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/spike.py
--rw-r--r--   0        0        0     4287 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/stitch.py
--rw-r--r--   0        0        0     7315 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/string.py
--rw-r--r--   0        0        0     1579 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/surfaceome.py
--rw-r--r--   0        0        0     4412 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/switches_elm.py
--rw-r--r--   0        0        0     3225 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.44/pypath/inputs/talklr.py
--rw-r--r--   0        0        0     2616 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/tcdb.py
--rw-r--r--   0        0        0     2119 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/tfcensus.py
--rw-r--r--   0        0        0     7926 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/threedcomplex.py
--rw-r--r--   0        0        0    17368 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/threedid.py
--rw-r--r--   0        0        0     3692 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/topdb.py
--rw-r--r--   0        0        0     1453 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.44/pypath/inputs/transmir.py
--rw-r--r--   0        0        0     9902 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.44/pypath/inputs/trip.py
--rw-r--r--   0        0        0     5196 2023-03-19 23:05:05.810094 pypath_omnipath-0.14.44/pypath/inputs/unichem.py
--rw-r--r--   0        0        0    31311 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/uniprot.py
--rw-r--r--   0        0        0     7607 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.44/pypath/inputs/wang.py
--rw-r--r--   0        0        0     2171 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/inputs/wojtowicz2020.py
--rw-r--r--   0        0        0     1619 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.44/pypath/inputs/zhong2015.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/internals/__init__.py
--rw-r--r--   0        0        0    11896 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/internals/annot_formats.py
--rw-r--r--   0        0        0    21507 2023-03-23 08:10:01.341026 pypath_omnipath-0.14.44/pypath/internals/input_formats.py
--rw-r--r--   0        0        0    43762 2023-03-27 19:06:47.600564 pypath_omnipath-0.14.44/pypath/internals/intera.py
--rw-r--r--   0        0        0     7533 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/internals/license.py
--rw-r--r--   0        0        0     7257 2023-03-06 18:13:55.980766 pypath_omnipath-0.14.44/pypath/internals/maps.py
--rw-r--r--   0        0        0     4199 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/internals/refs.py
--rw-r--r--   0        0        0     9673 2023-03-10 13:53:12.961501 pypath_omnipath-0.14.44/pypath/internals/resource.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.14.44/pypath/legacy/__init__.py
--rw-r--r--   0        0        0     4608 2022-11-29 10:17:12.492224 pypath_omnipath-0.14.44/pypath/legacy/db_categories.py
--rw-r--r--   0        0        0   556645 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.44/pypath/legacy/main.py
--rw-r--r--   0        0        0     1768 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/__init__.py
--rw-r--r--   0        0        0    18012 2023-02-23 11:35:21.780049 pypath_omnipath-0.14.44/pypath/omnipath/app.py
--rw-r--r--   0        0        0    16321 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.44/pypath/omnipath/bel.py
--rw-r--r--   0        0        0    16758 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/cellphonedb.py
--rw-r--r--   0        0        0     1477 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/databases/__init__.py
--rw-r--r--   0        0        0     1848 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/databases/build.py
--rw-r--r--   0        0        0     1729 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.44/pypath/omnipath/databases/builtins.json
--rw-r--r--   0        0        0      522 2022-01-24 11:42:01.191613 pypath_omnipath-0.14.44/pypath/omnipath/databases/classes.json
--rw-r--r--   0        0        0     8342 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/databases/define.py
--rw-r--r--   0        0        0    34353 2023-03-27 20:50:05.365575 pypath_omnipath-0.14.44/pypath/omnipath/export.py
--rw-r--r--   0        0        0     4180 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/omnipath/legacy.py
--rw-r--r--   0        0        0     1792 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/param.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/omnipath/server/__init__.py
--rw-r--r--   0        0        0   122926 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/omnipath/server/_html.py
--rw-r--r--   0        0        0    10455 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/omnipath/server/build.py
--rw-r--r--   0        0        0    17217 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/omnipath/server/generate_about_page.py
--rw-r--r--   0        0        0    11122 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/omnipath/server/legacy.py
--rw-r--r--   0        0        0    78537 2023-03-28 11:28:50.358833 pypath_omnipath-0.14.44/pypath/omnipath/server/run.py
--rw-r--r--   0        0        0     4740 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.44/pypath/reader/field.py
--rw-r--r--   0        0        0     1620 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.44/pypath/reader/network.py
--rw-r--r--   0        0        0     1013 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/resources/__init__.py
--rw-r--r--   0        0        0    13818 2023-03-10 18:26:35.393005 pypath_omnipath-0.14.44/pypath/resources/controller.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/resources/data/__init__.py
--rw-r--r--   0        0        0      139 2023-01-10 18:56:49.559042 pypath_omnipath-0.14.44/pypath/resources/data/complex_input_template.json
--rw-r--r--   0        0        0      239 2023-01-10 18:56:35.023580 pypath_omnipath-0.14.44/pypath/resources/data/enz_sub_input_template.json
--rw-r--r--   0        0        0   176308 2023-03-28 21:50:23.075796 pypath_omnipath-0.14.44/pypath/resources/data/resources.json
--rw-r--r--   0        0        0   100457 2023-03-27 21:02:20.438700 pypath_omnipath-0.14.44/pypath/resources/data_formats.py
--rw-r--r--   0        0        0   179216 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.44/pypath/resources/descriptions.py
--rw-r--r--   0        0        0     2817 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.44/pypath/resources/licenses.py
--rw-r--r--   0        0        0     5389 2023-03-20 15:20:34.662810 pypath_omnipath-0.14.44/pypath/resources/network.py
--rw-r--r--   0        0        0    71931 2023-03-28 21:22:52.400511 pypath_omnipath-0.14.44/pypath/resources/urls.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.14.44/pypath/share/__init__.py
--rw-r--r--   0        0        0     1801 2023-03-08 22:39:02.796456 pypath_omnipath-0.14.44/pypath/share/cache.py
--rw-r--r--   0        0        0    69219 2023-03-10 17:52:17.522496 pypath_omnipath-0.14.44/pypath/share/common.py
--rw-r--r--   0        0        0      852 2023-01-16 16:04:45.977246 pypath_omnipath-0.14.44/pypath/share/constants.py
--rw-r--r--   0        0        0    57036 2023-03-28 21:12:57.964394 pypath_omnipath-0.14.44/pypath/share/curl.py
--rw-r--r--   0        0        0     6176 2022-12-05 01:12:34.031728 pypath_omnipath-0.14.44/pypath/share/log.py
--rw-r--r--   0        0        0    17323 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/share/lookup/_manytomany.py
--rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/share/lookup/_onetomany.py
--rw-r--r--   0        0        0     2525 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/share/lookup/_onetomany2.py
--rw-r--r--   0        0        0     5284 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.44/pypath/share/progress.py
--rw-r--r--   0        0        0     4426 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/share/session.py
--rw-r--r--   0        0        0     9674 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/share/settings.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.492224 pypath_omnipath-0.14.44/pypath/utils/__init__.py
--rw-r--r--   0        0        0    37321 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.44/pypath/utils/go.py
--rw-r--r--   0        0        0    56014 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/utils/homology.py
--rw-r--r--   0        0        0   107387 2023-03-23 11:43:35.584291 pypath_omnipath-0.14.44/pypath/utils/mapping.py
--rw-r--r--   0        0        0     5765 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/utils/pdb.py
--rw-r--r--   0        0        0    11855 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.44/pypath/utils/proteomicsdb.py
--rw-r--r--   0        0        0   109034 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.44/pypath/utils/pyreact.py
--rw-r--r--   0        0        0     7265 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.44/pypath/utils/reflists.py
--rw-r--r--   0        0        0     8802 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.44/pypath/utils/residues.py
--rw-r--r--   0        0        0    11325 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.44/pypath/utils/seq.py
--rw-r--r--   0        0        0    11255 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/utils/taxonomy.py
--rw-r--r--   0        0        0    11956 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/utils/unichem.py
--rw-r--r--   0        0        0    17936 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/utils/uniprot.py
--rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.44/pypath/visual/__init__.py
--rw-r--r--   0        0        0    26879 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/visual/drawing.py
--rw-r--r--   0        0        0    21128 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/visual/igraph_drawing/__init__.py
--rw-r--r--   0        0        0    13835 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/visual/igraph_drawing/edge.py
--rw-r--r--   0        0        0     4769 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.44/pypath/visual/igraph_drawing/vertex.py
--rw-r--r--   0        0        0   156771 2022-12-05 01:12:34.038395 pypath_omnipath-0.14.44/pypath/visual/plot.py
--rw-r--r--   0        0        0     2748 2023-03-28 21:50:04.559745 pypath_omnipath-0.14.44/pyproject.toml
--rw-r--r--   0        0        0    13401 1970-01-01 00:00:00.000000 pypath_omnipath-0.14.44/setup.py
--rw-r--r--   0        0        0    13555 1970-01-01 00:00:00.000000 pypath_omnipath-0.14.44/PKG-INFO
+-rw-r--r--   0        0        0    35141 2016-11-05 19:50:35.500333 pypath_omnipath-0.14.48/LICENSE
+-rw-r--r--   0        0        0    11492 2023-03-28 22:05:50.316062 pypath_omnipath-0.14.48/README.rst
+-rw-r--r--   0        0        0     2743 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/__init__.py
+-rw-r--r--   0        0        0     2057 2023-04-12 15:39:36.242305 pypath_omnipath-0.14.48/pypath/_metadata.py
+-rw-r--r--   0        0        0      666 2022-12-05 01:12:34.011729 pypath_omnipath-0.14.48/pypath/biocypher/__init__.py
+-rw-r--r--   0        0        0     7863 2022-12-05 01:12:34.011729 pypath_omnipath-0.14.48/pypath/biocypher/adapter.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.502224 pypath_omnipath-0.14.48/pypath/core/__init__.py
+-rw-r--r--   0        0        0   174945 2023-03-29 12:47:27.521270 pypath_omnipath-0.14.48/pypath/core/annot.py
+-rw-r--r--   0        0        0     4327 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/core/attrs.py
+-rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/core/common.py
+-rw-r--r--   0        0        0    19000 2023-03-29 12:48:22.415968 pypath_omnipath-0.14.48/pypath/core/complex.py
+-rw-r--r--   0        0        0    13228 2023-03-29 23:28:02.614928 pypath_omnipath-0.14.48/pypath/core/entity.py
+-rw-r--r--   0        0        0    37353 2022-11-29 10:17:12.502224 pypath_omnipath-0.14.48/pypath/core/enz_sub.py
+-rw-r--r--   0        0        0    20612 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/core/evidence.py
+-rw-r--r--   0        0        0    95812 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/core/interaction.py
+-rw-r--r--   0        0        0    30155 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/core/intercell.py
+-rw-r--r--   0        0        0   230647 2022-11-29 10:17:12.505557 pypath_omnipath-0.14.48/pypath/core/intercell_annot.py
+-rw-r--r--   0        0        0   140737 2023-03-29 23:08:59.315836 pypath_omnipath-0.14.48/pypath/core/network.py
+-rw-r--r--   0        0        0      138 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/data/__init__.py
+-rw-r--r--   0        0        0     1300 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/embl_colors
+-rw-r--r--   0        0        0      271 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/ensembl_biomart_query.xml
+-rw-r--r--   0        0        0      227 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/goose_ancestors.sql
+-rw-r--r--   0        0        0      712 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/goose_annotations.sql
+-rw-r--r--   0        0        0      120 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/goose_terms.sql
+-rw-r--r--   0        0        0      185 2023-03-30 00:53:33.672441 pypath_omnipath-0.14.48/pypath/data/licenses/afl_v3.json
+-rw-r--r--   0        0        0      186 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/apache_2.0.json
+-rw-r--r--   0        0        0      190 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/artistic_2.0.json
+-rw-r--r--   0        0        0      199 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/biocarta.json
+-rw-r--r--   0        0        0      188 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/bsd.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_2.5.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_3.0.json
+-rw-r--r--   0        0        0      205 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_4.0.json
+-rw-r--r--   0        0        0      242 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc-nd_3.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.168281 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc-nd_4.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_2.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_3.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_4.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_sa_3.0.json
+-rw-r--r--   0        0        0      241 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nc_sa_4.0.json
+-rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nd_3.0.json
+-rw-r--r--   0        0        0      228 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_nd_4.0.json
+-rw-r--r--   0        0        0      224 2023-03-30 00:45:57.463174 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_sa_2.5.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_sa_3.0.json
+-rw-r--r--   0        0        0      223 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_by_sa_4.0.json
+-rw-r--r--   0        0        0      233 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cc_zero.json
+-rw-r--r--   0        0        0      196 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cellcellinteractions.json
+-rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/composite.json
+-rw-r--r--   0        0        0      166 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/cosmic.json
+-rw-r--r--   0        0        0      194 2022-03-18 18:18:43.477819 pypath_omnipath-0.14.48/pypath/data/licenses/cytosig.json
+-rw-r--r--   0        0        0      182 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/dsl.json
+-rw-r--r--   0        0        0      185 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/elm.json
+-rw-r--r--   0        0        0      174 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/data/licenses/embl-ebi.json
+-rw-r--r--   0        0        0      212 2023-04-05 14:14:07.817106 pypath_omnipath-0.14.48/pypath/data/licenses/eul.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/gnu_gpl_v2.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/gnu_gpl_v3.json
+-rw-r--r--   0        0        0      200 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/gnu_lgpl_v3.json
+-rw-r--r--   0        0        0      311 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/hgnc.json
+-rw-r--r--   0        0        0      150 2022-09-15 18:20:39.089511 pypath_omnipath-0.14.48/pypath/data/licenses/hpo.json
+-rw-r--r--   0        0        0      139 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/hprd.json
+-rw-r--r--   0        0        0      168 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/i2d.json
+-rw-r--r--   0        0        0      189 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/informal.json
+-rw-r--r--   0        0        0      175 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/kegg.json
+-rw-r--r--   0        0        0      174 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/kinase-com.json
+-rw-r--r--   0        0        0      268 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mirecords.json
+-rw-r--r--   0        0        0      184 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mirtarbase.json
+-rw-r--r--   0        0        0      154 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mit.json
+-rw-r--r--   0        0        0      165 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/mppi.json
+-rw-r--r--   0        0        0      360 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/nar.json
+-rw-r--r--   0        0        0      179 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/no_license.json
+-rw-r--r--   0        0        0      177 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/pathwaycommons.json
+-rw-r--r--   0        0        0      351 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/pdb.json
+-rw-r--r--   0        0        0      363 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/phosphonetworks.json
+-rw-r--r--   0        0        0      464 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/licenses/unspecified.json
+-rw-r--r--   0        0        0     5731 2023-03-29 13:56:06.759376 pypath_omnipath-0.14.48/pypath/data/settings.yaml
+-rw-r--r--   0        0        0     1150 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/www/favicon.ico
+-rw-r--r--   0        0        0      486 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/www/http500.html
+-rw-r--r--   0        0        0      324 2022-01-24 11:42:01.171614 pypath_omnipath-0.14.48/pypath/data/www/index.html
+-rw-r--r--   0        0        0     5815 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/formats/obo.py
+-rw-r--r--   0        0        0     8624 2023-03-09 00:29:38.782357 pypath_omnipath-0.14.48/pypath/formats/sqldump.py
+-rw-r--r--   0        0        0     1358 2023-03-09 17:12:37.914407 pypath_omnipath-0.14.48/pypath/formats/sqlite.py
+-rw-r--r--   0        0        0     7508 2023-03-13 13:39:42.775048 pypath_omnipath-0.14.48/pypath/formats/xml.py
+-rw-r--r--   0        0        0     2204 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/__init__.py
+-rw-r--r--   0        0        0     1075 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/abs.py
+-rw-r--r--   0        0        0     3155 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/acsn.py
+-rw-r--r--   0        0        0     2422 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/adhesome.py
+-rw-r--r--   0        0        0     2343 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/almen2009.py
+-rw-r--r--   0        0        0     5340 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/baccin2019.py
+-rw-r--r--   0        0        0     6319 2022-12-05 01:12:34.015062 pypath_omnipath-0.14.48/pypath/inputs/biogps.py
+-rw-r--r--   0        0        0     5016 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/biogrid.py
+-rw-r--r--   0        0        0    10223 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/biomart.py
+-rw-r--r--   0        0        0     5365 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/biomodels.py
+-rw-r--r--   0        0        0     1794 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/ca1.py
+-rw-r--r--   0        0        0     2760 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/cancercellmap.py
+-rw-r--r--   0        0        0     5541 2023-03-23 11:43:45.220378 pypath_omnipath-0.14.48/pypath/inputs/cancerdrugsdb.py
+-rw-r--r--   0        0        0     1907 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/cancersea.py
+-rw-r--r--   0        0        0     3358 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cell.py
+-rw-r--r--   0        0        0     6338 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cellcall.py
+-rw-r--r--   0        0        0     1551 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/cellcellinteractions.py
+-rw-r--r--   0        0        0     9191 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/cellchatdb.py
+-rw-r--r--   0        0        0    15036 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cellinker.py
+-rw-r--r--   0        0        0     9174 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cellphonedb.py
+-rw-r--r--   0        0        0     5398 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/celltalkdb.py
+-rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/celltypist.py
+-rw-r--r--   0        0        0    13899 2023-03-09 16:16:55.198353 pypath_omnipath-0.14.48/pypath/inputs/chembl.py
+-rw-r--r--   0        0        0     3454 2023-04-07 15:34:02.552665 pypath_omnipath-0.14.48/pypath/inputs/clinvar.py
+-rw-r--r--   0        0        0     5564 2023-03-30 21:50:08.109288 pypath_omnipath-0.14.48/pypath/inputs/collectri.py
+-rw-r--r--   0        0        0     7920 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/common.py
+-rw-r--r--   0        0        0     2656 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/compleat.py
+-rw-r--r--   0        0        0     4509 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/complexportal.py
+-rw-r--r--   0        0        0     4036 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/comppi.py
+-rw-r--r--   0        0        0     2788 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/connectomedb.py
+-rw-r--r--   0        0        0     2793 2023-03-23 12:55:34.154293 pypath_omnipath-0.14.48/pypath/inputs/corum.py
+-rw-r--r--   0        0        0     4779 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/cosmic.py
+-rw-r--r--   0        0        0     4234 2023-03-29 21:02:25.987565 pypath_omnipath-0.14.48/pypath/inputs/cpad.py
+-rw-r--r--   0        0        0     1989 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/cpdb.py
+-rw-r--r--   0        0        0     3412 2022-12-05 01:12:34.018396 pypath_omnipath-0.14.48/pypath/inputs/credentials.py
+-rw-r--r--   0        0        0     3344 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/csa.py
+-rw-r--r--   0        0        0     3547 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/cspa.py
+-rw-r--r--   0        0        0     5114 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/ctdbase.py
+-rw-r--r--   0        0        0     3343 2023-03-22 17:05:50.626476 pypath_omnipath-0.14.48/pypath/inputs/cytosig.py
+-rw-r--r--   0        0        0     4765 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/dbptm.py
+-rw-r--r--   0        0        0     2833 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/deathdomain.py
+-rw-r--r--   0        0        0     4384 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/depod.py
+-rw-r--r--   0        0        0     3721 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.48/pypath/inputs/dgidb.py
+-rw-r--r--   0        0        0     4921 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/dip.py
+-rw-r--r--   0        0        0    68257 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/disgenet.py
+-rw-r--r--   0        0        0    17135 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/domino.py
+-rw-r--r--   0        0        0    12715 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/dorothea.py
+-rw-r--r--   0        0        0    20676 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/drugbank.py
+-rw-r--r--   0        0        0     4706 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/drugcentral.py
+-rw-r--r--   0        0        0     4803 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/ebi.py
+-rw-r--r--   0        0        0     4929 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/elm.py
+-rw-r--r--   0        0        0     2523 2023-03-28 12:11:30.004207 pypath_omnipath-0.14.48/pypath/inputs/embopress.py
+-rw-r--r--   0        0        0     4524 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/embrace.py
+-rw-r--r--   0        0        0     1220 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/encode.py
+-rw-r--r--   0        0        0     1982 2023-04-05 00:14:36.657341 pypath_omnipath-0.14.48/pypath/inputs/ensembl.py
+-rw-r--r--   0        0        0     3152 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/exocarta.py
+-rw-r--r--   0        0        0     3425 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/genecards.py
+-rw-r--r--   0        0        0    26086 2023-03-28 21:26:09.280054 pypath_omnipath-0.14.48/pypath/inputs/go.py
+-rw-r--r--   0        0        0     2356 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/gpcrdb.py
+-rw-r--r--   0        0        0     1937 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/graphviz.py
+-rw-r--r--   0        0        0     8093 2023-03-28 11:43:53.797828 pypath_omnipath-0.14.48/pypath/inputs/guide2pharma.py
+-rw-r--r--   0        0        0     1597 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/havugimana.py
+-rw-r--r--   0        0        0     1628 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/hgnc.py
+-rw-r--r--   0        0        0     3763 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/hippie.py
+-rw-r--r--   0        0        0    12568 2023-03-20 14:49:33.714166 pypath_omnipath-0.14.48/pypath/inputs/hmdb.py
+-rw-r--r--   0        0        0     4862 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/homologene.py
+-rw-r--r--   0        0        0    10335 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/hpmr.py
+-rw-r--r--   0        0        0     4781 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/hpo.py
+-rw-r--r--   0        0        0     2748 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/hprd.py
+-rw-r--r--   0        0        0     1491 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/htri.py
+-rw-r--r--   0        0        0     1773 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/humancellmap.py
+-rw-r--r--   0        0        0     2048 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/humap.py
+-rw-r--r--   0        0        0     8093 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/huri.py
+-rw-r--r--   0        0        0     2665 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/i3d.py
+-rw-r--r--   0        0        0     6713 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/icellnet.py
+-rw-r--r--   0        0        0     8076 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/ielm.py
+-rw-r--r--   0        0        0     3914 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/imweb.py
+-rw-r--r--   0        0        0     2242 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/innatedb.py
+-rw-r--r--   0        0        0     3005 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/instruct.py
+-rw-r--r--   0        0        0     5688 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/intact.py
+-rw-r--r--   0        0        0     1741 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/integrins.py
+-rw-r--r--   0        0        0     8866 2023-03-28 21:43:59.156468 pypath_omnipath-0.14.48/pypath/inputs/interpro.py
+-rw-r--r--   0        0        0     2530 2023-03-29 19:46:17.335600 pypath_omnipath-0.14.48/pypath/inputs/intogen.py
+-rw-r--r--   0        0        0     1708 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/ipi.py
+-rw-r--r--   0        0        0     3630 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/iptmnet.py
+-rw-r--r--   0        0        0     3192 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/italk.py
+-rw-r--r--   0        0        0     2557 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/kea.py
+-rw-r--r--   0        0        0    20673 2023-03-29 12:38:13.194490 pypath_omnipath-0.14.48/pypath/inputs/kegg.py
+-rw-r--r--   0        0        0    14746 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/kegg_api.py
+-rw-r--r--   0        0        0     1932 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/kinasedotcom.py
+-rw-r--r--   0        0        0     2522 2023-03-29 14:45:43.764405 pypath_omnipath-0.14.48/pypath/inputs/kirouac2010.py
+-rw-r--r--   0        0        0     4327 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/lambert2018.py
+-rw-r--r--   0        0        0     2174 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/laudanna.py
+-rw-r--r--   0        0        0     5633 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/li2012.py
+-rw-r--r--   0        0        0     2625 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/lincs.py
+-rw-r--r--   0        0        0     2926 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/lmpid.py
+-rw-r--r--   0        0        0     1549 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/lncdisease.py
+-rw-r--r--   0        0        0     2026 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/lncrnadb.py
+-rw-r--r--   0        0        0     7887 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/locate.py
+-rw-r--r--   0        0        0     3648 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/lrdb.py
+-rw-r--r--   0        0        0     2907 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/macrophage.py
+-rw-r--r--   0        0        0      568 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/main.py
+-rw-r--r--   0        0        0     2334 2023-03-28 17:55:35.707415 pypath_omnipath-0.14.48/pypath/inputs/matrisome.py
+-rw-r--r--   0        0        0     4171 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/matrixdb.py
+-rw-r--r--   0        0        0     1107 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/mcam.py
+-rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/membranome.py
+-rw-r--r--   0        0        0     4296 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/mimp.py
+-rw-r--r--   0        0        0     1365 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/mir2disease.py
+-rw-r--r--   0        0        0     3865 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/mirbase.py
+-rw-r--r--   0        0        0     1742 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/mirdeathdb.py
+-rw-r--r--   0        0        0     1659 2023-03-29 17:59:15.511751 pypath_omnipath-0.14.48/pypath/inputs/mirecords.py
+-rw-r--r--   0        0        0     2177 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/mirtarbase.py
+-rw-r--r--   0        0        0     1069 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/mitab.py
+-rw-r--r--   0        0        0     3166 2023-03-23 12:55:18.904569 pypath_omnipath-0.14.48/pypath/inputs/mppi.py
+-rw-r--r--   0        0        0    11491 2023-04-04 23:37:06.309559 pypath_omnipath-0.14.48/pypath/inputs/msigdb.py
+-rw-r--r--   0        0        0     2100 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/ncrdeathdb.py
+-rw-r--r--   0        0        0     1830 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/negatome.py
+-rw-r--r--   0        0        0     1758 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/netbiol.py
+-rw-r--r--   0        0        0     6376 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/netpath.py
+-rw-r--r--   0        0        0     2994 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.48/pypath/inputs/oma.py
+-rw-r--r--   0        0        0     3600 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/ontology.py
+-rw-r--r--   0        0        0     2845 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/opm.py
+-rw-r--r--   0        0        0     2313 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/oreganno.py
+-rw-r--r--   0        0        0     4003 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/panglaodb.py
+-rw-r--r--   0        0        0     3558 2022-12-05 01:12:37.954873 pypath_omnipath-0.14.48/pypath/inputs/pathophenodb.py
+-rw-r--r--   0        0        0     4593 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/pathwaycommons.py
+-rw-r--r--   0        0        0     1071 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/pazar.py
+-rw-r--r--   0        0        0     6333 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/pdb.py
+-rw-r--r--   0        0        0     2411 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/pdzbase.py
+-rw-r--r--   0        0        0     6660 2022-12-05 01:12:34.021729 pypath_omnipath-0.14.48/pypath/inputs/pepcyber.py
+-rw-r--r--   0        0        0     9162 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/pfam.py
+-rw-r--r--   0        0        0     6669 2023-02-23 11:38:30.888776 pypath_omnipath-0.14.48/pypath/inputs/pharos.py
+-rw-r--r--   0        0        0     1673 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/phobius.py
+-rw-r--r--   0        0        0     2299 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/phosphatome.py
+-rw-r--r--   0        0        0     3433 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/phosphoelm.py
+-rw-r--r--   0        0        0     2200 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/phosphonetworks.py
+-rw-r--r--   0        0        0     1299 2022-11-29 10:17:12.515557 pypath_omnipath-0.14.48/pypath/inputs/phosphopoint.py
+-rw-r--r--   0        0        0    37326 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/phosphosite.py
+-rw-r--r--   0        0        0     9976 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/pisa.py
+-rw-r--r--   0        0        0     1850 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/pro.py
+-rw-r--r--   0        0        0     3189 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/progeny.py
+-rw-r--r--   0        0        0     7531 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/proteinatlas.py
+-rw-r--r--   0        0        0     3573 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/proteins.py
+-rw-r--r--   0        0        0     3808 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/protmapper.py
+-rw-r--r--   0        0        0     2463 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/pubchem.py
+-rw-r--r--   0        0        0     4224 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/pubmed.py
+-rw-r--r--   0        0        0     4418 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/ramilowski2015.py
+-rw-r--r--   0        0        0     5426 2023-03-22 21:01:49.738609 pypath_omnipath-0.14.48/pypath/inputs/ramp.py
+-rw-r--r--   0        0        0     6496 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/rdata.py
+-rw-r--r--   0        0        0    40102 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/reaction.py
+-rw-r--r--   0        0        0     7539 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/scconnect.py
+-rw-r--r--   0        0        0     2455 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/science.py
+-rw-r--r--   0        0        0     5578 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/signalink.py
+-rw-r--r--   0        0        0    11727 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/signor.py
+-rw-r--r--   0        0        0     5681 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/spike.py
+-rw-r--r--   0        0        0     4287 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/stitch.py
+-rw-r--r--   0        0        0     7315 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/string.py
+-rw-r--r--   0        0        0     1579 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/surfaceome.py
+-rw-r--r--   0        0        0     4412 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/switches_elm.py
+-rw-r--r--   0        0        0     3225 2022-11-29 10:17:12.528890 pypath_omnipath-0.14.48/pypath/inputs/talklr.py
+-rw-r--r--   0        0        0     2616 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/tcdb.py
+-rw-r--r--   0        0        0     2119 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/tfcensus.py
+-rw-r--r--   0        0        0     7926 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/threedcomplex.py
+-rw-r--r--   0        0        0    17368 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/threedid.py
+-rw-r--r--   0        0        0     3692 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/topdb.py
+-rw-r--r--   0        0        0     1453 2022-11-29 10:17:12.522224 pypath_omnipath-0.14.48/pypath/inputs/transmir.py
+-rw-r--r--   0        0        0     9902 2022-11-29 10:17:12.525557 pypath_omnipath-0.14.48/pypath/inputs/trip.py
+-rw-r--r--   0        0        0     5196 2023-03-19 23:05:05.810094 pypath_omnipath-0.14.48/pypath/inputs/unichem.py
+-rw-r--r--   0        0        0    31311 2022-12-05 01:12:34.025062 pypath_omnipath-0.14.48/pypath/inputs/uniprot.py
+-rw-r--r--   0        0        0     7602 2023-03-29 16:56:14.179505 pypath_omnipath-0.14.48/pypath/inputs/wang.py
+-rw-r--r--   0        0        0     2171 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/inputs/wojtowicz2020.py
+-rw-r--r--   0        0        0     1619 2022-11-29 10:17:12.518890 pypath_omnipath-0.14.48/pypath/inputs/zhong2015.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/__init__.py
+-rw-r--r--   0        0        0    11896 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/annot_formats.py
+-rw-r--r--   0        0        0    21507 2023-03-23 08:10:01.341026 pypath_omnipath-0.14.48/pypath/internals/input_formats.py
+-rw-r--r--   0        0        0    43762 2023-03-27 19:06:47.600564 pypath_omnipath-0.14.48/pypath/internals/intera.py
+-rw-r--r--   0        0        0     7533 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/license.py
+-rw-r--r--   0        0        0     7257 2023-03-06 18:13:55.980766 pypath_omnipath-0.14.48/pypath/internals/maps.py
+-rw-r--r--   0        0        0     4199 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/internals/refs.py
+-rw-r--r--   0        0        0     9673 2023-03-10 13:53:12.961501 pypath_omnipath-0.14.48/pypath/internals/resource.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.14.48/pypath/legacy/__init__.py
+-rw-r--r--   0        0        0     4608 2022-11-29 10:17:12.492224 pypath_omnipath-0.14.48/pypath/legacy/db_categories.py
+-rw-r--r--   0        0        0   556645 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.48/pypath/legacy/main.py
+-rw-r--r--   0        0        0     1768 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/__init__.py
+-rw-r--r--   0        0        0    18012 2023-02-23 11:35:21.780049 pypath_omnipath-0.14.48/pypath/omnipath/app.py
+-rw-r--r--   0        0        0    16321 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.48/pypath/omnipath/bel.py
+-rw-r--r--   0        0        0    16758 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/cellphonedb.py
+-rw-r--r--   0        0        0     1477 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/databases/__init__.py
+-rw-r--r--   0        0        0     1848 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/databases/build.py
+-rw-r--r--   0        0        0     1729 2022-12-05 01:12:34.028395 pypath_omnipath-0.14.48/pypath/omnipath/databases/builtins.json
+-rw-r--r--   0        0        0      522 2022-01-24 11:42:01.191613 pypath_omnipath-0.14.48/pypath/omnipath/databases/classes.json
+-rw-r--r--   0        0        0     8342 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/databases/define.py
+-rw-r--r--   0        0        0    34353 2023-03-27 20:50:05.365575 pypath_omnipath-0.14.48/pypath/omnipath/export.py
+-rw-r--r--   0        0        0     4180 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/legacy.py
+-rw-r--r--   0        0        0     1792 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/param.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/omnipath/server/__init__.py
+-rw-r--r--   0        0        0   122926 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/_html.py
+-rw-r--r--   0        0        0    10455 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/build.py
+-rw-r--r--   0        0        0    17217 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/generate_about_page.py
+-rw-r--r--   0        0        0    11122 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/omnipath/server/legacy.py
+-rw-r--r--   0        0        0    79104 2023-04-06 10:09:25.133831 pypath_omnipath-0.14.48/pypath/omnipath/server/run.py
+-rw-r--r--   0        0        0     4740 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/reader/field.py
+-rw-r--r--   0        0        0     1620 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/reader/network.py
+-rw-r--r--   0        0        0     1013 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/resources/__init__.py
+-rw-r--r--   0        0        0    14229 2023-03-30 21:45:15.125990 pypath_omnipath-0.14.48/pypath/resources/controller.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/resources/data/__init__.py
+-rw-r--r--   0        0        0      139 2023-01-10 18:56:49.559042 pypath_omnipath-0.14.48/pypath/resources/data/complex_input_template.json
+-rw-r--r--   0        0        0      239 2023-01-10 18:56:35.023580 pypath_omnipath-0.14.48/pypath/resources/data/enz_sub_input_template.json
+-rw-r--r--   0        0        0   176408 2023-04-05 14:14:26.002955 pypath_omnipath-0.14.48/pypath/resources/data/resources.json
+-rw-r--r--   0        0        0   100689 2023-03-29 23:22:52.815513 pypath_omnipath-0.14.48/pypath/resources/data_formats.py
+-rw-r--r--   0        0        0   179216 2022-11-29 10:17:12.512224 pypath_omnipath-0.14.48/pypath/resources/descriptions.py
+-rw-r--r--   0        0        0     2817 2022-11-29 10:17:12.508891 pypath_omnipath-0.14.48/pypath/resources/licenses.py
+-rw-r--r--   0        0        0     5389 2023-03-20 15:20:34.662810 pypath_omnipath-0.14.48/pypath/resources/network.py
+-rw-r--r--   0        0        0    72005 2023-03-29 17:58:54.799225 pypath_omnipath-0.14.48/pypath/resources/urls.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.485558 pypath_omnipath-0.14.48/pypath/share/__init__.py
+-rw-r--r--   0        0        0     1801 2023-03-08 22:39:02.796456 pypath_omnipath-0.14.48/pypath/share/cache.py
+-rw-r--r--   0        0        0    69255 2023-04-07 15:32:55.789532 pypath_omnipath-0.14.48/pypath/share/common.py
+-rw-r--r--   0        0        0      852 2023-01-16 16:04:45.977246 pypath_omnipath-0.14.48/pypath/share/constants.py
+-rw-r--r--   0        0        0    57036 2023-03-28 21:12:57.964394 pypath_omnipath-0.14.48/pypath/share/curl.py
+-rw-r--r--   0        0        0     6176 2022-12-05 01:12:34.031728 pypath_omnipath-0.14.48/pypath/share/log.py
+-rw-r--r--   0        0        0    17323 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/lookup/_manytomany.py
+-rw-r--r--   0        0        0     1988 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany.py
+-rw-r--r--   0        0        0     2525 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany2.py
+-rw-r--r--   0        0        0     5284 2022-11-29 10:17:12.482225 pypath_omnipath-0.14.48/pypath/share/progress.py
+-rw-r--r--   0        0        0     4426 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/share/session.py
+-rw-r--r--   0        0        0     9674 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/share/settings.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.492224 pypath_omnipath-0.14.48/pypath/utils/__init__.py
+-rw-r--r--   0        0        0    37321 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/go.py
+-rw-r--r--   0        0        0    56014 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/homology.py
+-rw-r--r--   0        0        0   107424 2023-03-29 12:54:39.165798 pypath_omnipath-0.14.48/pypath/utils/mapping.py
+-rw-r--r--   0        0        0     5765 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/pdb.py
+-rw-r--r--   0        0        0    11855 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/proteomicsdb.py
+-rw-r--r--   0        0        0   109034 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/utils/pyreact.py
+-rw-r--r--   0        0        0     7265 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/reflists.py
+-rw-r--r--   0        0        0     8802 2022-11-29 10:17:12.498891 pypath_omnipath-0.14.48/pypath/utils/residues.py
+-rw-r--r--   0        0        0    11325 2022-11-29 10:17:12.495558 pypath_omnipath-0.14.48/pypath/utils/seq.py
+-rw-r--r--   0        0        0    11255 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/taxonomy.py
+-rw-r--r--   0        0        0    11956 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/unichem.py
+-rw-r--r--   0        0        0    17936 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/utils/uniprot.py
+-rw-r--r--   0        0        0        0 2022-11-29 10:17:12.478891 pypath_omnipath-0.14.48/pypath/visual/__init__.py
+-rw-r--r--   0        0        0    26879 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/drawing.py
+-rw-r--r--   0        0        0    21128 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/__init__.py
+-rw-r--r--   0        0        0    13835 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/edge.py
+-rw-r--r--   0        0        0     4769 2022-12-05 01:12:34.035061 pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/vertex.py
+-rw-r--r--   0        0        0   156771 2022-12-05 01:12:34.038395 pypath_omnipath-0.14.48/pypath/visual/plot.py
+-rw-r--r--   0        0        0     2761 2023-04-12 15:39:36.242305 pypath_omnipath-0.14.48/pyproject.toml
+-rw-r--r--   0        0        0    13420 1970-01-01 00:00:00.000000 pypath_omnipath-0.14.48/setup.py
+-rw-r--r--   0        0        0    13585 1970-01-01 00:00:00.000000 pypath_omnipath-0.14.48/PKG-INFO
```

### Comparing `pypath_omnipath-0.14.44/LICENSE` & `pypath_omnipath-0.14.48/LICENSE`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/README.rst` & `pypath_omnipath-0.14.48/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 The development of ``pypath`` is coordinated by `Dénes Türei`_ in the
 `Saez Lab`_, with the contribution of developers and scientists from
 other groups:
 
 * Erva Ulusoy, Melih Darcan, Ömer Kaan Vural, Tennur Kılıç, Elif Çevrim,
   Bünyamin Şen and Atabey Ünlü in the
   `HU Biological Data Science Lab (PI: Tunca Doğan)`_ created many new input
-  in `pypath`;
+  modules in `pypath`;
 * Leila Gul, Dezső Módos, Márton Ölbei and Tamás Korcsmáros in the
   `Korcsmaros Lab`_ contributed to the overall design of OmniPath, the
   design and implementation of the intercellular communication database,
   and with various case studies and tutorials;
 * Michael Klein from the group of `Fabian Theis`_ developed the
   `Python client`_ for the OmniPath web service;
 * Charles Tapley Hoyt and Daniel Domingo-Fernández added the BEL export
```

### Comparing `pypath_omnipath-0.14.44/pypath/__init__.py` & `pypath_omnipath-0.14.48/pypath/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/_metadata.py` & `pypath_omnipath-0.14.48/pypath/_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 import os
 import pathlib
 import importlib.metadata
 
 import toml
 
-_VERSION = '0.14.44'
+_VERSION = '0.14.48'
 
 
 def get_metadata():
     """
     Basic package metadata.
 
     Retrieves package metadata from the current project directory or from
```

### Comparing `pypath_omnipath-0.14.44/pypath/biocypher/__init__.py` & `pypath_omnipath-0.14.48/pypath/biocypher/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/biocypher/adapter.py` & `pypath_omnipath-0.14.48/pypath/biocypher/adapter.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/annot.py` & `pypath_omnipath-0.14.48/pypath/core/annot.py`

 * *Files 1% similar despite different names*

```diff
@@ -6449,32 +6449,47 @@
 
     def _load_resources(self, definitions, reference_set):
 
         for cls in definitions:
 
             cls = cls if callable(cls) else getattr(self._module, cls)
 
-            try:
+            total_attempts = settings.get('annot_load_resource_attempts')
 
-                annot = cls(
-                    ncbi_tax_id = self.ncbi_tax_id,
-                    reference_set = reference_set,
-                )
+            for attempt in range(total_attempts):
 
-                self.annots[annot.name] = annot
+                try:
 
-            except Exception as e:
+                    self._log(
+                        f'Loading annotation resource `{cls.__name__}`; '
+                        f'attempt {attempt + 1} of {total_attempts}.'
+                    )
+
+                    annot = cls(
+                        ncbi_tax_id = self.ncbi_tax_id,
+                        reference_set = reference_set,
+                    )
+
+                    self.annots[annot.name] = annot
+
+                    self._log(
+                        f'Successfully loaded resource `{cls.__name__}` '
+                        f'({annot.name}).'
+                    )
+                    break
+
+                except Exception as e:
 
-                exc = sys.exc_info()
-                self._log(
-                    'Failed to load annotations from resource `%s`:' % (
-                        cls.__name__ if hasattr(cls, '__name__') else str(cls)
+                    exc = sys.exc_info()
+                    self._log(
+                        'Failed to load annotations from resource `%s`:' % (
+                            cls.__name__ if hasattr(cls, '__name__') else str(cls)
+                        )
                     )
-                )
-                self._log_traceback()
+                    self._log_traceback()
 
 
     def make_dataframe(self, reference_set = None):
 
         if self.create_dataframe:
 
             self.df = self.to_dataframe(reference_set = reference_set)
```

### Comparing `pypath_omnipath-0.14.44/pypath/core/attrs.py` & `pypath_omnipath-0.14.48/pypath/core/attrs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/common.py` & `pypath_omnipath-0.14.48/pypath/core/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/complex.py` & `pypath_omnipath-0.14.48/pypath/core/complex.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,51 +632,61 @@
             return
 
         self.data = {}
         self.summaries = {}
 
         for res in self.resources:
 
-            self._log('Loading resource `%s`.' % str(res))
+            total_attempts = settings.get('complex_load_resource_attempts')
 
-            try:
+            for attempt in range(total_attempts):
 
-                if not callable(res):
+                try:
 
-                    if res in globals():
+                    self._log(
+                        f'Loading resource `{str(res)}`; '
+                        f'attempt {attempt + 1}/{total_attempts}.'
+                    )
 
-                        res = globals()[res]
+                    if not callable(res):
 
-                if callable(res):
+                        if res in globals():
 
-                    processor = res()
+                            res = globals()[res]
 
-                elif hasattr(res, 'complexes'):
+                    if callable(res):
 
-                    processor = res
+                        processor = res()
 
-                if hasattr(processor, 'summary'):
+                    elif hasattr(res, 'complexes'):
 
-                    self.summaries[processor.name] = processor.summary
+                        processor = res
 
-                for key, cplex in iteritems(processor.complexes):
+                    if hasattr(processor, 'summary'):
 
-                    if key in self.data:
+                        self.summaries[processor.name] = processor.summary
 
-                        self.data[key] += cplex
+                    for key, cplex in iteritems(processor.complexes):
 
-                    else:
+                        if key in self.data:
 
-                        self.data[key] = cplex
+                            self.data[key] += cplex
 
-            except Exception:
+                        else:
 
-                exc = sys.exc_info()
-                self._log('Failed to load resource `%s`:' % str(res))
-                self._log_traceback()
+                            self.data[key] = cplex
+
+                    self._log(f'Successfully loaded resource `{str(res)}`.')
+                    break
+
+                except Exception:
+
+                    exc = sys.exc_info()
+                    self._log('Failed to load resource `%s`:' % str(res))
+                    self._log_traceback()
 
         resource.AbstractResource.load(self)
         self.update_index()
         self.update_summaries()
 
 
     def load_from_pickle(self, pickle_file):
```

### Comparing `pypath_omnipath-0.14.44/pypath/core/entity.py` & `pypath_omnipath-0.14.48/pypath/core/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,16 +211,14 @@
 
         self.identifier = identifier
         self.id_type = id_type
         self.entity_type = entity_type
         self.taxon = taxon
 
 
-
-
     @staticmethod
     def entity_name_str(entity):
 
         return (
             entity
                 if isinstance(entity, common.basestring) else
             str(entity)
@@ -340,84 +338,84 @@
 
 
     @classmethod
     def filter_entity_type(cls, entities, entity_type):
         """
         Filters an iterable of entities or identifiers keeping only the ones
         of type(s) in ``entity_type``.
-        
+
         :param iterable entities:
             A list, set, tuple or other iterable yielding entities or
             identifiers.
         :param str,set entity_type:
             One or more entity types e.g. ``{'protein', 'mirna'}``.
-        
+
         :returns:
             Same type of object as ``entities`` if the type of the object is
             list, set or tuple, otherwise a generator.
         """
-        
+
         if not entity_type or not entities:
-            
+
             return entities
-        
+
         entity_type = common.to_set(entity_type)
         obj_type = (
             type(entities)
                 if isinstance(entities, common.list_like) else
             lambda x: x
         )
-        
+
         return obj_type(
             e
             for e in entities
             if cls._get_entity_type(e) in entity_type
         )
-    
-    
+
+
     @classmethod
     def only_proteins(cls, entities):
-        
+
         return cls.filter_entity_type(entities, entity_type = 'protein')
-    
-    
+
+
     @classmethod
     def only_complexes(cls, entities):
-        
+
         return cls.filter_entity_type(entities, entity_type = 'complex')
-    
-    
+
+
     @classmethod
     def only_mirnas(cls, entities):
-        
+
         return cls.filter_entity_type(entities, entity_type = 'mirna')
 
 
     @classmethod
     def count_entity_type(cls, entities, entity_type):
         """
         Counts elements in an iterable of entities or identifiers of type(s)
         in ``entity_type``.
-        
+
         :param iterable entities:
             A list, set, tuple or other iterable yielding entities or
             identifiers.
         :param str,set entity_type:
             One or more entity types e.g. ``{'protein', 'mirna'}``.
-        
+
         :returns:
             int
         """
-        
+
         entities = (
             entities
                 if isinstance(entities, common.list_like) else
             list(entities)
         )
-        
+
         return len(
             cls.filter_entity_type(
                 entities,
                 entity_type = entity_type,
             )
         )
```

### Comparing `pypath_omnipath-0.14.44/pypath/core/enz_sub.py` & `pypath_omnipath-0.14.48/pypath/core/enz_sub.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/evidence.py` & `pypath_omnipath-0.14.48/pypath/core/evidence.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/interaction.py` & `pypath_omnipath-0.14.48/pypath/core/interaction.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/intercell.py` & `pypath_omnipath-0.14.48/pypath/core/intercell.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/intercell_annot.py` & `pypath_omnipath-0.14.48/pypath/core/intercell_annot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/core/network.py` & `pypath_omnipath-0.14.48/pypath/core/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,23 +679,64 @@
         :arg bool only_directions:
             If ``True``, no new interactions will be created but direction
             and effect sign evidences will be added to existing interactions.
         :arg int first_n:
             Load only the first n interactions.
         """
 
-        self._log('Loading network data from resource `%s`.' % resource.name)
+        total_attempts = settings.get('network_load_resource_attempts')
 
-        self._read_resource(
-            resource,
-            reread = reread,
-            redownload = redownload,
-            keep_raw = keep_raw,
-            first_n = first_n,
-        )
+        for attempt in range(total_attempts):
+
+            try:
+
+                self._log(
+                    f'Loading network data from resource `{resource.name}`; '
+                    f'attempt {attempt + 1} of {total_attempts}.'
+                )
+
+                self._read_resource(
+                    resource,
+                    reread = reread,
+                    redownload = redownload,
+                    keep_raw = keep_raw,
+                    first_n = first_n,
+                )
+
+                self._log(
+                    'Successfully read interactions '
+                    f'from resource `{resource.name}`.'
+                )
+                break
+
+            except Exception as e:
+
+                exc = sys.exc_info()
+                self._log(
+                    'Failed to read interactions '
+                    f'from resource `{resource.name}`:'
+                )
+                self._log_traceback()
+
+                try:
+
+                    traceback.print_tb(e.__traceback__, file = sys.stdout)
+
+                except:
+
+                    self._log('Failed to handle exception.')
+                    self._log_traceback()
+
+                if attempt == total_attempts - 1:
+
+                    self._log(
+                        f'Not loading `{resource.name}`: giving up after '
+                        f'{total_attempts} attempts.'
+                    )
+                    return
 
         allow_loops = self._allow_loops(
             allow_loops = allow_loops,
             resource = resource,
         )
 
         self._log('Loops allowed for resource `%s`: %s' % (
@@ -798,14 +839,15 @@
 
         self._log('Expanding complexes for `%s`: %s' % (
             networkinput.name, str(expand_complexes),
         ))
 
         edge_list = []
         edge_list_mapped = []
+        self.edge_list_mapped = []
         infile = None
         _name = networkinput.name.lower()
 
         edges_cache = os.path.join(
             self.cache_dir,
             '%s_%s_%s.edges.pickle' % (
                 _name,
@@ -940,41 +982,30 @@
 
                     _store_cache = curl.CACHE
 
                     if isinstance(redownload, bool):
 
                         curl.CACHE = not redownload
 
-                    # this try-except needs to be removed
-                    # once correct exception handling will
-                    # be implemented in every input function
                     try:
+
                         infile = input_func(**networkinput.input_args)
 
                     except Exception as e:
+
                         self._log(
-                            'Error in method `%s` of the '
+                            f'Error in method `{input_func.__name__}` of the '
                             'pypath.inputs module. '
-                            'Skipping to next resource. '
-                            'See below the traceback.' % input_func.__name__
                         )
-                        self._log_traceback()
-
-                        try:
-                            traceback.print_tb(
-                                e.__traceback__,
-                                file = sys.stdout
-                            )
 
-                        except Exception as e:
+                        raise e
 
-                            self._log('Failed handling exception.')
-                            self._log_traceback()
+                    finally:
 
-                    curl.CACHE = _store_cache
+                        curl.CACHE = _store_cache
 
                 elif os.path.isfile(networkinput.input):
 
                     infile = curl.Curl(
                         networkinput.input,
                         large = True,
                         silent = False,
@@ -1089,40 +1120,40 @@
                         line = [
                             x.replace('\n', '').replace('\r', '')
                                 if hasattr(x, 'replace') else
                             x
                             for x in line
                         ]
 
-                    ## 1) filters
+                    # 1) filters
                     if self._filters(
                         line,
                         networkinput.positive_filters,
                         networkinput.negative_filters
                     ):
 
                         input_filtered += 1
                         continue
 
-                    ## 2) direction
+                    # 2) direction
                     # reading names and attributes:
                     if is_directed and not isinstance(is_directed, tuple):
 
                         this_edge_dir = True
 
                     else:
 
                         this_edge_dir = self._process_direction(
                             line,
                             dir_col,
                             dir_val,
                             dir_sep,
                         )
 
-                    ## 3) references
+                    # 3) references
                     refs = []
 
                     if ref_col is not None:
 
                         if line[ref_col] is None:
 
                             refs = ()
@@ -1137,36 +1168,38 @@
 
                         else:
 
                             refs = line[ref_col].split(ref_sep)
 
                         refs = common.del_empty(list(set(refs)))
 
-                    refs = pubmed_input.only_pmids([str(r).strip() for r in refs])
+                    refs = pubmed_input.only_pmids(
+                        [str(r).strip() for r in refs]
+                    )
 
                     if len(refs) == 0 and must_have_references:
 
                         ref_filtered += 1
                         continue
 
-                    ## 4) entity types
+                    # 4) entity types
                     entity_type_a = self._process_field(
                         networkinput.entity_type_a,
                         line,
                     )
                     entity_type_b = self._process_field(
                         networkinput.entity_type_b,
                         line,
                     )
 
-                    ## 5) ID types
+                    # 5) ID types
                     id_type_a = self._process_field(networkinput.id_type_a, line)
                     id_type_b = self._process_field(networkinput.id_type_b, line)
 
-                    ## 6) organisms
+                    # 6) organisms
                     # to give an easy way for input definition:
                     if isinstance(networkinput.ncbi_tax_id, int):
 
                         taxon_a = (
                             constants.NOT_ORGANISM_SPECIFIC
                                 if entity_type_a in SMOL_TYPES else
                             networkinput.ncbi_tax_id
@@ -1224,25 +1257,25 @@
                         taxon_a = taxon_b = self.ncbi_tax_id
 
                     if taxon_a is None or taxon_b is None:
 
                         taxon_filtered += 1
                         continue
 
-                    ## 7) effect (sign)
+                    # 7) effect (sign)
                     positive = False
                     negative = False
 
                     if isinstance(sign, tuple):
 
                         positive, negative = (
                             self._process_sign(line[sign[0]], sign)
                         )
 
-                    ## 8) resources (source databases)
+                    # 8) resources (source databases)
                     resource = (
                         line[networkinput.resource]
                             if isinstance(networkinput.resource, int) else
                         line[networkinput.resource[0]].split(
                             networkinput.resource[1]
                         )
                             if (
@@ -1265,19 +1298,19 @@
                         )
                         for sec_res in resource
                         if sec_res != _resource.name
                     )
 
                     resource.add(networkinput.name)
 
-                    ## 9) interacting partners
+                    # 9) interacting partners
                     id_a = self._process_partner(networkinput.id_col_a, line)
                     id_b = self._process_partner(networkinput.id_col_b, line)
 
-                    ## 10) further attributes
+                    # 10) further attributes
                     # getting additional edge and node attributes
                     attrs_edge = self._process_attrs(
                         line,
                         networkinput.extra_edge_attrs,
                         lnum,
                     )
                     attrs_node_a = self._process_attrs(
@@ -1287,38 +1320,38 @@
                     )
                     attrs_node_b = self._process_attrs(
                         line,
                         networkinput.extra_node_attrs_b,
                         lnum,
                     )
 
-                    ## 11) creating the Evidence object
+                    # 11) creating the Evidence object
                     evidences = evidence.Evidences(
                         evidences = (
                             evidence.Evidence(
                                 resource = _res,
                                 references = refs,
                                 attrs = attrs_edge,
                             )
                             for _res in
                             _resources_secondary + (_resource,)
                         )
                     )
 
-                    ## 12) node attributes that
-                    ##     depend on the interaction direction
+                    # 12) node attributes that
+                    #     depend on the interaction direction
                     if networkinput.mark_source:
 
                         attrs_node_a[networkinput.mark_source] = this_edge_dir
 
                     if networkinput.mark_target:
 
                         attrs_node_b[networkinput.mark_target] = this_edge_dir
 
-                    ## 13) all interaction data goes into a dict
+                    # 13) all interaction data goes into a dict
                     new_edge = {
                         'id_a': id_a,
                         'id_b': id_b,
                         'id_type_a': id_type_a,
                         'id_type_b': id_type_b,
                         'entity_type_a': entity_type_a,
                         'entity_type_b': entity_type_b,
@@ -1351,35 +1384,22 @@
                         break
 
             except Exception as e:
 
                 self._log(
                     'Error at loading resource `%s`.' % networkinput.name
                 )
-                self._log_traceback()
 
-                try:
-
-                    traceback.print_tb(
-                        e.__traceback__,
-                        file = sys.stdout
-                    )
-
-                except Exception as e:
-
-                    self._log('Failed handling exception.')
-                    self._log_traceback()
-
-                return None
+                raise e
 
             if hasattr(infile, 'close'):
 
                 infile.close()
 
-            ## 14) ID translation of edges
+            # 14) ID translation of edges
             edge_list_mapped = self._map_list(
                 edge_list,
                 expand_complexes = expand_complexes,
             )
 
             self._log(
                 '%u lines have been read from %s, '
@@ -3379,52 +3399,59 @@
 
         new = cls(ncbi_tax_id = ncbi_tax_id, **kwargs)
 
         new.load_dorothea(levels = levels, make_df = make_df)
 
         return new
 
+
     def load_collectri(self, **kwargs):
 
-        self.load(netres.collectri, **kwargs)
+        self.load(network_resources.collectri, **kwargs)
 
 
     @classmethod
     def collectri(cls, ncbi_tax_id = 9606, **kwargs):
         """
         Initializes a new ``Network`` object with loading the transcriptional
         regulation network from CollecTRI.
-
-        :arg NontType,set levels:
-            The confidence levels to include.
         """
 
         make_df = kwargs.pop('make_df', False)
 
         new = cls(ncbi_tax_id = ncbi_tax_id, **kwargs)
 
         new.load_collectri(make_df = make_df)
 
         return new
 
 
     def load_transcription(
             self,
+            collectri = True,
             dorothea = True,
             original_resources = True,
             dorothea_levels = None,
             exclude = None,
             reread = False,
             redownload = False,
             allow_loops = None,
             **kwargs
         ):
 
         make_df = kwargs.pop('make_df', None)
 
+        if collectri:
+
+            self.load_collectri(
+                reread = reread,
+                redownload = redownload,
+                allow_loops = allow_loops,
+            )
+
         if dorothea:
 
             self.load_dorothea(
                 levels = dorothea_levels,
                 reread = reread,
                 redownload = redownload,
                 allow_loops = allow_loops,
```

### Comparing `pypath_omnipath-0.14.44/pypath/data/embl_colors` & `pypath_omnipath-0.14.48/pypath/data/embl_colors`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/data/goose_annotations.sql` & `pypath_omnipath-0.14.48/pypath/data/goose_annotations.sql`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/data/settings.yaml` & `pypath_omnipath-0.14.48/pypath/data/settings.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 msigdb_version: '2023.1'
 
 # Module settings
 network_expand_complexes: false
 network_allow_loops: false
 network_keep_original_names: true
 network_pickle_cache: true
+network_load_resource_attempts: 3
 go_pickle_cache: true
 network_extra_directions: !!set
   PhosphoSite_noref: null
   PhosphoSite: null
   STRING: null
   CancerCellMap: null
   ACSN: null
@@ -147,14 +148,21 @@
 keep_noref: false
 annot_infer_complexes: true
   # the annotation classes should infer complex annotations
   # from protein annotations
 annot_composite_database_name: OmniPath
   # the resource name for annotation categories
   # combined from multiple original resources
+annot_load_resource_attempts: 3
+  # number of attempts to load a resource
+  # when building the Annotations database
+
+complex_load_resource_attempts: 3
+  # number of attempts to load a resource
+  # when building the Complexes database
 
 # load small, specific categories from CellPhoneDB
   # in the intercell database
 intercell_cellphonedb_categories: true
 intercell_baccin_categories: true # same for Baccin2019 and some others
 intercell_hpmr_categories: true
 intercell_surfaceome_categories: true
```

### Comparing `pypath_omnipath-0.14.44/pypath/data/www/favicon.ico` & `pypath_omnipath-0.14.48/pypath/data/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/formats/obo.py` & `pypath_omnipath-0.14.48/pypath/formats/obo.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/formats/sqldump.py` & `pypath_omnipath-0.14.48/pypath/formats/sqldump.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/formats/sqlite.py` & `pypath_omnipath-0.14.48/pypath/formats/sqlite.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/formats/xml.py` & `pypath_omnipath-0.14.48/pypath/formats/xml.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/__init__.py` & `pypath_omnipath-0.14.48/pypath/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/abs.py` & `pypath_omnipath-0.14.48/pypath/inputs/abs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/acsn.py` & `pypath_omnipath-0.14.48/pypath/inputs/acsn.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/adhesome.py` & `pypath_omnipath-0.14.48/pypath/inputs/adhesome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/almen2009.py` & `pypath_omnipath-0.14.48/pypath/inputs/almen2009.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/baccin2019.py` & `pypath_omnipath-0.14.48/pypath/inputs/baccin2019.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/biogps.py` & `pypath_omnipath-0.14.48/pypath/inputs/biogps.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/biogrid.py` & `pypath_omnipath-0.14.48/pypath/inputs/biogrid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/biomart.py` & `pypath_omnipath-0.14.48/pypath/inputs/biomart.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/biomodels.py` & `pypath_omnipath-0.14.48/pypath/inputs/biomodels.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ca1.py` & `pypath_omnipath-0.14.48/pypath/inputs/ca1.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cancercellmap.py` & `pypath_omnipath-0.14.48/pypath/inputs/cancercellmap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cancerdrugsdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/cancerdrugsdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cancersea.py` & `pypath_omnipath-0.14.48/pypath/inputs/cancersea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cell.py` & `pypath_omnipath-0.14.48/pypath/inputs/cell.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cellcall.py` & `pypath_omnipath-0.14.48/pypath/inputs/cellcall.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cellcellinteractions.py` & `pypath_omnipath-0.14.48/pypath/inputs/cellcellinteractions.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cellchatdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/cellchatdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cellinker.py` & `pypath_omnipath-0.14.48/pypath/inputs/cellinker.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cellphonedb.py` & `pypath_omnipath-0.14.48/pypath/inputs/cellphonedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/celltalkdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/celltalkdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/celltypist.py` & `pypath_omnipath-0.14.48/pypath/inputs/celltypist.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/chembl.py` & `pypath_omnipath-0.14.48/pypath/inputs/chembl.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/clinvar.py` & `pypath_omnipath-0.14.48/pypath/inputs/clinvar.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,22 +28,21 @@
 Variant data from the Clinvar database.
 """
 
 from __future__ import annotations
 
 import io
 import csv
-import sys
+import ctypes
 import collections
 
 import pypath.share.curl as curl
 import pypath.resources.urls as urls
 
-csv.field_size_limit(sys.maxsize)
-
+csv.field_size_limit(int(ctypes.c_ulong(-1).value // 2))
 
 def clinvar_raw() -> list[tuple]:
     """
     Retrieves variant data from the Clinvar database.
 
     Returns:
         Variants as a list of named tuples.
@@ -140,8 +139,8 @@
             nsv = row['nsv'],
             citation_source = row['citation_source'],
             citation_id = row['citation_id']
         )
 
         result.add(citation)
 
-    return list(result)
+    return list(result)
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/collectri.py` & `pypath_omnipath-0.14.48/pypath/inputs/collectri.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         result.append(
             CollectriRecord(
                 tf = l[0],
                 target = target_id,
                 effect = int(l[2]),
                 tf_category = l[3],
-                resources = l[4],
+                resources = l[4].replace('DoRothEA_A', 'DoRothEA-A'),
                 pubmed = l[5],
                 target_type = 'mirna' if mmirna else 'protein',
             )
         )
 
     return result
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/common.py` & `pypath_omnipath-0.14.48/pypath/inputs/common.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/compleat.py` & `pypath_omnipath-0.14.48/pypath/inputs/compleat.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/complexportal.py` & `pypath_omnipath-0.14.48/pypath/inputs/complexportal.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/comppi.py` & `pypath_omnipath-0.14.48/pypath/inputs/comppi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/connectomedb.py` & `pypath_omnipath-0.14.48/pypath/inputs/connectomedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/corum.py` & `pypath_omnipath-0.14.48/pypath/inputs/corum.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cosmic.py` & `pypath_omnipath-0.14.48/pypath/inputs/cosmic.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cpad.py` & `pypath_omnipath-0.14.48/pypath/inputs/cpad.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cpdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/cpdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/credentials.py` & `pypath_omnipath-0.14.48/pypath/inputs/credentials.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/csa.py` & `pypath_omnipath-0.14.48/pypath/inputs/csa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cspa.py` & `pypath_omnipath-0.14.48/pypath/inputs/cspa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ctdbase.py` & `pypath_omnipath-0.14.48/pypath/inputs/ctdbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/cytosig.py` & `pypath_omnipath-0.14.48/pypath/inputs/cytosig.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/dbptm.py` & `pypath_omnipath-0.14.48/pypath/inputs/dbptm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/deathdomain.py` & `pypath_omnipath-0.14.48/pypath/inputs/deathdomain.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/depod.py` & `pypath_omnipath-0.14.48/pypath/inputs/depod.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/dgidb.py` & `pypath_omnipath-0.14.48/pypath/inputs/dgidb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/dip.py` & `pypath_omnipath-0.14.48/pypath/inputs/dip.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/disgenet.py` & `pypath_omnipath-0.14.48/pypath/inputs/disgenet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/domino.py` & `pypath_omnipath-0.14.48/pypath/inputs/domino.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/dorothea.py` & `pypath_omnipath-0.14.48/pypath/inputs/dorothea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/drugbank.py` & `pypath_omnipath-0.14.48/pypath/inputs/drugbank.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/drugcentral.py` & `pypath_omnipath-0.14.48/pypath/inputs/drugcentral.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ebi.py` & `pypath_omnipath-0.14.48/pypath/inputs/ebi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/elm.py` & `pypath_omnipath-0.14.48/pypath/inputs/elm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/embopress.py` & `pypath_omnipath-0.14.48/pypath/inputs/embopress.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/embrace.py` & `pypath_omnipath-0.14.48/pypath/inputs/embrace.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/encode.py` & `pypath_omnipath-0.14.48/pypath/inputs/encode.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ensembl.py` & `pypath_omnipath-0.14.48/pypath/inputs/ensembl.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #  See accompanying file LICENSE.txt or copy at
 #      http://www.gnu.org/licenses/gpl-3.0.html
 #
 #  Website: http://pypath.omnipathdb.org/
 #
 
 import collections
+import warnings
 
 import bs4
 
 import pypath.resources.urls as urls
 import pypath.share.curl as curl
 
 
@@ -44,15 +45,19 @@
         List of named tuples.
     """
 
     record = None
     result = []
     url = urls.urls['ensembl']['species']
     c = curl.Curl(url)
-    soup = bs4.BeautifulSoup(c.result, 'html.parser')
+
+    with warnings.catch_warnings():
+
+        warnings.simplefilter('ignore', bs4.XMLParsedAsHTMLWarning)
+        soup = bs4.BeautifulSoup(c.result, 'html.parser')
 
     for r in soup.find('table').find_all('tr'):
 
         if not record:
 
             record = collections.namedtuple(
                 'EnsemblOrganism',
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/exocarta.py` & `pypath_omnipath-0.14.48/pypath/inputs/exocarta.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/genecards.py` & `pypath_omnipath-0.14.48/pypath/inputs/genecards.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/go.py` & `pypath_omnipath-0.14.48/pypath/inputs/go.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/gpcrdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/gpcrdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/graphviz.py` & `pypath_omnipath-0.14.48/pypath/inputs/graphviz.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/guide2pharma.py` & `pypath_omnipath-0.14.48/pypath/inputs/guide2pharma.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/havugimana.py` & `pypath_omnipath-0.14.48/pypath/inputs/havugimana.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/hgnc.py` & `pypath_omnipath-0.14.48/pypath/inputs/hgnc.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/hippie.py` & `pypath_omnipath-0.14.48/pypath/inputs/hippie.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/hmdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/hmdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/homologene.py` & `pypath_omnipath-0.14.48/pypath/inputs/homologene.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/hpmr.py` & `pypath_omnipath-0.14.48/pypath/inputs/hpmr.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/hpo.py` & `pypath_omnipath-0.14.48/pypath/inputs/hpo.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/hprd.py` & `pypath_omnipath-0.14.48/pypath/inputs/hprd.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/htri.py` & `pypath_omnipath-0.14.48/pypath/inputs/htri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/humancellmap.py` & `pypath_omnipath-0.14.48/pypath/inputs/humancellmap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/humap.py` & `pypath_omnipath-0.14.48/pypath/inputs/humap.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/huri.py` & `pypath_omnipath-0.14.48/pypath/inputs/huri.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/i3d.py` & `pypath_omnipath-0.14.48/pypath/inputs/i3d.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/icellnet.py` & `pypath_omnipath-0.14.48/pypath/inputs/icellnet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ielm.py` & `pypath_omnipath-0.14.48/pypath/inputs/ielm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/imweb.py` & `pypath_omnipath-0.14.48/pypath/inputs/imweb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/innatedb.py` & `pypath_omnipath-0.14.48/pypath/inputs/innatedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/instruct.py` & `pypath_omnipath-0.14.48/pypath/inputs/instruct.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/intact.py` & `pypath_omnipath-0.14.48/pypath/inputs/intact.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/integrins.py` & `pypath_omnipath-0.14.48/pypath/inputs/integrins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/interpro.py` & `pypath_omnipath-0.14.48/pypath/inputs/interpro.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/intogen.py` & `pypath_omnipath-0.14.48/pypath/inputs/intogen.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 import csv
 import collections
 
 import pypath.resources.urls as urls
 import pypath.share.curl as curl
 import pypath.share.common as common
+import pypath.share.settings as settings
 import pypath.utils.mapping as mapping
 
 
 def intogen_annotations():
     """
     Returns a list of cancer driver genes with their annotations,
     according to the IntOGen database.
@@ -48,21 +49,23 @@
             'oncodrive_role_prob',
         ],
     )
 
 
     url = urls.urls['intogen']['db2014_2']
 
-    c = curl.Curl(
-        url,
-        large = True,
-        silent = False,
-        files_needed = ['Drivers_type_role.tsv'],
-        compr = 'zip',
-    )
+    with settings.context(curl_connect_timeout = 100):
+
+        c = curl.Curl(
+            url,
+            large = True,
+            silent = False,
+            files_needed = ['Drivers_type_role.tsv'],
+            compr = 'zip',
+        )
 
     for _ in xrange(7):
 
         __ = c.result['Drivers_type_role.tsv'].readline()
 
     data = csv.DictReader(
         c.result['Drivers_type_role.tsv'],
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ipi.py` & `pypath_omnipath-0.14.48/pypath/inputs/ipi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/iptmnet.py` & `pypath_omnipath-0.14.48/pypath/inputs/iptmnet.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/italk.py` & `pypath_omnipath-0.14.48/pypath/inputs/italk.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/kea.py` & `pypath_omnipath-0.14.48/pypath/inputs/kea.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/kegg.py` & `pypath_omnipath-0.14.48/pypath/inputs/kegg.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,14 +276,15 @@
         '->': ('post_translational', 'stimulation'),
         '=>': ('transcriptional', 'stimulation'),
         '//': ('post_translational', 'missing'),
         '-|': ('post_translational', 'inhibition'),
         '=|': ('transcriptional', 'inhibition'),
         '--': ('post_translational', 'undirected'),
         '>>': ('post_translational', 'enzyme_enzyme'),
+        '==': ('post_translational', 'missing'),
     }
 
 
     def process_entity(e):
 
         if isinstance(e, common.basestring):
 
@@ -483,15 +484,16 @@
 
             enames[_id] = (name, entity_type)
 
         return enames[_id]
 
 
     recollect = re.compile(r'^(GENE|PERTURBANT|VARIANT|METABOLITE)')
-    recon = re.compile(r'(->|--|//|-\||=>|>>|=\|)')
+    recon = re.compile(r'(->|--|//|-\||=>|>>|=\||==)')
+    rewrongspace = re.compile(r'(\d+) (?=\d+)')
     result = set()
     url = urls.urls['kegg_pws']['medicus']
     c = curl.Curl(url, silent = False, large = True)
     enames = {}
     collecting = None
 
     for row in c.result:
@@ -551,14 +553,15 @@
 
             pw_type = row.strip().split()[-1].lower()
 
         elif row.startswith('  EXPANDED'):
 
             connections = renetref.sub('', row)
             connections = recon.sub(' \g<1> ', connections)
+            connections = rewrongspace.sub('\g<1>,', connections)
             connections = connections.split()[1:]
 
         elif row.startswith('///'):
 
             result.update(
                 set(get_interactions(
                     connections,
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/kegg_api.py` & `pypath_omnipath-0.14.48/pypath/inputs/kegg_api.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/kinasedotcom.py` & `pypath_omnipath-0.14.48/pypath/inputs/kinasedotcom.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/kirouac2010.py` & `pypath_omnipath-0.14.48/pypath/inputs/kirouac2010.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/lambert2018.py` & `pypath_omnipath-0.14.48/pypath/inputs/lambert2018.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/laudanna.py` & `pypath_omnipath-0.14.48/pypath/inputs/laudanna.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/li2012.py` & `pypath_omnipath-0.14.48/pypath/inputs/li2012.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/lincs.py` & `pypath_omnipath-0.14.48/pypath/inputs/lincs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/lmpid.py` & `pypath_omnipath-0.14.48/pypath/inputs/lmpid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/lncdisease.py` & `pypath_omnipath-0.14.48/pypath/inputs/lncdisease.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/lncrnadb.py` & `pypath_omnipath-0.14.48/pypath/inputs/lncrnadb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/locate.py` & `pypath_omnipath-0.14.48/pypath/inputs/locate.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/lrdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/lrdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/macrophage.py` & `pypath_omnipath-0.14.48/pypath/inputs/macrophage.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/main.py` & `pypath_omnipath-0.14.48/pypath/inputs/main.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/matrisome.py` & `pypath_omnipath-0.14.48/pypath/inputs/matrisome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/matrixdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/matrixdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mcam.py` & `pypath_omnipath-0.14.48/pypath/inputs/mcam.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/membranome.py` & `pypath_omnipath-0.14.48/pypath/inputs/membranome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mimp.py` & `pypath_omnipath-0.14.48/pypath/inputs/mimp.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mir2disease.py` & `pypath_omnipath-0.14.48/pypath/inputs/mir2disease.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mirbase.py` & `pypath_omnipath-0.14.48/pypath/inputs/mirbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mirdeathdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/mirdeathdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mirecords.py` & `pypath_omnipath-0.14.48/pypath/inputs/mirecords.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             'target_genesymbol',
             'mirna_organism',
             'target_organism',
             'pmid',
         ),
     )
 
-    url = urls.urls['mirecords']['url']
+    url = urls.urls['mirecords']['url_rescued']
     c = curl.Curl(url, silent = False, large = True)
 
     tbl = inputs_common.read_xls(c.fileobj.name)
 
     c.close()
 
     return [
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mirtarbase.py` & `pypath_omnipath-0.14.48/pypath/inputs/mirtarbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mitab.py` & `pypath_omnipath-0.14.48/pypath/inputs/mitab.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/mppi.py` & `pypath_omnipath-0.14.48/pypath/inputs/mppi.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/msigdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/msigdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     'wikipathways': ('c2.cp.wikipathways', 'm2.cp.wikipathways'),
     'mirna_targets_mirdb': ('c3.mir.mirdb', 'm3.mirdb'),
     'mirna_targets_legacy': ('c3.mir.mir_legacy', None),
     'tf_targets_gtrf': ('c3.tft.gtrd', 'm3.gtrd'),
     'tf_targets_legacy': ('c3.tft.tft_legacy', None),
     'cancer_gene_neighborhoods': ('c4.cgn', None),
     'cancer_modules': ('c4.cm', None),
-    'go_biological_process': ('c5.bp', 'm5.bp'),
-    'go_molecular_function': ('c5.mf', 'm5.mf'),
-    'go_cellular_component': ('c5.cc', 'm5.cc'),
+    'go_biological_process': ('c5.go.bp', 'm5.go.bp'),
+    'go_molecular_function': ('c5.go.mf', 'm5.go.mf'),
+    'go_cellular_component': ('c5.go.cc', 'm5.go.cc'),
     'human_phenotype_ontology': ('c5.hpo', None),
     'mouse_phenotype_ontology': (None, 'm5.mpt'),
     'oncogenic_signatures': ('c6.all', None),
     'immunesigdb': ('c7.immunesigdb', None),
     'vaccine_response': ('c7.vax', None),
     'cell_type_signatures': ('c8.all', 'm8.all'),
 }
@@ -262,19 +262,20 @@
     lower level keys are geneset names and values are molecular identifiers.
 
     :arg str,NoneType registered_email:
         An email address registered at MSigDB. If `None` the `msigdb_email`
         from ``pypath.settings`` will be used.
     :arg set,NoneType only_collections:
         Limit the annotations only to these collections. For available
-        collections e.g. ``{'h.all', 'c2cgp'}`` refer to the MSigDB webpage:
+        collections e.g. ``{'h.all', 'c2.cgp'}`` refer to the MSigDB webpage:
         http://software.broadinstitute.org/gsea/downloads.jsp#msigdb
     :arg tuple exclude:
         Exclude the collections having their name starting with any of the
-        strings in this tuple. By default `c5` (Gene Ontology) is excluded.
+        strings in this tuple. By default `c5` and `m5` (Gene Ontology and
+        Human/Mouse Phenotype Ontology) is excluded.
     """
 
     collection_data = {}
 
     organisms = {9606: 0, 10090: 1}
     ncbi_tax_id = taxonomy.ensure_ncbi_tax_id(organism)
     idx = organisms.get(ncbi_tax_id, None)
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ncrdeathdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/ncrdeathdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/negatome.py` & `pypath_omnipath-0.14.48/pypath/inputs/negatome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/netbiol.py` & `pypath_omnipath-0.14.48/pypath/inputs/netbiol.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/netpath.py` & `pypath_omnipath-0.14.48/pypath/inputs/netpath.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/oma.py` & `pypath_omnipath-0.14.48/pypath/inputs/oma.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ontology.py` & `pypath_omnipath-0.14.48/pypath/inputs/ontology.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/opm.py` & `pypath_omnipath-0.14.48/pypath/inputs/opm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/oreganno.py` & `pypath_omnipath-0.14.48/pypath/inputs/oreganno.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/panglaodb.py` & `pypath_omnipath-0.14.48/pypath/inputs/panglaodb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pathophenodb.py` & `pypath_omnipath-0.14.48/pypath/inputs/pathophenodb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pathwaycommons.py` & `pypath_omnipath-0.14.48/pypath/inputs/pathwaycommons.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pazar.py` & `pypath_omnipath-0.14.48/pypath/inputs/pazar.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/pdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pdzbase.py` & `pypath_omnipath-0.14.48/pypath/inputs/pdzbase.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pepcyber.py` & `pypath_omnipath-0.14.48/pypath/inputs/pepcyber.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pfam.py` & `pypath_omnipath-0.14.48/pypath/inputs/pfam.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pharos.py` & `pypath_omnipath-0.14.48/pypath/inputs/pharos.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/phobius.py` & `pypath_omnipath-0.14.48/pypath/inputs/phobius.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/phosphatome.py` & `pypath_omnipath-0.14.48/pypath/inputs/phosphatome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/phosphoelm.py` & `pypath_omnipath-0.14.48/pypath/inputs/phosphoelm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/phosphonetworks.py` & `pypath_omnipath-0.14.48/pypath/inputs/phosphonetworks.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/phosphopoint.py` & `pypath_omnipath-0.14.48/pypath/inputs/phosphopoint.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/phosphosite.py` & `pypath_omnipath-0.14.48/pypath/inputs/phosphosite.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pisa.py` & `pypath_omnipath-0.14.48/pypath/inputs/pisa.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pro.py` & `pypath_omnipath-0.14.48/pypath/inputs/pro.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/progeny.py` & `pypath_omnipath-0.14.48/pypath/inputs/progeny.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/proteinatlas.py` & `pypath_omnipath-0.14.48/pypath/inputs/proteinatlas.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/proteins.py` & `pypath_omnipath-0.14.48/pypath/inputs/proteins.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/protmapper.py` & `pypath_omnipath-0.14.48/pypath/inputs/protmapper.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pubchem.py` & `pypath_omnipath-0.14.48/pypath/inputs/pubchem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/pubmed.py` & `pypath_omnipath-0.14.48/pypath/inputs/pubmed.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ramilowski2015.py` & `pypath_omnipath-0.14.48/pypath/inputs/ramilowski2015.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/ramp.py` & `pypath_omnipath-0.14.48/pypath/inputs/ramp.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/rdata.py` & `pypath_omnipath-0.14.48/pypath/inputs/rdata.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/reaction.py` & `pypath_omnipath-0.14.48/pypath/inputs/reaction.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/scconnect.py` & `pypath_omnipath-0.14.48/pypath/inputs/scconnect.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/science.py` & `pypath_omnipath-0.14.48/pypath/inputs/science.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/signalink.py` & `pypath_omnipath-0.14.48/pypath/inputs/signalink.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/signor.py` & `pypath_omnipath-0.14.48/pypath/inputs/signor.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/spike.py` & `pypath_omnipath-0.14.48/pypath/inputs/spike.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/stitch.py` & `pypath_omnipath-0.14.48/pypath/inputs/stitch.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/string.py` & `pypath_omnipath-0.14.48/pypath/inputs/string.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/surfaceome.py` & `pypath_omnipath-0.14.48/pypath/inputs/surfaceome.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/switches_elm.py` & `pypath_omnipath-0.14.48/pypath/inputs/switches_elm.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/talklr.py` & `pypath_omnipath-0.14.48/pypath/inputs/talklr.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/tcdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/tcdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/tfcensus.py` & `pypath_omnipath-0.14.48/pypath/inputs/tfcensus.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/threedcomplex.py` & `pypath_omnipath-0.14.48/pypath/inputs/threedcomplex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/threedid.py` & `pypath_omnipath-0.14.48/pypath/inputs/threedid.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/topdb.py` & `pypath_omnipath-0.14.48/pypath/inputs/topdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/transmir.py` & `pypath_omnipath-0.14.48/pypath/inputs/transmir.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/trip.py` & `pypath_omnipath-0.14.48/pypath/inputs/trip.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/unichem.py` & `pypath_omnipath-0.14.48/pypath/inputs/unichem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/uniprot.py` & `pypath_omnipath-0.14.48/pypath/inputs/uniprot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/wang.py` & `pypath_omnipath-0.14.48/pypath/inputs/wang.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 }
 
 
 ca1_interactions = ca1.ca1_interactions
 
 
 def hsn_interactions(
-        source: Literal['rescued', 'researchgate'] = 'researchgate',
+        source: Literal['rescued', 'researchgate'] = 'rescued',
     ) -> List[tuple]:
     """
     Downloads and processes HumanSignalingNetwork version 6
     (published 2014 Jan by Edwin Wang).
 
     Args
         source: The same file is available from two domains: the OmniPath
```

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/wojtowicz2020.py` & `pypath_omnipath-0.14.48/pypath/inputs/wojtowicz2020.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/inputs/zhong2015.py` & `pypath_omnipath-0.14.48/pypath/inputs/zhong2015.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/annot_formats.py` & `pypath_omnipath-0.14.48/pypath/internals/annot_formats.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/input_formats.py` & `pypath_omnipath-0.14.48/pypath/internals/input_formats.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/intera.py` & `pypath_omnipath-0.14.48/pypath/internals/intera.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/license.py` & `pypath_omnipath-0.14.48/pypath/internals/license.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/maps.py` & `pypath_omnipath-0.14.48/pypath/internals/maps.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/refs.py` & `pypath_omnipath-0.14.48/pypath/internals/refs.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/internals/resource.py` & `pypath_omnipath-0.14.48/pypath/internals/resource.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/legacy/db_categories.py` & `pypath_omnipath-0.14.48/pypath/legacy/db_categories.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/legacy/main.py` & `pypath_omnipath-0.14.48/pypath/legacy/main.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/__init__.py` & `pypath_omnipath-0.14.48/pypath/omnipath/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/app.py` & `pypath_omnipath-0.14.48/pypath/omnipath/app.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/bel.py` & `pypath_omnipath-0.14.48/pypath/omnipath/bel.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/cellphonedb.py` & `pypath_omnipath-0.14.48/pypath/omnipath/cellphonedb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/databases/__init__.py` & `pypath_omnipath-0.14.48/pypath/omnipath/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/databases/build.py` & `pypath_omnipath-0.14.48/pypath/omnipath/databases/build.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/databases/builtins.json` & `pypath_omnipath-0.14.48/pypath/omnipath/databases/builtins.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/databases/classes.json` & `pypath_omnipath-0.14.48/pypath/omnipath/databases/classes.json`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/databases/define.py` & `pypath_omnipath-0.14.48/pypath/omnipath/databases/define.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/export.py` & `pypath_omnipath-0.14.48/pypath/omnipath/export.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/legacy.py` & `pypath_omnipath-0.14.48/pypath/omnipath/legacy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/param.py` & `pypath_omnipath-0.14.48/pypath/omnipath/param.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/server/_html.py` & `pypath_omnipath-0.14.48/pypath/omnipath/server/_html.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/server/build.py` & `pypath_omnipath-0.14.48/pypath/omnipath/server/build.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/server/generate_about_page.py` & `pypath_omnipath-0.14.48/pypath/omnipath/server/generate_about_page.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/server/legacy.py` & `pypath_omnipath-0.14.48/pypath/omnipath/server/legacy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/omnipath/server/run.py` & `pypath_omnipath-0.14.48/pypath/omnipath/server/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,28 @@
 import sys
 import os
 import re
 import copy
 import collections
 import itertools
 import hashlib
+import warnings
+import contextlib
 
 from pypath.share import session as session_mod
 
 _logger = session_mod.Logger(name = 'server')
 _log = _logger._log
 
 try:
     import twisted.web.resource
     import twisted.web.server
-    import twisted.internet
+    import twisted.internet.reactor
     TwistedWebResource = twisted.web.resource.Resource
-    TwistedWebSite = Twisted.web.server.Site
+    TwistedWebSite = twisted.web.server.Site
     TWISTED_NOT_DONE_YET = twisted.web.server.NOT_DONE_YET
     twisted_listen_tcp = twisted.internet.reactor.listenTCP
     twisted_run = twisted.internet.reactor.run
 except:
     _log('No module `twisted` available. Necessary to run HTTP server.', -1)
     class TwistedWebResource: pass
     class TwistedWebSite: pass
@@ -81,14 +83,30 @@
 
 
 def stop_server():
 
     reactor.removeAll()
 
 
+@contextlib.contextmanager
+def ignore_pandas_copywarn():
+
+    try:
+
+        with warnings.catch_warnings():
+
+            warnings.simplefilter('ignore', pd.errors.SettingWithCopyWarning)
+
+            yield
+
+    finally:
+
+        pass
+
+
 class BaseServer(TwistedWebResource, session_mod.Logger):
 
 
     recomment = re.compile(b'<!--\s*Title:(.*?)-->')
 
 
     def __init__(self):
@@ -1296,14 +1314,17 @@
 
         for name, fname in iteritems(self.input_files):
 
             if name not in self.to_load:
 
                 continue
 
+            fname_gz = f'{fname}.gz'
+            fname = fname_gz if os.path.exists(fname_gz) else fname
+
             self._log('Loading dataset `%s` from file `%s`.' % (name, fname))
 
             if not os.path.exists(fname):
 
                 self._log(
                     'Missing table: `%s`.' % fname
                 )
@@ -1374,20 +1395,23 @@
 
         if 'complexes' not in self.data:
 
             return
 
         self._log('Preprocessing complexes.')
         tbl = self.data['complexes']
-        tbl['set_sources'] = pd.Series(
-            [set(s.split(';')) for s in tbl.sources]
-        )
-        tbl['set_proteins'] = pd.Series(
-            [set(c.split('_')) for c in tbl.components]
-        )
+
+        tbl = tbl[~tbl.components.isna()]
+
+        with ignore_pandas_copywarn():
+
+            tbl['set_sources'] = [set(s.split(';')) for s in tbl.sources]
+            tbl['set_proteins'] = [set(c.split('_')) for c in tbl.components]
+
+        self.data['complexes'] = tbl
 
 
     def _preprocess_annotations_old(self):
 
         if 'annotations' not in self.data:
 
             return
@@ -2762,15 +2786,15 @@
             ]
 
             if composite:
 
                 composite_to_remove = {
                     comp_res
                     for comp_res in composite
-                    if not res_ctrl.secondary_resources(comp_res) & res
+                    if not res_ctrl.secondary_resources(comp_res, True) & res
                 }
 
                 res = res - composite_to_remove
 
             return res
 
 
@@ -2793,18 +2817,21 @@
 
             _set_res_col = tbl.set_sources
 
             _res_to_keep = [
                 filter_resources(ress)
                 for ress in _set_res_col
             ]
-            tbl[res_col] = [
-                ';'.join(sorted(ress))
-                for ress in _res_to_keep
-            ]
+
+            with ignore_pandas_copywarn():
+
+                tbl[res_col] = [
+                    ';'.join(sorted(ress))
+                    for ress in _res_to_keep
+                ]
 
             if prefix_col:
 
                 _prefix_col = getattr(tbl, prefix_col)
 
                 _new_prefix_col = [
 
@@ -2820,15 +2847,17 @@
                         if isinstance(pref_ress, common.basestring) else
 
                     pref_ress
 
                     for i, pref_ress in enumerate(_prefix_col)
                 ]
 
-                tbl[prefix_col] = _new_prefix_col
+                with ignore_pandas_copywarn():
+
+                    tbl[prefix_col] = _new_prefix_col
 
             bool_idx = [bool(res) for res in tbl[res_col]]
 
         tbl = tbl.loc[bool_idx]
 
         return tbl
```

### Comparing `pypath_omnipath-0.14.44/pypath/reader/field.py` & `pypath_omnipath-0.14.48/pypath/reader/field.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/reader/network.py` & `pypath_omnipath-0.14.48/pypath/reader/network.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/resources/__init__.py` & `pypath_omnipath-0.14.48/pypath/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/resources/controller.py` & `pypath_omnipath-0.14.48/pypath/resources/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from typing import Iterable, Literal
 
 import json
 import os
 import copy
 import importlib as imp
 import itertools
+import functools
 
 import pypath.share.session as session_mod
 import pypath.share.common as common
 import pypath.internals.resource as resource_base
 import pypath.resources.network as netres
 from . import licenses as licenses
 
@@ -200,19 +201,34 @@
         if name in self.synonyms:
 
             name = self.synonyms[name]
 
         return name
 
 
-    def secondary_resources(self, name):
+    @functools.cache
+    def secondary_resources(self, name, postfix = False):
+        """
+        Args:
+            name:
+                Name of a composite resource.
+            postfix:
+                Append the name of the primary resource to the secondary,
+                separated by an underscore, e.g. "TFactS_CollecTRI".
+        """
 
         name = self.name(name)
 
-        return self.secondary[name] if name in self.secondary else set()
+        secondary = self.secondary.get(name, set())
+
+        if postfix:
+
+            secondary = {f'{sec}_{name}' for sec in secondary}
+
+        return secondary
 
 
     def _get(self, name, dct):
 
         if name in dct:
 
             return dct[name]
```

### Comparing `pypath_omnipath-0.14.44/pypath/resources/data/resources.json` & `pypath_omnipath-0.14.48/pypath/resources/data/resources.json`

 * *Files 0% similar despite different names*

```diff
@@ -10957,64 +10957,70 @@
 0002acc0: 2020 2254 5252 5553 5422 2c0a 2020 2020    "TRRUST",.    
 0002acd0: 2020 2253 4947 4e4f 5222 2c0a 2020 2020    "SIGNOR",.    
 0002ace0: 2020 2243 7974 5265 6722 2c0a 2020 2020    "CytReg",.    
 0002acf0: 2020 2247 4552 4544 4222 2c0a 2020 2020    "GEREDB",.    
 0002ad00: 2020 2250 6176 6c69 6469 7322 2c0a 2020    "Pavlidis",.  
 0002ad10: 2020 2020 2244 6f52 6f74 6845 415f 4122      "DoRothEA_A"
 0002ad20: 2c0a 2020 2020 2020 224e 544e 5563 7572  ,.      "NTNUcur
-0002ad30: 6174 696f 6e22 0a20 2020 205d 0a20 2020  ation".    ].   
-0002ad40: 2022 7572 6c73 223a 207b 0a20 2020 2020   "urls": {.     
-0002ad50: 2022 7765 6270 6167 6573 223a 205b 2268   "webpages": ["h
-0002ad60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0002ad70: 6d2f 7361 657a 6c61 622f 436f 6c6c 6563  m/saezlab/Collec
-0002ad80: 5452 4922 5d0a 2020 2020 7d0a 2020 7d2c  TRI"].    }.  },
-0002ad90: 0a20 2022 4578 5452 4922 3a20 7b0a 2020  .  "ExTRI": {.  
-0002ada0: 2020 226c 6963 656e 7365 223a 2022 4343    "license": "CC
-0002adb0: 2042 5920 342e 3022 0a20 207d 2c0a 2020   BY 4.0".  },.  
-0002adc0: 2247 4f41 223a 207b 0a20 2020 2022 6c69  "GOA": {.    "li
-0002add0: 6365 6e73 6522 3a20 2243 4320 4259 2034  cense": "CC BY 4
-0002ade0: 2e30 220a 2020 207d 2c0a 2020 2243 7974  .0".   },.  "Cyt
-0002adf0: 5265 6722 3a20 7b0a 2020 2020 226c 6963  Reg": {.    "lic
-0002ae00: 656e 7365 223a 2022 4343 2042 5920 342e  ense": "CC BY 4.
-0002ae10: 3022 0a20 207d 2c0a 2020 2247 4552 4544  0".  },.  "GERED
-0002ae20: 4222 3a20 7b0a 2020 2020 226c 6963 656e  B": {.    "licen
-0002ae30: 7365 223a 2022 4163 6164 656d 6963 2066  se": "Academic f
-0002ae40: 7265 6520 6c69 6365 6e73 6522 0a20 207d  ree license".  }
-0002ae50: 2c0a 2020 2250 6176 6c69 6469 7322 3a20  ,.  "Pavlidis": 
-0002ae60: 7b0a 2020 2020 226c 6963 656e 7365 223a  {.    "license":
-0002ae70: 2022 4343 2042 5920 342e 3022 0a20 2020   "CC BY 4.0".   
-0002ae80: 7d2c 0a20 2022 446f 526f 7468 4541 5f41  },.  "DoRothEA_A
-0002ae90: 223a 207b 0a20 2020 2022 6c69 6365 6e73  ": {.    "licens
-0002aea0: 6522 3a20 2243 6f6d 706f 7369 7465 222c  e": "Composite",
-0002aeb0: 0a20 2020 2022 636f 6d70 6f6e 656e 7473  .    "components
-0002aec0: 223a 205b 0a20 2020 2020 2022 5041 5a41  ": [.      "PAZA
-0002aed0: 5222 2c0a 2020 2020 2020 224f 5265 6741  R",.      "ORegA
-0002aee0: 6e6e 6f22 2c0a 2020 2020 2020 2248 5452  nno",.      "HTR
-0002aef0: 4964 6222 2c0a 2020 2020 2020 2253 4947  Idb",.      "SIG
-0002af00: 4e4f 5222 2c0a 2020 2020 2020 2244 6f52  NOR",.      "DoR
-0002af10: 6f74 6845 412d 7265 7669 6577 7322 0a20  othEA-reviews". 
-0002af20: 2020 205d 0a20 207d 2c0a 2020 224e 544e     ].  },.  "NTN
-0002af30: 5563 7572 6174 696f 6e22 3a20 7b0a 2020  Ucuration": {.  
-0002af40: 2020 226c 6963 656e 7365 223a 2022 4343    "license": "CC
-0002af50: 2042 5920 342e 3022 0a20 207d 2c0a 2020   BY 4.0".  },.  
-0002af60: 2252 614d 5022 3a20 7b0a 2020 2020 2266  "RaMP": {.    "f
-0002af70: 756c 6c5f 6e61 6d65 223a 2022 5265 6c61  ull_name": "Rela
-0002af80: 7469 6f6e 616c 2044 6174 6162 6173 6520  tional Database 
-0002af90: 666f 7220 4d65 7461 626f 6c6f 6d69 6320  for Metabolomic 
-0002afa0: 5061 7468 7761 7973 222c 0a20 2020 2022  Pathways",.    "
-0002afb0: 6c69 6365 6e73 6522 3a20 2255 6e73 7065  license": "Unspe
-0002afc0: 6369 6669 6564 204e 432d 5341 222c 0a20  cified NC-SA",. 
-0002afd0: 2020 2022 7572 6c73 223a 207b 0a20 2020     "urls": {.   
-0002afe0: 2020 2022 7765 6270 6167 6573 223a 205b     "webpages": [
-0002aff0: 2268 7474 7073 3a2f 2f72 616d 7064 622e  "https://rampdb.
-0002b000: 6e69 682e 676f 762f 225d 2c0a 2020 2020  nih.gov/"],.    
-0002b010: 2020 2261 7274 6963 6c65 7322 3a20 5b0a    "articles": [.
-0002b020: 2020 2020 2020 2020 2268 7474 7073 3a2f          "https:/
-0002b030: 2f61 6361 6465 6d69 632e 6f75 702e 636f  /academic.oup.co
-0002b040: 6d2f 6269 6f69 6e66 6f72 6d61 7469 6373  m/bioinformatics
-0002b050: 2f61 7274 6963 6c65 2f33 392f 312f 6274  /article/39/1/bt
-0002b060: 6163 3732 362f 3638 3237 3238 3722 2c0a  ac726/6827287",.
-0002b070: 2020 2020 2020 2020 2268 7474 7073 3a2f          "https:/
-0002b080: 2f77 7777 2e6d 6470 692e 636f 6d2f 3232  /www.mdpi.com/22
-0002b090: 3138 2d31 3938 392f 382f 312f 3136 220a  18-1989/8/1/16".
-0002b0a0: 2020 2020 2020 5d0a 2020 2020 7d0a 2020        ].    }.  
-0002b0b0: 7d0a 7d0a                                }.}.
+0002ad30: 6174 696f 6e22 0a20 2020 205d 2c0a 2020  ation".    ],.  
+0002ad40: 2020 2275 726c 7322 3a20 7b0a 2020 2020    "urls": {.    
+0002ad50: 2020 2277 6562 7061 6765 7322 3a20 5b22    "webpages": ["
+0002ad60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0002ad70: 6f6d 2f73 6165 7a6c 6162 2f43 6f6c 6c65  om/saezlab/Colle
+0002ad80: 6354 5249 225d 0a20 2020 207d 0a20 207d  cTRI"].    }.  }
+0002ad90: 2c0a 2020 2245 7854 5249 223a 207b 0a20  ,.  "ExTRI": {. 
+0002ada0: 2020 2022 6c69 6365 6e73 6522 3a20 2243     "license": "C
+0002adb0: 4320 4259 2034 2e30 220a 2020 7d2c 0a20  C BY 4.0".  },. 
+0002adc0: 2022 474f 4122 3a20 7b0a 2020 2020 226c   "GOA": {.    "l
+0002add0: 6963 656e 7365 223a 2022 4343 2042 5920  icense": "CC BY 
+0002ade0: 342e 3022 0a20 2020 7d2c 0a20 2022 4379  4.0".   },.  "Cy
+0002adf0: 7452 6567 223a 207b 0a20 2020 2022 6c69  tReg": {.    "li
+0002ae00: 6365 6e73 6522 3a20 2243 4320 4259 2034  cense": "CC BY 4
+0002ae10: 2e30 220a 2020 7d2c 0a20 2022 4745 5245  .0".  },.  "GERE
+0002ae20: 4442 223a 207b 0a20 2020 2022 6c69 6365  DB": {.    "lice
+0002ae30: 6e73 6522 3a20 2241 464c 2033 2e30 220a  nse": "AFL 3.0".
+0002ae40: 2020 7d2c 0a20 2022 5061 766c 6964 6973    },.  "Pavlidis
+0002ae50: 223a 207b 0a20 2020 2022 7379 6e6f 6e79  ": {.    "synony
+0002ae60: 6d73 223a 205b 2250 6176 6c69 6469 7332  ms": ["Pavlidis2
+0002ae70: 3032 3122 5d2c 0a20 2020 2022 6c69 6365  021"],.    "lice
+0002ae80: 6e73 6522 3a20 2243 4320 4259 2034 2e30  nse": "CC BY 4.0
+0002ae90: 220a 2020 207d 2c0a 2020 2244 6f52 6f74  ".   },.  "DoRot
+0002aea0: 6845 412d 4122 3a20 7b0a 2020 2020 226c  hEA-A": {.    "l
+0002aeb0: 6963 656e 7365 223a 2022 436f 6d70 6f73  icense": "Compos
+0002aec0: 6974 6522 2c0a 2020 2020 2263 6f6d 706f  ite",.    "compo
+0002aed0: 6e65 6e74 7322 3a20 5b0a 2020 2020 2020  nents": [.      
+0002aee0: 2250 415a 4152 222c 0a20 2020 2020 2022  "PAZAR",.      "
+0002aef0: 4f52 6567 416e 6e6f 222c 0a20 2020 2020  ORegAnno",.     
+0002af00: 2022 4854 5249 6462 222c 0a20 2020 2020   "HTRIdb",.     
+0002af10: 2022 5349 474e 4f52 222c 0a20 2020 2020   "SIGNOR",.     
+0002af20: 2022 446f 526f 7468 4541 2d72 6576 6965   "DoRothEA-revie
+0002af30: 7773 220a 2020 2020 5d0a 2020 7d2c 0a20  ws".    ].  },. 
+0002af40: 2022 4e54 4e55 6375 7261 7469 6f6e 223a   "NTNUcuration":
+0002af50: 207b 0a20 2020 2022 7379 6e6f 6e79 6d73   {.    "synonyms
+0002af60: 223a 205b 224e 544e 552e 4375 7261 7465  ": ["NTNU.Curate
+0002af70: 6422 5d2c 0a20 2020 2022 6c69 6365 6e73  d"],.    "licens
+0002af80: 6522 3a20 2243 4320 4259 2034 2e30 220a  e": "CC BY 4.0".
+0002af90: 2020 7d2c 0a20 2022 5261 4d50 223a 207b    },.  "RaMP": {
+0002afa0: 0a20 2020 2022 6675 6c6c 5f6e 616d 6522  .    "full_name"
+0002afb0: 3a20 2252 656c 6174 696f 6e61 6c20 4461  : "Relational Da
+0002afc0: 7461 6261 7365 2066 6f72 204d 6574 6162  tabase for Metab
+0002afd0: 6f6c 6f6d 6963 2050 6174 6877 6179 7322  olomic Pathways"
+0002afe0: 2c0a 2020 2020 226c 6963 656e 7365 223a  ,.    "license":
+0002aff0: 2022 556e 7370 6563 6966 6965 6420 4e43   "Unspecified NC
+0002b000: 2d53 4122 2c0a 2020 2020 2275 726c 7322  -SA",.    "urls"
+0002b010: 3a20 7b0a 2020 2020 2020 2277 6562 7061  : {.      "webpa
+0002b020: 6765 7322 3a20 5b22 6874 7470 733a 2f2f  ges": ["https://
+0002b030: 7261 6d70 6462 2e6e 6968 2e67 6f76 2f22  rampdb.nih.gov/"
+0002b040: 5d2c 0a20 2020 2020 2022 6172 7469 636c  ],.      "articl
+0002b050: 6573 223a 205b 0a20 2020 2020 2020 2022  es": [.        "
+0002b060: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
+0002b070: 2e6f 7570 2e63 6f6d 2f62 696f 696e 666f  .oup.com/bioinfo
+0002b080: 726d 6174 6963 732f 6172 7469 636c 652f  rmatics/article/
+0002b090: 3339 2f31 2f62 7461 6337 3236 2f36 3832  39/1/btac726/682
+0002b0a0: 3732 3837 222c 0a20 2020 2020 2020 2022  7287",.        "
+0002b0b0: 6874 7470 733a 2f2f 7777 772e 6d64 7069  https://www.mdpi
+0002b0c0: 2e63 6f6d 2f32 3231 382d 3139 3839 2f38  .com/2218-1989/8
+0002b0d0: 2f31 2f31 3622 0a20 2020 2020 205d 0a20  /1/16".      ]. 
+0002b0e0: 2020 207d 0a20 207d 2c0a 2020 224c 616d     }.  },.  "Lam
+0002b0f0: 6265 7274 3230 3138 223a 207b 0a20 2020  bert2018": {.   
+0002b100: 2022 6c69 6365 6e73 6522 3a20 2245 554c   "license": "EUL
+0002b110: 220a 2020 7d0a 7d0a                      ".  }.}.
```

### Comparing `pypath_omnipath-0.14.44/pypath/resources/data_formats.py` & `pypath_omnipath-0.14.48/pypath/resources/data_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -3068,16 +3068,28 @@
                 if common.is_str(line[1]) and line[1][:5] == 'CHEBI' else
             'uniprot'
         ),
         positive_filters = [
             (10, True), # only direct interactions
             lambda line: line[4] == 'chemical' or line[5] == 'chemical',
         ],
-        entity_type_a = (4, {'chemical': 'small_molecule'}),
-        entity_type_b = (5, {'chemical': 'small_molecule'}),
+        entity_type_a = (
+            4,
+            {
+                'chemical': 'small_molecule',
+                'smallmolecule': 'small_molecule',
+            }
+        ),
+        entity_type_b = (
+            5,
+            {
+                'chemical': 'small_molecule',
+                'smallmolecule': 'small_molecule',
+            }
+        ),
         is_directed = (
             6,
             [
                 'up-regulates',
                 'up-regulates activity',
                 'up-regulates quantity by stabilization',
                 'down-regulates',
```

### Comparing `pypath_omnipath-0.14.44/pypath/resources/descriptions.py` & `pypath_omnipath-0.14.48/pypath/resources/descriptions.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/resources/licenses.py` & `pypath_omnipath-0.14.48/pypath/resources/licenses.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/resources/network.py` & `pypath_omnipath-0.14.48/pypath/resources/network.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/resources/urls.py` & `pypath_omnipath-0.14.48/pypath/resources/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1005,15 +1005,16 @@
             'allNcRNACelldeathData.txt',
         'url_rescued': 'https://rescued.omnipathdb.org/'
             'ncRDeathDB_allNcRNACelldeathData.txt',
     },
     'mirecords': {
         'label': 'miRecords experimentally validated'\
             'miRNA-target interactions',
-        'url': 'http://c1.accurascience.com/miRecords/download_data.php?v=4'
+        'url': 'http://c1.accurascience.com/miRecords/download_data.php?v=4',
+        'url_rescued': 'http://rescued.omnipathdb.org/miRecords_v4.xls',
     },
     'mirtarbase': {
         'label': 'miRTarBase experimentally validated'\
             'miRNA-target interactions',
         'strong_old': 'http://mirtarbase.mbc.nctu.edu.tw/cache/download/'\
             '6.1/miRTarBase_SE_WR.xls',
         'strong': 'https://mirtarbase.cuhk.edu.cn/~miRTarBase/'\
```

### Comparing `pypath_omnipath-0.14.44/pypath/share/cache.py` & `pypath_omnipath-0.14.48/pypath/share/cache.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/common.py` & `pypath_omnipath-0.14.48/pypath/share/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 #  Distributed under the GPLv3 License.
 #  See accompanying file LICENSE.txt or copy at
 #      http://www.gnu.org/licenses/gpl-3.0.html
 #
 #  Website: http://pypath.omnipathdb.org/
 #
 
+from __future__ import annotations
+
 #TODO requires cleaning, check what functions are not used and may be removed.
 #Some parts can go to jsons.
 
 from future.utils import iteritems
 from past.builtins import xrange, range, reduce
 
 from typing import (
```

### Comparing `pypath_omnipath-0.14.44/pypath/share/constants.py` & `pypath_omnipath-0.14.48/pypath/share/constants.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/curl.py` & `pypath_omnipath-0.14.48/pypath/share/curl.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/log.py` & `pypath_omnipath-0.14.48/pypath/share/log.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/lookup/_manytomany.py` & `pypath_omnipath-0.14.48/pypath/share/lookup/_manytomany.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/lookup/_onetomany.py` & `pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/lookup/_onetomany2.py` & `pypath_omnipath-0.14.48/pypath/share/lookup/_onetomany2.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/progress.py` & `pypath_omnipath-0.14.48/pypath/share/progress.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/session.py` & `pypath_omnipath-0.14.48/pypath/share/session.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/share/settings.py` & `pypath_omnipath-0.14.48/pypath/share/settings.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/go.py` & `pypath_omnipath-0.14.48/pypath/utils/go.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/homology.py` & `pypath_omnipath-0.14.48/pypath/utils/homology.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/mapping.py` & `pypath_omnipath-0.14.48/pypath/utils/mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,14 +734,15 @@
 
                     c = curl.Curl(
                         url,
                         post = post,
                         large = True,
                         silent = False,
                         cache = False,
+                        slow = True,
                     )
 
                     if c.result is not None:
 
                         break
 
             if c.result is None or c.fileobj.read(5) == '<!DOC':
```

### Comparing `pypath_omnipath-0.14.44/pypath/utils/pdb.py` & `pypath_omnipath-0.14.48/pypath/utils/pdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/proteomicsdb.py` & `pypath_omnipath-0.14.48/pypath/utils/proteomicsdb.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/pyreact.py` & `pypath_omnipath-0.14.48/pypath/utils/pyreact.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/reflists.py` & `pypath_omnipath-0.14.48/pypath/utils/reflists.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/residues.py` & `pypath_omnipath-0.14.48/pypath/utils/residues.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/seq.py` & `pypath_omnipath-0.14.48/pypath/utils/seq.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/taxonomy.py` & `pypath_omnipath-0.14.48/pypath/utils/taxonomy.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/unichem.py` & `pypath_omnipath-0.14.48/pypath/utils/unichem.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/utils/uniprot.py` & `pypath_omnipath-0.14.48/pypath/utils/uniprot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/visual/drawing.py` & `pypath_omnipath-0.14.48/pypath/visual/drawing.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/visual/igraph_drawing/__init__.py` & `pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/__init__.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/visual/igraph_drawing/edge.py` & `pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/edge.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/visual/igraph_drawing/vertex.py` & `pypath_omnipath-0.14.48/pypath/visual/igraph_drawing/vertex.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pypath/visual/plot.py` & `pypath_omnipath-0.14.48/pypath/visual/plot.py`

 * *Files identical despite different names*

### Comparing `pypath_omnipath-0.14.44/pyproject.toml` & `pypath_omnipath-0.14.48/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pypath-omnipath"
-version = "0.14.44"
+version = "0.14.48"
 description = "Molecular signaling prior knowledge processing"
 license = "GPL-3.0-only"
 authors = [
     "Denes Turei <turei.denes@gmail.com>",
     "Nicolàs Palacio",
     "Sebastian Lobentanzer",
     "Olga Ivanova",
@@ -56,14 +56,15 @@
 future = "*"
 glom = "*"
 lxml = "*"
 matplotlib = "*"
 numpy = "*"
 openpyxl = "*"
 pandas = "*"
+psutil = "*"
 pycurl = "*"
 pyreadr = "*"
 PyYAML = "*"
 rdata = "*"
 requests = "*"
 scipy = "*"
 sqlparse = "*"
```

### Comparing `pypath_omnipath-0.14.44/setup.py` & `pypath_omnipath-0.14.48/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
  'future',
  'glom',
  'lxml',
  'matplotlib',
  'numpy',
  'openpyxl',
  'pandas',
+ 'psutil',
  'pycurl',
  'pyreadr',
  'pysftp>=0.2.9,<0.3.0',
  'rdata',
  'requests',
  'scipy',
  'sqlparse',
@@ -55,17 +56,17 @@
 
 entry_points = \
 {'bio2bel': ['omnipath = pypath.omnipath.bel'],
  'console_scripts': ['bio2bel_omnipath = pypath.omnipath.bel:main']}
 
 setup_kwargs = {
     'name': 'pypath-omnipath',
-    'version': '0.14.44',
+    'version': '0.14.48',
     'description': 'Molecular signaling prior knowledge processing',
-    'long_description': "============================================================================\n*pypath:* A Python module for molecular signaling prior knowledge processing\n============================================================================\n\n|Demo|\n\nOmniPath\n========\n\nAre you interested in OmniPath data? Check out our R package OmnipathR_,\nthe most popular and most versatile access point to OmniPath, a database\nbuilt from more than 150 original resources. If you use Python and don't\nneed to build the database yourself, try our `Python client`_. Read more\nabout the `web service here`_.\n\n.. _OmnipathR: https://r.omnipathdb.org\n.. _`Python client`: https://github.com/saezlab/omnipath\n.. _`web service here`: https://pypath.omnipathdb.org/webservice.html\n\nDo you need pypath?\n===================\n\nPypath is the database builder of OmniPath. For most people the data\ndistributed in OmniPath is satisfying (see above), they don't really need\npypath. Typically you need pypath to:\n\n* Build a custom or very fresh version of the OmniPath database(s)\n* Use one of the utilities such as ID translation, homology translation, etc.\n  (see the `utils module`_)\n* Access the raw or preprocessed data directly from the original resources\n  (see the `inputs module`_)\n\n.. _`utils module`: https://github.com/saezlab/pypath/tree/master/pypath/utils\n.. _`inputs module`: https://github.com/saezlab/pypath/tree/master/pypath/inputs\n\nInstallation\n============\n\n**From PyPI:**\n\n.. code:: bash\n\n    pip install pypath-omnipath\n\n**From Git:**\n\n.. code:: bash\n\n    pip install git+https://github.com/saezlab/pypath.git\n\nDocs\n====\n\nRead the `reference documentation`_ or check out the tutorials_. The most\ncomprehensive guide to *pypath* is `The Pypath Book`_.\n\n.. _`reference documentation`: https://pypath.omnipathdb.org/\n.. _tutorials: https://workflows.omnipathdb.org/\n.. _`The Pypath Book`: https://pypath.omnipathdb.org/notebooks/manual.html\n\nGet help\n========\n\nShould you have a question or experiencing an issue, please write us by\nthe `Github issues`_ page.\n\nFeatures\n========\n\n**pypath** is a Python module for processing molecular biology data resources,\ncombining them into databases and providing a versatile interface in Python\nas well as exporting the data for access through other platforms such as\nR_, `web service`_, Cytoscape_ and BEL (Biological Expression Language).\n\n.. _R: https://r.omnipathdb.org/\n.. _`web service`: https://omnipathdb.org/\n.. _Cytoscape: https://apps.cytoscape.org/apps/omnipath\n\n**pypath** provides access to more than 100 resources! It builds 5 major\ncombined databases and within these we can distinguish different datasets.\nThe 5 major databases are interactions (molecular interaction network or\npathways), enzyme-substrate relationships, protein complexes, molecular\nannotations (functional roles, localizations, and more) and inter-cellular\ncommunication roles.\n\n**pypath** consists of a number of submodules and each of them again contains\na number of submodules. Overall **pypath** consists of around 100 modules.\nThe most important higher level submodules:\n\n* *pypath.core:* contains the database classes e.g. network, complex,\n  annotations, etc\n* *pypath.inputs:* contains the resource specific methods which directly\n  downlad and preprocess data from the original sources\n* *pypath.omnipath:* higher level applications, e.g. a database manager, a\n  web server\n* *pypath.utils:* stand alone useful utilities, e.g. identifier translator,\n  Gene Ontology processor, BioPax processor, etc\n\nIntegrated databases\n--------------------\n\nIn the beginning the primary aim of ``pypath`` was to build networks from\nmultiple sources using an igraph object as the fundament of the integrated\ndata structure. From version 0.7 and 0.8 this design principle started to\nchange. Today ``pypath`` builds a number of different databases, exposes them\nby a rich API and each of them can be converted to ``pandas.DataFrame``.\nThe modules and classes responsible for the integrated databases are located\nin ``pypath.core``. The five main databases are the followings:\n\n* *network* - ``core.network``\n* *enzyme-substrate* - ``core.enz_sub``\n* *complexes* - ``core.complex``\n* *annotations* - ``core.annot``\n* *intercell* - ``core.intercell``\n\nSome of the databases have different variants (e.g. PPI and transcriptional\nnetwork) and all can be customized by many parameters.\n\nDatabase management\n-------------------\n\nThe databases above can be loaded by calling the appropriate classes.\nHowever building the databases require time and memory so we want to avoid\nbuilding them more often than necessary or keeping more than one copies\nin the memory. Some of the modules listed above have a method ``get_db``\nwhich ensures only one instance of the database is loaded. But there is a\nmore full featured database management system available in **pypath**,\nthis is the **pypath.omnipath** module. This module is able to build the\ndatabases, automatically saves them to ``pickle`` files and loads them from\nthere in subsequent sessions. **pypath** comes with a number of database\ndefinitions and users can add more. The ``pickle`` files are located by\ndefault in the ``~/.pypath/pickles/`` directory. With the ``omnipath``\nmodule it's easy to get an instance of a database. For example to get the\n`omnipath` PPI network dataset:\n\n.. code:: python\n\n    from pypath import omnipath\n    op = omnipath.db.get_db('omnipath')\n\n**Important:** Building the databases for the first time requires the\ndownload of several MB or GB of data from the original resources. This\nnormally takes long time and is prone of errors (e.g. truncated or empty\ndownloads due to interrupted HTTP connection). In this case you should check\nthe log to find the path of the problematic cache file, check the contents\nof this file to find out the reason and possibly delete the file to ensure\nanother download attempt when you call the database build again. Sometimes\nthe original resources change their content or go offline. If you encounter\nsuch case please open an issue at https://github.com/saezlab/pypath/issues\nso we can fix it in ``pypath``. Once all the necessary contents are\ndownloaded and stored in the cache, the database builds are much faster,\nbut still can take minutes.\n\nFurther modules in pypath\n-------------------------\n\nApart from the databases, **pypath** has many submodules with standalone\nfunctionality which can be used in other modules and scripts. Below we\npresent a few of these.\n\nID conversion\n-------------\n\nThe ID conversion module ``utils.mapping`` translates between a large variety\nof gene, protein, miRNA and small molecule ID types. It has the feature to\ntranslate secondary UniProt ACs to primaries, and Trembl ACs to SwissProt,\nusing primary Gene Symbols to find the connections. This module automatically\nloads and stores the necessary conversion tables. Many tables\nare predefined, such as all the IDs in **UniProt mapping service,** while\nusers are able to load any table from **file** using the classes provided\nin the module ``input_formats``. An example how to translate identifiers:\n\n.. code:: python\n\n    from pypath.utils import mapping\n    mapping.map_name('P00533', 'uniprot', 'genesymbol')\n    # {'EGFR'}\n\n\nHomology translation\n--------------------\n\nThe ``pypath.utils.homology`` module is able to find the orthologs of genes\nbetween two organisms. It uses data both from NCBI HomoloGene, Ensembl and\nUniProt. This module is really simple to use:\n\n.. code:: python\n\n    from pypath.utils import homology\n    homology.translate('P00533', 10090) # translating the human EGFR to mouse\n    # ['Q01279'] # it returns the mouse Egfr UniProt AC\n\nIt is able to handle any ID type supported by ``pypath.utils.mapping``.\nAlternatively, you can access a complete dictionary of orthologous genes,\nor translate columns in a pandas data frame.\n\nFAQ\n===\n\n**Does it run on my old Python?**\n\nMost likely it doesn't. The oldest supported version, currently 3.9, is\ndefined in our `pyproject.toml`_.\n\n.. _`pyproject.toml`: https://github.com/saezlab/pypath/blob/master/pyproject.toml\n\n**Is there something similar in R?**\n\n`OmniPath's R client`_, besides accessing data from OmniPath, provides many\nsimilar services as pypath: `ID translation`_, `homology translation`_,\n`taxonomy support`_, `GO support`_, and many more.\n\n.. _`OmniPath's R client`: https://r.omnipathdb.org\n.. _`ID translation`: https://r.omnipathdb.org/reference/translate_ids.html\n.. _`homology translation`: https://r.omnipathdb.org/reference/homologene_uniprot_orthology.html\n.. _`taxonomy support`: https://r.omnipathdb.org/reference/ncbi_taxid.html\n.. _`GO support`: https://r.omnipathdb.org/reference/go_annot_download.html\n\n`Questions about OmniPath`_\n\n.. _`Questions about OmniPath`: https://omnipathdb.org/#faq\n\nContact\n=======\n\nWe prefer to keep all communication within the `Github issues`_. About private\nor sensitive matters feel free to contact us by omnipathdb@gmail.com.\n\n.. _`Github issues`: https://github.com/saezlab/pypath/issues\n\nImpressum\n=========\n\nThe development of ``pypath`` is coordinated by `Dénes Türei`_ in the\n`Saez Lab`_, with the contribution of developers and scientists from\nother groups:\n\n* Erva Ulusoy, Melih Darcan, Ömer Kaan Vural, Tennur Kılıç, Elif Çevrim,\n  Bünyamin Şen and Atabey Ünlü in the\n  `HU Biological Data Science Lab (PI: Tunca Doğan)`_ created many new input\n  in `pypath`;\n* Leila Gul, Dezső Módos, Márton Ölbei and Tamás Korcsmáros in the\n  `Korcsmaros Lab`_ contributed to the overall design of OmniPath, the\n  design and implementation of the intercellular communication database,\n  and with various case studies and tutorials;\n* Michael Klein from the group of `Fabian Theis`_ developed the\n  `Python client`_ for the OmniPath web service;\n* Charles Tapley Hoyt and Daniel Domingo-Fernández added the BEL export\n  module.\n* From the `Saez Lab`_, Olga Ivanova introduced the resource manager in\n  `pypath`, Sophia Müller-Dott added the CollecTRI gene regulatory network,\n  while Nicolàs Palacio, Sebastian Lobentanzer and Ahmet Rifaioglu\n  have done various maintenance and refactoring works. Aurelien Dugourd and\n  Christina Schmidt helped with the design of the metabolomics related\n  datasets and services.\n* The `R package`_ and the `Cytoscape app`_ are developed and maintained by\n  Francesco Ceccarelli, Attila Gábor, Alberto Valdeolivas, Dénes Türei and\n  Nicolàs Palacio;\n* The first logo of OmniPath has been designed by Jakob Wirbel (Saez Lab),\n  the current logo by Dénes Türei, while the cover graphics for Nature Methods\n  is the work of Spencer Phillips from EMBL-EBI.\n\n.. _`Saez Lab`: https://saezlab.org/\n.. _`HU Biological Data Science Lab (PI: Tunca Doğan)`: https://yunus.hacettepe.edu.tr/~tuncadogan/\n.. _`Dénes Türei`: https://denes.omnipathdb.org/\n.. _`R package`: https://r.omnipathdb.org\n.. _`Cytoscape app`: https://apps.cytoscape.org/apps/omnipath\n.. _`Fabian Theis`: https://www.helmholtz-munich.de/en/icb/research-groups/theis-lab/\n.. _`Korcsmaros Lab`: https://korcsmaroslab.org/\n\nHistory and releases\n====================\n\nSee here_ a bird eye view of pypath's development history. For more details\nabout recent developments see the `Github releases`_.\n\n.. _here: https://pypath.omnipathdb.org/releasehistory.html\n.. _`Github releases`: https://github.com/saezlab/pypath/releases\n\n.. |Demo| image:: https://raw.githubusercontent.com/saezlab/pypath/master/docs/source/_static/img/pypath-demo.webp\n",
+    'long_description': "============================================================================\n*pypath:* A Python module for molecular signaling prior knowledge processing\n============================================================================\n\n|Demo|\n\nOmniPath\n========\n\nAre you interested in OmniPath data? Check out our R package OmnipathR_,\nthe most popular and most versatile access point to OmniPath, a database\nbuilt from more than 150 original resources. If you use Python and don't\nneed to build the database yourself, try our `Python client`_. Read more\nabout the `web service here`_.\n\n.. _OmnipathR: https://r.omnipathdb.org\n.. _`Python client`: https://github.com/saezlab/omnipath\n.. _`web service here`: https://pypath.omnipathdb.org/webservice.html\n\nDo you need pypath?\n===================\n\nPypath is the database builder of OmniPath. For most people the data\ndistributed in OmniPath is satisfying (see above), they don't really need\npypath. Typically you need pypath to:\n\n* Build a custom or very fresh version of the OmniPath database(s)\n* Use one of the utilities such as ID translation, homology translation, etc.\n  (see the `utils module`_)\n* Access the raw or preprocessed data directly from the original resources\n  (see the `inputs module`_)\n\n.. _`utils module`: https://github.com/saezlab/pypath/tree/master/pypath/utils\n.. _`inputs module`: https://github.com/saezlab/pypath/tree/master/pypath/inputs\n\nInstallation\n============\n\n**From PyPI:**\n\n.. code:: bash\n\n    pip install pypath-omnipath\n\n**From Git:**\n\n.. code:: bash\n\n    pip install git+https://github.com/saezlab/pypath.git\n\nDocs\n====\n\nRead the `reference documentation`_ or check out the tutorials_. The most\ncomprehensive guide to *pypath* is `The Pypath Book`_.\n\n.. _`reference documentation`: https://pypath.omnipathdb.org/\n.. _tutorials: https://workflows.omnipathdb.org/\n.. _`The Pypath Book`: https://pypath.omnipathdb.org/notebooks/manual.html\n\nGet help\n========\n\nShould you have a question or experiencing an issue, please write us by\nthe `Github issues`_ page.\n\nFeatures\n========\n\n**pypath** is a Python module for processing molecular biology data resources,\ncombining them into databases and providing a versatile interface in Python\nas well as exporting the data for access through other platforms such as\nR_, `web service`_, Cytoscape_ and BEL (Biological Expression Language).\n\n.. _R: https://r.omnipathdb.org/\n.. _`web service`: https://omnipathdb.org/\n.. _Cytoscape: https://apps.cytoscape.org/apps/omnipath\n\n**pypath** provides access to more than 100 resources! It builds 5 major\ncombined databases and within these we can distinguish different datasets.\nThe 5 major databases are interactions (molecular interaction network or\npathways), enzyme-substrate relationships, protein complexes, molecular\nannotations (functional roles, localizations, and more) and inter-cellular\ncommunication roles.\n\n**pypath** consists of a number of submodules and each of them again contains\na number of submodules. Overall **pypath** consists of around 100 modules.\nThe most important higher level submodules:\n\n* *pypath.core:* contains the database classes e.g. network, complex,\n  annotations, etc\n* *pypath.inputs:* contains the resource specific methods which directly\n  downlad and preprocess data from the original sources\n* *pypath.omnipath:* higher level applications, e.g. a database manager, a\n  web server\n* *pypath.utils:* stand alone useful utilities, e.g. identifier translator,\n  Gene Ontology processor, BioPax processor, etc\n\nIntegrated databases\n--------------------\n\nIn the beginning the primary aim of ``pypath`` was to build networks from\nmultiple sources using an igraph object as the fundament of the integrated\ndata structure. From version 0.7 and 0.8 this design principle started to\nchange. Today ``pypath`` builds a number of different databases, exposes them\nby a rich API and each of them can be converted to ``pandas.DataFrame``.\nThe modules and classes responsible for the integrated databases are located\nin ``pypath.core``. The five main databases are the followings:\n\n* *network* - ``core.network``\n* *enzyme-substrate* - ``core.enz_sub``\n* *complexes* - ``core.complex``\n* *annotations* - ``core.annot``\n* *intercell* - ``core.intercell``\n\nSome of the databases have different variants (e.g. PPI and transcriptional\nnetwork) and all can be customized by many parameters.\n\nDatabase management\n-------------------\n\nThe databases above can be loaded by calling the appropriate classes.\nHowever building the databases require time and memory so we want to avoid\nbuilding them more often than necessary or keeping more than one copies\nin the memory. Some of the modules listed above have a method ``get_db``\nwhich ensures only one instance of the database is loaded. But there is a\nmore full featured database management system available in **pypath**,\nthis is the **pypath.omnipath** module. This module is able to build the\ndatabases, automatically saves them to ``pickle`` files and loads them from\nthere in subsequent sessions. **pypath** comes with a number of database\ndefinitions and users can add more. The ``pickle`` files are located by\ndefault in the ``~/.pypath/pickles/`` directory. With the ``omnipath``\nmodule it's easy to get an instance of a database. For example to get the\n`omnipath` PPI network dataset:\n\n.. code:: python\n\n    from pypath import omnipath\n    op = omnipath.db.get_db('omnipath')\n\n**Important:** Building the databases for the first time requires the\ndownload of several MB or GB of data from the original resources. This\nnormally takes long time and is prone of errors (e.g. truncated or empty\ndownloads due to interrupted HTTP connection). In this case you should check\nthe log to find the path of the problematic cache file, check the contents\nof this file to find out the reason and possibly delete the file to ensure\nanother download attempt when you call the database build again. Sometimes\nthe original resources change their content or go offline. If you encounter\nsuch case please open an issue at https://github.com/saezlab/pypath/issues\nso we can fix it in ``pypath``. Once all the necessary contents are\ndownloaded and stored in the cache, the database builds are much faster,\nbut still can take minutes.\n\nFurther modules in pypath\n-------------------------\n\nApart from the databases, **pypath** has many submodules with standalone\nfunctionality which can be used in other modules and scripts. Below we\npresent a few of these.\n\nID conversion\n-------------\n\nThe ID conversion module ``utils.mapping`` translates between a large variety\nof gene, protein, miRNA and small molecule ID types. It has the feature to\ntranslate secondary UniProt ACs to primaries, and Trembl ACs to SwissProt,\nusing primary Gene Symbols to find the connections. This module automatically\nloads and stores the necessary conversion tables. Many tables\nare predefined, such as all the IDs in **UniProt mapping service,** while\nusers are able to load any table from **file** using the classes provided\nin the module ``input_formats``. An example how to translate identifiers:\n\n.. code:: python\n\n    from pypath.utils import mapping\n    mapping.map_name('P00533', 'uniprot', 'genesymbol')\n    # {'EGFR'}\n\n\nHomology translation\n--------------------\n\nThe ``pypath.utils.homology`` module is able to find the orthologs of genes\nbetween two organisms. It uses data both from NCBI HomoloGene, Ensembl and\nUniProt. This module is really simple to use:\n\n.. code:: python\n\n    from pypath.utils import homology\n    homology.translate('P00533', 10090) # translating the human EGFR to mouse\n    # ['Q01279'] # it returns the mouse Egfr UniProt AC\n\nIt is able to handle any ID type supported by ``pypath.utils.mapping``.\nAlternatively, you can access a complete dictionary of orthologous genes,\nor translate columns in a pandas data frame.\n\nFAQ\n===\n\n**Does it run on my old Python?**\n\nMost likely it doesn't. The oldest supported version, currently 3.9, is\ndefined in our `pyproject.toml`_.\n\n.. _`pyproject.toml`: https://github.com/saezlab/pypath/blob/master/pyproject.toml\n\n**Is there something similar in R?**\n\n`OmniPath's R client`_, besides accessing data from OmniPath, provides many\nsimilar services as pypath: `ID translation`_, `homology translation`_,\n`taxonomy support`_, `GO support`_, and many more.\n\n.. _`OmniPath's R client`: https://r.omnipathdb.org\n.. _`ID translation`: https://r.omnipathdb.org/reference/translate_ids.html\n.. _`homology translation`: https://r.omnipathdb.org/reference/homologene_uniprot_orthology.html\n.. _`taxonomy support`: https://r.omnipathdb.org/reference/ncbi_taxid.html\n.. _`GO support`: https://r.omnipathdb.org/reference/go_annot_download.html\n\n`Questions about OmniPath`_\n\n.. _`Questions about OmniPath`: https://omnipathdb.org/#faq\n\nContact\n=======\n\nWe prefer to keep all communication within the `Github issues`_. About private\nor sensitive matters feel free to contact us by omnipathdb@gmail.com.\n\n.. _`Github issues`: https://github.com/saezlab/pypath/issues\n\nImpressum\n=========\n\nThe development of ``pypath`` is coordinated by `Dénes Türei`_ in the\n`Saez Lab`_, with the contribution of developers and scientists from\nother groups:\n\n* Erva Ulusoy, Melih Darcan, Ömer Kaan Vural, Tennur Kılıç, Elif Çevrim,\n  Bünyamin Şen and Atabey Ünlü in the\n  `HU Biological Data Science Lab (PI: Tunca Doğan)`_ created many new input\n  modules in `pypath`;\n* Leila Gul, Dezső Módos, Márton Ölbei and Tamás Korcsmáros in the\n  `Korcsmaros Lab`_ contributed to the overall design of OmniPath, the\n  design and implementation of the intercellular communication database,\n  and with various case studies and tutorials;\n* Michael Klein from the group of `Fabian Theis`_ developed the\n  `Python client`_ for the OmniPath web service;\n* Charles Tapley Hoyt and Daniel Domingo-Fernández added the BEL export\n  module.\n* From the `Saez Lab`_, Olga Ivanova introduced the resource manager in\n  `pypath`, Sophia Müller-Dott added the CollecTRI gene regulatory network,\n  while Nicolàs Palacio, Sebastian Lobentanzer and Ahmet Rifaioglu\n  have done various maintenance and refactoring works. Aurelien Dugourd and\n  Christina Schmidt helped with the design of the metabolomics related\n  datasets and services.\n* The `R package`_ and the `Cytoscape app`_ are developed and maintained by\n  Francesco Ceccarelli, Attila Gábor, Alberto Valdeolivas, Dénes Türei and\n  Nicolàs Palacio;\n* The first logo of OmniPath has been designed by Jakob Wirbel (Saez Lab),\n  the current logo by Dénes Türei, while the cover graphics for Nature Methods\n  is the work of Spencer Phillips from EMBL-EBI.\n\n.. _`Saez Lab`: https://saezlab.org/\n.. _`HU Biological Data Science Lab (PI: Tunca Doğan)`: https://yunus.hacettepe.edu.tr/~tuncadogan/\n.. _`Dénes Türei`: https://denes.omnipathdb.org/\n.. _`R package`: https://r.omnipathdb.org\n.. _`Cytoscape app`: https://apps.cytoscape.org/apps/omnipath\n.. _`Fabian Theis`: https://www.helmholtz-munich.de/en/icb/research-groups/theis-lab/\n.. _`Korcsmaros Lab`: https://korcsmaroslab.org/\n\nHistory and releases\n====================\n\nSee here_ a bird eye view of pypath's development history. For more details\nabout recent developments see the `Github releases`_.\n\n.. _here: https://pypath.omnipathdb.org/releasehistory.html\n.. _`Github releases`: https://github.com/saezlab/pypath/releases\n\n.. |Demo| image:: https://raw.githubusercontent.com/saezlab/pypath/master/docs/source/_static/img/pypath-demo.webp\n",
     'author': 'Denes Turei',
     'author_email': 'turei.denes@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://omnipathdb.org/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pypath_omnipath-0.14.44/PKG-INFO` & `pypath_omnipath-0.14.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypath-omnipath
-Version: 0.14.44
+Version: 0.14.48
 Summary: Molecular signaling prior knowledge processing
 Home-page: https://omnipathdb.org/
 License: GPL-3.0-only
 Keywords: systems biology,molecular biology,omics,network,signaling
 Author: Denes Turei
 Author-email: turei.denes@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -34,14 +34,15 @@
 Requires-Dist: future
 Requires-Dist: glom
 Requires-Dist: lxml
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
+Requires-Dist: psutil
 Requires-Dist: pybel; extra == "bel"
 Requires-Dist: pycurl
 Requires-Dist: pyreadr
 Requires-Dist: pysftp (>=0.2.9,<0.3.0)
 Requires-Dist: python-igraph; extra == "graph"
 Requires-Dist: rdata
 Requires-Dist: requests
@@ -293,15 +294,15 @@
 The development of ``pypath`` is coordinated by `Dénes Türei`_ in the
 `Saez Lab`_, with the contribution of developers and scientists from
 other groups:
 
 * Erva Ulusoy, Melih Darcan, Ömer Kaan Vural, Tennur Kılıç, Elif Çevrim,
   Bünyamin Şen and Atabey Ünlü in the
   `HU Biological Data Science Lab (PI: Tunca Doğan)`_ created many new input
-  in `pypath`;
+  modules in `pypath`;
 * Leila Gul, Dezső Módos, Márton Ölbei and Tamás Korcsmáros in the
   `Korcsmaros Lab`_ contributed to the overall design of OmniPath, the
   design and implementation of the intercellular communication database,
   and with various case studies and tutorials;
 * Michael Klein from the group of `Fabian Theis`_ developed the
   `Python client`_ for the OmniPath web service;
 * Charles Tapley Hoyt and Daniel Domingo-Fernández added the BEL export
```

