# Comparing `tmp/peptides-0.3.1.tar.gz` & `tmp/peptides-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptides-0.3.1.tar", last modified: Thu Sep  1 15:53:31 2022, max compression
+gzip compressed data, was "peptides-0.3.2.tar", last modified: Wed Apr 12 18:37:34 2023, max compression
```

## Comparing `peptides-0.3.1.tar` & `peptides-0.3.2.tar`

### file list

```diff
@@ -1,221 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.021622 peptides-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-09-01 15:53:26.000000 peptides-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-09-01 15:53:26.000000 peptides-0.3.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-01 15:53:26.000000 peptides-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9761 2022-09-01 15:53:31.021622 peptides-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8115 2022-09-01 15:53:26.000000 peptides-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.993621 peptides-0.3.1/peptides/
--rw-r--r--   0 runner    (1001) docker     (121)    90917 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.989621 peptides-0.3.1/peptides/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.989621 peptides-0.3.1/peptides/datasets/Chou1989/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Chou1989/alpha/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Chou1989/alpha/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Chou1989/alpha+beta/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Chou1989/alpha+beta/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Chou1989/alpha_beta/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Chou1989/alpha_beta/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Chou1989/beta/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Chou1989/beta/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.989621 peptides-0.3.1/peptides/datasets/ChouZhang1995/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/ChouZhang1995/alpha/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/ChouZhang1995/alpha/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/ChouZhang1995/alpha+beta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/ChouZhang1995/alpha+beta/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/ChouZhang1995/alpha_beta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/ChouZhang1995/alpha_beta/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/ChouZhang1995/beta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/ChouZhang1995/beta/mean.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.993621 peptides-0.3.1/peptides/datasets/Nakashima1986/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Nakashima1986/all/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/all/mean.csv
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/all/sd.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha/mean.csv
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha/sd.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha+beta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha+beta/mean.csv
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha+beta/sd.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha_beta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha_beta/mean.csv
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/alpha_beta/sd.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Nakashima1986/beta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/beta/mean.csv
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/beta/sd.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/datasets/Nakashima1986/zeta/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/datasets/Nakashima1986/zeta/mean.csv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.993621 peptides-0.3.1/peptides/tables/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides/tables/aa_frequencies/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/aa_frequencies/KingJukes.csv
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/aa_frequencies/SwissProt2021.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.001621 peptides-0.3.1/peptides/tables/blosum/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM10.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM6.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM7.csv
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM8.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/blosum/BLOSUM9.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.001621 peptides-0.3.1/peptides/tables/boman/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/boman/Boman.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.001621 peptides-0.3.1/peptides/tables/charge/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/charge/sign.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.001621 peptides-0.3.1/peptides/tables/cruciani/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/cruciani/PP1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/cruciani/PP2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/cruciani/PP3.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.001621 peptides-0.3.1/peptides/tables/fasgai/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/fasgai/F1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/fasgai/F2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/fasgai/F3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/fasgai/F4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/fasgai/F5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/fasgai/F6.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.009621 peptides-0.3.1/peptides/tables/hydrophobicity/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Aboderin.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/AbrahamLeo.csv
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Argos.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Barley.csv
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/BlackMould.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/BullBreese.csv
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Casari.csv
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Chothia.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Cid.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Cowan3.4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Cowan7.5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Eisenberg.csv
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Engelman.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Fasman.csv
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Fauchere.csv
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Goldsack.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Guy.csv
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/HoppWoods.csv
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Janin.csv
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Jones.csv
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Juretic.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Kidera.csv
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Kuhn.csv
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/KyteDoolittle.csv
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Levitt.csv
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Manavalan.csv
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Miyazawa.csv
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Parker.csv
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Ponnuswamy.csv
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Prabhakaran.csv
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Rao.csv
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Rose.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Roseman.csv
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Sweet.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Tanford.csv
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Welling.csv
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Wilson.csv
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Wolfenden.csv
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/Zimmerman.csv
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/interfaceScale_pH2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/interfaceScale_pH8.csv
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/octanolScale_pH2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/octanolScale_pH8.csv
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/oiScale_pH2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/hydrophobicity/oiScale_pH8.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.009621 peptides-0.3.1/peptides/tables/instability/
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/instability/Guruprasad.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.009621 peptides-0.3.1/peptides/tables/kidera/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF10.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF6.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF7.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF8.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/kidera/KF9.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.009621 peptides-0.3.1/peptides/tables/linker_index/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/linker_index/Suyama.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.009621 peptides-0.3.1/peptides/tables/mass_shift/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/mass_shift/15n.csv
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/mass_shift/silac_13c.csv
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/mass_shift/silac_13c15n.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.013621 peptides-0.3.1/peptides/tables/molecular_weight/
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/molecular_weight/expasy.csv
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/molecular_weight/mascot.csv
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/molecular_weight/monoisotopic.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.013621 peptides-0.3.1/peptides/tables/mswhim/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/mswhim/MSWHIM1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/mswhim/MSWHIM2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/mswhim/MSWHIM3.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.013621 peptides-0.3.1/peptides/tables/pcp_descriptors/
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pcp_descriptors/E1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pcp_descriptors/E2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pcp_descriptors/E3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pcp_descriptors/E4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pcp_descriptors/E5.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.013621 peptides-0.3.1/peptides/tables/physical_descriptors/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/physical_descriptors/PD1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/physical_descriptors/PD2.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.013621 peptides-0.3.1/peptides/tables/pk/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Bjellqvist.csv
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Dawson.csv
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/EMBOSS.csv
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Lehninger.csv
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Murray.csv
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Rodwell.csv
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Sillero.csv
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Solomon.csv
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/pk/Stryer.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.017622 peptides-0.3.1/peptides/tables/protfp/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP6.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP7.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/protfp/ProtFP8.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.017622 peptides-0.3.1/peptides/tables/sneath/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/sneath/SV1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/sneath/SV2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/sneath/SV3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/sneath/SV4.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.017622 peptides-0.3.1/peptides/tables/st_scales/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST6.csv
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST7.csv
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/st_scales/ST8.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.017622 peptides-0.3.1/peptides/tables/t_scales/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/t_scales/T1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/t_scales/T2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/t_scales/T3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/t_scales/T4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/t_scales/T5.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.017622 peptides-0.3.1/peptides/tables/vhse/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE6.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE7.csv
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/vhse/VHSE8.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:31.021622 peptides-0.3.1/peptides/tables/z_scales/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/z_scales/Z1.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/z_scales/Z2.csv
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/z_scales/Z3.csv
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/z_scales/Z4.csv
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-01 15:53:26.000000 peptides-0.3.1/peptides/tables/z_scales/Z5.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 15:53:30.997621 peptides-0.3.1/peptides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9761 2022-09-01 15:53:30.000000 peptides-0.3.1/peptides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6507 2022-09-01 15:53:30.000000 peptides-0.3.1/peptides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 15:53:30.000000 peptides-0.3.1/peptides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-01 15:53:30.000000 peptides-0.3.1/peptides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 15:53:30.000000 peptides-0.3.1/peptides.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-01 15:53:30.000000 peptides-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-09-01 15:53:31.021622 peptides-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7569 2022-09-01 15:53:26.000000 peptides-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.188833 peptides-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-12 18:37:30.000000 peptides-0.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-12 18:37:30.000000 peptides-0.3.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-12 18:37:30.000000 peptides-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-04-12 18:37:34.188833 peptides-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-12 18:37:30.000000 peptides-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/
+-rw-r--r--   0 runner    (1001) docker     (123)    95083 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.152833 peptides-0.3.2/peptides/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.148833 peptides-0.3.2/peptides/datasets/Chou1989/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/datasets/Chou1989/alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Chou1989/alpha/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/datasets/Chou1989/alpha+beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Chou1989/alpha+beta/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/datasets/Chou1989/alpha_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Chou1989/alpha_beta/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/datasets/Chou1989/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Chou1989/beta/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.152833 peptides-0.3.2/peptides/datasets/ChouZhang1995/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/datasets/ChouZhang1995/alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/ChouZhang1995/alpha/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/ChouZhang1995/alpha+beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/ChouZhang1995/alpha+beta/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/ChouZhang1995/alpha_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/ChouZhang1995/alpha_beta/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/ChouZhang1995/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/ChouZhang1995/beta/mean.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.152833 peptides-0.3.2/peptides/datasets/Nakashima1986/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/Nakashima1986/all/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/all/mean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/all/sd.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha/mean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha/sd.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha+beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha+beta/mean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha+beta/sd.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha_beta/mean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/alpha_beta/sd.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/Nakashima1986/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/beta/mean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/beta/sd.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/datasets/Nakashima1986/zeta/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/datasets/Nakashima1986/zeta/mean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides/tables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.160833 peptides-0.3.2/peptides/tables/aa_frequencies/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/aa_frequencies/KingJukes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/aa_frequencies/SwissProt2021.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.164833 peptides-0.3.2/peptides/tables/blosum/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/blosum/BLOSUM9.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.164833 peptides-0.3.2/peptides/tables/boman/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/boman/Boman.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.164833 peptides-0.3.2/peptides/tables/charge/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/charge/sign.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.164833 peptides-0.3.2/peptides/tables/cruciani/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/cruciani/PP1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/cruciani/PP2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/cruciani/PP3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.164833 peptides-0.3.2/peptides/tables/fasgai/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/fasgai/F1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/fasgai/F2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/fasgai/F3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/fasgai/F4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/fasgai/F5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/fasgai/F6.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.172833 peptides-0.3.2/peptides/tables/hydrophobicity/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Aboderin.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/AbrahamLeo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Argos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Barley.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/BlackMould.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/BullBreese.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Casari.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Chothia.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Cid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Cowan3.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Cowan7.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Eisenberg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Engelman.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Fasman.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Fauchere.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Goldsack.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Guy.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/HoppWoods.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Janin.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Jones.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Juretic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Kidera.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Kuhn.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/KyteDoolittle.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Levitt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Manavalan.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Miyazawa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Parker.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Ponnuswamy.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Prabhakaran.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Rao.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Rose.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Roseman.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Sweet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Tanford.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Welling.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Wilson.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Wolfenden.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/Zimmerman.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/interfaceScale_pH2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/interfaceScale_pH8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/octanolScale_pH2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/octanolScale_pH8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/oiScale_pH2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/hydrophobicity/oiScale_pH8.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.172833 peptides-0.3.2/peptides/tables/instability/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/instability/Guruprasad.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/kidera/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/kidera/KF9.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/linker_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/linker_index/Suyama.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/mass_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/mass_shift/15n.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/mass_shift/silac_13c.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/mass_shift/silac_13c15n.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/molecular_weight/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/molecular_weight/expasy.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/molecular_weight/mascot.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/molecular_weight/monoisotopic.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/mswhim/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/mswhim/MSWHIM1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/mswhim/MSWHIM2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/mswhim/MSWHIM3.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/pcp_descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pcp_descriptors/E1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pcp_descriptors/E2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pcp_descriptors/E3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pcp_descriptors/E4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pcp_descriptors/E5.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.176833 peptides-0.3.2/peptides/tables/physical_descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/physical_descriptors/PD1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/physical_descriptors/PD2.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.180833 peptides-0.3.2/peptides/tables/pk/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Bjellqvist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Dawson.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/EMBOSS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Lehninger.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Murray.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Rodwell.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Sillero.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Solomon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/pk/Stryer.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.180833 peptides-0.3.2/peptides/tables/protfp/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/protfp/ProtFP8.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.180833 peptides-0.3.2/peptides/tables/sneath/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/sneath/SV1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/sneath/SV2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/sneath/SV3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/sneath/SV4.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.184833 peptides-0.3.2/peptides/tables/st_scales/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/st_scales/ST8.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.184833 peptides-0.3.2/peptides/tables/svger/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER11.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/svger/SVGER9.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.184833 peptides-0.3.2/peptides/tables/t_scales/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/t_scales/T1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/t_scales/T2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/t_scales/T3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/t_scales/T4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/t_scales/T5.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.188833 peptides-0.3.2/peptides/tables/vhse/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/vhse/VHSE8.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.188833 peptides-0.3.2/peptides/tables/z_scales/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/z_scales/Z1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/z_scales/Z2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/z_scales/Z3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/z_scales/Z4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 18:37:30.000000 peptides-0.3.2/peptides/tables/z_scales/Z5.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:37:34.156833 peptides-0.3.2/peptides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-04-12 18:37:34.000000 peptides-0.3.2/peptides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-04-12 18:37:34.000000 peptides-0.3.2/peptides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:37:34.000000 peptides-0.3.2/peptides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 18:37:34.000000 peptides-0.3.2/peptides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:37:34.000000 peptides-0.3.2/peptides.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-12 18:37:34.000000 peptides-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-12 18:37:34.188833 peptides-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-12 18:37:30.000000 peptides-0.3.2/setup.py
```

### Comparing `peptides-0.3.1/CHANGELOG.md` & `peptides-0.3.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/peptides.py/compare/v0.3.1...HEAD
+[Unreleased]: https://github.com/althonos/peptides.py/compare/v0.3.2...HEAD
+
+
+## [v0.3.2] - 2023-04-01
+[v0.3.2]: https://github.com/althonos/peptides.py/compare/v0.3.1...v0.3.2
+
+### Added
+- `Peptide.svger_descriptors` to compute SVGER descriptors from Tong *et al.* (2016).
+
+### Fixed
+- `Peptide.physical_descriptors` not being computed by `Peptide.descriptors`.
+
+### Documentation
+- Refactor documentation of individual descriptors into their own class.
+- Add missing `PCPDescriptors` and `PhysicalDescriptors` to the API documentation.
 
 
 ## [v0.3.1] - 2022-09-01
 [v0.3.1]: https://github.com/althonos/peptides.py/compare/v0.3.0...v0.3.1
 
 ### Fixed
 - `peptides.datasets` data files missing from the source distribution.
```

### Comparing `peptides-0.3.1/COPYING` & `peptides-0.3.2/COPYING`

 * *Files identical despite different names*

### Comparing `peptides-0.3.1/PKG-INFO` & `peptides-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: peptides
-Version: 0.3.1
+Version: 0.3.2
 Summary: Physicochemical properties, indices and descriptors for amino-acid sequences.
 Home-page: https://github.com/althonos/peptides.py
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/peptides.py/issues
 Project-URL: Changelog, https://github.com/althonos/peptides.py/blob/master/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/peptides.py/
-Project-URL: Builds, https://git.embl.de/larralde/peptides.py/-/pipelines
+Project-URL: Builds, https://github.com/althonos/peptides.py/actions
 Project-URL: PyPI, https://pypi.org/project/peptides
 Keywords: bioinformatics,protein,sequence,peptide,qsar
 Platform: posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # `peptides.py` [![Stars](https://img.shields.io/github/stars/althonos/peptides.py.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/peptides.py/stargazers)
 
 *Physicochemical properties, indices and descriptors for amino-acid sequences.*
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/peptides.py/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/peptides.py/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/peptides.py/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/peptides.py/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/peptides.py?style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/peptides.py/)
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/gpl-3.0/)
 [![PyPI](https://img.shields.io/pypi/v/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/peptides?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/peptides)
 [![Wheel](https://img.shields.io/pypi/wheel/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides/#files)
 [![Python Implementations](https://img.shields.io/badge/impl-universal-success.svg?style=flat-square&maxAge=3600&label=impl)](https://pypi.org/project/peptides/#files)
```

### Comparing `peptides-0.3.1/README.md` & `peptides-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # `peptides.py` [![Stars](https://img.shields.io/github/stars/althonos/peptides.py.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/peptides.py/stargazers)
 
 *Physicochemical properties, indices and descriptors for amino-acid sequences.*
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/peptides.py/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/peptides.py/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/peptides.py/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/peptides.py/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/peptides.py?style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/peptides.py/)
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/gpl-3.0/)
 [![PyPI](https://img.shields.io/pypi/v/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/peptides?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/peptides)
 [![Wheel](https://img.shields.io/pypi/wheel/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides/#files)
 [![Python Implementations](https://img.shields.io/badge/impl-universal-success.svg?style=flat-square&maxAge=3600&label=impl)](https://pypi.org/project/peptides/#files)
```

### Comparing `peptides-0.3.1/peptides/__init__.py` & `peptides-0.3.2/peptides/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,133 +16,449 @@
     import numpy
     _sum = numpy.sum
 except ImportError:
     numpy = None
     _sum = sum
 
 __all__ = ["Peptide", "tables", "datasets"]
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 __author__ = "Martin Larralde <martin.larralde@embl.de>"
 __license__ = "GPLv3"
 __credits__ = """
 Daniel Osorio, Paola Rondón-Villarreal and Rodrigo Torres for ``Peptides``.
 Alan Bleasby for the ``hmoment`` binary of the EMBOSS.
 Dong-Sheng Cao, Nan Xiao, Qing-Song Xu, and Alex F. Chen for ``Rcpi``.
 """.strip()
 
 
 class BLOSUMIndices(typing.NamedTuple):
+    """The BLOSUM62-derived indices of a peptide.
+
+    BLOSUM indices were derived of physicochemical properties that have
+    been subjected to a VARIMAX analysis and an alignment matrix of the
+    20 natural AAs using the BLOSUM62 matrix.
+
+    References:
+        - Georgiev, A. G.
+          *Interpretable Numerical Descriptors of Amino Acid Space*.
+          Journal of Computational Biology. May 2009;16(5):703–23.
+          :doi:`10.1089/cmb.2008.0173`. :pmid:`19432540`.
+
+    """
     blosum1: float
     blosum2: float
     blosum3: float
     blosum4: float
     blosum5: float
     blosum6: float
     blosum7: float
     blosum8: float
     blosum9: float
     blosum10: float
 
 
 class CrucianiProperties(typing.NamedTuple):
+    """The Cruciani properties of a peptide.
+
+    The Cruciani properties are a collection of scaled principal
+    component scores that summarize a broad set of descriptors
+    calculated based on the interaction of each amino acid residue with
+    several chemical groups (or "probes"), such as charged ions, methyl,
+    hydroxyl groups, and so forth.
+
+    References:
+        - Cruciani, G., M. Baroni, E. Carosati, M. Clementi, R. Valigi,
+          and S. Clementi.
+          *Peptide Studies by Means of Principal Properties of Amino
+          Acids Derived from MIF Descriptors*. Journal of Chemometrics.
+          2004;18(3-4):146–55. :doi:`10.1002/cem.856`.
+
+    """
     pp1: float
     pp2: float
     pp3: float
 
 
 class FasgaiVectors(typing.NamedTuple):
+    """FASGAI vectors of a peptide.
+
+    The FASGAI vectors (Factor Analysis Scales of Generalized Amino
+    Acid Information) are a set of amino acid descriptors, that reflect
+    hydrophobicity, alpha and turn propensities, bulky properties,
+    compositional characteristics, local flexibility, and electronic
+    properties, that can be utilized to represent the sequence
+    structural features of peptides or protein motifs.
+
+    References:
+        - Liang, G., G. Chen, W. Niu, and Z. Li.
+          *Factor Analysis Scales of Generalized Amino Acid Information
+          as Applied in Predicting Interactions between the Human
+          Amphiphysin-1 SH3 Domains and Their Peptide Ligands*.
+          Chemical Biology & Drug Design. Apr 2008;71(4):345–51.
+          :doi:`10.1111/j.1747-0285.2008.00641.x`. :pmid:`18318694`.
+
+    """
     f1: float
     f2: float
     f3: float
     f4: float
     f5: float
     f6: float
 
 
 class KideraFactors(typing.NamedTuple):
+    """The Kidera factors of a peptide.
+
+    The Kidera Factors were originally derived by applying multivariate
+    analysis to 188 physical properties of the 20 amino acids and using
+    dimension reduction techniques.
+
+    Attributes:
+        kf1 (`float`): A factor modeling the helix / bend preference.
+        kf2 (`float`): A factor modeling the side-chain size of each
+            residue (:aaindex:`KIDA850101`).
+        kf3 (`float`): A factor modeling the extended structured preference.
+        kf4 (`float`): A factor representing the hydrophobicity.
+        kf5 (`float`): A factor modeling the double-bend preference.
+        kf6 (`float`): A factor modeling the partial specific volume.
+        kf7 (`float`): A factor modeling the flat extended preference.
+        kf8 (`float`): A factor modeling the occurence in alpha regions.
+        kf9 (`float`): A factor encoding the pK-C.
+        kf10 (`float`): A factor representing the surrounding hydrophobicity.
+
+    References:
+        - Kidera, A., Y. Konishi, M. Oka, T. Ooi, and H. A. Scheraga.
+          *Statistical Analysis of the Physical Properties of the 20
+          Naturally Occurring Amino Acids*. Journal of Protein Chemistry.
+          Feb 1985;4(1):23–55. :doi:`10.1007/BF01025492`.
+
+    """
     kf1: float
     kf2: float
     kf3: float
     kf4: float
     kf5: float
     kf6: float
     kf7: float
     kf8: float
     kf9: float
     kf10: float
 
 
 class MSWHIMScores(typing.NamedTuple):
+    """The MS-WHIM scores of a peptide.
+
+    MS-WHIM scores were derived from 36 electrostatic potential
+    properties derived from the three-dimensional structure of the
+    20 natural amino acids.
+
+    References:
+        - Bravi, G., E. Gancia, P. Mascagni, M. Pegna, R. Todeschini,
+          and A. Zaliani.
+          *MS-WHIM, New 3D Theoretical Descriptors Derived from
+          Molecular Surface Properties: A Comparative 3D QSAR Study in a
+          Series of Steroids*. Journal of Computer-Aided Molecular
+          Design. Jan 1997;11(1):79-92.
+          :doi:`10.1023/a:1008079512289`. :pmid:`9139115`
+        - Gancia, E., G. Bravi, P. Mascagni, and A. Zaliani.
+          *Global 3D-QSAR Methods: MS-WHIM and Autocorrelation*. Journal
+          of Computer-Aided Molecular Design. Mar 2000;14(3):293–306.
+          :doi:`10.1023/a:1008142124682`. :pmid:`10756483`.
+        - Zaliani, A., and E. Gancia.
+          *MS-WHIM Scores for Amino Acids: A New 3D-Description for
+          Peptide QSAR and QSPR Studies*. Journal of Chemical
+          Information and Computer Sciences. May 1999;39(3):525–33.
+          :doi:`10.1021/ci980211b`.
+
+    """
     mswhim1: float
     mswhim2: float
     mswhim3: float
 
 
 class PhysicalDescriptors(typing.NamedTuple):
+    """The Physical Descriptors of a peptide.
+
+    The PP descriptors were constructed by improving on existing
+    PCA-derived descriptors (Z-scales, MS-WHIM and T-scales) after
+    correcting for the hydrophilicity of Methionine, Asparagine and
+    Tryptophan based on Feng *et al*.
+
+    Attributes:
+        pd1 (`float`): A descriptor related to residue volume.
+        pd2 (`float`): A descriptor related to hydrophilicity.
+
+    Note:
+        Barley *et al* insisted on maintaining a minimal number of
+        descriptors as a way to reduce the chances of finding spurious
+        QSAM models that would be affected by mutation between
+        interaction sites.
+
+    References:
+        - Barley, M. H., N. J. Turner, and R. Goodacre.
+          *Improved Descriptors for the Quantitative Structure–Activity
+          Relationship Modeling of Peptides and Proteins*. Journal of
+          Chemical Information and Modeling. Feb 2018;58(2):234–43.
+          :doi:`10.1021/acs.jcim.7b00488`. :pmid:`29338232`.
+        - Feng, X., J. Sanchis, M. T. Reetz, and H. Rabitz.
+          *Enhancing the Efficiency of Directed Evolution in Focused
+          Enzyme Libraries by the Adaptive Substituent Reordering
+          Algorithm*. Chemistry. Apr 2012;18(18):5646–54.
+          :doi:`10.1002/chem.201103811`. :pmid:`22434591`.
+
+    """
     pd1: float
     pd2: float
 
 
 class PCPDescriptors(typing.NamedTuple):
+    """The Physical-Chemical Properties descriptors of a peptide.
+
+    The PCP descriptors were constructed by performing multidimensional
+    scaling of 237 physical-chemical properties.
+
+    References:
+        - Mathura, V. S., and W. Braun.
+          *New Quantitative Descriptors of Amino Acids Based on
+          Multidimensional Scaling of a Large Number of
+          Physical–Chemical Properties*.
+          Molecular Modeling Annual. Dec 2001;7(12):445–53.
+          :doi:`10.1007/s00894-001-0058-5`.
+        - Mathura, V. S., D. Paris, and M. J. Mullan.
+          *A Novel Physico-Chemical Property Based Model for Studying
+          the Effects of Mutation on the Aggregation of Peptides*.
+          Protein and Peptide Letters. 2009;16(8):991–98.
+          :doi:`10.2174/092986609788923220`. :pmid:`19689427`.
+
+    """
     e1: float
     e2: float
     e3: float
     e4: float
     e5: float
 
 
 class ProtFPDescriptors(typing.NamedTuple):
+    """The ProtFP descriptors of a peptide.
+
+    The ProtFP set was constructed from a large initial selection of
+    indices obtained from the `AAindex <https://www.genome.jp/aaindex/>`_
+    database for all 20 naturally occurring amino acids.
+
+    References:
+        - van Westen, G. J., R. F. Swier, J. K. Wegner, A. P. Ijzerman,
+          H. W. van Vlijmen, and A. Bender.
+          *Benchmarking of Protein Descriptor Sets in Proteochemometric
+          Modeling (Part 1): Comparative Study of 13 Amino Acid
+          Descriptor Sets*. Journal of Cheminformatics. Sep 2013;5(1):41.
+          :doi:`10.1186/1758-2946-5-41`. :pmid:`24059694`.
+        - van Westen, G. J., R. F. Swier, I. Cortes-Ciriano,
+          J. K. Wegner, J. P. Overington, A. P. Ijzerman,
+          H. W. van Vlijmen, and A. Bender.
+          *Benchmarking of Protein Descriptor Sets in Proteochemometric
+          Modeling (Part 2): Modeling Performance of 13 Amino Acid
+          Descriptor Sets*. Journal of Cheminformatics. Sep 2013;5(1):42.
+          :doi:`10.1186/1758-2946-5-42`. :pmid:`24059743`.
+
+    """
     protfp1: float
     protfp2: float
     protfp3: float
     protfp4: float
     protfp5: float
     protfp6: float
     protfp7: float
     protfp8: float
 
 
 class SneathVectors(typing.NamedTuple):
+    """The Sneath vectors of a peptide.
+
+    These vectors were obtained in Sneath (1996) by running PCA on the
+    `ϕ coefficient <https://en.wikipedia.org/wiki/Phi_coefficient>`_
+    to explain the dissimilarity between the 20 natural amino acids
+    based on binary state encoding of 134 physical and chemical
+    properties (such as presence/absence of a —CH₃ group, step-wise
+    optical rotation, etc.).
+
+    Attributes:
+        sv1 (`float`): A descriptor representing mainly aliphatic properties
+            of each residue (:aaindex:`SNEP660101`).
+        sv2 (`float`): A descriptor putatively modeling the number of
+            reactive groups (:aaindex:`SNEP660102`).
+        sv3 (`float`): A descriptor representing the aromatic properties
+            of each residue (:aaindex:`SNEP660103`).
+        sv4 (`float`): A descriptor with uncertain interpretation
+            (:aaindex:`SNEP660104`).
+
+    References:
+        - Sneath, P. H. A.
+          *Relations between Chemical Structure and Biological Activity
+          in Peptides*.
+          Journal of Theoretical Biology. Nov 1996;12(2):157–95.
+          :doi:`10.1016/0022-5193(66)90112-3`. :pmid:`4291386`.
+
+    """
     sv1: float
     sv2: float
     sv3: float
     sv4: float
 
 
 class STScales(typing.NamedTuple):
+    """The ST-scales of a peptide.
+
+    The ST-scales were proposed in Yang *et al* (2010), taking 827
+    properties into account which are mainly constitutional,
+    topological, geometrical, hydrophobic, electronic, and steric
+    properties of a total set of 167 amino acids.
+
+    References:
+        - Yang, L., M. Shu, K. Ma, H. Mei, Y. Jiang, and Z. Li.
+          *ST-Scale as a Novel Amino Acid Descriptor and Its Application
+          in QSAM of Peptides and Analogues*.
+          Amino Acids. Mar 2010;38(3):805–16.
+          :doi:`10.1007/s00726-009-0287-y`. :pmid:`19373543`.
+
+    """
     st1: float
     st2: float
     st3: float
     st4: float
     st5: float
     st6: float
     st7: float
     st8: float
 
 
+class SVGERDescriptors(typing.NamedTuple):
+    """The SVGER descriptors of a peptide.
+
+    SVGER descriptors were constructed by Principal Component Analysis
+    of 74 geometrical descriptors (`svger1` to `svger6`), 44 eigenvalue
+    descriptors (`svger7`, `svger8` and `svger9`), and 41 Randić 
+    descriptors (`svger10` and `svger11`) computed for the 20 proteinogenic 
+    amino acids.
+
+    References:
+        - Tong, J., L. Li, M. Bai, and K. Li. 
+          *A New Descriptor of Amino Acids-SVGER and Its Applications in 
+          Peptide QSAR*. Molecular Informatics 36, no. 5–6 (2017): 1501023. 
+          :doi:`10.1002/minf.201501023`.
+        - Randic, M. 
+          *Molecular Shape Profiles*. Journal of Chemical Information and 
+          Computer Sciences 35, no. 3 (1 May 1995): 373–82. 
+          :doi:`10.1021/ci00025a005`.
+
+    """
+    svger1: float
+    svger2: float
+    svger3: float
+    svger4: float
+    svger5: float
+    svger6: float
+    svger7: float
+    svger8: float
+    svger9: float
+    svger10: float
+    svger11: float
+
+
 class TScales(typing.NamedTuple):
+    """The T-scales of a peptide.
+
+    The T-scales are based on 67 common topological descriptors of 135
+    amino acids. These topological descriptors are based on the
+    connectivity table of amino acids alone, and to not explicitly
+    consider 3D properties of each structure.
+
+    References:
+        - Tian, F., P. Zhou, and Z. Li.
+          *T-Scale as a Novel Vector of Topological Descriptors for
+          Amino Acids and Its Application in QSARs of Peptides*.
+          Journal of Molecular Structure. Mar 2007;830(1):106–15.
+          :doi:`10.1016/j.molstruc.2006.07.004`.
+
+    """
     t1: float
     t2: float
     t3: float
     t4: float
     t5: float
 
 
 class VHSEScales(typing.NamedTuple):
+    """The VHSE-scales of a peptide.
+
+    The VHSE-scales (principal components score Vectors of Hydrophobic,
+    Steric, and Electronic properties), are derived from principal
+    components analysis (PCA) on independent families of 18 hydrophobic
+    properties, 17 steric properties, and 15 electronic properties,
+    respectively, which are included in total 50 physicochemical
+    variables of 20 coded amino acids.
+
+    Attribute:
+        vhse1 (`float`): A descriptor representing hydrophobic properties.
+        vhse2 (`float`): Another descriptor representing hydrophobic
+            properties.
+        vhse3 (`float`): A descriptor representing steric properties.
+        vhse4 (`float`): Another descriptor representing steric properties.
+        vhse5 (`float`): A descriptor representing electronic properties.
+        vhse6 (`float`): A second descriptor representing electronic
+            properties.
+        vhse7 (`float`): A third descriptor representing electronic
+            properties.
+        vhse8 (`float`): A fourth descriptor representing electronic
+            properties.
+
+    References:
+        - Mei, H., Z. H. Liao, Y. Zhou, and S. Z. Li. *A New Set of
+          Amino Acid Descriptors and Its Application in Peptide QSARs*.
+          Biopolymers. 2005;80(6):775-86.
+          :doi:`10.1002/bip.20296`. :pmid:`15895431`.
+
+    """
     vhse1: float
     vhse2: float
     vhse3: float
     vhse4: float
     vhse5: float
     vhse6: float
     vhse7: float
     vhse8: float
 
 
 class ZScales(typing.NamedTuple):
+    """The Z-scales of a peptide.
+
+    The Z-scales were proposed in Sandberg *et al* (1998) based on
+    physicochemical properties of proteogenic and non-proteogenic
+    amino acids, including NMR data and thin-layer chromatography
+    (TLC) data.
+
+    Attributes:
+        z1 (`float`): A descriptor quantifying lipophilicity.
+        z2 (`float`): A descriptor modeling steric properties like steric
+            bulk and polarizability.
+        z3 (`float`): A descriptor quantifying electronic properties like
+            polarity and charge.
+        z4 (`float`): A descriptor relating to electronegativity, heat of
+            formation, electrophilicity and hardness.
+        z5 (`float`): Another descriptor relating to electronegativity,
+            heat of formation, electrophilicity and hardness.
+
+    References:
+        - Sandberg, M., L. Eriksson, J. Jonsson, M. Sjöström, and
+          S. Wold. *New Chemical Descriptors Relevant for the Design of
+          Biologically Active Peptides. A Multivariate Characterization
+          of 87 Amino Acids*.
+          Journal of Medicinal Chemistry. Jul 1998;41(14):2481–91.
+          :doi:`10.1021/jm9700575`. :pmid:`9651153`.
+
+    """
     z1: float
     z2: float
     z3: float
     z4: float
     z5: float
 
 
@@ -431,37 +747,40 @@
             [108..., 111..., 111..., 114..., 115...]
 
         .. versionadded:: 0.3.0
 
         """
         if window < 1:
             raise ValueError("Window must be strictly positive")
+
         # skip computing profile is window is larger than the available
         # number of residues in the peptide sequence
-        if len(self) + 1 > window:
+        if len(self) >= window:
             # build a look-up table and index values
             lut = [table.get(aa, default) for aa in self._CODE1]
             if numpy is None:
                 values = [lut[i] for i in self.encoded]
             else:
                 values = numpy.take(lut, self.encoded)  # type: ignore
             # don't perform window averaging if window is 1
-            if window == 1:
-                p = list(values)
+            if window <= 1:
+                return list(values)
             elif window > 1:
                 p = []
                 # use a rolling sum over the window
                 s = 0.0
                 for i in range(window):
                     s += values[i]
                 for j in range(window, len(self)):
                     p.append(s / window)
                     s -= values[j-window]
                     s += values[j]
                 p.append(s / window)
+        else:
+            p = []
 
         return p
 
     # --- Sequence properties -----------------------------------------------
 
     def counts(self) -> typing.Dict[str, int]:
         """Return a table of amino-acid counts in the peptide.
@@ -1626,19 +1945,17 @@
 
         """
         return self.profile(tables.LINKER_INDEX["Suyama"], window=window)
 
     # --- Descriptors --------------------------------------------------------
 
     def blosum_indices(self) -> BLOSUMIndices:
-        """Compute the BLOSUM62-derived indices of a peptide sequence.
+        """Compute the BLOSUM62-derived indices of the peptide.
 
-        BLOSUM indices were derived of physicochemical properties that have
-        been subjected to a VARIMAX analysis and an alignment matrix of the
-        20 natural AAs using the BLOSUM62 matrix.
+        See `~peptides.BLOSUMIndices` for more information.
 
         Returns:
             `peptides.BLOSUMIndices`: The computed average BLOSUM indices
             for all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("KLKLLLLLKLK")
@@ -1651,73 +1968,50 @@
             BLOSUM5    0.3173
             BLOSUM6    0.2527
             BLOSUM7    0.1464
             BLOSUM8    0.1427
             BLOSUM9   -0.2145
             BLOSUM10  -0.3218
 
-        References:
-            - Georgiev, A. G.
-              *Interpretable Numerical Descriptors of Amino Acid Space*.
-              Journal of Computational Biology. May 2009;16(5):703–23.
-              :doi:`10.1089/cmb.2008.0173`. :pmid:`19432540`.
-
         """
         out = []
         for i in range(len(tables.BLOSUM)):
             p = self.profile(tables.BLOSUM[f"BLOSUM{i+1}"])
             out.append(_sum(p) / len(self))
         return BLOSUMIndices(*out)
 
     def cruciani_properties(self) -> CrucianiProperties:
-        """Compute the Cruciani properties of protein sequence.
+        """Compute the Cruciani properties of the peptide.
 
-        The Cruciani properties are a collection of scaled principal
-        component scores that summarize a broad set of descriptors
-        calculated based on the interaction of each amino acid residue with
-        several chemical groups (or "probes"), such as charged ions, methyl,
-        hydroxyl groups, and so forth.
+        See `~peptides.CrucianiProperties` for more information.
 
         Returns:
             `peptides.CrucianiProperties`: The computed average Cruciani
             properties of all the amino acids in the corresponding peptide
             sequence.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
             >>> for i, b in enumerate(peptide.cruciani_properties()):
             ...     print(f"PP{i+1:<3} {b: .4f}")
             PP1   -0.1130
             PP2   -0.0220
             PP3    0.2735
 
-        References:
-            - Cruciani, G., M. Baroni, E. Carosati, M. Clementi, R. Valigi,
-              and S. Clementi.
-              *Peptide Studies by Means of Principal Properties of Amino
-              Acids Derived from MIF Descriptors*.
-              Journal of Chemometrics. 2004;18(3-4):146–55.
-              :doi:`10.1002/cem.856`.
-
         """
         out = []
         for i in range(len(tables.CRUCIANI)):
             p = self.profile(tables.CRUCIANI[f"PP{i+1}"])
             out.append(_sum(p) / len(self))
         return CrucianiProperties(*out)
 
     def fasgai_vectors(self) -> FasgaiVectors:
-        """Compute the FASGAI vectors of a protein sequence.
+        """Compute the FASGAI vectors of the peptide.
 
-        The FASGAI vectors (Factor Analysis Scales of Generalized Amino
-        Acid Information) is a set of amino acid descriptors, that reflects
-        hydrophobicity, alpha and turn propensities, bulky properties,
-        compositional characteristics, local flexibility, and electronic
-        properties, that can be utilized to represent the sequence
-        structural features of peptides or protein motifs.
+        See `~peptides.FasgaiVectors` for more information.
 
         Returns:
             `peptides.FasgaiVectors`: The computed average FASGAI vectors
             for all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
@@ -1726,44 +2020,29 @@
             F1   -0.13675
             F2   -0.45485
             F3   -0.11695
             F4   -0.45800
             F5   -0.38015
             F6    0.52740
 
-        References:
-            - Liang, G., G. Chen, W. Niu, and Z. Li.
-              *Factor Analysis Scales of Generalized Amino Acid Information
-              as Applied in Predicting Interactions between the Human
-              Amphiphysin-1 SH3 Domains and Their Peptide Ligands*.
-              Chemical Biology & Drug Design. Apr 2008;71(4):345–51.
-              :doi:`10.1111/j.1747-0285.2008.00641.x`. :pmid:`18318694`.
-
         """
         out = []
         for i in range(len(tables.FASGAI)):
             p = self.profile(tables.FASGAI[f"F{i+1}"])
             out.append(_sum(p) / len(self))
         return FasgaiVectors(*out)
 
     def kidera_factors(self) -> KideraFactors:
-        """Compute the Kidera factors of a protein sequence.
+        """Compute the Kidera factors of the peptide.
 
-        The Kidera Factors were originally derived by applying multivariate
-        analysis to 188 physical properties of the 20 amino acids and using
-        dimension reduction techniques.
+        See `~peptides.KideraFactors` for more information.
 
         Returns:
-            `peptides.KideraFactors`: The compute average of Kidera factors
-            for all the amino acids in the peptide. *KF1* models helix/bend
-            preference, *KF2* the side-chain size, *KF3* the extended
-            structure preference, *KF5* the double-bend preference, *KF6*
-            the partial specific volume, *KF7* the flat extended preference,
-            *KF8* the occurence in alpha regions, *KF9* the pK-C, *KF10*
-            the surrounding hydrophobicity.
+            `peptides.KideraFactors`: The computed average Kidera factors
+            for all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("KLKLLLLLKLK")
             >>> for i, kf in enumerate(peptide.kidera_factors()):
             ...     print(f"KF{i+1:<3} {kf: .4f}")
             KF1   -0.7855
             KF2    0.2982
@@ -1772,77 +2051,49 @@
             KF5    0.2100
             KF6   -1.8936
             KF7    1.0291
             KF8   -0.5127
             KF9    0.1118
             KF10   0.8100
 
-        References:
-            - Kidera, A., Y. Konishi, M. Oka, T. Ooi, and H. A. Scheraga.
-              *Statistical Analysis of the Physical Properties of the 20
-              Naturally Occurring Amino Acids*.
-              Journal of Protein Chemistry. Feb 1985;4(1):23–55.
-              :doi:`10.1007/BF01025492`.
-
         """
         out = []
         for i in range(len(tables.KIDERA)):
             p = self.profile(tables.KIDERA[f"KF{i+1}"])
             out.append(_sum(p) / len(self))
         return KideraFactors(*out)
 
     def ms_whim_scores(self) -> MSWHIMScores:
-        """Compute the MS-WHIM scores of a protein sequence.
+        """Compute the MS-WHIM scores of the peptide.
 
-        MS-WHIM scores were derived from 36 electrostatic potential
-        properties derived from the three-dimensional structure of the
-        20 natural amino acids.
+        See `~peptides.MSWHIMScores` for more information.
 
         Returns:
             `peptides.MSWHIMScores`: The compute average of MS-WHIM scores
             of all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("KLKLLLLLKLK")
             >>> for i, mw in enumerate(peptide.ms_whim_scores()):
             ...     print(f"MSWHIM{i+1:<3} {mw: .4f}")
             MSWHIM1   -0.6564
             MSWHIM2    0.4873
             MSWHIM3    0.1164
 
-        References:
-            - Bravi, G., E. Gancia, P. Mascagni, M. Pegna, R. Todeschini,
-              and A. Zaliani.
-              *MS-WHIM, New 3D Theoretical Descriptors Derived from
-              Molecular Surface Properties: A Comparative 3D QSAR Study in a
-              Series of Steroids*. Journal of Computer-Aided Molecular
-              Design. Jan 1997;11(1):79-92.
-              :doi:`10.1023/a:1008079512289`. :pmid:`9139115`
-            - Gancia, E., G. Bravi, P. Mascagni, and A. Zaliani.
-              *Global 3D-QSAR Methods: MS-WHIM and Autocorrelation*. Journal
-              of Computer-Aided Molecular Design. Mar 2000;14(3):293–306.
-              :doi:`10.1023/a:1008142124682`. :pmid:`10756483`.
-            - Zaliani, A., and E. Gancia.
-              *MS-WHIM Scores for Amino Acids: A New 3D-Description for
-              Peptide QSAR and QSPR Studies*. Journal of Chemical
-              Information and Computer Sciences. May 1999;39(3):525–33.
-              :doi:`10.1021/ci980211b`.
-
         """
         out = []
         for i in range(len(tables.MSWHIM)):
             p = self.profile(tables.MSWHIM[f"MSWHIM{i+1}"])
             out.append(_sum(p) / len(self))
         return MSWHIMScores(*out)
 
     def pcp_descriptors(self) -> PCPDescriptors:
-        """Compute the Physical-Chemical Properties of a protein sequence.
+        """Compute the Physical-Chemical Properties descriptors of the peptide.
 
-        The PCP descriptors were constructed by performing multidimensional
-        scaling of 237 physical-chemical properties.
+        See `~peptides.PCPDescriptors` for more information.
 
         Returns:
             `peptides.PCPDescriptors`: The computed average of PCP
             descriptors of all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
@@ -1850,86 +2101,49 @@
             ...     print(f"E{i+1:<3} {pcp: .5f}")
             E1    0.01090
             E2    0.03810
             E3    0.12505
             E4    0.04095
             E5   -0.10595
 
-        References:
-            - Mathura, V. S., and W. Braun.
-              *New Quantitative Descriptors of Amino Acids Based on
-              Multidimensional Scaling of a Large Number of
-              Physical–Chemical Properties*.
-              Molecular Modeling Annual. Dec 2001;7(12):445–53.
-              :doi:`10.1007/s00894-001-0058-5`.
-            - Mathura, V. S., D. Paris, and M. J. Mullan.
-              *A Novel Physico-Chemical Property Based Model for Studying
-              the Effects of Mutation on the Aggregation of Peptides*.
-              Protein and Peptide Letters. 2009;16(8):991–98.
-              :doi:`10.2174/092986609788923220`. :pmid:`19689427`.
-
         """
         out = []
         for i in range(len(tables.PCP_DESCRIPTORS)):
             p = self.profile(tables.PCP_DESCRIPTORS[f"E{i+1}"])
             out.append(_sum(p) / len(self))
         return PCPDescriptors(*out)
 
     def physical_descriptors(self) -> PhysicalDescriptors:
-        """Compute the Physical Descriptors of a protein sequence.
+        """Compute the Physical Descriptors of the peptide.
 
-        The PP descriptors were constructed by improving on existing
-        PCA-derived descriptors (Z-scales, MS-WHIM and T-scales) after
-        correcting for the hydrophilicity of Methionine, Asparagine and
-        Tryptophan based on Feng *et al*.
+        See `~peptides.PhysicalDescriptors` for more information.
 
         Returns:
             `peptides.PhyiscalDescriptors`: The computed average of Physical
             Descriptors of all the amino acids in the peptide. *PD1* is
             related to volume while *PD2* is related to hydrophilicity.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
             >>> for i, pd in enumerate(peptide.physical_descriptors()):
             ...     print(f"PD{i+1:<3} {pd: .4f}")
             PD1    0.1190
             PD2    0.2825
 
-        Note:
-            Barley *et al* insisted on maintaining a minimal number of
-            descriptors as a way to reduce the chances of finding spurious
-            QSAM models that would be affected by mutation between
-            interaction sites.
-
-        References:
-          - Barley, M. H., N. J. Turner, and R. Goodacre.
-            *Improved Descriptors for the Quantitative Structure–Activity
-            Relationship Modeling of Peptides and Proteins*. Journal of
-            Chemical Information and Modeling. Feb 2018;58(2):234–43.
-            :doi:`10.1021/acs.jcim.7b00488`. :pmid:`29338232`.
-          - Feng, X., J. Sanchis, M. T. Reetz, and H. Rabitz.
-            *Enhancing the Efficiency of Directed Evolution in Focused
-            Enzyme Libraries by the Adaptive Substituent Reordering
-            Algorithm*. Chemistry. Apr 2012;18(18):5646–54.
-            :doi:`10.1002/chem.201103811`. :pmid:`22434591`.
-
         """
         out = []
         for i in range(len(tables.PHYSICAL_DESCRIPTORS)):
             p = self.profile(tables.PHYSICAL_DESCRIPTORS[f"PD{i+1}"])
             out.append(_sum(p) / len(self))
         return PhysicalDescriptors(*out)
 
     def protfp_descriptors(self) -> ProtFPDescriptors:
-        """Compute the ProtFP descriptors of a protein sequence.
+        """Compute the ProtFP descriptors of the peptide.
 
-        The ProtFP descriptor set was constructed from a large initial
-        selection of indices obtained from the
-        `AAindex <https://www.genome.jp/aaindex/>`_ database for all 20
-        naturally occurring amino acids.
+        See `~peptides.ProtFPDescriptors` for more information.
 
         Returns:
             `peptides.ProtFPDescriptors`: The computed average of ProtFP
             descriptors of all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
@@ -1940,83 +2154,50 @@
             ProtFP3    1.9930
             ProtFP4   -0.2845
             ProtFP5    0.7315
             ProtFP6    0.7000
             ProtFP7    0.1715
             ProtFP8    0.1135
 
-        References:
-            - van Westen, G. J., R. F. Swier, J. K. Wegner, A. P. Ijzerman,
-              H. W. van Vlijmen, and A. Bender.
-              *Benchmarking of Protein Descriptor Sets in Proteochemometric
-              Modeling (Part 1): Comparative Study of 13 Amino Acid
-              Descriptor Sets*. Journal of Cheminformatics. Sep 2013;5(1):41.
-              :doi:`10.1186/1758-2946-5-41`. :pmid:`24059694`.
-            - van Westen, G. J., R. F. Swier, I. Cortes-Ciriano,
-              J. K. Wegner, J. P. Overington, A. P. Ijzerman,
-              H. W. van Vlijmen, and A. Bender.
-              *Benchmarking of Protein Descriptor Sets in Proteochemometric
-              Modeling (Part 2): Modeling Performance of 13 Amino Acid
-              Descriptor Sets*. Journal of Cheminformatics. Sep 2013;5(1):42.
-              :doi:`10.1186/1758-2946-5-42`. :pmid:`24059743`.
-
         """
         out = []
         for i in range(len(tables.PROTFP)):
             p = self.profile(tables.PROTFP[f"ProtFP{i+1}"])
             out.append(_sum(p) / len(self))
         return ProtFPDescriptors(*out)
 
     def sneath_vectors(self) -> SneathVectors:
-        """Compute the Sneath vectors for a protein sequence.
+        """Compute the Sneath vectors for the peptide.
 
-        These vectors were obtained in Sneath (1996) by running PCA on the
-        `ϕ coefficient <https://en.wikipedia.org/wiki/Phi_coefficient>`_
-        to explain the dissimilarity between the 20 natural amino acids
-        based on binary state encoding of 134 physical and chemical
-        properties (such as presence/absence of a —CH₃ group, step-wise
-        optical rotation, etc.).
+        See `~peptides.SneathVectors` for more information.
 
         Returns:
             `peptides.SneathVectors`: The computed average of Sneath vectors
-            of all the amino acids in the peptide. *SV1* appears to
-            represent mainly aliphatic properties, *SV2* may model the
-            number of reactive groups, *SV3* the aromatic properties, but
-            *SV4* has no certain interpretation.
+            of all the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
             >>> for i, fp in enumerate(peptide.sneath_vectors()):
             ...     print(f"SV{i+1:<3} {fp: .5f}")
             SV1    0.19620
             SV2    0.04655
             SV3    0.04050
             SV4    0.02775
 
-        References:
-            - Sneath, P. H. A.
-              *Relations between Chemical Structure and Biological Activity
-              in Peptides*.
-              Journal of Theoretical Biology. Nov 1996;12(2):157–95.
-              :doi:`10.1016/0022-5193(66)90112-3`. :pmid:`4291386`.
-
         """
         out = []
         for i in range(len(tables.SNEATH)):
             p = self.profile(tables.SNEATH[f"SV{i+1}"])
             out.append(_sum(p) / len(self))
         return SneathVectors(*out)
 
     def st_scales(self) -> STScales:
-        """Compute the ST-scales of a protein sequence.
+        """Compute the ST-scales of the peptide.
 
-        The ST-scales were proposed in Yang *et al* (2010), taking 827
-        properties into account which are mainly constitutional,
-        topological, geometrical, hydrophobic, electronic, and steric
-        properties of a total set of 167 amino acids.
+        See `~peptides.STScales` for more information.
 
         Returns:
             `peptides.STScales`: The computed average of ST-scales of all
             the amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
@@ -2027,35 +2208,43 @@
             ST3    0.05150
             ST4    0.07135
             ST5   -0.27905
             ST6   -0.80995
             ST7    0.58020
             ST8    0.54400
 
-        References:
-            - Yang, L., M. Shu, K. Ma, H. Mei, Y. Jiang, and Z. Li.
-              *ST-Scale as a Novel Amino Acid Descriptor and Its Application
-              in QSAM of Peptides and Analogues*.
-              Amino Acids. Mar 2010;38(3):805–16.
-              :doi:`10.1007/s00726-009-0287-y`. :pmid:`19373543`.
-
         """
         out = []
         for i in range(len(tables.ST_SCALES)):
             p = self.profile(tables.ST_SCALES[f"ST{i+1}"])
             out.append(_sum(p) / len(self))
         return STScales(*out)
 
+    def svger_descriptors(self) -> SVGERDescriptors:
+        """Compute the SVGER descriptors of the peptide.
+
+        See `~peptides.SVGERDescriptors` for more information.
+
+        Returns:
+            `peptides.SVGERDescriptors`: The computed average of SVGER
+            descriptors of all the amino acids in the peptide.
+
+        .. versionadded:: 0.3.2
+
+        """
+        out = []
+        for i in range(len(tables.SVGER)):
+            p = self.profile(tables.SVGER[f"SVGER{i+1}"])
+            out.append(_sum(p) / len(self))
+        return SVGERDescriptors(*out)
+
     def t_scales(self) -> TScales:
-        """Compute the T-scales of a protein sequence.
+        """Compute the T-scales of the peptide.
 
-        The T-scales are based on 67 common topological descriptors of 135
-        amino acids. These topological descriptors are based on the
-        connectivity table of amino acids alone, and to not explicitly
-        consider 3D properties of each structure.
+        See `~peptides.TScales` for more information.
 
         Returns:
             `peptides.TScales`: The computed average of T-scales of all the
             amino acids in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
@@ -2063,37 +2252,25 @@
             ...     print(f"T{i+1:<3} {t: .4f}")
             T1   -3.2700
             T2   -0.0035
             T3   -0.3855
             T4   -0.1475
             T5    0.7585
 
-        References:
-            - Tian, F., P. Zhou, and Z. Li.
-              *T-Scale as a Novel Vector of Topological Descriptors for
-              Amino Acids and Its Application in QSARs of Peptides*.
-              Journal of Molecular Structure. Mar 2007;830(1):106–15.
-              :doi:`10.1016/j.molstruc.2006.07.004`.
-
         """
         out = []
         for i in range(len(tables.T_SCALES)):
             p = self.profile(tables.T_SCALES[f"T{i+1}"])
             out.append(_sum(p) / len(self))
         return TScales(*out)
 
     def vhse_scales(self) -> VHSEScales:
-        """Compute the VHSE-scales of a protein sequence.
+        """Compute the VHSE-scales of the peptide.
 
-        The VHSE-scales (principal components score Vectors of Hydrophobic,
-        Steric, and Electronic properties), are derived from principal
-        components analysis (PCA) on independent families of 18 hydrophobic
-        properties, 17 steric properties, and 15 electronic properties,
-        respectively, which are included in total 50 physicochemical
-        variables of 20 coded amino acids.
+        See `~peptides.VHSEScales` for more information.
 
         Returns:
             `peptides.VHSEScales`: The computed average of VHSE-scales of
             the amino acids in the peptide. *VHSE1* and *VHSE2* represent
             hydrophobic properties, *VHSE3* and *VHSE4* represent steric
             properties, while *VHSE5*, *VHSE6*, *VHSE7* and *VHSE8*
             represent electronic properties.
@@ -2107,76 +2284,56 @@
             VHSE3   -0.0055
             VHSE4    0.7955
             VHSE5    0.4355
             VHSE6    0.2485
             VHSE7    0.1740
             VHSE8   -0.0960
 
-        References:
-            - Mei, H., Z. H. Liao, Y. Zhou, and S. Z. Li. *A New Set of
-              Amino Acid Descriptors and Its Application in Peptide QSARs*.
-              Biopolymers. 2005;80(6):775-86.
-              :doi:`10.1002/bip.20296`. :pmid:`15895431`.
-
         """
         out = []
         for i in range(len(tables.VHSE)):
             p = self.profile(tables.VHSE[f"VHSE{i+1}"])
             out.append(_sum(p) / len(self))
         return VHSEScales(*out)
 
     def z_scales(self) -> ZScales:
-        """Compute the Z-scales of a protein sequence.
+        """Compute the Z-scales of the peptide.
 
-        The Z-scales were proposed in Sandberg *et al* (1998) based on
-        physicochemical properties of proteogenic and non-proteogenic
-        amino acids, including NMR data and thin-layer chromatography
-        (TLC) data.
+        See `~peptides.ZScales` for more information.
+
+        Returns:
+            `peptides.ZScales`: The computed average of Z-scales of all
+            the amino acid in the peptide.
 
         Example:
             >>> peptide = Peptide("QWGRRCCGWGPGRRYCVRWC")
             >>> for i, z in enumerate(peptide.z_scales()):
             ...     print(f"Z{i+1:<3} {0.0+round(z,5): .4f}")
             Z1    0.5520
             Z2    0.0985
             Z3    0.0000
             Z4    0.8130
             Z5   -0.8285
 
-        Returns:
-            `peptides.ZScales`: The computed average of Z-scales of all
-            the amino acid in the peptide. *Z1* quantifies lipophilicity,
-            *Z2* models steric properties (like steric bulk and
-            polarizability), *Z3* quantifies electronic properties (like
-            polarity and charge) while *Z4* and *Z5* relate
-            electronegativity, heat of formation, electrophilicity, and
-            hardness.
-
-        References:
-            - Sandberg, M., L. Eriksson, J. Jonsson, M. Sjöström, and
-              S. Wold. *New Chemical Descriptors Relevant for the Design of
-              Biologically Active Peptides. A Multivariate Characterization
-              of 87 Amino Acids*.
-              Journal of Medicinal Chemistry. Jul 1998;41(14):2481–91.
-              :doi:`10.1021/jm9700575`. :pmid:`9651153`.
-
         """
         out = []
         for i in range(len(tables.Z_SCALES)):
             p = self.profile(tables.Z_SCALES[f"Z{i+1}"])
             out.append(_sum(p) / len(self))
         return ZScales(*out)
 
     __DESCRIPTORS = {
         "BLOSUM": blosum_indices,
         "PP": cruciani_properties,
         "F": fasgai_vectors,
         "KF": kidera_factors,
         "MSWHIM": ms_whim_scores,
         "E": pcp_descriptors,
+        "PD": physical_descriptors,
         "ProtFP": protfp_descriptors,
         "SV": sneath_vectors,
         "ST": st_scales,
+        "SVGER": svger_descriptors,
         "T": t_scales,
         "VHSE": vhse_scales,
         "Z": z_scales,
     }
```

### Comparing `peptides-0.3.1/peptides/tables/instability/Guruprasad.csv` & `peptides-0.3.2/peptides/tables/instability/Guruprasad.csv`

 * *Files identical despite different names*

### Comparing `peptides-0.3.1/peptides.egg-info/PKG-INFO` & `peptides-0.3.2/peptides.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: peptides
-Version: 0.3.1
+Version: 0.3.2
 Summary: Physicochemical properties, indices and descriptors for amino-acid sequences.
 Home-page: https://github.com/althonos/peptides.py
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/peptides.py/issues
 Project-URL: Changelog, https://github.com/althonos/peptides.py/blob/master/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/peptides.py/
-Project-URL: Builds, https://git.embl.de/larralde/peptides.py/-/pipelines
+Project-URL: Builds, https://github.com/althonos/peptides.py/actions
 Project-URL: PyPI, https://pypi.org/project/peptides
 Keywords: bioinformatics,protein,sequence,peptide,qsar
 Platform: posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # `peptides.py` [![Stars](https://img.shields.io/github/stars/althonos/peptides.py.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/peptides.py/stargazers)
 
 *Physicochemical properties, indices and descriptors for amino-acid sequences.*
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/peptides.py/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/peptides.py/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/peptides.py/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/peptides.py/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/peptides.py?style=flat-square&maxAge=3600)](https://codecov.io/gh/althonos/peptides.py/)
 [![License](https://img.shields.io/badge/license-GPLv3-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/gpl-3.0/)
 [![PyPI](https://img.shields.io/pypi/v/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/peptides?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/peptides)
 [![Wheel](https://img.shields.io/pypi/wheel/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/peptides.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/peptides/#files)
 [![Python Implementations](https://img.shields.io/badge/impl-universal-success.svg?style=flat-square&maxAge=3600&label=impl)](https://pypi.org/project/peptides/#files)
```

### Comparing `peptides-0.3.1/peptides.egg-info/SOURCES.txt` & `peptides-0.3.2/peptides.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,25 @@
 peptides/tables/st_scales/ST2.csv
 peptides/tables/st_scales/ST3.csv
 peptides/tables/st_scales/ST4.csv
 peptides/tables/st_scales/ST5.csv
 peptides/tables/st_scales/ST6.csv
 peptides/tables/st_scales/ST7.csv
 peptides/tables/st_scales/ST8.csv
+peptides/tables/svger/SVGER1.csv
+peptides/tables/svger/SVGER10.csv
+peptides/tables/svger/SVGER11.csv
+peptides/tables/svger/SVGER2.csv
+peptides/tables/svger/SVGER3.csv
+peptides/tables/svger/SVGER4.csv
+peptides/tables/svger/SVGER5.csv
+peptides/tables/svger/SVGER6.csv
+peptides/tables/svger/SVGER7.csv
+peptides/tables/svger/SVGER8.csv
+peptides/tables/svger/SVGER9.csv
 peptides/tables/t_scales/T1.csv
 peptides/tables/t_scales/T2.csv
 peptides/tables/t_scales/T3.csv
 peptides/tables/t_scales/T4.csv
 peptides/tables/t_scales/T5.csv
 peptides/tables/vhse/VHSE1.csv
 peptides/tables/vhse/VHSE2.csv
```

### Comparing `peptides-0.3.1/setup.cfg` & `peptides-0.3.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 	Typing :: Typed
 project_urls = 
 	Bug Tracker = https://github.com/althonos/peptides.py/issues
 	Changelog = https://github.com/althonos/peptides.py/blob/master/CHANGELOG.md
 	Coverage = https://codecov.io/gh/althonos/peptides.py/
-	Builds = https://git.embl.de/larralde/peptides.py/-/pipelines
+	Builds = https://github.com/althonos/peptides.py/actions
 	PyPI = https://pypi.org/project/peptides
 
 [options]
 zip_safe = true
-packages = peptides
+packages = peptides, peptides.tables, peptides.datasets
 python_requires = >=3.6
 test_suite = tests
 include_package_data = true
 setup_requires = 
 	setuptools >=46.4
 	astor ~=0.6
```

### Comparing `peptides-0.3.1/setup.py` & `peptides-0.3.2/setup.py`

 * *Files identical despite different names*

