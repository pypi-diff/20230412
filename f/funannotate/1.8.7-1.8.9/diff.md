# Comparing `tmp/funannotate-1.8.7.tar.gz` & `tmp/funannotate-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funannotate-1.8.7.tar", last modified: Sat Apr 17 21:15:34 2021, max compression
+gzip compressed data, was "funannotate-1.8.9.tar", last modified: Mon Aug  2 04:50:33 2021, max compression
```

## Comparing `funannotate-1.8.7.tar` & `funannotate-1.8.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.258609 funannotate-1.8.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-04-17 21:15:25.000000 funannotate-1.8.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-04-17 21:15:25.000000 funannotate-1.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-04-17 21:15:34.258609 funannotate-1.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2021-04-17 21:15:25.000000 funannotate-1.8.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.234609 funannotate-1.8.7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     9283 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/annotate.rst
--rw-r--r--   0 runner    (1001) docker     (121)    41605 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/commands.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/compare.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7289 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/conda.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5192 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/databases.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/evidence.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)      815 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)      461 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/manual.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13142 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/predict.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4692 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12080 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4763 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/update.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-04-17 21:15:25.000000 funannotate-1.8.7/docs/utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.246609 funannotate-1.8.7/funannotate/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    75843 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/annotate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.254609 funannotate-1.8.7/funannotate/aux_scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6927 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/augustus_parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2661 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/enrichment_parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3848 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/fasta2agp.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)    21217 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/filterGenemark.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)     5716 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/filterIntronsFindStrand.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)   144316 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/funannotate-BUSCO2-py2.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   144417 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/funannotate-BUSCO2.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14956 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/funannotate-p2g.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    22880 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/funannotate-runEVM.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4623 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/genemark_gtf2gff3.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)      642 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/getEggNog.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     7994 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/hmmer_parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14425 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/iprscan-local.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3206 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/iprscan2annotations.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    65930 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/pal2nal.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)     3842 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/phobius-multiproc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    35348 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/phobius-remote.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)    15288 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/runIPRscan.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      389 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/sam2bam.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)     9448 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/tbl2asn_parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8768 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/trinity.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5461 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/trnascan2gff3.pl
--rwxr-xr-x   0 runner    (1001) docker     (121)      723 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/aux_scripts/xmlcombine.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17100 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/check.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8072 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    59286 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.258609 funannotate-1.8.7/funannotate/config/
--rw-r--r--   0 runner    (1001) docker     (121)   121918 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/EOG092C0B3U.prfl
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/TruSeq3-PE.fa
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/TruSeq3-SE.fa
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/busco_test.fa
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/codeml.config
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/extrinsic.E.XNT.RM.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    12708 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/smcogs.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/test.sbt
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/config/tf_interpro.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     2275 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/downloads.json
--rwxr-xr-x   0 runner    (1001) docker     (121)     7170 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/fix.py
--rw-r--r--   0 runner    (1001) docker     (121)    33569 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/funannotate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.226608 funannotate-1.8.7/funannotate/html_template/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.258609 funannotate-1.8.7/funannotate/html_template/css/
--rw-r--r--   0 runner    (1001) docker     (121)   121260 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/html_template/css/bootstrap.min.css
--rwxr-xr-x   0 runner    (1001) docker     (121)      291 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/html_template/css/starter-template.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.258609 funannotate-1.8.7/funannotate/html_template/js/
--rwxr-xr-x   0 runner    (1001) docker     (121)    36868 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/html_template/js/bootstrap.min.js
--rwxr-xr-x   0 runner    (1001) docker     (121)     2130 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/html_template/js/ie-emulation-modes-warning.js
--rwxr-xr-x   0 runner    (1001) docker     (121)      641 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/html_template/js/ie10-viewport-bug-workaround.js
--rwxr-xr-x   0 runner    (1001) docker     (121)    95957 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/html_template/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     8553 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/interlap.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      449 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/iprscan.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   394247 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/library.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8910 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/mask.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5091 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/outgroups.py
--rw-r--r--   0 runner    (1001) docker     (121)   105346 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/predict.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14874 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)    11244 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/resources.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    31196 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/setupDB.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2836 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/sort.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6604 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/species.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12267 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/stackedBarGraph.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18411 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/test.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    62088 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/train.py
--rwxr-xr-x   0 runner    (1001) docker     (121)   123934 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/update.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.258609 funannotate-1.8.7/funannotate/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      943 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/bam2gff3.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    51646 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/contrast.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1256 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/gbk2parts.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1597 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/gff2prot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18472 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/gff2tbl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2476 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/gff_reformat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3210 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/quarry2gff3.py
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3977 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/stringtie2gff3.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7034 2021-04-17 21:15:25.000000 funannotate-1.8.7/funannotate/utilities/tbl2gbk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-17 21:15:34.250609 funannotate-1.8.7/funannotate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-04-17 21:15:34.000000 funannotate-1.8.7/funannotate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2021-04-17 21:15:34.000000 funannotate-1.8.7/funannotate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-17 21:15:34.000000 funannotate-1.8.7/funannotate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-04-17 21:15:34.000000 funannotate-1.8.7/funannotate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-04-17 21:15:34.000000 funannotate-1.8.7/funannotate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-17 21:15:34.000000 funannotate-1.8.7/funannotate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-17 21:15:34.258609 funannotate-1.8.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3704 2021-04-17 21:15:25.000000 funannotate-1.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.743580 funannotate-1.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1322 2021-08-02 04:50:19.000000 funannotate-1.8.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2021-08-02 04:50:19.000000 funannotate-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4628 2021-08-02 04:50:33.743580 funannotate-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3470 2021-08-02 04:50:19.000000 funannotate-1.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.731580 funannotate-1.8.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     9283 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/annotate.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    41605 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/compare.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7289 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/conda.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5192 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2771 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/databases.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3048 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3333 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/evidence.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/manual.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13142 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/predict.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4702 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12080 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4763 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/update.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5468 2021-08-02 04:50:19.000000 funannotate-1.8.9/docs/utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.735580 funannotate-1.8.9/funannotate/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    77901 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.739580 funannotate-1.8.9/funannotate/aux_scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6927 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/augustus_parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2661 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/enrichment_parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5716 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/fasta2agp.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    21217 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/filterGenemark.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5716 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/filterIntronsFindStrand.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)   144316 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/funannotate-BUSCO2-py2.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)   144417 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/funannotate-BUSCO2.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14956 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/funannotate-p2g.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    23181 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/funannotate-runEVM.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4623 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/genemark_gtf2gff3.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)      642 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/getEggNog.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7994 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/hmmer_parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14425 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/iprscan-local.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3206 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/iprscan2annotations.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    65930 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/pal2nal.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3842 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/phobius-multiproc.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    35348 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/phobius-remote.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15288 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/runIPRscan.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      389 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/sam2bam.sh
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9458 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/tbl2asn_parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8768 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/trinity.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5461 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/trnascan2gff3.pl
+-rwxr-xr-x   0 runner    (1001) docker     (121)      723 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/aux_scripts/xmlcombine.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    17100 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/check.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9393 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    59286 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.739580 funannotate-1.8.9/funannotate/config/
+-rw-r--r--   0 runner    (1001) docker     (121)   121918 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/EOG092C0B3U.prfl
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/TruSeq3-PE.fa
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/TruSeq3-SE.fa
+-rw-r--r--   0 runner    (1001) docker     (121)     3810 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/busco_test.fa
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/codeml.config
+-rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/extrinsic.E.XNT.RM.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    12708 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/smcogs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1523 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/test.sbt
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/config/tf_interpro.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2275 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4312 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/downloads.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7170 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/fix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33569 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/funannotate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.731580 funannotate-1.8.9/funannotate/html_template/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.739580 funannotate-1.8.9/funannotate/html_template/css/
+-rw-r--r--   0 runner    (1001) docker     (121)   121260 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/html_template/css/bootstrap.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (121)      291 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/html_template/css/starter-template.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.743580 funannotate-1.8.9/funannotate/html_template/js/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    36868 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/html_template/js/bootstrap.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2130 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/html_template/js/ie-emulation-modes-warning.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)      641 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/html_template/js/ie10-viewport-bug-workaround.js
+-rwxr-xr-x   0 runner    (1001) docker     (121)    95957 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/html_template/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)     8553 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/interlap.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      449 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/iprscan.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)   396617 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8910 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5091 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/outgroups.py
+-rw-r--r--   0 runner    (1001) docker     (121)   106444 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/predict.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    14874 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11244 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    31196 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/setupDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2836 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/sort.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6604 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/species.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12267 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/stackedBarGraph.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    18411 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    62088 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)   123934 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/update.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.743580 funannotate-1.8.9/funannotate/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      943 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/bam2gff3.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    51646 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/contrast.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1256 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/gbk2parts.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1597 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/gff2prot.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    18472 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/gff2tbl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2476 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/gff_reformat.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3210 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/quarry2gff3.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2213 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3977 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/stringtie2gff3.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7034 2021-08-02 04:50:19.000000 funannotate-1.8.9/funannotate/utilities/tbl2gbk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-02 04:50:33.735580 funannotate-1.8.9/funannotate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4628 2021-08-02 04:50:33.000000 funannotate-1.8.9/funannotate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3137 2021-08-02 04:50:33.000000 funannotate-1.8.9/funannotate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-02 04:50:33.000000 funannotate-1.8.9/funannotate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-08-02 04:50:33.000000 funannotate-1.8.9/funannotate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2021-08-02 04:50:33.000000 funannotate-1.8.9/funannotate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-08-02 04:50:33.000000 funannotate-1.8.9/funannotate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-02 04:50:33.743580 funannotate-1.8.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3704 2021-08-02 04:50:19.000000 funannotate-1.8.9/setup.py
```

### Comparing `funannotate-1.8.7/LICENSE.md` & `funannotate-1.8.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/PKG-INFO` & `funannotate-1.8.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funannotate
-Version: 1.8.7
+Version: 1.8.9
 Summary: funannotate: eukaryotic genome annotation pipeline
 Home-page: https://github.com/nextgenusfs/funannotate
 Author: Jon Palmer
 Author-email: nextgenusfs@gmail.com
 License: BSD-2
 Description: 
         [![Latest Github release](https://img.shields.io/github/release/nextgenusfs/funannotate.svg)](https://github.com/nextgenusfs/funannotate/releases/latest)
@@ -44,14 +44,22 @@
         conda config --add channels defaults
         conda config --add channels bioconda
         conda config --add channels conda-forge
         
         #then create environment
         conda create -n funannotate funannotate
         ```
+        If `conda` is taking forever to solve the environment, I would recommend giving [mamba](https://github.com/mamba-org/mamba) a try:
+        ```
+        #install mamba into base environment
+        conda install -n base mamba
+        
+        #then use mamba as drop in replacmeent
+        mamba create -n funannotate funannotate
+        ```
         
         If you want to use GeneMark-ES/ET you will need to install that manually following developers instructions:
         http://topaz.gatech.edu/GeneMark/license_download.cgi
         
         Note that you will need to change the shebang line for all perl scripts in GeneMark to use `/usr/bin/env perl`.
         You will then also need to add `gmes_petap.pl` to the $PATH or set the environmental variable $GENEMARK_PATH to the gmes_petap directory.
```

### Comparing `funannotate-1.8.7/README.md` & `funannotate-1.8.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -35,14 +35,22 @@
 conda config --add channels defaults
 conda config --add channels bioconda
 conda config --add channels conda-forge
 
 #then create environment
 conda create -n funannotate funannotate
 ```
+If `conda` is taking forever to solve the environment, I would recommend giving [mamba](https://github.com/mamba-org/mamba) a try:
+```
+#install mamba into base environment
+conda install -n base mamba
+
+#then use mamba as drop in replacmeent
+mamba create -n funannotate funannotate
+```
 
 If you want to use GeneMark-ES/ET you will need to install that manually following developers instructions:
 http://topaz.gatech.edu/GeneMark/license_download.cgi
 
 Note that you will need to change the shebang line for all perl scripts in GeneMark to use `/usr/bin/env perl`.
 You will then also need to add `gmes_petap.pl` to the $PATH or set the environmental variable $GENEMARK_PATH to the gmes_petap directory.
```

### Comparing `funannotate-1.8.7/docs/Makefile` & `funannotate-1.8.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/annotate.rst` & `funannotate-1.8.9/docs/annotate.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/commands.rst` & `funannotate-1.8.9/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/compare.rst` & `funannotate-1.8.9/docs/compare.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/conda.rst` & `funannotate-1.8.9/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/conf.py` & `funannotate-1.8.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/databases.rst` & `funannotate-1.8.9/docs/databases.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/dependencies.rst` & `funannotate-1.8.9/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/docker.rst` & `funannotate-1.8.9/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/evidence.rst` & `funannotate-1.8.9/docs/evidence.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/index.rst` & `funannotate-1.8.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/install.rst` & `funannotate-1.8.9/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     
     #setup bioconda repository
     conda config --add channels defaults
     conda config --add channels bioconda
     conda config --add channels conda-forge
     
     #then create environment
-    conda create -n funannotate python=2.7 funannotate
+    conda create -n funannotate funannotate
     
     
 Please setup database and test your installation locally using the following:
 
 .. code-block:: none
 	
 	#start up conda ENV
```

### Comparing `funannotate-1.8.7/docs/make.bat` & `funannotate-1.8.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/predict.rst` & `funannotate-1.8.9/docs/predict.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/prepare.rst` & `funannotate-1.8.9/docs/prepare.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     $ funannotate clean
 
 	Usage:       funannotate clean <arguments>
 	version:     1.7.0
 
 	Description: The script sorts contigs by size, starting with shortest contigs it uses minimap2
-				 to find contigs duplicated elsewhere, and then removes duplicated contigs.
+	             to find contigs duplicated elsewhere, and then removes duplicated contigs.
 	
 	Arguments:   
 	  -i, --input    Multi-fasta genome file (Required)
 	  -o, --out      Cleaned multi-fasta output file (Required)
 	  -p, --pident   Percent identity of overlap. Default = 95
 	  -c, --cov      Percent coverage of overlap. Default = 95
 	  -m, --minlen   Minimum length of contig to keep. Default = 500
@@ -37,16 +37,16 @@
 
     $funannotate sort
 
 	Usage:       funannotate sort <arguments>
 	version:     1.7.0
 
 	Description: This script sorts the input contigs by size (longest->shortest) and then relabels
-				 the contigs with a simple name (e.g. scaffold_1).  Augustus can have problems with
-				 some complicated contig names.
+	             the contigs with a simple name (e.g. scaffold_1).  Augustus can have problems with
+		     some complicated contig names.
 	
 	Arguments:   
 	  -i, --input    Multi-fasta genome file. (Required)
 	  -o, --out      Sorted by size and relabeled output file. (Required)
 	  -b, --base     Base name to relabel contigs. Default: scaffold
 	  --minlen       Shorter contigs are discarded. Default: 0
 
@@ -58,25 +58,26 @@
 This is an essential step in the annotation process. As of v1.4.0 repeatmasking has been decoupled from :code:`funannotate predict` in order to make it more flexible and accomodate those users that don't have access to the RepBase library (a requirement of RepeatMasker). The :code:`funannotate mask` command default is to run simple masking using tantan.  The script is a wrapper for RepeatModeler and RepeatMasker, however you can use any external program to softmask your assembly.  Softmasking is where repeats are represented by lowercase letters and all non-repetitive regions are uppercase letters. One alternative to RepeatMasker is RED (REpeat Detector) you can find a wrapper for this program `Redmask <https://github.com/nextgenusfs/redmask>`_.
 
 .. code-block:: none
     
     $funannotate mask
     
 	Usage:       funannotate mask <arguments>
-	version:     1.7.0
+	version:     1.8.6
 
 	Description: This script is a wrapper for repeat masking. Default is to run very simple
-				 repeat masking with tantan. The script can also run RepeatMasker and/or 
-				 RepeatModeler. It will generate a softmasked genome. Tantan is probably not
-				 sufficient for soft-masking an assembly, but with RepBase no longer being
-				 available RepeatMasker/Modeler may not be functional for many users.
-	
-	Arguments:   
-	  -i, --input                    Multi-FASTA genome file. (Required)
-	  -o, --out                      Output softmasked FASTA file. (Required)
+		     repeat masking with tantan. The script can also run RepeatMasker and/or
+		     RepeatModeler. It will generate a softmasked genome. Tantan is probably not
+		     sufficient for soft-masking an assembly, but with RepBase no longer being
+		     available RepeatMasker/Modeler may not be functional for many users.
+
+	Arguments:
+	  -i, --input                  Multi-FASTA genome file. (Required)
+	  -o, --out                    Output softmasked FASTA file. (Required)
 
 	Optional:
-	  -m, --method                   Method to use. Default: tantan [repeatmasker, repeatmodeler]
-	  -s, --repeatmasker_species     Species to use for RepeatMasker
-	  -l, --repeatmodeler_lib        Custom repeat database (FASTA format)
-	  --cpus                         Number of cpus to use. Default: 2
-	  --debug                        Keep intermediate files
+	  -m, --method                 Method to use. Default: tantan [repeatmasker, repeatmodeler]
+	  -s, --repeatmasker_species   Species to use for RepeatMasker
+	  -l, --repeatmodeler_lib      Custom repeat database (FASTA format)
+	  --cpus                       Number of cpus to use. Default: 2
+	  --debug                      Keep intermediate files
+
```

### Comparing `funannotate-1.8.7/docs/tutorials.rst` & `funannotate-1.8.9/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/update.rst` & `funannotate-1.8.9/docs/update.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/docs/utilities.rst` & `funannotate-1.8.9/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/annotate.py` & `funannotate-1.8.9/funannotate/annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 import funannotate.library as lib
+from funannotate.aux_scripts.fasta2agp import parse_scaffolds_makeagp
 import sys
 import os
 import subprocess
 import shutil
 import argparse
 import re
 from natsort import natsorted
@@ -180,68 +181,89 @@
     '''
     IDi, DBi, OGi, Genei, COGi, Desci, ECi = (None,)*7
     with open(input, 'r') as infile:
         for line in infile:
             if line.startswith('#query'):  # this is HEADER
                 line = line.rstrip()
                 headerCols = line.split('\t')
-                IDi = 0
+                IDi = item2index(headerCols, '#query')
                 Genei = item2index(headerCols, 'Preferred_name')
                 DBi = item2index(headerCols, 'eggNOG OGs')
                 OGi = item2index(headerCols, 'best_og_name')
                 COGi = item2index(headerCols, 'best_og_cat')
                 Desci = item2index(headerCols, 'best_og_desc')
                 ECi = item2index(headerCols, 'EC')
                 break
-    if not IDi:  # then no header file, so have to guess
-        IDi, DBi, OGi, Genei, COGi, Desci, ECi = (0, 4, 8, 11, 9, 10, 13)
+    return IDi, DBi, OGi, Genei, COGi, Desci, ECi
+
+def getEggNogHeadersv212(input):
+    '''
+    function to get the headers from eggnog mapper annotations
+    '''
+    IDi, DBi, OGi, Genei, COGi, Desci, ECi = (None,)*7
+    with open(input, 'r') as infile:
+        for line in infile:
+            if line.startswith('#query'):  # this is HEADER
+                line = line.rstrip()
+                headerCols = line.split('\t')
+                IDi = item2index(headerCols, '#query')
+                Genei = item2index(headerCols, 'Preferred_name')
+                DBi = item2index(headerCols, 'eggNOG_OGs')
+                OGi = item2index(headerCols, 'max_annot_lvl')
+                COGi = item2index(headerCols, 'COG_category')
+                Desci = item2index(headerCols, 'Description')
+                ECi = item2index(headerCols, 'EC')
+                break
     return IDi, DBi, OGi, Genei, COGi, Desci, ECi
 
 def parseEggNoggMapper(input, output, GeneDict):
     # try to parse header
     version, prefix = getEggnogVersion(input)
+    lib.log.info('EggNog version parsed as {}'.format(version))
     if version and version > ('2.0.0') and version < ('2.0.5'):
         lib.log.error('Unable to parse emapper results from v{}, please use either v1.0.3 or >=v2.0.5'.format(version))
         return {}
     if not prefix:  # we have to guess here, sorry
         prefix = 'ENOG50'
     if not version:  # also then we guess
         version = '2.1.0'
     lib.log.debug('EggNog annotation detected as emapper v{} and DB prefix {}'.format(version, prefix))
     Definitions = {}
     # indexes from header file
     if version < ('2.0.0'):
         IDi, DBi, OGi, Genei, COGi, Desci, ECi = getEggNogHeaders(input)
-    else:
+    elif version < ('2.1.2'):
         IDi, DBi, OGi, Genei, COGi, Desci, ECi = getEggNogHeadersv2(input)
+    else:
+        IDi, DBi, OGi, Genei, COGi, Desci, ECi = getEggNogHeadersv212(input)
     # take annotations file from eggnog-mapper and create annotations
     with open(output, 'w') as out:
         with open(input, 'r') as infile:
             for line in infile:
                 line = line.replace('\n', '')
                 if line.startswith('#'):
                     continue
                 cols = line.split('\t')
                 cols = ['' if x=='-' else x for x in cols]
                 ID = cols[IDi]
                 Description = cols[Desci].split('. ')[0]
                 Gene = ''
-                if cols[Genei] != '':
+                if cols[Genei] not in ['', '-']:
                     if not '_' in cols[Genei] and not '.' in cols[Genei] and number_present(cols[Genei]) and len(cols[Genei]) > 2 and not morethanXnumbers(cols[Genei], 3):
                         Gene = cols[Genei]
                 if version < ('2.0.0'):
                     EC = None
                     DB = cols[DBi].split('[')[0]
                     OGs = cols[OGi].split(',')
                     NOG = ''
                     for x in OGs:
                         if DB in x:
                             NOG = prefix + x.split('@')[0]
                     COGs = cols[COGi].replace(' ', '')
-                else:  # means we have v2 or great
+                elif version < ('2.1.2'):  # means we have v2 or great
                     try:
                         NOG, DB = cols[OGi].split('@')
                     except ValueError:  # means either 0 or more than 1 "best_OG" drop for now
                         lib.log.debug("EggNog Parse ERROR: {}".format(line))
                         continue
                     OGs = cols[DBi].split(',')
                     if NOG == 'seed_ortholog': # not sure if this is bug, but get second to last OG from all
@@ -250,21 +272,38 @@
                     NOG = prefix+NOG
                     EC = cols[ECi]
                     if ',' in EC: # this is least common ancestor approach
                         EC = os.path.commonprefix(EC.split(',')).rstrip('.')
                     COGs = cols[COGi].replace(' ', '')
                     if len(COGs) > 1:
                         COGs = ''.join([c + ',' for c in COGs]).rstrip(',')
-
+                else:
+                    DB = cols[OGi]
+                    EC = cols[ECi]
+                    if ',' in EC: # this is least common ancestor approach
+                        EC = os.path.commonprefix(EC.split(',')).rstrip('.')
+                    NOG = ''
+                    OGs = cols[DBi].split(',')
+                    for ogx in OGs:
+                        nog_acc, taxname = ogx.split('@')
+                        if taxname == DB:
+                            NOG = nog_acc
+                    NOG = prefix+NOG
+                    COGs = cols[COGi].replace(' ', '')
+                    if len(COGs) > 1:
+                       COGs = ''.join([c + ',' for c in COGs]).rstrip(',')
+                #print(line)
+                #print(ID, Gene, Description, DB, EC, NOG, COGs)
                 if EC and EC != '':
                     out.write("%s\tEC_number\t%s\n" % (ID, EC))
                 if NOG == '':
                     continue
                 if not NOG in Definitions:
                     Definitions[NOG] = Description
+
                 out.write("%s\tnote\tEggNog:%s\n" % (ID, NOG))
                 if COGs != '':
                     out.write("%s\tnote\tCOG:%s\n" % (ID, COGs))
                 if Gene != '':
                     product = Gene.lower()+'p'
                     product = capfirst(product)
                     GeneID = ID
@@ -1295,18 +1334,21 @@
     lib.annotation_summary(Scaffolds, final_stats, tbl=final_tbl,
                            previous=existingStats, database=FUNDB,
                            command=' '.join(sys.argv),
                            organism=organism_name)
 
     # write AGP output so all files in correct directory
     lib.log.info("Creating AGP file and corresponding contigs file")
-    agp2fasta = os.path.join(parentdir, 'aux_scripts', 'fasta2agp.pl')
-    AGP = os.path.join(ResultsFolder, organism_name+'.agp')
-    cmd = ['perl', agp2fasta, organism_name+'.scaffolds.fa']
-    lib.runSubprocess2(cmd, ResultsFolder, lib.log, AGP)
+    # no reason to use suprocess here, we should be able to import and run
+    #agp2fasta = os.path.join(parentdir, 'aux_scripts', 'fasta2agp.py')
+    agp_final = os.path.join(ResultsFolder, organism_name+'.agp')
+    agp_contigs = os.path.join(ResultsFolder, organism_name+'.contigs.fsa')
+    parse_scaffolds_makeagp(final_fasta, agp_final, agp_contigs)
+    #cmd = ['python', agp2fasta, organism_name+'.scaffolds.fa',AGP]
+    #lib.runSubprocess(cmd, ResultsFolder, lib.log)
 
     # write secondary metabolite clusters output using the final genome in gbk format
     if lib.checkannotations(antismash_input):
         lib.log.info(
             "Cross referencing SM cluster hits with MIBiG database version %s" % versDB.get('mibig'))
         # do a blast best hit search against MIBiG database for cluster annotation, but looping through gene cluster hits
         AllProts = []
```

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/augustus_parallel.py` & `funannotate-1.8.9/funannotate/aux_scripts/augustus_parallel.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/enrichment_parallel.py` & `funannotate-1.8.9/funannotate/aux_scripts/enrichment_parallel.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/filterGenemark.pl` & `funannotate-1.8.9/funannotate/aux_scripts/filterGenemark.pl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/filterIntronsFindStrand.pl` & `funannotate-1.8.9/funannotate/aux_scripts/filterIntronsFindStrand.pl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/funannotate-BUSCO2-py2.py` & `funannotate-1.8.9/funannotate/aux_scripts/funannotate-BUSCO2-py2.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/funannotate-BUSCO2.py` & `funannotate-1.8.9/funannotate/aux_scripts/funannotate-BUSCO2.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/funannotate-p2g.py` & `funannotate-1.8.9/funannotate/aux_scripts/funannotate-p2g.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/funannotate-runEVM.py` & `funannotate-1.8.9/funannotate/aux_scripts/funannotate-runEVM.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
 def create_partitions(fasta, genes, partition_list, proteins=False,
                       transcripts=False, repeats=False, num=50,
                       tmpdir='.', interval=2000, partitions=True,
                       debug=False):
     # function to create EVM partition intervals that do not split genes
     if not os.path.isdir(tmpdir):
         os.makedirs(tmpdir)
-    SeqRecords = SeqIO.index(fasta, 'fasta')
+    f_idx = fasta + ".idx"
+    SeqRecords = SeqIO.index_db(f_idx, fasta, 'fasta')
     PID = os.getpid()
     bedGenes = os.path.join(tmpdir, 'genes.{}.bed'.format(PID))
     superGenes = os.path.join(tmpdir, 'genes.{}.supergenes.bed'.format(PID))
     interGenes = gene_blocks_to_interlap(genes)
     if proteins:
         interProteins = exonerate_blocks_to_interlap(proteins)
     if transcripts:
@@ -193,58 +194,58 @@
                 totalGeneCount, superGeneCount))
         # parse Results and get coordinates to partitions
         Partitions = {}
         Commands = {}
         for k, v in natsorted(merged.items()):
             if not k in ChrGeneCounts:  # no genes, so can safely skip
                 continue
-            #print(k)
-            #solve_partitions(v, interval=interval)
             Partitions[k] = []
             next_start = None
             if len(v) > num:
-                chunks = math.ceil(len(v)/num)
-                num_genes = int(round(len(v)/chunks))
-                chunks = int(chunks)
-                for i in range(chunks):
-                    if k in Commands:
-                        continue
-                    i = i+1
-                    if i == 1:
-                        start = 1
-                    else:
-                        start = next_start
-                    loc = i*num_genes
-                    if i == chunks:
-                        end = len(SeqRecords[k])
-                    else:
-                        if loc >= len(v):
+                if not any(z >= interval for z in [w[2] for w in v]):  # this means there no intervals on this contig
+                    Commands[k] = {'n': len(v)}
+                    lib.log.debug('{} --> {} bp'.format(k, len(SeqRecords[k])))
+                else:
+                    chunks = math.ceil(len(v)/num)
+                    num_genes = int(round(len(v)/chunks))
+                    chunks = int(chunks)
+                    for i in range(chunks):
+                        if k in Commands:
+                            continue
+                        i = i+1
+                        if i == 1:
+                            start = 1
+                        else:
+                            start = next_start
+                        loc = i*num_genes
+                        if i == chunks:
                             end = len(SeqRecords[k])
                         else:
-                            # new function to return the tuple to split
-                            splitTup, idx = getBreakPoint(v, loc, direction='reverse', gap=interval)
-                            if not splitTup:
-                                splitTup, idx = getBreakPoint(v, loc, direction='forward', gap=interval)
-                            #print(Partitions[k])
-                            #print(k, start, splitTup)
-                            end = splitTup[0]-1
-                            next_start = v[idx-1][1]+1
-                    if not end:
-                        Commands[k] = {'n': len(v)}
-                        lib.log.debug('{} --> {} bp'.format(
-                            k, len(SeqRecords[k])))
-                    else:
-                        partLen = end-start
-                        if partLen < 10000:
-                            continue
-                        Partitions[k].append((start, end))
-                        partName = '{}_{}-{}'.format(k, start, end)
-                        Commands[partName] = {'n': num_genes, 'chr': k}
-                        lib.log.debug('{} --> {} bp'.format(partName, partLen))
-                    start, end = (None,)*2
+                            if loc >= len(v):
+                                end = len(SeqRecords[k])
+                            else:
+                                # new function to return the tuple to split
+                                splitTup, idx = getBreakPoint(v, loc, direction='reverse', gap=interval)
+                                if not splitTup:
+                                    splitTup, idx = getBreakPoint(v, loc, direction='forward', gap=interval)
+                                end = splitTup[0]-1
+                                next_start = v[idx-1][1]+1
+                        if not end:
+                            Commands[k] = {'n': len(v)}
+                            lib.log.debug('{} --> {} bp'.format(
+                                k, len(SeqRecords[k])))
+                        else:
+                            partLen = end-start
+                            if partLen < 10000:
+                                continue
+                            Partitions[k].append((start, end))
+                            partName = '{}_{}-{}'.format(k, start, end)
+                            Commands[partName] = {'n': num_genes, 'chr': k}
+                            lib.log.debug('{} --> {} bp'.format(partName, partLen))
+                        start, end = (None,)*2
             else:
                 Commands[k] = {'n': len(v)}
                 lib.log.debug('{} --> {} bp'.format(k, len(SeqRecords[k])))
         # now loop through partitions and write files for EVM
         with open(partition_list, 'w') as partout:
             for chr, p in natsorted(Partitions.items()):
                 chrDir = os.path.join(tmpdir, chr)
@@ -341,15 +342,15 @@
                                             os.path.basename(transcripts))
                     RangeFinder(interTranscripts, chr, 1, len(SeqRecords[chr]),
                                 tranPred)
                 if repeats:
                     repPred = os.path.join(chrDir, os.path.basename(repeats))
                     RangeFinder(interRepeats, chr, 1, len(SeqRecords[chr]),
                                 repPred)
-
+    SeqRecords.close()
     return Commands
 
 
 def RangeFinder(input, chr, start, end, output, EVM=False):
     '''
     if not EVM:
         EVM = os.environ['EVM_HOME']
@@ -382,15 +383,15 @@
     # takes list of tuples of coords and a starting index (idx). finds closest
     # break point in between tuple coordSorted
     solution = False
     while not solution:
         try:
             start, end, diff, num_genes = tupList[idx]
         except IndexError:
-            return False
+            return False, idx
         if diff >= gap:
             #phase = int(round(diff/2))
             solution = tupList[idx]
             #print(idx, tupList[idx])
         else:
             if direction == 'reverse':
                 idx -= 1
```

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/genemark_gtf2gff3.pl` & `funannotate-1.8.9/funannotate/aux_scripts/genemark_gtf2gff3.pl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/getEggNog.sh` & `funannotate-1.8.9/funannotate/aux_scripts/getEggNog.sh`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/hmmer_parallel.py` & `funannotate-1.8.9/funannotate/aux_scripts/hmmer_parallel.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/iprscan-local.py` & `funannotate-1.8.9/funannotate/aux_scripts/iprscan-local.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/iprscan2annotations.py` & `funannotate-1.8.9/funannotate/aux_scripts/iprscan2annotations.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/pal2nal.pl` & `funannotate-1.8.9/funannotate/aux_scripts/pal2nal.pl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/phobius-multiproc.py` & `funannotate-1.8.9/funannotate/aux_scripts/phobius-multiproc.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/phobius-remote.pl` & `funannotate-1.8.9/funannotate/aux_scripts/phobius-remote.pl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/runIPRscan.py` & `funannotate-1.8.9/funannotate/aux_scripts/runIPRscan.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/tbl2asn_parallel.py` & `funannotate-1.8.9/funannotate/aux_scripts/tbl2asn_parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,19 +95,19 @@
     # make sure ouput that will be appended to is not there
     for file in [os.path.join(folder, 'genome.val'), os.path.join(folder, 'errorsummary.val'), os.path.join(folder, 'genome.gbf'), discrepency]:
         lib.SafeRemove(file)
     # get funannotate version
     fun_version = lib.get_version()
     # input should be a folder
     if not os.path.isdir(folder):
-        lib.log.error("tbl2asn error: %s is not a directory, exiting" % folder)
+        sys.stderr.write("tbl2asn error: %s is not a directory, exiting\n" % folder)
         sys.exit(1)
     # based on organism, isolate, strain, construct meta info for -j flag
     if not organism:
-        lib.log.error("tbl2asn error: organism not specified")
+        sys.stderr.write("tbl2asn error: organism not specified\n")
         sys.exit(1)
     meta = "[organism=" + organism + "]"
     if isolate:
         isolate_meta = "[isolate=" + isolate + "]"
         meta = meta + " " + isolate_meta
     if strain:
         strain_meta = "[strain=" + strain + "]"
```

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/trinity.py` & `funannotate-1.8.9/funannotate/aux_scripts/trinity.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/trnascan2gff3.pl` & `funannotate-1.8.9/funannotate/aux_scripts/trnascan2gff3.pl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/aux_scripts/xmlcombine.py` & `funannotate-1.8.9/funannotate/aux_scripts/xmlcombine.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/check.py` & `funannotate-1.8.9/funannotate/check.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/clean.py` & `funannotate-1.8.9/funannotate/clean.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
                         print_function, unicode_literals)
 
 import sys
 import os
 import subprocess
 import argparse
 import signal
+import uuid
+import shutil
 from multiprocessing import Pool
 from Bio.SeqIO.FastaIO import SimpleFastaParser
 from funannotate.library import CheckDependencies, softwrap, countfasta
 
 
 def calcN50(input):
     lengths = []
@@ -29,40 +31,60 @@
     else:
         medianpos = int(len(nlist) / 2)
         N50 = int(nlist[medianpos])
     return N50
 
 
 def Sortbysize(input, n50, minlen=500):
+    IUPAC = {'A', 'C', 'G', 'T', 'R', 'Y',
+             'S', 'W', 'K', 'M', 'B', 'D',
+             'H', 'V', 'N'}
     contigs = []
     keep = []
     Seqs = []
+    bad = []
     with open(input, 'r') as infile:
         for header, sequence in SimpleFastaParser(infile):
+            characters = {}
+            for nuc in sequence:
+                nuc = nuc.upper()
+                if not nuc in characters:
+                    characters[nuc] = 1
+                else:
+                    characters[nuc] += 1
+            for c in characters.keys():
+                if not c in IUPAC:
+                    bad.append(header)
+                    print('ERROR: {} contains non-IUPAC [{}] character, removing'.format(header, c))
+            if len(characters) < 4:
+                bad.append(header)
+                print('ERROR: {} contains only {} nucleotides, removing'.format(header, len(characters)))
             Seqs.append((header, len(sequence)))
     # sort by length
     sortedSeqs = sorted(Seqs, key=lambda x: x[1], reverse=True)
     # loop through and return contigs and keepers
     for name, length in sortedSeqs:
+        if name in bad:
+            continue
         if length >= minlen:
             if n50:
                 if length >= n50:
                     keep.append(name)
                 else:
                     contigs.append(name)
             else:
                 contigs.append(name)
     return contigs, keep
 
 
 def generateFastas(input, index, Contigs, query):
     # loop through fasta once, generating query and reference
     contiglist = Contigs[index+1:] + keepers
-    with open('query_{}.fa'.format(index), 'w') as qFasta:
-        with open('reference_{}.fa'.format(index), 'w') as rFasta:
+    with open(os.path.join(tmpdir, 'query_{}.fa'.format(index)), 'w') as qFasta:
+        with open(os.path.join(tmpdir, 'reference_{}.fa'.format(index)), 'w') as rFasta:
             with open(input, 'r') as infile:
                 for Id, Sequence in SimpleFastaParser(infile):
                     if Id == query:
                         qFasta.write('>%s\n%s\n' % (Id, softwrap(Sequence)))
                     elif Id in contiglist:
                         rFasta.write('>%s\n%s\n' % (Id, softwrap(Sequence)))
 
@@ -94,18 +116,19 @@
     os.remove(minitmp)
     return (output, garbage)
 
 
 def align_contigs(mp_args):
     scaffolds, i = mp_args
     generateFastas(GENOME, i, scaffolds, scaffolds[i])
-    out = runMinimap2('query_{}.fa'.format(i), 'reference_{}.fa'.format(
-        i), scaffolds[i], i, min_pident=PIDENT, min_cov=COV)
-    os.remove('query_{}.fa'.format(i))
-    os.remove('reference_{}.fa'.format(i))
+    out = runMinimap2(os.path.join(tmpdir, 'query_{}.fa'.format(i)),
+                      os.path.join(tmpdir, 'reference_{}.fa'.format(i)),
+                      scaffolds[i], i, min_pident=PIDENT, min_cov=COV)
+    os.remove(os.path.join(tmpdir, 'query_{}.fa'.format(i)))
+    os.remove(os.path.join(tmpdir, 'reference_{}.fa'.format(i)))
     return out
 
 
 def multithread_aligning(scaffolds):
     original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
     p = Pool(CPUS)
     signal.signal(signal.SIGINT, original_sigint_handler)
@@ -138,28 +161,38 @@
                         default=95, help='percent identity of contig')
     parser.add_argument('-c', '--cov', type=int,
                         default=95, help='coverage of contig')
     parser.add_argument('-m', '--minlen', type=int,
                         default=500, help='Minimum length of contig')
     parser.add_argument('--cpus', default=2, type=int,
                         help='Number of CPUs to use')
+    parser.add_argument('--tmpdir',
+                        help='TMP directory to use')
     parser.add_argument('--exhaustive', action='store_true',
                         help='Compute every contig, else stop at N50')
     parser.add_argument('--debug', action='store_true',
                         help='Debug the output')
     args = parser.parse_args(args)
 
     # setup some global variables used in functions above
-    global GENOME, CPUS, PIDENT, COV, keepers, repeats
+    global GENOME, CPUS, PIDENT, COV, keepers, repeats, tmpdir
     GENOME = args.input
     CPUS = args.cpus
     PIDENT = args.pident
     COV = args.cov
     keepers, repeats = ([],)*2
 
+    # write in a tmpdir
+    if args.tmpdir:
+        tmpdir = args.tmpdir
+    else:
+        tmpdir = 'clean_{}'.format(str(uuid.uuid4()))
+    if not os.path.isdir(tmpdir):
+        os.makedirs(tmpdir)
+
     # run some checks of dependencies first
     programs = ['minimap2']
     CheckDependencies(programs)
 
     # calculate N50 of assembly
     n50 = calcN50(args.input)
 
@@ -199,10 +232,12 @@
     # finally write a new reference based on list of keepers
     with open(args.out, 'w') as output:
         with open(args.input, 'r') as input:
             for title, sequence in SimpleFastaParser(input):
                 if title in keepers:
                     output.write('>{}\n{}\n'.format(title, softwrap(sequence)))
 
+    shutil.rmtree(tmpdir)
+
 
 if __name__ == "__main__":
     main(sys.argv[1:])
```

### Comparing `funannotate-1.8.7/funannotate/compare.py` & `funannotate-1.8.9/funannotate/compare.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/EOG092C0B3U.prfl` & `funannotate-1.8.9/funannotate/config/EOG092C0B3U.prfl`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/busco_test.fa` & `funannotate-1.8.9/funannotate/config/busco_test.fa`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/codeml.config` & `funannotate-1.8.9/funannotate/config/codeml.config`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/extrinsic.E.XNT.RM.cfg` & `funannotate-1.8.9/funannotate/config/extrinsic.E.XNT.RM.cfg`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/smcogs.txt` & `funannotate-1.8.9/funannotate/config/smcogs.txt`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/test.sbt` & `funannotate-1.8.9/funannotate/config/test.sbt`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/config/tf_interpro.txt` & `funannotate-1.8.9/funannotate/config/tf_interpro.txt`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/database.py` & `funannotate-1.8.9/funannotate/database.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/downloads.json` & `funannotate-1.8.9/funannotate/downloads.json`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/fix.py` & `funannotate-1.8.9/funannotate/fix.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/funannotate.py` & `funannotate-1.8.9/funannotate/funannotate.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/html_template/css/bootstrap.min.css` & `funannotate-1.8.9/funannotate/html_template/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/html_template/js/bootstrap.min.js` & `funannotate-1.8.9/funannotate/html_template/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/html_template/js/ie-emulation-modes-warning.js` & `funannotate-1.8.9/funannotate/html_template/js/ie-emulation-modes-warning.js`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/html_template/js/ie10-viewport-bug-workaround.js` & `funannotate-1.8.9/funannotate/html_template/js/ie10-viewport-bug-workaround.js`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/html_template/js/jquery.min.js` & `funannotate-1.8.9/funannotate/html_template/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/interlap.py` & `funannotate-1.8.9/funannotate/interlap.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/library.py` & `funannotate-1.8.9/funannotate/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -2888,14 +2888,16 @@
                                          'partialStart': fivepartial,
                                          'partialStop': threepartial,
                                          'pseudo': False
                                          }
     # now we need to sort coordinates, get protein/transcript sequences and capture UTRs
     SeqRecords = SeqIO.to_dict(SeqIO.parse(fasta, 'fasta'))
     for k, v in list(Genes.items()):
+        # @nextgenusfs we should clarify or rename this variable to indicate
+        # i is the i-th transcript, right??
         for i in range(0, len(v['ids'])):
             if v['type'] in ['mRNA', 'tRNA', 'ncRNA']:
                 if v['strand'] == '+':
                     sortedExons = sorted(v['mRNA'][i], key=lambda tup: tup[0])
                 else:
                     sortedExons = sorted(v['mRNA'][i], key=lambda tup: tup[0],
                                          reverse=True)
@@ -2904,20 +2906,36 @@
                 Genes[k]['transcript'].append(mrnaSeq)
             if v['type'] == 'mRNA':
                 if v['strand'] == '+':
                     sortedCDS = sorted(v['CDS'][i], key=lambda tup: tup[0])
                 else:
                     sortedCDS = sorted(v['CDS'][i], key=lambda tup: tup[0],
                                        reverse=True)
-                # get the codon_start by getting first CDS phase + 1
+
                 cdsSeq = getSeqRegions(SeqRecords, v['contig'], sortedCDS)
+                # If the translation starts in middle of a codon,
+                # we need to truncate the CDS seq either at start or end
+                # depending on strand.
+                if v['codon_start'][i] > 1:
+                    if v['strand'] == "+":
+                        # drop first N bases based on codon_start
+                        # to reflect the translation frame
+                        cdsSeq = cdsSeq[v['codon_start'][i]-1:]
+                    elif v['strand'] == "-":
+                        # drop last N bases based on codon_start
+                        # to reflect the translation frame (because this is
+                        # is reverse strand gene)
+                        endTrunc = len(cdsSeq) - (v['codon_start'][i] - 1)
+                        cdsSeq = cdsSeq[0:endTrunc]
+                    else:
+                        # could trigger more of a warning/error
+                        print("ERROR strand (%s) is nonsensical for %s"%(v['strand'],k))
                 Genes[k]['cds_transcript'].append(cdsSeq)
                 Genes[k]['CDS'][i] = sortedCDS
-                protSeq, codon_start = (None,)*2
-                protSeq = translate(cdsSeq, v['strand'], v['codon_start'][i]-1)
+                protSeq = translate(cdsSeq, v['strand'],0)
                 if protSeq:
                     Genes[k]['protein'].append(protSeq)
                     if protSeq.endswith('*'):
                         Genes[k]['partialStop'][i] = False
                     else:
                         Genes[k]['partialStop'][i] = True
                     if v['codon_start'][i] == 1 and protSeq.startswith('M'):
@@ -4497,16 +4515,15 @@
                 else:
                     sortedCDS = sorted(v['CDS'][i], key=lambda tup: tup[0], reverse=True)
                 #get the codon_start by getting first CDS phase + 1
                 indexStart = [x for x, y in enumerate(v['CDS'][i]) if y[0] == sortedCDS[0][0]]
                 cdsSeq = getSeqRegions(SeqRecords, v['contig'], sortedCDS)
                 if gap_filter:
                     cdsSeq, v['CDS'][i] = start_end_gap(cdsSeq, v['CDS'][i])
-                Genes[k]['cds_transcript'].append(cdsSeq)
-                Genes[k]['CDS'][i] = sortedCDS
+
                 protSeq, codon_start = (None,)*2
                 try:
                     currentphase = v['phase'][i]
                 except IndexError:
                     pass
                 if '?' in v['phase'][i]: #dont know the phase -- malformed GFF3, try to find best CDS
                     translateResults = []
@@ -4526,14 +4543,24 @@
                     try:
                         codon_start = int(v['phase'][i][indexStart[0]]) + 1
                     except IndexError:
                         pass
                     #translate and get protein sequence
                     protSeq = translate(cdsSeq, v['strand'], codon_start-1)
                 Genes[k]['codon_start'][i] = codon_start
+                if codon_start > 1:
+                    if v['strand'] == '+':
+                        cdsSeq = cdsSeq[codon_start - 1:]
+                    elif v['strand'] == '-':
+                        endTrunc = len(cdsSeq) - codon_start -1
+                        cdsSeq = cdsSeq[0:endTrunc]
+                    else:
+                        print("ERROR nonsensical strand (%s) for gene %s"%([v['strand'],k]))
+                Genes[k]['cds_transcript'].append(cdsSeq)
+                Genes[k]['CDS'][i] = sortedCDS
                 v['protein'].append(protSeq)
                 if protSeq:
                     if protSeq.endswith('*'):
                         v['partialStop'][i] = False
                     else:
                         v['partialStop'][i] = True
                     if v['codon_start'][i] == 1 and v['protein'][i].startswith('M'):
@@ -6269,33 +6296,46 @@
         mrnaSeq = getSeqRegions(SeqRecords, v['contig'], sortedExons)
         Genes[k]['transcript'].append(mrnaSeq)
 
         # get the codon_start by getting first CDS phase + 1
         indexStart = [x for x, y in enumerate(
             v['CDS'][i]) if y[0] == sortedCDS[0][0]]
         cdsSeq = getSeqRegions(SeqRecords, v['contig'], sortedCDS)
-        Genes[k]['cds_transcript'].append(cdsSeq)
+        # this seems to be missing removal of codon_start overhang?
+
         Genes[k]['CDS'][i] = sortedCDS
-        protSeq, codon_start = (None,)*2
+
+        protSeq,codon_start = (None,)*2
+
         if '?' in v['phase'][i]:  # dont know the phase -- malformed GFF3, try to find best CDS
             translateResults = []
             for y in [1, 2, 3]:
                 protSeq = translate(cdsSeq, v['strand'], y-1)
                 numStops = protSeq.count('*')
                 if protSeq[-1] == '*':
                     numStops -= 1
                 translateResults.append((y, numStops, protSeq))
             sortedResults = sorted(translateResults, key=lambda tup: tup[1])
             codon_start = sortedResults[0][0]
             protSeq = sortedResults[0][2]
         else:
             codon_start = int(v['phase'][i][indexStart[0]]) + 1
             # translate and get protein sequence
+            cdsSeq  = cdsSeq[codon_start-1:]
             protSeq = translate(cdsSeq, v['strand'], codon_start-1)
         Genes[k]['codon_start'][i] = codon_start
+        if codon_start > 1:
+            if v['strand'] == '+':
+                cdsSeq = cdsSeq[codon_start - 1:]
+            elif v['strand'] == '-':
+                endTrunc = len(cdsSeq) - codon_start -1
+                cdsSeq = cdsSeq[0:endTrunc]
+            else:
+                print("ERROR nonsensical strand (%s) for gene %s"%([v['strand'],k]))
+        Genes[k]['cds_transcript'].append(cdsSeq)
         if protSeq:
             Genes[k]['protein'].append(protSeq)
             if protSeq.endswith('*'):
                 Genes[k]['partialStop'][i] = False
             else:
                 Genes[k]['partialStop'][i] = True
             if codon_start == 1 and protSeq.startswith('M'):
@@ -6760,14 +6800,25 @@
                                     if not line.startswith('\n'):
                                         out2.write('%s' % (line))
                             else:
                                 for line in gene_model:
                                     # remove the Name attribute as it sticks around in GBK file
                                     line = re.sub(';Name=.*$', ';', line)
                                     out.write('%s' % (line))
+    else:  # if nothing to remove, just print out GFF
+        with open(output, 'w') as out:
+            with open(gff, 'r') as GFF:
+                for line in GFF:
+                    if '\tstart_codon\t' in line:
+                        continue
+                    if '\tstop_codon\t' in line:
+                        continue
+                    # remove the Name attribute as it sticks around in GBK file
+                    line = re.sub(';Name=.*$', ';', line)
+                    out.write(line)
 
 
 def CleantRNAtbl(GFF, TBL, output):
     # clean up genbank tbl file from gag output
     # try to read through GFF file, make dictionary of tRNA genes and products
     TRNA = {}
     matches = []
```

### Comparing `funannotate-1.8.7/funannotate/mask.py` & `funannotate-1.8.9/funannotate/mask.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/outgroups.py` & `funannotate-1.8.9/funannotate/outgroups.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/predict.py` & `funannotate-1.8.9/funannotate/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,21 +568,23 @@
         lib.log.info('Skipping CodingQuarry as no --rna_bam passed')
     else:
         lib.log.info('Skipping CodingQuarry as $QUARRY_PATH not found as ENV')
 
     # let user know what will be run and from what source
     lib.log.debug(RunModes)
     RunBusco = False
-    lib.log.info(
-        'Parsed training data, run ab-initio gene predictors as follows:')
+    AllPretrained = True
+    lib.log.info('Parsed training data, run ab-initio gene predictors as follows:')
     AbInitio = [['Program', 'Training-Method']]
     for k, v in natsorted(list(RunModes.items())):
         AbInitio.append([k, v])
         if 'busco' == v:
             RunBusco = True
+        if v != 'pretrained':
+            AllPretrained = False
     abinitio_table = lib.print_table(AbInitio, return_str=True)
     sys.stderr.write(abinitio_table)
     if 'QUARRY_PATH' in os.environ and not 'codingquarry' in RunModes and StartWeights['codingquarry'] > 0:
         lib.log.info(
             'CodingQuarry will be skipped --> --rna_bam required for training')
         StartWeights['codingquarry'] = 0
 
@@ -1351,45 +1353,46 @@
                                busco_final)
                 total = lib.countGFFgenes(busco_final)
                 lib.log.info('{:,} BUSCO predictions validated'.format(total))
             else:
                 lib.log.info("Existing BUSCO results found: {:} containing {:,} predictions".format(
                     busco_final, lib.countGFFgenes(busco_final)))
             FinalTrainingModels = busco_final
-
+        elif args.pasa_gff:
+            # check for training data, if no training data, then train using PASA
+            lib.log.info("Filtering PASA data for suitable training set")
+            trainingModels = os.path.join(args.out, 'predict_misc', 'pasa.training.tmp.gtf')
+            # convert PASA GFF to GTF format
+            lib.gff3_to_gtf(PASA_GFF, MaskGenome, trainingModels)
+            # now get best models by cross-ref with intron BAM hints
+            if lib.which('filterGenemark.pl'):
+                FILTERGENE = 'filterGenemark.pl'
+            else:
+                FILTERGENE = os.path.join(parentdir, 'aux_scripts', 'filterGenemark.pl')
+            cmd = [FILTERGENE, os.path.abspath(trainingModels),
+                    os.path.abspath(hints_all)]
+            lib.runSubprocess4(cmd, os.path.join(args.out, 'predict_misc'), lib.log)
+            totalTrain = lib.selectTrainingModels(PASA_GFF,
+                                                  MaskGenome,
+                                                  os.path.join(args.out, 'predict_misc', 'pasa.training.tmp.f.good.gtf'),
+                                                  FinalTrainingModels)
+        else:  # unable to get training models
+            if not AllPretrained:
+                lib.log.error('RunBusco is set to False and args.pasa_gff is None --> cannot generate training set. If you are reading this it is a bug, please report.')
+                sys.exit(1)
         ######################
         #     Augustus       #
         ######################
         aug_out = os.path.join(args.out, 'predict_misc', 'augustus.gff3')
         if args.augustus_gff:
             aug_out = args.augustus_gff
         else:
             if not lib.checkannotations(aug_out):
-                if args.pasa_gff and RunModes['augustus'] == 'pasa':
-                    # check for training data, if no training data, then train using PASA
-                    lib.log.info("Filtering PASA data for suitable training set")
-                    trainingModels = os.path.join(args.out, 'predict_misc', 'pasa.training.tmp.gtf')
-                    # convert PASA GFF to GTF format
-                    lib.gff3_to_gtf(PASA_GFF, MaskGenome, trainingModels)
-                    # now get best models by cross-ref with intron BAM hints
-                    if lib.which('filterGenemark.pl'):
-                        FILTERGENE = 'filterGenemark.pl'
-                    else:
-                        FILTERGENE = os.path.join(parentdir, 'aux_scripts', 'filterGenemark.pl')
-                    cmd = [FILTERGENE, os.path.abspath(trainingModels),
-                           os.path.abspath(hints_all)]
-                    lib.runSubprocess4(cmd,
-                                       os.path.join(args.out, 'predict_misc'),
-                                       lib.log)
-                    totalTrain = lib.selectTrainingModels(PASA_GFF,
-                                                          MaskGenome,
-                                                          os.path.join(args.out, 'predict_misc', 'pasa.training.tmp.f.good.gtf'),
-                                                          FinalTrainingModels)
-                elif RunModes['augustus'] == 'busco':
-                    totalTrain = lib.countGFFgenes(FinalTrainingModels)
+                # ensure we have a count of gene models
+                totalTrain = lib.countGFFgenes(FinalTrainingModels)
 
                 if RunModes['augustus'] != 'pretrained':
                     # now train augustus
                     if totalTrain < int(args.min_training_models):
                         lib.log.error("Not enough gene models {:} to train Augustus ({:} required), exiting".format(
                             totalTrain, int(args.min_training_models)))
                         sys.exit(1)
@@ -1543,36 +1546,33 @@
                         checkQuarry = lib.runCodingQuarryTrained(MaskGenome, aug_species, os.path.join(
                             args.out, 'predict_misc', 'CodingQuarry'), args.cpus, Quarry)
                         if not checkQuarry:
                             Quarry = False
                     else:
                         Quarry = False
             else:
-                lib.log.info(
-                    'Using existing CodingQuarry results: {:}'.format(Quarry))
+                lib.log.info('Using existing CodingQuarry results: {:}'.format(Quarry))
         else:
             Quarry = False
 
         # report gene numbers
         if Quarry:
             cqCount = lib.countGFFgenes(Quarry)
             lib.log.info('{:,} predictions from CodingQuarry'.format(cqCount))
             if os.path.isdir(os.path.join(args.out, 'predict_misc', 'CodingQuarry', 'ParameterFiles')):
                 lib.copyDirectory(os.path.join(args.out, 'predict_misc', 'CodingQuarry',
                                                'ParameterFiles'), os.path.join(LOCALPARAMETERS, 'codingquarry'))
         else:
             if StartWeights['codingquarry'] > 0:
-                lib.log.debug(
-                    'CodingQuarry failed, removing from training parameters')
+                lib.log.debug('CodingQuarry failed, removing from training parameters')
                 trainingData['codingquarry'] = [{}]
 
         # run snap prediction
         SNAP = False
-        SnapPredictions = os.path.join(
-            args.out, 'predict_misc', 'snap-predictions.gff3')
+        SnapPredictions = os.path.join(args.out, 'predict_misc', 'snap-predictions.gff3')
         if 'snap' in RunModes:
             if not lib.checkannotations(SnapPredictions):
                 if RunModes['snap'] == 'pretrained' and StartWeights['snap'] > 0 and os.path.isfile(os.path.join(LOCALPARAMETERS, aug_species+'.snap.hmm')):
                     lib.log.info(
                         'Running SNAP gene prediction, using pre-trained HMM profile')
                     lib.runSnapTrained(MaskGenome, os.path.join(
                         LOCALPARAMETERS, aug_species+'.snap.hmm'), os.path.join(args.out, 'predict_misc'), SnapPredictions)
@@ -1587,22 +1587,22 @@
                     'Existing snap predictions found {:}'.format(SnapPredictions))
             if lib.checkannotations(SnapPredictions):
                 snapCount = lib.countGFFgenes(SnapPredictions)
                 lib.log.info('{:,} predictions from SNAP'.format(snapCount))
                 if snapCount > 0:
                     SNAP = True
                 else:
-                    lib.log.info(
-                        'SNAP prediction failed, moving on without result')
-            if SNAP and os.path.isfile(os.path.join(args.out, 'predict_misc', 'snap-trained.hmm')):
-                shutil.copyfile(os.path.join(args.out, 'predict_misc', 'snap-trained.hmm'),
-                                os.path.join(LOCALPARAMETERS, aug_species+'.snap.hmm'))
-            else:
-                lib.log.debug('snap failed removing from training parameters')
-                trainingData['snap'] = [{}]
+                    lib.log.info('SNAP prediction failed, moving on without result')
+            if RunModes['snap'] != 'pretrained':
+                if SNAP and os.path.isfile(os.path.join(args.out, 'predict_misc', 'snap-trained.hmm')):
+                    shutil.copyfile(os.path.join(args.out, 'predict_misc', 'snap-trained.hmm'),
+                                    os.path.join(LOCALPARAMETERS, aug_species+'.snap.hmm'))
+                else:
+                    lib.log.debug('snap failed removing from training parameters')
+                    trainingData['snap'] = [{}]
 
         # run Glimmer predictions
         GLIMMER = False
         GlimmerPredictions = os.path.join(
             args.out, 'predict_misc', 'glimmerhmm-predictions.gff3')
         if 'glimmerhmm' in RunModes:
             if not lib.checkannotations(GlimmerPredictions):
@@ -1618,28 +1618,27 @@
                         lib.runGlimmerHMM(MaskGenome, FinalTrainingModels, os.path.join(
                             args.out, 'predict_misc'), GlimmerPredictions)
             else:
                 lib.log.info('Existing GlimmerHMM predictions found: {:}'.format(
                     GlimmerPredictions))
             if lib.checkannotations(GlimmerPredictions):
                 glimmerCount = lib.countGFFgenes(GlimmerPredictions)
-                lib.log.info(
-                    '{:,} predictions from GlimmerHMM'.format(glimmerCount))
+                lib.log.info('{:,} predictions from GlimmerHMM'.format(glimmerCount))
                 if glimmerCount > 0:
                     GLIMMER = True
                 else:
                     lib.log.info(
                         'GlimmerHMM prediction failed, moving on without result')
-            if GLIMMER and os.path.isdir(os.path.join(args.out, 'predict_misc', 'glimmerhmm')):
-                lib.copyDirectory(os.path.join(args.out, 'predict_misc', 'glimmerhmm'), os.path.join(
-                    LOCALPARAMETERS, 'glimmerhmm'))
-            else:
-                lib.log.debug(
-                    'GlimmerHMM failed, removing from training parameters')
-                trainingData = [{}]
+            if RunModes['glimmerhmm'] != 'pretrained':
+                if GLIMMER and os.path.isdir(os.path.join(args.out, 'predict_misc', 'glimmerhmm')):
+                    lib.copyDirectory(os.path.join(args.out, 'predict_misc', 'glimmerhmm'), os.path.join(
+                        LOCALPARAMETERS, 'glimmerhmm'))
+                else:
+                    lib.log.debug('GlimmerHMM failed, removing from training parameters')
+                    trainingData = [{}]
 
         # EVM related input tasks, find all predictions and concatenate together
         pred_in = [Augustus]
         if GeneMark:
             pred_in.append(GeneMark)
         if args.pasa_gff:
             pred_in.append(PASA_GFF)
@@ -1878,14 +1877,25 @@
         args.out, 'predict_results', organism_name+'.validation.txt')
     final_error = os.path.join(
         args.out, 'predict_results', organism_name+'.error.summary.txt')
     final_fixes = os.path.join(
         args.out, 'predict_results', organism_name+'.models-need-fixing.txt')
     final_stats = os.path.join(args.out, 'predict_results', organism_name+'.stats.json')
 
+    # generate output files
+    shutil.copyfile(tbl_file, final_tbl)
+    lib.tbl2allout(final_tbl, MaskGenome, final_gff, final_proteins,
+                   final_transcripts, final_cds_transcripts, final_fasta)
+    lib.annotation_summary(MaskGenome, final_stats, tbl=final_tbl,
+                           transcripts=Transcripts, proteins=Exonerate,
+                           database=FUNDB, command=' '.join(sys.argv),
+                           organism=organism_name)
+    total = lib.countGFFgenes(final_gff)
+    lib.log.info("Collecting final annotation files for {:,} total gene models".format(total))
+
     # run tbl2asn in new directory directory
     # setup SBT file
     SBT = os.path.join(parentdir, 'config', 'test.sbt')
     discrep = os.path.join(args.out, 'predict_results',
                            organism_name + '.discrepency.report.txt')
     lib.log.info("Converting to final Genbank format")
     # have to run as subprocess because of multiprocessing issues
@@ -1897,29 +1907,38 @@
     if args.strain:
         cmd += ['--strain', args.strain]
     lib.log.debug(' '.join(cmd))
     subprocess.call(cmd)
     # check if completed successfully
     if not lib.checkannotations(os.path.join(gag3dir, 'genome.gbf')):
         lib.log.info('ERROR: GBK file conversion failed, tbl2asn parallel script has died')
-        sys.exit(1)
+        lib.log.info('Trying single threaded tbl2asn as backup')
+        meta = "[organism=" + args.species + "]"
+        if args.isolate:
+            isolate_meta = "[isolate=" + args.isolate + "]"
+            meta = meta + " " + isolate_meta
+        if args.strain:
+            strain_meta = "[strain=" + args.strain + "]"
+            meta = meta + " " + strain_meta
+        fun_version = lib.get_version()
+        cmd = ['tbl2asn', '-y', '"Annotated using '+fun_version+'"', '-N', '1',
+            '-t', SBT, '-M', 'n', '-j', '"'+meta+'"', '-V', 'b',
+            '-c', 'f', '-T', '-a', 'r10u', '-p', gag3dir]
+        subprocess.call(cmd)
+        if not lib.checkannotations(os.path.join(gag3dir, 'genome.gbf')):
+            lib.log.info('CMD: {}'.format(' '.join(cmd)))
+            lib.log.info('ERROR: tbl2asn also failed in single threaded mode, check tbl2asn installation/compilation')
+            sys.exit(1)
+        else:
+            lib.log.debug('{}'.format(' '.join(cmd)))
 
     # retrieve files/reorganize
     shutil.copyfile(os.path.join(gag3dir, 'genome.gbf'), final_gbk)
-    shutil.copyfile(os.path.join(gag3dir, 'genome.tbl'), final_tbl)
     shutil.copyfile(os.path.join(gag3dir, 'genome.val'), final_validation)
     shutil.copyfile(os.path.join(gag3dir, 'errorsummary.val'), final_error)
-    lib.tbl2allout(final_tbl, MaskGenome, final_gff, final_proteins,
-                   final_transcripts, final_cds_transcripts, final_fasta)
-    lib.annotation_summary(MaskGenome, final_stats, tbl=final_tbl,
-                           transcripts=Transcripts, proteins=Exonerate,
-                           database=FUNDB, command=' '.join(sys.argv),
-                           organism=organism_name)
-    total = lib.countGFFgenes(final_gff)
-    lib.log.info("Collecting final annotation files for {:,} total gene models".format(total))
 
     lib.log.info("Funannotate predict is finished, output files are in the %s/predict_results folder" % (args.out))
 
     # check if there are error that need to be fixed
     errors = lib.ncbiCheckErrors(
         final_error, final_validation, prefix, final_fixes)
     if errors > 0:
@@ -1939,16 +1958,16 @@
   funannotate update -i {:} --cpus {:} \\\n\
             --left illumina_forward_RNAseq_R1.fastq.gz \\\n\
             --right illumina_forward_RNAseq_R2.fastq.gz \\\n\
             --jaccard_clip\n".format(args.out, args.cpus))
     else:
         lib.log.info("Your next step might be functional annotation, suggested commands:\n\
 -------------------------------------------------------\n\
-Run InterProScan (Docker required): \nfunannotate iprscan -i {:} -m docker -c {:}\n\n\
-Run antiSMASH: \nfunannotate remote -i {:} -m antismash -e youremail@server.edu\n\n\
+Run InterProScan (manual install): \nfunannotate iprscan -i {:} -c {:}\n\n\
+Run antiSMASH (optional): \nfunannotate remote -i {:} -m antismash -e youremail@server.edu\n\n\
 Annotate Genome: \nfunannotate annotate -i {:} --cpus {:} --sbt yourSBTfile.txt\n\
 -------------------------------------------------------\n\
                 ".format(args.out,
                          args.cpus,
                          args.out,
                          args.out,
                          args.cpus))
```

### Comparing `funannotate-1.8.7/funannotate/remote.py` & `funannotate-1.8.9/funannotate/remote.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/resources.py` & `funannotate-1.8.9/funannotate/resources.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/setupDB.py` & `funannotate-1.8.9/funannotate/setupDB.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/sort.py` & `funannotate-1.8.9/funannotate/sort.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/species.py` & `funannotate-1.8.9/funannotate/species.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/stackedBarGraph.py` & `funannotate-1.8.9/funannotate/stackedBarGraph.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/test.py` & `funannotate-1.8.9/funannotate/test.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/train.py` & `funannotate-1.8.9/funannotate/train.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/update.py` & `funannotate-1.8.9/funannotate/update.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/bam2gff3.py` & `funannotate-1.8.9/funannotate/utilities/bam2gff3.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/contrast.py` & `funannotate-1.8.9/funannotate/utilities/contrast.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/gbk2parts.py` & `funannotate-1.8.9/funannotate/utilities/gbk2parts.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/gff2prot.py` & `funannotate-1.8.9/funannotate/utilities/gff2prot.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/gff2tbl.py` & `funannotate-1.8.9/funannotate/utilities/gff2tbl.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/gff_reformat.py` & `funannotate-1.8.9/funannotate/utilities/gff_reformat.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/quarry2gff3.py` & `funannotate-1.8.9/funannotate/utilities/quarry2gff3.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/stats.py` & `funannotate-1.8.9/funannotate/utilities/stats.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/stringtie2gff3.py` & `funannotate-1.8.9/funannotate/utilities/stringtie2gff3.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate/utilities/tbl2gbk.py` & `funannotate-1.8.9/funannotate/utilities/tbl2gbk.py`

 * *Files identical despite different names*

### Comparing `funannotate-1.8.7/funannotate.egg-info/PKG-INFO` & `funannotate-1.8.9/funannotate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funannotate
-Version: 1.8.7
+Version: 1.8.9
 Summary: funannotate: eukaryotic genome annotation pipeline
 Home-page: https://github.com/nextgenusfs/funannotate
 Author: Jon Palmer
 Author-email: nextgenusfs@gmail.com
 License: BSD-2
 Description: 
         [![Latest Github release](https://img.shields.io/github/release/nextgenusfs/funannotate.svg)](https://github.com/nextgenusfs/funannotate/releases/latest)
@@ -44,14 +44,22 @@
         conda config --add channels defaults
         conda config --add channels bioconda
         conda config --add channels conda-forge
         
         #then create environment
         conda create -n funannotate funannotate
         ```
+        If `conda` is taking forever to solve the environment, I would recommend giving [mamba](https://github.com/mamba-org/mamba) a try:
+        ```
+        #install mamba into base environment
+        conda install -n base mamba
+        
+        #then use mamba as drop in replacmeent
+        mamba create -n funannotate funannotate
+        ```
         
         If you want to use GeneMark-ES/ET you will need to install that manually following developers instructions:
         http://topaz.gatech.edu/GeneMark/license_download.cgi
         
         Note that you will need to change the shebang line for all perl scripts in GeneMark to use `/usr/bin/env perl`.
         You will then also need to add `gmes_petap.pl` to the $PATH or set the environmental variable $GENEMARK_PATH to the gmes_petap directory.
```

### Comparing `funannotate-1.8.7/funannotate.egg-info/SOURCES.txt` & `funannotate-1.8.9/funannotate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 funannotate.egg-info/SOURCES.txt
 funannotate.egg-info/dependency_links.txt
 funannotate.egg-info/entry_points.txt
 funannotate.egg-info/requires.txt
 funannotate.egg-info/top_level.txt
 funannotate/aux_scripts/augustus_parallel.py
 funannotate/aux_scripts/enrichment_parallel.py
-funannotate/aux_scripts/fasta2agp.pl
+funannotate/aux_scripts/fasta2agp.py
 funannotate/aux_scripts/filterGenemark.pl
 funannotate/aux_scripts/filterIntronsFindStrand.pl
 funannotate/aux_scripts/funannotate-BUSCO2-py2.py
 funannotate/aux_scripts/funannotate-BUSCO2.py
 funannotate/aux_scripts/funannotate-p2g.py
 funannotate/aux_scripts/funannotate-runEVM.py
 funannotate/aux_scripts/genemark_gtf2gff3.pl
```

### Comparing `funannotate-1.8.7/setup.py` & `funannotate-1.8.9/setup.py`

 * *Files identical despite different names*

