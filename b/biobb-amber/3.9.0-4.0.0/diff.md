# Comparing `tmp/biobb_amber-3.9.0.tar.gz` & `tmp/biobb_amber-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_amber-3.9.0.tar", last modified: Tue Dec 27 14:35:05 2022, max compression
+gzip compressed data, was "dist/biobb_amber-4.0.0.tar", last modified: Wed Apr 12 08:30:49 2023, max compression
```

## Comparing `biobb_amber-3.9.0.tar` & `biobb_amber-4.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/
--rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573      882 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     3333 2022-12-27 14:33:01.000000 biobb_amber-3.9.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      154 2022-12-27 14:32:43.000000 biobb_amber-3.9.0/biobb_amber/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/ambpdb/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       43 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/ambpdb/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7403 2022-12-27 12:27:45.000000 biobb_amber-3.9.0/biobb_amber/ambpdb/amber_to_pdb.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1779 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/ambpdb/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/cphstats/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       59 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/cphstats/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17670 2022-12-27 12:30:10.000000 biobb_amber-3.9.0/biobb_amber/cphstats/cestats_run.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2138 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/cphstats/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17601 2022-12-27 12:30:57.000000 biobb_amber-3.9.0/biobb_amber/cphstats/cphstats_run.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/cpptraj/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       54 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/cpptraj/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1839 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/cpptraj/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10930 2022-12-27 12:45:56.000000 biobb_amber-3.9.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/leap/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      102 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/leap/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1993 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/leap/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    26409 2022-12-27 12:49:56.000000 biobb_amber-3.9.0/biobb_amber/leap/leap_add_ions.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8018 2022-12-27 12:52:38.000000 biobb_amber-3.9.0/biobb_amber/leap/leap_build_linear_structure.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16758 2022-12-27 12:53:48.000000 biobb_amber-3.9.0/biobb_amber/leap/leap_gen_top.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    21795 2022-12-27 12:54:46.000000 biobb_amber-3.9.0/biobb_amber/leap/leap_solvate.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/nab/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       51 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/nab/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1668 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/nab/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8602 2022-12-27 12:57:26.000000 biobb_amber-3.9.0/biobb_amber/nab/nab_build_dna_structure.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/parmed/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       73 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/parmed/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1764 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/parmed/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9083 2022-12-27 12:59:06.000000 biobb_amber-3.9.0/biobb_amber/parmed/parmed_cpinutil.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7540 2022-12-27 13:01:12.000000 biobb_amber-3.9.0/biobb_amber/parmed/parmed_hmassrepartition.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/pdb4amber/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       47 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/pdb4amber/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1697 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/pdb4amber/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7597 2022-12-27 14:13:17.000000 biobb_amber-3.9.0/biobb_amber/pdb4amber/pdb4amber_run.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/pmemd/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       41 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/pmemd/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2221 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/pmemd/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    25555 2022-12-27 14:14:26.000000 biobb_amber-3.9.0/biobb_amber/pmemd/pmemd_mdrun.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/process/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       62 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/process/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1734 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/process/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8977 2022-12-27 14:22:11.000000 biobb_amber-3.9.0/biobb_amber/process/process_mdout.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9044 2022-12-27 14:21:17.000000 biobb_amber-3.9.0/biobb_amber/process/process_minout.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber/sander/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       43 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/sander/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2248 2022-05-26 11:32:14.000000 biobb_amber-3.9.0/biobb_amber/sander/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    28667 2022-12-27 14:23:22.000000 biobb_amber-3.9.0/biobb_amber/sander/sander_mdrun.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      882 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1475 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      954 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       12 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/biobb_amber.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2022-12-27 14:35:05.000000 biobb_amber-3.9.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2422 2022-12-27 14:32:16.000000 biobb_amber-3.9.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      882 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5315 2023-04-12 08:29:08.000000 biobb_amber-4.0.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      155 2023-04-12 08:28:56.000000 biobb_amber-4.0.0/biobb_amber/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7407 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/amber_to_pdb.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1898 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/ambpdb/common.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/cphstats/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       60 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17622 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/cestats_run.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2327 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    17574 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cphstats/cphstats_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       54 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1968 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11027 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/leap/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      105 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2144 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    26378 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_add_ions.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8046 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_build_linear_structure.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16671 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_gen_top.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    21736 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/leap/leap_solvate.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/nab/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       51 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/nab/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1769 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/nab/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8722 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/nab/nab_build_dna_structure.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/parmed/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/parmed/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1887 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/parmed/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9081 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/parmed/parmed_cpinutil.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7633 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/parmed/parmed_hmassrepartition.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       47 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1810 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7603 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pdb4amber/pdb4amber_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/pmemd/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       41 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/pmemd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2414 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pmemd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    25615 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/pmemd/pmemd_mdrun.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/process/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       63 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1841 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9046 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/process_mdout.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9149 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/process/process_minout.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber/sander/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       43 2022-05-26 11:32:14.000000 biobb_amber-4.0.0/biobb_amber/sander/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2472 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/sander/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    29424 2023-04-12 08:27:46.000000 biobb_amber-4.0.0/biobb_amber/sander/sander_mdrun.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      882 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1475 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      954 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       12 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/biobb_amber.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-12 08:30:49.000000 biobb_amber-4.0.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2422 2023-04-12 08:28:45.000000 biobb_amber-4.0.0/setup.py
```

### Comparing `biobb_amber-3.9.0/LICENSE` & `biobb_amber-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_amber-3.9.0/PKG-INFO` & `biobb_amber-4.0.0/biobb_amber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb_amber
-Version: 3.9.0
+Name: biobb-amber
+Version: 4.0.0
 Summary: Biobb_amber is a BioBB category for AMBER MD package.
 Home-page: https://github.com/bioexcel/biobb_amber
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_amber.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility MD Amber
```

### Comparing `biobb_amber-3.9.0/biobb_amber/ambpdb/amber_to_pdb.py` & `biobb_amber-4.0.0/biobb_amber/ambpdb/amber_to_pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 """Module containing the AmberToPDB class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
-from biobb_common.tools import file_utils as fu
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.ambpdb.common import *
+from biobb_amber.ambpdb.common import check_input_path, check_output_path
+
 
 class AmberToPDB(BiobbObject):
     """
     | biobb_amber AmberToPDB
     | Wrapper of the `AmberTools (AMBER MD Package) ambpdb tool <https://ambermd.org/AmberTools.php>`_ module.
     | Generates a PDB structure from AMBER topology (parmtop) and coordinates (crd) files, using the ambpdb tool from the AmberTools MD package.
 
@@ -57,17 +57,17 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_top_path': input_top_path,
-                    'input_crd_path': input_crd_path},
-            'out': { 'output_pdb_path': output_pdb_path }
+            'in': {'input_top_path': input_top_path,
+                   'input_crd_path': input_crd_path},
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'ambpdb')
 
         # Check the properties
@@ -78,34 +78,35 @@
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], "input_top_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_crd_path"] = check_input_path(self.io_dict["in"]["input_crd_path"], "input_crd_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Command line
         self.cmd = [self.binary_path,
-               '-p', self.stage_io_dict['in']['input_top_path'],
-               '-c', self.stage_io_dict['in']['input_crd_path'],
-               '> ', self.stage_io_dict['out']['output_pdb_path']
-               ]
-               
-         # Run Biobb block
+                    '-p', self.stage_io_dict['in']['input_top_path'],
+                    '-c', self.stage_io_dict['in']['input_crd_path'],
+                    '> ', self.stage_io_dict['out']['output_pdb_path']
+                    ]
+
+        # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporary file(s)
         self.tmp_files.extend([
@@ -113,23 +114,25 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def amber_to_pdb(input_top_path: str, input_crd_path: str, output_pdb_path: str,
-           properties: dict = None, **kwargs) -> int:
+                 properties: dict = None, **kwargs) -> int:
     """Create :class:`AmberToPDB <amber.amber_to_pdb.AmberToPDB>`amber.amber_to_pdb.AmberToPDB class and
     execute :meth:`launch() <amber.amber_to_pdb.AmberToPDB.launch>` method"""
 
-    return AmberToPDB( input_top_path=input_top_path,
-                        input_crd_path=input_crd_path,
-                        output_pdb_path=output_pdb_path,
-                        properties=properties).launch()
+    return AmberToPDB(input_top_path=input_top_path,
+                      input_crd_path=input_crd_path,
+                      output_pdb_path=output_pdb_path,
+                      properties=properties).launch()
+
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description='Generates a PDB structure from AMBER topology (parmtop) and coordinates (crd) files, using the ambpdb tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
@@ -140,13 +143,14 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
     amber_to_pdb(input_top_path=args.input_top_path,
-                input_crd_path=args.input_crd_path,
-                output_pdb_path=args.output_pdb_path,
-                properties=properties)
+                 input_crd_path=args.input_crd_path,
+                 output_pdb_path=args.output_pdb_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/ambpdb/common.py` & `biobb_amber-4.0.0/biobb_amber/cphstats/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-""" Common functions for package biobb_amber.amb2pdb """
+""" Common functions for package biobb_amber.cphstats """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 # CHECK OUTPUT PARAMETERS
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_top_path': ['top','prmtop','parmtop'],
-		'input_crd_path': ['crd','mdcrd','inpcrd','rst','rst7'],
-        'output_pdb_path': ['pdb']
-	}
-	return ext in formats[argument]
+    """ Checks if file format is compatible """
+    formats = {
+        'input_cpin_path': ['cpin', 'txt', 'in'],
+        'input_cpout_path': ['cpout', 'zip', 'gzip', 'gz'],
+        'input_cein_path': ['cein', 'txt', 'in'],
+        'input_ceout_path': ['ceout', 'zip', 'gzip', 'gz'],
+        'output_dat_path': ['dat', 'out', 'txt', 'o'],
+        'output_population_path': ['dat', 'out', 'txt', 'o'],
+        'output_chunk_path': ['dat', 'out', 'txt', 'o'],
+        'output_cumulative_path': ['dat', 'out', 'txt', 'o'],
+        'output_conditional_path': ['dat', 'out', 'txt', 'o'],
+        'output_chunk_conditional_path': ['dat', 'out', 'txt', 'o'],
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_amber-3.9.0/biobb_amber/cphstats/cestats_run.py` & `biobb_amber-4.0.0/biobb_amber/cphstats/cestats_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 
 """Module containing the Cestats class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
-from biobb_common.tools import file_utils as fu
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.cphstats.common import *
+from biobb_amber.cphstats.common import check_input_path, check_output_path
+
 
 class CestatsRun(BiobbObject):
     """
     | biobb_amber CestatsRun
     | Wrapper of the `AmberTools (AMBER MD Package) cestats tool <https://ambermd.org/AmberTools.php>`_ module.
     | Analyzing the results of constant Redox potential MD simulations using cestats tool from the AMBER MD package.
 
@@ -77,22 +75,22 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_cein_path': input_cein_path,
-                    'input_ceout_path': input_ceout_path },
-            'out': {    'output_dat_path': output_dat_path,
-                        'output_population_path': output_population_path,
-                        'output_chunk_path': output_chunk_path,
-                        'output_cumulative_path': output_cumulative_path,
-                        'output_conditional_path': output_conditional_path,
-                        'output_chunk_conditional_path': output_chunk_conditional_path }
+            'in': {'input_cein_path': input_cein_path,
+                   'input_ceout_path': input_ceout_path},
+            'out': {'output_dat_path': output_dat_path,
+                    'output_population_path': output_population_path,
+                    'output_chunk_path': output_chunk_path,
+                    'output_cumulative_path': output_cumulative_path,
+                    'output_conditional_path': output_conditional_path,
+                    'output_chunk_conditional_path': output_chunk_conditional_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.timestep = properties.get('timestep', 0.002)
         self.verbose = properties.get('verbose', False)
         self.interval = properties.get('interval', 1000)
@@ -114,40 +112,41 @@
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_cein_path"] = check_input_path(self.io_dict["in"]["input_cein_path"], "input_cein_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_ceout_path"] = check_input_path(self.io_dict["in"]["input_ceout_path"], "input_ceout_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"],"output_dat_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_population_path"] = check_output_path(self.io_dict["out"]["output_population_path"],"output_population_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_chunk_path"] = check_output_path(self.io_dict["out"]["output_chunk_path"],"output_chunk_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_cumulative_path"] = check_output_path(self.io_dict["out"]["output_cumulative_path"],"output_cumulative_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_chunk_conditional_path"] = check_output_path(self.io_dict["out"]["output_chunk_conditional_path"],"output_chunk_conditional_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_conditional_path"] = check_output_path(self.io_dict["out"]["output_conditional_path"],"output_conditional_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"], "output_dat_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_population_path"] = check_output_path(self.io_dict["out"]["output_population_path"], "output_population_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_chunk_path"] = check_output_path(self.io_dict["out"]["output_chunk_path"], "output_chunk_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cumulative_path"] = check_output_path(self.io_dict["out"]["output_cumulative_path"], "output_cumulative_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_chunk_conditional_path"] = check_output_path(self.io_dict["out"]["output_chunk_conditional_path"], "output_chunk_conditional_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_conditional_path"] = check_output_path(self.io_dict["out"]["output_conditional_path"], "output_conditional_path", True, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the CestatsRun module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Command line
         # cphstats -i 4LYT.equil.cpin 0/4LYT.md1.cpout -o pH0_calcpka.dat --population pH0_populations.dat
         self.cmd = [self.binary_path,
-               '-O',
-               '-i', self.stage_io_dict['in']['input_cein_path'],
-               '-o', self.stage_io_dict['out']['output_dat_path'],
-               self.stage_io_dict['in']['input_ceout_path']
-               ]
+                    '-O',
+                    '-i', self.stage_io_dict['in']['input_cein_path'],
+                    '-o', self.stage_io_dict['out']['output_dat_path'],
+                    self.stage_io_dict['in']['input_ceout_path']
+                    ]
 
         if self.io_dict['out']['output_population_path']:
             self.cmd.append('--population ')
             self.cmd.append(self.stage_io_dict['out']['output_population_path'])
 
         if self.io_dict['out']['output_chunk_path']:
             self.cmd.append('--chunk-out ')
@@ -215,32 +214,34 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cestats_run(input_cein_path: str, input_ceout_path: str,
-            output_dat_path: str,
-            output_population_path: str = None, output_chunk_path: str = None,
-            output_conditional_path: str = None, output_chunk_conditional_path: str=None,
-            output_cumulative_path: str = None,
-            properties: dict = None, **kwargs) -> int:
+                output_dat_path: str,
+                output_population_path: str = None, output_chunk_path: str = None,
+                output_conditional_path: str = None, output_chunk_conditional_path: str = None,
+                output_cumulative_path: str = None,
+                properties: dict = None, **kwargs) -> int:
     """Create :class:`CestatsRun <cestats.chpstats_run.CestatsRun>`cestats.chpstats_run.CestatsRun class and
     execute :meth:`launch() <cestats.chpstats_run.CestatsRun.launch>` method"""
 
-    return CestatsRun( input_cein_path=input_cein_path,
-                    input_ceout_path=input_ceout_path,
-                    output_dat_path=output_dat_path,
-                    output_population_path=output_population_path,
-                    output_chunk_path=output_chunk_path,
-                    output_chunk_conditional_path=output_chunk_conditional_path,
-                    output_conditional_path=output_conditional_path,
-                    output_cumulative_path=output_cumulative_path,
-                    properties=properties).launch()
+    return CestatsRun(input_cein_path=input_cein_path,
+                      input_ceout_path=input_ceout_path,
+                      output_dat_path=output_dat_path,
+                      output_population_path=output_population_path,
+                      output_chunk_path=output_chunk_path,
+                      output_chunk_conditional_path=output_chunk_conditional_path,
+                      output_conditional_path=output_conditional_path,
+                      output_cumulative_path=output_cumulative_path,
+                      properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Analyzing the results of constant Redox potential MD simulations using cestats tool from the AMBER MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -254,19 +255,20 @@
     required_args.add_argument('--output_chunk_conditional_path', required=False, help='Output file with a time series of the conditional probabilities over a trajectory split up into chunks. Accepted formats: dat, out, txt, o.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    cestats_run(    input_cein_path=args.input_cein_path,
-                    input_ceout_path=args.input_ceout_path,
-                    output_dat_path=args.output_dat_path,
-                    output_population_path=args.output_population_path,
-                    output_chunk_path=args.output_chunk_path,
-                    output_cumulative_path=args.output_cumulative_path,
-                    output_conditional_path=args.output_conditional_path,
-                    output_chunk_conditional_path=args.output_chunk_conditional_path,
-                    properties=properties)
+    cestats_run(input_cein_path=args.input_cein_path,
+                input_ceout_path=args.input_ceout_path,
+                output_dat_path=args.output_dat_path,
+                output_population_path=args.output_population_path,
+                output_chunk_path=args.output_chunk_path,
+                output_cumulative_path=args.output_cumulative_path,
+                output_conditional_path=args.output_conditional_path,
+                output_chunk_conditional_path=args.output_chunk_conditional_path,
+                properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/cphstats/common.py` & `biobb_amber-4.0.0/biobb_amber/parmed/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-""" Common functions for package biobb_amber.cphstats """
+""" Common functions for package biobb_amber.parmed """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 # CHECK OUTPUT PARAMETERS
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_cpin_path': ['cpin','txt','in'],
-		'input_cpout_path': ['cpout','zip','gzip','gz'],
-		'input_cein_path': ['cein','txt','in'],
-		'input_ceout_path': ['ceout','zip','gzip','gz'],
-		'output_dat_path': ['dat','out','txt','o'],
-		'output_population_path': ['dat','out','txt','o'],
-		'output_chunk_path': ['dat','out','txt','o'],
-		'output_cumulative_path': ['dat','out','txt','o'],
-		'output_conditional_path': ['dat','out','txt','o'],
-		'output_chunk_conditional_path': ['dat','out','txt','o'],
-	}
-	return ext in formats[argument]
+    """ Checks if file format is compatible """
+    formats = {
+        'input_top_path': ['top', 'prmtop', 'parmtop'],
+        'output_top_path': ['top', 'prmtop', 'parmtop'],
+        'output_cpin_path': ['cpin']
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_amber-3.9.0/biobb_amber/cphstats/cphstats_run.py` & `biobb_amber-4.0.0/biobb_amber/cphstats/cphstats_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 
 """Module containing the Cphstats class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
-from biobb_common.tools import file_utils as fu
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.cphstats.common import *
+from biobb_amber.cphstats.common import check_input_path, check_output_path
+
 
 class CphstatsRun(BiobbObject):
     """
     | biobb_amber CphstatsRun
     | Wrapper of the `AmberTools (AMBER MD Package) cphstats tool <https://ambermd.org/AmberTools.php>`_ module.
     | Analyzing the results of constant pH MD simulations using cphstats tool from the AMBER MD package.
 
@@ -77,22 +75,22 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_cpin_path': input_cpin_path,
-                    'input_cpout_path': input_cpout_path },
-            'out': {    'output_dat_path': output_dat_path,
-                        'output_population_path': output_population_path,
-                        'output_chunk_path': output_chunk_path,
-                        'output_cumulative_path': output_cumulative_path,
-                        'output_conditional_path': output_conditional_path,
-                        'output_chunk_conditional_path': output_chunk_conditional_path }
+            'in': {'input_cpin_path': input_cpin_path,
+                   'input_cpout_path': input_cpout_path},
+            'out': {'output_dat_path': output_dat_path,
+                    'output_population_path': output_population_path,
+                    'output_chunk_path': output_chunk_path,
+                    'output_cumulative_path': output_cumulative_path,
+                    'output_conditional_path': output_conditional_path,
+                    'output_chunk_conditional_path': output_chunk_conditional_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.timestep = properties.get('timestep', 0.002)
         self.verbose = properties.get('verbose', False)
         self.interval = properties.get('interval', 1000)
@@ -114,40 +112,41 @@
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_cpin_path"] = check_input_path(self.io_dict["in"]["input_cpin_path"], "input_cpin_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_cpout_path"] = check_input_path(self.io_dict["in"]["input_cpout_path"], "input_cpout_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"],"output_dat_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_population_path"] = check_output_path(self.io_dict["out"]["output_population_path"],"output_population_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_chunk_path"] = check_output_path(self.io_dict["out"]["output_chunk_path"],"output_chunk_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_cumulative_path"] = check_output_path(self.io_dict["out"]["output_cumulative_path"],"output_cumulative_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_chunk_conditional_path"] = check_output_path(self.io_dict["out"]["output_chunk_conditional_path"],"output_chunk_conditional_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_conditional_path"] = check_output_path(self.io_dict["out"]["output_conditional_path"],"output_conditional_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"], "output_dat_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_population_path"] = check_output_path(self.io_dict["out"]["output_population_path"], "output_population_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_chunk_path"] = check_output_path(self.io_dict["out"]["output_chunk_path"], "output_chunk_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cumulative_path"] = check_output_path(self.io_dict["out"]["output_cumulative_path"], "output_cumulative_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_chunk_conditional_path"] = check_output_path(self.io_dict["out"]["output_chunk_conditional_path"], "output_chunk_conditional_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_conditional_path"] = check_output_path(self.io_dict["out"]["output_conditional_path"], "output_conditional_path", True, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the CphstatsRun module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Command line
         # cphstats -i 4LYT.equil.cpin 0/4LYT.md1.cpout -o pH0_calcpka.dat --population pH0_populations.dat
         self.cmd = [self.binary_path,
-               '-O',
-               '-i', self.stage_io_dict['in']['input_cpin_path'],
-               '-o', self.stage_io_dict['out']['output_dat_path'],
-               self.stage_io_dict['in']['input_cpout_path']
-               ]
+                    '-O',
+                    '-i', self.stage_io_dict['in']['input_cpin_path'],
+                    '-o', self.stage_io_dict['out']['output_dat_path'],
+                    self.stage_io_dict['in']['input_cpout_path']
+                    ]
 
         if self.io_dict['out']['output_population_path']:
             self.cmd.append('--population ')
             self.cmd.append(self.stage_io_dict['out']['output_population_path'])
 
         if self.io_dict['out']['output_chunk_path']:
             self.cmd.append('--chunk-out ')
@@ -215,32 +214,34 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cphstats_run(input_cpin_path: str, input_cpout_path: str,
-            output_dat_path: str,
-            output_population_path: str = None, output_chunk_path: str = None,
-            output_conditional_path: str = None, output_chunk_conditional_path: str=None,
-            output_cumulative_path: str = None,
-            properties: dict = None, **kwargs) -> int:
+                 output_dat_path: str,
+                 output_population_path: str = None, output_chunk_path: str = None,
+                 output_conditional_path: str = None, output_chunk_conditional_path: str = None,
+                 output_cumulative_path: str = None,
+                 properties: dict = None, **kwargs) -> int:
     """Create :class:`CphstatsRun <cphstats.chpstats_run.CphstatsRun>`cphstats.chpstats_run.CphstatsRun class and
     execute :meth:`launch() <cphstats.chpstats_run.CphstatsRun.launch>` method"""
 
-    return CphstatsRun( input_cpin_path=input_cpin_path,
-                    input_cpout_path=input_cpout_path,
-                    output_dat_path=output_dat_path,
-                    output_population_path=output_population_path,
-                    output_chunk_path=output_chunk_path,
-                    output_chunk_conditional_path=output_chunk_conditional_path,
-                    output_conditional_path=output_conditional_path,
-                    output_cumulative_path=output_cumulative_path,
-                    properties=properties).launch()
+    return CphstatsRun(input_cpin_path=input_cpin_path,
+                       input_cpout_path=input_cpout_path,
+                       output_dat_path=output_dat_path,
+                       output_population_path=output_population_path,
+                       output_chunk_path=output_chunk_path,
+                       output_chunk_conditional_path=output_chunk_conditional_path,
+                       output_conditional_path=output_conditional_path,
+                       output_cumulative_path=output_cumulative_path,
+                       properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Analyzing the results of constant pH MD simulations using cphstats tool from the AMBER MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -254,19 +255,20 @@
     required_args.add_argument('--output_chunk_conditional_path', required=False, help='Output file with a time series of the conditional probabilities over a trajectory split up into chunks. Accepted formats: dat, out, txt, o.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    cphstats_run(    input_cpin_path=args.input_cpin_path,
-                    input_cpout_path=args.input_cpout_path,
-                    output_dat_path=args.output_dat_path,
-                    output_population_path=args.output_population_path,
-                    output_chunk_path=args.output_chunk_path,
-                    output_cumulative_path=args.output_cumulative_path,
-                    output_conditional_path=args.output_conditional_path,
-                    output_chunk_conditional_path=args.output_chunk_conditional_path,
-                    properties=properties)
+    cphstats_run(input_cpin_path=args.input_cpin_path,
+                 input_cpout_path=args.input_cpout_path,
+                 output_dat_path=args.output_dat_path,
+                 output_population_path=args.output_population_path,
+                 output_chunk_path=args.output_chunk_path,
+                 output_cumulative_path=args.output_cumulative_path,
+                 output_conditional_path=args.output_conditional_path,
+                 output_chunk_conditional_path=args.output_chunk_conditional_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/cpptraj/common.py` & `biobb_amber-4.0.0/biobb_amber/cpptraj/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """ Common functions for package biobb_amber.cpptraj """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 # CHECK OUTPUT PARAMETERS
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_crd_path': ['crd','mdcrd','inpcrd','rst','rst7'],
-		'input_top_path': ['top','prmtop','parmtop'],
+    """ Checks if file format is compatible """
+    formats = {
+        'input_crd_path': ['crd', 'mdcrd', 'inpcrd', 'rst', 'rst7'],
+        'input_top_path': ['top', 'prmtop', 'parmtop'],
         'output_pdb_path': ['pdb'],
-		'output_crd_path': ['crd','mdcrd','inpcrd','rst','rst7']
-	}
-	return ext in formats[argument]
+        'output_crd_path': ['crd', 'mdcrd', 'inpcrd', 'rst', 'rst7']
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_amber-3.9.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py` & `biobb_amber-4.0.0/biobb_amber/cpptraj/cpptraj_randomize_ions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 
 """Module containing the CpptrajRandomizeIons class and the command line interface."""
 import argparse
-import shutil
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.cpptraj.common import *
+from biobb_amber.cpptraj.common import check_input_path, check_output_path
+
 
 class CpptrajRandomizeIons(BiobbObject):
     """
     | biobb_amber.cpptraj.cpptraj_randomize_ions CpptrajRandomizeIons
     | Wrapper of the `AmberTools (AMBER MD Package) cpptraj tool <https://ambermd.org/AmberTools.php>`_ module.
     | Swap specified ions with randomly selected solvent molecules using cpptraj tool from the AmberTools MD package.
 
@@ -96,57 +96,57 @@
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], "input_top_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_crd_path"] = check_input_path(self.io_dict["in"]["input_crd_path"], "input_crd_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"],"output_crd_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"], "output_crd_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the CpptrajRandomizeIons module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         if self.container_path:
             instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("cpptraj.in"))
             instructions_file_path = str(PurePath(self.container_volume_path).joinpath("cpptraj.in"))
         else:
             self.tmp_folder = fu.create_unique_dir()
             instructions_file = str(PurePath(self.tmp_folder).joinpath("cpptraj.in"))
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             instructions_file_path = instructions_file
 
-
         # create cpptraj.in file
         # trajin randomizeIons.crd
         # randomizeions :K+,Cl-,Na+ around :DA,DC,DG,DT,D?3,D?5 by 5.0 overlap 3.5
         # trajout solv_randion.crd restart
         # trajout solv_randion.pdb pdb
         # go
-        
+
         with open(instructions_file, 'w') as cpptrajin:
-                cpptrajin.write("trajin " + self.stage_io_dict['in']['input_crd_path'] + " \n")
-                cpptrajin.write("randomizeions " + self.ion_mask + " around " + self.solute_mask + " by " + str(self.distance) + " overlap " + str(self.overlap) + " \n")
-                cpptrajin.write("trajout " + self.stage_io_dict['out']['output_crd_path'] + " restart \n")
-                cpptrajin.write("trajout " + self.stage_io_dict['out']['output_pdb_path'] + " pdb \n")
-                cpptrajin.write("go\n");
+            cpptrajin.write("trajin " + self.stage_io_dict['in']['input_crd_path'] + " \n")
+            cpptrajin.write("randomizeions " + self.ion_mask + " around " + self.solute_mask + " by " + str(self.distance) + " overlap " + str(self.overlap) + " \n")
+            cpptrajin.write("trajout " + self.stage_io_dict['out']['output_crd_path'] + " restart \n")
+            cpptrajin.write("trajout " + self.stage_io_dict['out']['output_pdb_path'] + " pdb \n")
+            cpptrajin.write("go\n")
 
         # Command line
         self.cmd = [self.binary_path,
-               self.stage_io_dict['in']['input_top_path'],
-               '-i', instructions_file_path
-               ]
+                    self.stage_io_dict['in']['input_top_path'],
+                    '-i', instructions_file_path
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -158,25 +158,27 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def cpptraj_randomize_ions(input_top_path: str, input_crd_path: str,
-        output_pdb_path: str, output_crd_path: str,
-        properties: dict = None, **kwargs) -> int:
+                           output_pdb_path: str, output_crd_path: str,
+                           properties: dict = None, **kwargs) -> int:
     """Create :class:`CpptrajRandomizeIons <cpptraj.cpptraj_randomize_ions.CpptrajRandomizeIons>`cpptraj.cpptraj_randomize_ions.CpptrajRandomizeIons class and
 execute :meth:`launch() <cpptraj.cpptraj_randomize_ions.CpptrajRandomizeIons.launch>` method"""
 
-    return CpptrajRandomizeIons( input_top_path=input_top_path,
-                        input_crd_path=input_crd_path,
-                        output_pdb_path=output_pdb_path,
-                        output_crd_path=output_crd_path,
-                        properties=properties).launch()
+    return CpptrajRandomizeIons(input_top_path=input_top_path,
+                                input_crd_path=input_crd_path,
+                                output_pdb_path=output_pdb_path,
+                                output_crd_path=output_crd_path,
+                                properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Swap specified ions with randomly selected solvent molecules using cpptraj tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -187,14 +189,15 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
     cpptraj_randomize_ions(input_top_path=args.input_top_path,
-                        input_crd_path=args.input_crd_path,
-                        output_pdb_path=args.output_pdb_path,
-                        output_crd_path=args.output_crd_path,
-                        properties=properties)
+                           input_crd_path=args.input_crd_path,
+                           output_pdb_path=args.output_pdb_path,
+                           output_crd_path=args.output_crd_path,
+                           properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/leap/common.py` & `biobb_amber-4.0.0/biobb_amber/nab/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-""" Common functions for package biobb_amber.leap """
+""" Common functions for package biobb_amber.nab """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 # CHECK OUTPUT PARAMETERS
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_pdb_path': ['pdb'],
-		'input_lib_path': ['lib','zip'],
-		'input_frcmod_path': ['frcmod','zip'],
-		'input_params_path': ['in', 'leapin', 'txt', 'zip'],
-		'input_source_path': ['in', 'leapin', 'txt', 'zip'],
-        'output_pdb_path': ['pdb'],
-		'output_top_path': ['top','prmtop','parmtop'],
-		'output_crd_path': ['crd','mdcrd','inpcrd','rst','rst7']
-	}
-	return ext in formats[argument]
+    """ Checks if file format is compatible """
+    formats = {
+        'output_pdb_path': ['pdb']
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_amber-3.9.0/biobb_amber/leap/leap_add_ions.py` & `biobb_amber-4.0.0/biobb_amber/leap/leap_add_ions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
 
 """Module containing the LeapAddIons class and the command line interface."""
 import argparse
-import shutil, re
+import shutil
+import re
 from decimal import Decimal
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.leap.common import *
+from biobb_amber.leap.common import check_input_path, check_output_path
+
 
 class LeapAddIons(BiobbObject):
     """
     | biobb_amber LeapAddIons
     | Wrapper of the `AmberTools (AMBER MD Package) leap tool <https://ambermd.org/AmberTools.php>`_ module.
     | Adds counterions to a system box for an AMBER MD system using tLeap tool from the AmberTools MD package.
 
@@ -70,50 +72,49 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_pdb_path: str,
-        output_pdb_path: str, output_top_path: str, output_crd_path: str,
-        input_lib_path: str = None, input_frcmod_path: str = None,
-        input_params_path: str = None, input_source_path: str = None,
-        properties: dict = None, **kwargs):
+                 output_pdb_path: str, output_top_path: str, output_crd_path: str,
+                 input_lib_path: str = None, input_frcmod_path: str = None,
+                 input_params_path: str = None, input_source_path: str = None,
+                 properties: dict = None, **kwargs):
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path,
-                    'input_lib_path': input_lib_path,
-                    'input_frcmod_path': input_frcmod_path,
-                    'input_params_path': input_params_path,
-                    'input_source_path': input_source_path
-            },
-            'out': {    'output_pdb_path': output_pdb_path,
-                        'output_top_path': output_top_path,
-                        'output_crd_path': output_crd_path }
+            'in': {'input_pdb_path': input_pdb_path,
+                   'input_lib_path': input_lib_path,
+                   'input_frcmod_path': input_frcmod_path,
+                   'input_params_path': input_params_path,
+                   'input_source_path': input_source_path},
+            'out': {'output_pdb_path': output_pdb_path,
+                    'output_top_path': output_top_path,
+                    'output_crd_path': output_crd_path}
         }
 
         # Ligand Parameter lists
         self.ligands_lib_list = []
         if input_lib_path:
             self.ligands_lib_list.append(input_lib_path)
 
         self.ligands_frcmod_list = []
         if input_frcmod_path:
             self.ligands_frcmod_list.append(input_frcmod_path)
 
         # Properties specific for BB
         self.properties = properties
-        self.forcefield = properties.get('forcefield', ["protein.ff14SB","DNA.bsc1","gaff"])
+        self.forcefield = properties.get('forcefield', ["protein.ff14SB", "DNA.bsc1", "gaff"])
         self.water_type = properties.get('water_type', "TIP3PBOX")
         self.box_type = properties.get('box_type', "truncated_octahedron")
         self.ions_type = properties.get('ions_type', "ionsjc_tip3p")
         self.neutralise = properties.get('neutralise', True)
         self.ionic_concentration = properties.get('ionic_concentration', 50)
         self.positive_ions_number = properties.get('positive_ions_number', 0)
         self.positive_ions_type = properties.get('positive_ions_type', "Na+")
@@ -128,54 +129,55 @@
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_pdb_path"] = check_input_path(self.io_dict["in"]["input_pdb_path"], "input_pdb_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_lib_path"] = check_input_path(self.io_dict["in"]["input_lib_path"], "input_lib_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_frcmod_path"] = check_input_path(self.io_dict["in"]["input_frcmod_path"], "input_frcmod_path", True, out_log, self.__class__.__name__)
-        #self.io_dict["in"]["input_params_path"] = check_input_path(self.io_dict["in"]["input_params_path"], "input_params_path", True, out_log, self.__class__.__name__)
-        #self.io_dict["in"]["input_source_path"] = check_input_path(self.io_dict["in"]["input_source_path"], "input_source_path", True, out_log, self.__class__.__name__)
+        # self.io_dict["in"]["input_params_path"] = check_input_path(self.io_dict["in"]["input_params_path"], "input_params_path", True, out_log, self.__class__.__name__)
+        # self.io_dict["in"]["input_source_path"] = check_input_path(self.io_dict["in"]["input_source_path"], "input_source_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"],"output_top_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"],"output_crd_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"], "output_top_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"], "output_crd_path", False, out_log, self.__class__.__name__)
 
     def find_out_number_of_ions(self):
         """ Computes the number of positive and negative ions from the input ionic
         concentration and the number of water molecules in the system box."""
 
-        # Finding number of water molecules in the box
+        # Finding number of water molecules in the box
         cnt = 0
         with open(self.io_dict['in']['input_pdb_path']) as fp:
-           for line in fp:
-               # Water molecules are identified with different resids
-               # by different forcefields / MD packages
-               pq = re.compile((r'WAT|HOH|TP3|TIP3|SOL'), re.M)
-               if pq.search(line):
-                   # Incrementing number of water molecules just in the water
-                   # oxygen atom, ignoring hydrogen atoms
-                   pq2 = re.compile(r"H", re.M)
-                   if not pq2.search(line):
-                       cnt = cnt + 1
+            for line in fp:
+                # Water molecules are identified with different resids
+                # by different forcefields / MD packages
+                pq = re.compile((r'WAT|HOH|TP3|TIP3|SOL'), re.M)
+                if pq.search(line):
+                    # Incrementing number of water molecules just in the water
+                    # oxygen atom, ignoring hydrogen atoms
+                    pq2 = re.compile(r"H", re.M)
+                    if not pq2.search(line):
+                        cnt = cnt + 1
 
         # To get to X mM ions we need
         # n(NaCl) = #waters / 55 Mol * X M
         # where X M = X mM / 1000
         self.nio = int((cnt / 55) * (self.ionic_concentration / 1000))
 
     @launchlogger
     def launch(self):
         """Launches the execution of the LeapAddIons module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Water Type
         # leaprc.water.tip4pew, tip4pd, tip3p, spceb, spce, opc, fb4, fb3
         # Values: POL3BOX, QSPCFWBOX, SPCBOX, SPCFWBOX, TIP3PBOX, TIP3PFBOX, TIP4PBOX, TIP4PEWBOX, OPCBOX, OPC3BOX, TIP5PBOX.
         source_wat_command = "source leaprc.water.tip3p"
         if self.water_type == "TIP4PEWBOX":
@@ -186,33 +188,33 @@
             source_wat_command = "source leaprc.water.spce"
         if re.match(r"OPC", self.water_type):
             source_wat_command = "source leaprc.water.opc"
 
         # Counterions
         ions_command = ""
         if self.neutralise:
-            #ions_command = ions_command + "addions mol " + self.negative_ions_type + " 0 \n"
-            #ions_command = ions_command + "addions mol " + self.positive_ions_type + " 0 \n"
+            # ions_command = ions_command + "addions mol " + self.negative_ions_type + " 0 \n"
+            # ions_command = ions_command + "addions mol " + self.positive_ions_type + " 0 \n"
             ions_command = ions_command + "addionsRand mol " + self.negative_ions_type + " 0 \n"
             ions_command = ions_command + "addionsRand mol " + self.positive_ions_type + " 0 \n"
 
-        if self.ionic_concentration and self.negative_ions_number==0 and self.positive_ions_number==0:
+        if self.ionic_concentration and self.negative_ions_number == 0 and self.positive_ions_number == 0:
             self.find_out_number_of_ions()
-            nneg = self.nio # Update with function
-            npos = self.nio # Update with function
-            #ions_command = ions_command + "addions mol " + self.negative_ions_type + " " + str(nneg) + " \n"
-            #ions_command = ions_command + "addions mol " + self.positive_ions_type + " " + str(npos) + " \n"
+            nneg = self.nio  # Update with function
+            npos = self.nio  # Update with function
+            # ions_command = ions_command + "addions mol " + self.negative_ions_type + " " + str(nneg) + " \n"
+            # ions_command = ions_command + "addions mol " + self.positive_ions_type + " " + str(npos) + " \n"
             ions_command = ions_command + "addionsRand mol " + self.negative_ions_type + " " + str(nneg) + " \n"
             ions_command = ions_command + "addionsRand mol " + self.positive_ions_type + " " + str(npos) + " \n"
         else:
             if self.negative_ions_number != 0:
-                #ions_command = ions_command + "addions mol " + self.negative_ions_type + " " + str(self.negative_ions_number) + " \n"
+                # ions_command = ions_command + "addions mol " + self.negative_ions_type + " " + str(self.negative_ions_number) + " \n"
                 ions_command = ions_command + "addionsRand mol " + self.negative_ions_type + " " + str(self.negative_ions_number) + " \n"
             if self.positive_ions_number != 0:
-                #ions_command = ions_command + "addions mol " + self.positive_ions_type + " " + str(self.positive_ions_number) + " \n"
+                # ions_command = ions_command + "addions mol " + self.positive_ions_type + " " + str(self.positive_ions_number) + " \n"
                 ions_command = ions_command + "addionsRand mol " + self.positive_ions_type + " " + str(self.positive_ions_number) + " \n"
 
         ligands_lib_list = []
         if self.io_dict['in']['input_lib_path'] is not None:
             if self.io_dict['in']['input_lib_path'].endswith('.zip'):
                 ligands_lib_list = fu.unzip_list(self.stage_io_dict['in']['input_lib_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
@@ -246,67 +248,67 @@
             self.tmp_folder = None
         else:
             self.tmp_folder = fu.create_unique_dir()
             instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             instructions_file_path = instructions_file
 
-        #instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
+        # instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
         with open(instructions_file, 'w') as leapin:
-                # Forcefields loaded by default:
-                # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
-                #leapin.write("source leaprc.protein.ff14SB \n")
-                # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
-                #leapin.write("source leaprc.DNA.bsc1 \n")
-                # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
-                #leapin.write("source leaprc.gaff \n")
-
-                # Forcefields loaded from input forcefield property
-                for t in self.forcefield:
-                    leapin.write("source leaprc.{}\n".format(t))
-
-                # Additional Leap commands
-                for leap_commands in leap_source_list:
-                    leapin.write("source " + leap_commands + "\n")
-
-                # Water Model loaded from input water_model property
-                leapin.write(source_wat_command + " \n")
-
-                # Ions Type
-                if self.ions_type != "None":
-                    leapin.write("loadamberparams frcmod." + self.ions_type + "\n")
-
-                # Additional Amber parameters
-                for amber_params in amber_params_list:
-                    leapin.write("loadamberparams " + amber_params + "\n")
-
-                # Ligand(s) libraries (if any)
-                for amber_lib in ligands_lib_list:
-                    leapin.write("loadOff " + amber_lib + "\n")
-                for amber_frcmod in ligands_frcmod_list:
-                    leapin.write("loadamberparams " + amber_frcmod + "\n")
-
-                # Loading PDB file
-                leapin.write("mol = loadpdb " + self.stage_io_dict['in']['input_pdb_path'] + " \n")
-
-                # Adding ions
-                leapin.write(ions_command)
-
-                # Generating box
-                leapin.write("setBox mol vdw \n")
-
-                # Saving output PDB file, coordinates and topology
-                leapin.write("savepdb mol " + self.stage_io_dict['out']['output_pdb_path'] + " \n")
-                leapin.write("saveAmberParm mol " + self.stage_io_dict['out']['output_top_path'] + " " + self.stage_io_dict['out']['output_crd_path'] + "\n")
-                leapin.write("quit \n");
+            # Forcefields loaded by default:
+            # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
+            # leapin.write("source leaprc.protein.ff14SB \n")
+            # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
+            # leapin.write("source leaprc.DNA.bsc1 \n")
+            # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
+            # leapin.write("source leaprc.gaff \n")
+
+            # Forcefields loaded from input forcefield property
+            for t in self.forcefield:
+                leapin.write("source leaprc.{}\n".format(t))
+
+            # Additional Leap commands
+            for leap_commands in leap_source_list:
+                leapin.write("source " + leap_commands + "\n")
+
+            # Water Model loaded from input water_model property
+            leapin.write(source_wat_command + " \n")
+
+            # Ions Type
+            if self.ions_type != "None":
+                leapin.write("loadamberparams frcmod." + self.ions_type + "\n")
+
+            # Additional Amber parameters
+            for amber_params in amber_params_list:
+                leapin.write("loadamberparams " + amber_params + "\n")
+
+            # Ligand(s) libraries (if any)
+            for amber_lib in ligands_lib_list:
+                leapin.write("loadOff " + amber_lib + "\n")
+            for amber_frcmod in ligands_frcmod_list:
+                leapin.write("loadamberparams " + amber_frcmod + "\n")
+
+            # Loading PDB file
+            leapin.write("mol = loadpdb " + self.stage_io_dict['in']['input_pdb_path'] + " \n")
+
+            # Adding ions
+            leapin.write(ions_command)
+
+            # Generating box
+            leapin.write("setBox mol vdw \n")
+
+            # Saving output PDB file, coordinates and topology
+            leapin.write("savepdb mol " + self.stage_io_dict['out']['output_pdb_path'] + " \n")
+            leapin.write("saveAmberParm mol " + self.stage_io_dict['out']['output_top_path'] + " " + self.stage_io_dict['out']['output_crd_path'] + "\n")
+            leapin.write("quit \n")
 
         # Command line
         self.cmd = [self.binary_path,
-               '-f', instructions_file_path
-               ]
+                    '-f', instructions_file_path
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -315,19 +317,19 @@
 
             # Taking box info from input PDB file, CRYST1 tag (first line)
             with open(self.io_dict['in']['input_pdb_path']) as file:
                 lines = file.readlines()
                 pdb_line = lines[0]
 
             if 'OCTBOX' not in pdb_line:
-                fu.log('WARNING: box info not found in input PDB file (OCTBOX). Needed to correctly assign the octahedron box. Assuming cubic box.',self.out_log, self.global_log)
+                fu.log('WARNING: box info not found in input PDB file (OCTBOX). Needed to correctly assign the octahedron box. Assuming cubic box.', self.out_log, self.global_log)
             else:
                 # PDB info: CRYST1   86.316   86.316   86.316 109.47 109.47 109.47 P 1
                 # PDB info: OCTBOX   86.1942924  86.1942924  86.1942924 109.4712190 109.4712190 109.4712190
-                #regex_box = 'CRYST1\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*P 1'
+                # regex_box = 'CRYST1\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*P 1'
                 regex_box = r'OCTBOX\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)\s*(\d+\.\d+)'
                 box = re.findall(regex_box, pdb_line)[0]
                 box_line = ""
                 for coord in box:
                     box_line += "{:12.7f}".format(float(coord))
 
                 # PRMTOP info: 1.09471219E+02  8.63157502E+01  8.63157502E+01  8.63157502E+01
@@ -341,45 +343,45 @@
                 with open(self.io_dict['out']['output_crd_path']) as file:
                     lines = file.readlines()
                     crd_lines = lines[:-1]
 
                 # Adding old box coordinates (taken from the input pdb)
                 crd_lines.append(box_line)
 
-                with open(self.io_dict['out']['output_crd_path'],'w') as file:
+                with open(self.io_dict['out']['output_crd_path'], 'w') as file:
                     for line in crd_lines:
                         file.write(str(line))
                     file.write("\n")
 
                 # Now fixing IFBOX param in prmtop.
                 box_flag = False
                 ifbox_flag = 0
-                #%FLAG BOX_DIMENSIONS
-                #%FORMAT(5E16.8)
-                #1.09471219E+02  8.63157502E+01  8.63157502E+01  8.63157502E+01
+                # %FLAG BOX_DIMENSIONS
+                # %FORMAT(5E16.8)
+                # 1.09471219E+02  8.63157502E+01  8.63157502E+01  8.63157502E+01
 
                 tmp_parmtop = str(PurePath(self.tmp_folder).joinpath("top_temp.parmtop"))
                 shutil.copyfile(self.io_dict['out']['output_top_path'], tmp_parmtop)
 
-                with open(self.io_dict['out']['output_top_path'],'w') as new_top:
-                    with open(tmp_parmtop,'r') as old_top:
+                with open(self.io_dict['out']['output_top_path'], 'w') as new_top:
+                    with open(tmp_parmtop, 'r') as old_top:
                         for line in old_top:
                             if 'BOX_DIMENSIONS' in line:
                                 box_flag = True
                                 new_top.write(line)
                             elif box_flag and 'FORMAT' not in line:
                                 new_top.write(top_box_line + "\n")
                                 box_flag = False
-                            elif 'FLAG POINTERS' in line or ifbox_flag==1 or ifbox_flag==2 or ifbox_flag==3:
-                                ifbox_flag+=1
+                            elif 'FLAG POINTERS' in line or ifbox_flag == 1 or ifbox_flag == 2 or ifbox_flag == 3:
+                                ifbox_flag += 1
                                 new_top.write(line)
                             elif ifbox_flag == 4:
-                                #new_top.write(top_box_line + "\n")
+                                # new_top.write(top_box_line + "\n")
                                 new_top.write(line[:56] + '       2' + line[64:])
-                                ifbox_flag+=1
+                                ifbox_flag += 1
                             else:
                                 new_top.write(line)
 
         # remove temporary folder(s)
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             self.tmp_folder,
@@ -387,31 +389,33 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def leap_add_ions(input_pdb_path: str, output_pdb_path: str,
-           output_top_path: str, output_crd_path: str,
-           input_lib_path: str = None, input_frcmod_path: str = None,
-           input_params_path: str = None, input_source_path: str = None,
-           properties: dict = None, **kwargs) -> int:
+                  output_top_path: str, output_crd_path: str,
+                  input_lib_path: str = None, input_frcmod_path: str = None,
+                  input_params_path: str = None, input_source_path: str = None,
+                  properties: dict = None, **kwargs) -> int:
     """Create :class:`LeapAddIons <leap.leap_add_ions.LeapAddIons>`leap.leap_add_ions.LeapAddIons class and
     execute :meth:`launch() <leap.leap_add_ions.LeapAddIons.launch>` method"""
 
-    return LeapAddIons( input_pdb_path=input_pdb_path,
-                        input_lib_path=input_lib_path,
-                        input_frcmod_path=input_frcmod_path,
-                        input_params_path=input_params_path,
-                        input_source_path=input_source_path,
-                        output_pdb_path=output_pdb_path,
-                        output_top_path=output_top_path,
-                        output_crd_path=output_crd_path,
-                        properties=properties).launch()
+    return LeapAddIons(input_pdb_path=input_pdb_path,
+                       input_lib_path=input_lib_path,
+                       input_frcmod_path=input_frcmod_path,
+                       input_params_path=input_params_path,
+                       input_source_path=input_source_path,
+                       output_pdb_path=output_pdb_path,
+                       output_top_path=output_top_path,
+                       output_crd_path=output_crd_path,
+                       properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Adds counterions to a system box for an AMBER MD system using tLeap.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -425,19 +429,20 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output coordinates file (AMBER crd). Accepted formats: crd.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    leap_add_ions(   input_pdb_path=args.input_pdb_path,
-                    input_lib_path=args.input_lib_path,
-                    input_frcmod_path=args.input_frcmod_path,
-                    input_params_path=args.input_params_path,
-                    input_source_path=args.input_source_path,
-                    output_pdb_path=args.output_pdb_path,
-                    output_top_path=args.output_top_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    leap_add_ions(input_pdb_path=args.input_pdb_path,
+                  input_lib_path=args.input_lib_path,
+                  input_frcmod_path=args.input_frcmod_path,
+                  input_params_path=args.input_params_path,
+                  input_source_path=args.input_source_path,
+                  output_pdb_path=args.output_pdb_path,
+                  output_top_path=args.output_top_path,
+                  output_crd_path=args.output_crd_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biobb_amber-3.9.0/biobb_amber/leap/leap_build_linear_structure.py` & `biobb_amber-4.0.0/biobb_amber/leap/leap_build_linear_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 
 """Module containing the LeapBuildLinearStructure class and the command line interface."""
 import argparse
-import shutil
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.leap.common import *
+from biobb_amber.leap.common import check_output_path
+
 
 class LeapBuildLinearStructure(BiobbObject):
     """
     | biobb_amber.leap.leap_build_linear_structure LeapBuildLinearStructure
     | Wrapper of the `AmberTools (AMBER MD Package) leap tool <https://ambermd.org/AmberTools.php>`_ module.
     | Builds a linear (unfolded) 3D structure from an AA sequence using tLeap tool from the AmberTools MD package.
 
@@ -62,76 +62,77 @@
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             'in': {},
-            'out': { 'output_pdb_path': output_pdb_path }
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.sequence = properties.get('sequence', "ALA GLY SER PRO ARG ALA PRO GLY")
-        self.forcefield = properties.get('forcefield', ["protein.ff14SB","DNA.bsc1","gaff"])
+        self.forcefield = properties.get('forcefield', ["protein.ff14SB", "DNA.bsc1", "gaff"])
         self.build_library = properties.get('build_library', False)
         self.binary_path = properties.get('binary_path', 'tleap')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the LeapBuildLinearStructure module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # create .in file
-        #TC5b = sequence { NASN LEU TYR ILE GLN TRP LEU LYS ASP GLY GLY PRO SER SER GLY ARG PRO PRO PRO CSER }
-        #savepdb TC5b TC5b_linear.pdb
-        #quit
+        # TC5b = sequence { NASN LEU TYR ILE GLN TRP LEU LYS ASP GLY GLY PRO SER SER GLY ARG PRO PRO PRO CSER }
+        # savepdb TC5b TC5b_linear.pdb
+        # quit
 
         # Creating temporary folder & Leap configuration (instructions) file
         if self.container_path:
             instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
             instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
             self.tmp_folder = None
         else:
             self.tmp_folder = fu.create_unique_dir()
             instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             instructions_file_path = instructions_file
 
-        #instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
+        # instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
         with open(instructions_file, 'w') as leapin:
 
-                # Forcefields loaded from input forcefield property
-                for t in self.forcefield:
-                    leapin.write("source leaprc.{}\n".format(t))
-
-                leapin.write("struct = sequence {" + self.sequence + " } \n")
-                leapin.write("savepdb struct " + self.stage_io_dict['out']['output_pdb_path'] + "\n")
-                leapin.write("quit \n");
+            # Forcefields loaded from input forcefield property
+            for t in self.forcefield:
+                leapin.write("source leaprc.{}\n".format(t))
+
+            leapin.write("struct = sequence {" + self.sequence + " } \n")
+            leapin.write("savepdb struct " + self.stage_io_dict['out']['output_pdb_path'] + "\n")
+            leapin.write("quit \n")
 
         # Command line
         self.cmd = [self.binary_path,
-               '-f', instructions_file_path
-               ]
+                    '-f', instructions_file_path
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -143,22 +144,23 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def leap_build_linear_structure(output_pdb_path: str,
-           properties: dict = None, **kwargs) -> int:
+                                properties: dict = None, **kwargs) -> int:
     """Create :class:`LeapBuildLinearStructure <leap.leap_build_linear_structure.LeapBuildLinearStructure>`leap.leap_build_linear_structure.LeapBuildLinearStructure class and
     execute :meth:`launch() <leap.leap_build_linear_structure.LeapBuildLinearStructure.launch>` method"""
 
-    return LeapBuildLinearStructure(
-                        output_pdb_path=output_pdb_path,
-                        properties=properties).launch()
+    return LeapBuildLinearStructure(output_pdb_path=output_pdb_path,
+                                    properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Building a linear (unfolded) 3D structure from an AA sequence.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -166,11 +168,12 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
     leap_build_linear_structure(output_pdb_path=args.output_pdb_path,
-             properties=properties)
+                                properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/leap/leap_gen_top.py` & `biobb_amber-4.0.0/biobb_amber/leap/leap_gen_top.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 
 """Module containing the LeapGenTop class and the command line interface."""
 import argparse
-import shutil
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.leap.common import *
+from biobb_amber.leap.common import check_input_path, check_output_path
+
 
 class LeapGenTop(BiobbObject):
     """
     | biobb_amber.leap.leap_gen_top LeapGenTop
     | Wrapper of the `AmberTools (AMBER MD Package) leap tool <https://ambermd.org/AmberTools.php>`_ module.
     | Generates a MD topology from a molecule structure using tLeap tool from the AmberTools MD package.
 
@@ -58,80 +58,80 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_pdb_path: str, output_pdb_path: str,
-    output_top_path: str, output_crd_path: str,
-    input_lib_path: str = None, input_frcmod_path: str = None,
-    input_params_path: str = None, input_source_path: str = None,
-    properties: dict = None, **kwargs):
+                 output_top_path: str, output_crd_path: str,
+                 input_lib_path: str = None, input_frcmod_path: str = None,
+                 input_params_path: str = None, input_source_path: str = None,
+                 properties: dict = None, **kwargs):
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path,
-                    'input_lib_path': input_lib_path,
-                    'input_frcmod_path': input_frcmod_path,
-                    'input_params_path': input_params_path,
-                    'input_source_path': input_source_path
-             },
-            'out': {    'output_pdb_path': output_pdb_path,
-                        'output_top_path': output_top_path,
-                        'output_crd_path': output_crd_path }
+            'in': {'input_pdb_path': input_pdb_path,
+                   'input_lib_path': input_lib_path,
+                   'input_frcmod_path': input_frcmod_path,
+                   'input_params_path': input_params_path,
+                   'input_source_path': input_source_path},
+            'out': {'output_pdb_path': output_pdb_path,
+                    'output_top_path': output_top_path,
+                    'output_crd_path': output_crd_path}
         }
 
         # # Ligand Parameter lists
         # self.ligands_lib_list = []
         # if input_lib_path:
         #     self.ligands_lib_list.append(input_lib_path)
         #
         # self.ligands_frcmod_list = []
         # if input_frcmod_path:
         #     self.ligands_frcmod_list.append(input_frcmod_path)
 
         # Properties specific for BB
         self.properties = properties
-        self.forcefield = properties.get('forcefield', ["protein.ff14SB","DNA.bsc1","gaff"])
+        self.forcefield = properties.get('forcefield', ["protein.ff14SB", "DNA.bsc1", "gaff"])
         self.binary_path = properties.get('binary_path', 'tleap')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_pdb_path"] = check_input_path(self.io_dict["in"]["input_pdb_path"], "input_pdb_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_lib_path"] = check_input_path(self.io_dict["in"]["input_lib_path"], "input_lib_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_frcmod_path"] = check_input_path(self.io_dict["in"]["input_frcmod_path"], "input_frcmod_path", True, out_log, self.__class__.__name__)
-        #self.io_dict["in"]["input_params_path"] = check_input_path(self.io_dict["in"]["input_params_path"], "input_params_path", True, out_log, self.__class__.__name__)
-        #self.io_dict["in"]["input_source_path"] = check_input_path(self.io_dict["in"]["input_source_path"], "input_source_path", True, out_log, self.__class__.__name__)
+        # self.io_dict["in"]["input_params_path"] = check_input_path(self.io_dict["in"]["input_params_path"], "input_params_path", True, out_log, self.__class__.__name__)
+        # self.io_dict["in"]["input_source_path"] = check_input_path(self.io_dict["in"]["input_source_path"], "input_source_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"],"output_top_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"],"output_crd_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"], "output_top_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"], "output_crd_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the LeapGenTop module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         ligands_lib_list = []
         if self.io_dict['in']['input_lib_path'] is not None:
             if self.io_dict['in']['input_lib_path'].endswith('.zip'):
                 ligands_lib_list = fu.unzip_list(self.stage_io_dict['in']['input_lib_path'], dest_dir=self.tmp_folder, out_log=self.out_log)
             else:
@@ -166,55 +166,55 @@
         else:
             self.tmp_folder = fu.create_unique_dir()
             instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             instructions_file_path = instructions_file
 
         with open(instructions_file, 'w') as leapin:
-                # Forcefields loaded by default:
-                # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
-                #leapin.write("source leaprc.protein.ff14SB \n")
-                # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
-                #leapin.write("source leaprc.DNA.bsc1 \n")
-                # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
-                #leapin.write("source leaprc.gaff \n")
-
-                # Forcefields loaded from input forcefield property
-                for t in self.forcefield:
-                    leapin.write("source leaprc.{}\n".format(t))
-
-                # Additional Leap commands
-                for leap_commands in leap_source_list:
-                    leapin.write("source " + leap_commands + "\n")
-
-                # Additional Amber parameters
-                for amber_params in amber_params_list:
-                    leapin.write("loadamberparams " + amber_params + "\n")
-
-                # Ions libraries
-                leapin.write("loadOff atomic_ions.lib \n")
-                
-                # Ligand(s) libraries (if any)
-                for amber_lib in ligands_lib_list:
-                    leapin.write("loadOff " + amber_lib + "\n")
-                for amber_frcmod in ligands_frcmod_list:
-                    leapin.write("loadamberparams " + amber_frcmod + "\n")
-
-                # Loading PDB file
-                leapin.write("mol = loadpdb " + self.stage_io_dict['in']['input_pdb_path'] + " \n")
-
-                # Saving output PDB file, coordinates and topology
-                leapin.write("savepdb mol " + self.stage_io_dict['out']['output_pdb_path'] + " \n")
-                leapin.write("saveAmberParm mol " + self.stage_io_dict['out']['output_top_path'] + " " + self.stage_io_dict['out']['output_crd_path'] + "\n")
-                leapin.write("quit \n");
+            # Forcefields loaded by default:
+            # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
+            # leapin.write("source leaprc.protein.ff14SB \n")
+            # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
+            # leapin.write("source leaprc.DNA.bsc1 \n")
+            # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
+            # leapin.write("source leaprc.gaff \n")
+
+            # Forcefields loaded from input forcefield property
+            for t in self.forcefield:
+                leapin.write("source leaprc.{}\n".format(t))
+
+            # Additional Leap commands
+            for leap_commands in leap_source_list:
+                leapin.write("source " + leap_commands + "\n")
+
+            # Additional Amber parameters
+            for amber_params in amber_params_list:
+                leapin.write("loadamberparams " + amber_params + "\n")
+
+            # Ions libraries
+            leapin.write("loadOff atomic_ions.lib \n")
+
+            # Ligand(s) libraries (if any)
+            for amber_lib in ligands_lib_list:
+                leapin.write("loadOff " + amber_lib + "\n")
+            for amber_frcmod in ligands_frcmod_list:
+                leapin.write("loadamberparams " + amber_frcmod + "\n")
+
+            # Loading PDB file
+            leapin.write("mol = loadpdb " + self.stage_io_dict['in']['input_pdb_path'] + " \n")
+
+            # Saving output PDB file, coordinates and topology
+            leapin.write("savepdb mol " + self.stage_io_dict['out']['output_pdb_path'] + " \n")
+            leapin.write("saveAmberParm mol " + self.stage_io_dict['out']['output_top_path'] + " " + self.stage_io_dict['out']['output_crd_path'] + "\n")
+            leapin.write("quit \n")
 
         # Command line
         self.cmd = [self.binary_path,
-               '-f', instructions_file_path
-               ]
+                    '-f', instructions_file_path
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -226,31 +226,33 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def leap_gen_top(input_pdb_path: str, output_pdb_path: str,
-           output_top_path: str, output_crd_path: str,
-           input_lib_path: str = None, input_frcmod_path: str = None,
-           input_params_path: str = None, input_source_path: str = None,
-           properties: dict = None, **kwargs) -> int:
+                 output_top_path: str, output_crd_path: str,
+                 input_lib_path: str = None, input_frcmod_path: str = None,
+                 input_params_path: str = None, input_source_path: str = None,
+                 properties: dict = None, **kwargs) -> int:
     """Create :class:`LeapGenTop <leap.leap_gen_top.LeapGenTop>`leap.leap_gen_top.LeapGenTop class and
     execute :meth:`launch() <leap.leap_gen_top.LeapGenTop.launch>` method"""
 
-    return LeapGenTop( input_pdb_path=input_pdb_path,
-                        input_lib_path=input_lib_path,
-                        input_frcmod_path=input_frcmod_path,
-                        input_params_path=input_params_path,
-                        input_source_path=input_source_path,
-                        output_pdb_path=output_pdb_path,
-                        output_top_path=output_top_path,
-                        output_crd_path=output_crd_path,
-                        properties=properties).launch()
+    return LeapGenTop(input_pdb_path=input_pdb_path,
+                      input_lib_path=input_lib_path,
+                      input_frcmod_path=input_frcmod_path,
+                      input_params_path=input_params_path,
+                      input_source_path=input_source_path,
+                      output_pdb_path=output_pdb_path,
+                      output_top_path=output_top_path,
+                      output_crd_path=output_crd_path,
+                      properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generating a MD topology from a molecule structure using tLeap program from AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -264,19 +266,20 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output coordinates file (AMBER crd). Accepted formats: crd.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    leap_gen_top(     input_pdb_path=args.input_pdb_path,
-                    input_lib_path=args.input_lib_path,
-                    input_frcmod_path=args.input_frcmod_path,
-                    input_params_path=args.input_params_path,
-                    input_source_path=args.input_source_path,
-                    output_pdb_path=args.output_pdb_path,
-                    output_top_path=args.output_top_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    leap_gen_top(input_pdb_path=args.input_pdb_path,
+                 input_lib_path=args.input_lib_path,
+                 input_frcmod_path=args.input_frcmod_path,
+                 input_params_path=args.input_params_path,
+                 input_source_path=args.input_source_path,
+                 output_pdb_path=args.output_pdb_path,
+                 output_top_path=args.output_top_path,
+                 output_crd_path=args.output_crd_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biobb_amber-3.9.0/biobb_amber/leap/leap_solvate.py` & `biobb_amber-4.0.0/biobb_amber/leap/leap_solvate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
 """Module containing the LeapSolvate class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
+import re
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.leap.common import *
+from biobb_amber.leap.common import check_input_path, check_output_path
+
 
 class LeapSolvate(BiobbObject):
     """
     | biobb_amber LeapSolvate
     | Wrapper of the `AmberTools (AMBER MD Package) leap tool <https://ambermd.org/AmberTools.php>`_ module.
     | Creates and solvates a system box for an AMBER MD system using tLeap tool from the AmberTools MD package.
 
@@ -71,50 +72,49 @@
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
     def __init__(self, input_pdb_path: str, output_pdb_path: str,
-    output_top_path: str, output_crd_path: str,
-    input_lib_path: str = None, input_frcmod_path: str = None,
-    input_params_path: str = None, input_source_path: str = None,
-    properties: dict = None, **kwargs):
+                 output_top_path: str, output_crd_path: str,
+                 input_lib_path: str = None, input_frcmod_path: str = None,
+                 input_params_path: str = None, input_source_path: str = None,
+                 properties: dict = None, **kwargs):
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path,
-                    'input_lib_path': input_lib_path,
-                    'input_frcmod_path': input_frcmod_path,
-                    'input_params_path': input_params_path,
-                    'input_source_path': input_source_path
-            },
-            'out': {    'output_pdb_path': output_pdb_path,
-                        'output_top_path': output_top_path,
-                        'output_crd_path': output_crd_path }
+            'in': {'input_pdb_path': input_pdb_path,
+                   'input_lib_path': input_lib_path,
+                   'input_frcmod_path': input_frcmod_path,
+                   'input_params_path': input_params_path,
+                   'input_source_path': input_source_path},
+            'out': {'output_pdb_path': output_pdb_path,
+                    'output_top_path': output_top_path,
+                    'output_crd_path': output_crd_path}
         }
 
         # # Ligand Parameter lists
         # self.ligands_lib_list = []
         # if input_lib_path:
         #     self.ligands_lib_list.append(input_lib_path)
         #
         # self.ligands_frcmod_list = []
         # if input_frcmod_path:
         #     self.ligands_frcmod_list.append(input_frcmod_path)
 
         # Properties specific for BB
         self.properties = properties
-        self.forcefield = properties.get('forcefield', ["protein.ff14SB","DNA.bsc1","gaff"])
+        self.forcefield = properties.get('forcefield', ["protein.ff14SB", "DNA.bsc1", "gaff"])
         self.water_type = properties.get('water_type', "TIP3PBOX")
         self.box_type = properties.get('box_type', "truncated_octahedron")
         self.ions_type = properties.get('ions_type', "ionsjc_tip3p")
         self.neutralise = properties.get('neutralise', False)
         self.iso = properties.get('iso', False)
         self.positive_ions_number = properties.get('positive_ions_number', 0)
         self.positive_ions_type = properties.get('positive_ions_type', "Na+")
@@ -131,39 +131,40 @@
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_pdb_path"] = check_input_path(self.io_dict["in"]["input_pdb_path"], "input_pdb_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_lib_path"] = check_input_path(self.io_dict["in"]["input_lib_path"], "input_lib_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_frcmod_path"] = check_input_path(self.io_dict["in"]["input_frcmod_path"], "input_frcmod_path", True, out_log, self.__class__.__name__)
-        #self.io_dict["in"]["input_params_path"] = check_input_path(self.io_dict["in"]["input_params_path"], "input_params_path", True, out_log, self.__class__.__name__)
-        #self.io_dict["in"]["input_source_path"] = check_input_path(self.io_dict["in"]["input_source_path"], "input_source_path", True, out_log, self.__class__.__name__)
+        # self.io_dict["in"]["input_params_path"] = check_input_path(self.io_dict["in"]["input_params_path"], "input_params_path", True, out_log, self.__class__.__name__)
+        # self.io_dict["in"]["input_source_path"] = check_input_path(self.io_dict["in"]["input_source_path"], "input_source_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"],"output_top_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"],"output_crd_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"], "output_top_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_crd_path"] = check_output_path(self.io_dict["out"]["output_crd_path"], "output_crd_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the LeapSolvate module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         box_command = "solvateOct"
         if self.box_type == "cubic":
             box_command = "solvateBox"
 
         # Forcefield
-        #source_ff_command = "source leaprc." + self.forcefield
+        # source_ff_command = "source leaprc." + self.forcefield
 
         # Water Type
         # leaprc.water.tip4pew, tip4pd, tip3p, spceb, spce, opc, fb4, fb3
         # Values: POL3BOX, QSPCFWBOX, SPCBOX, SPCFWBOX, TIP3PBOX, TIP3PFBOX, TIP4PBOX, TIP4PEWBOX, OPCBOX, OPC3BOX, TIP5PBOX.
         source_wat_command = "source leaprc.water.tip3p"
         if self.water_type == "TIP4PEWBOX":
             source_wat_command = "leaprc.water.tip4pew"
@@ -221,66 +222,66 @@
         else:
             self.tmp_folder = fu.create_unique_dir()
             instructions_file = str(PurePath(self.tmp_folder).joinpath("leap.in"))
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             instructions_file_path = instructions_file
 
         with open(instructions_file, 'w') as leapin:
-                # Forcefields loaded by default:
-                # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
-                #leapin.write("source leaprc.protein.ff14SB \n")
-                # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
-                #leapin.write("source leaprc.DNA.bsc1 \n")
-                # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
-                #leapin.write("source leaprc.gaff \n")
-
-                # Forcefields loaded from input forcefield property
-                for t in self.forcefield:
-                    leapin.write("source leaprc.{}\n".format(t))
-
-                # Additional Leap commands
-                for leap_commands in leap_source_list:
-                    leapin.write("source " + leap_commands + "\n")
-
-                # Ions Type
-                if self.ions_type != "None":
-                    leapin.write("loadamberparams frcmod." + self.ions_type + "\n")
-
-                # Additional Amber parameters
-                for amber_params in amber_params_list:
-                    leapin.write("loadamberparams " + amber_params + "\n")
-
-                # Water Model loaded from input water_model property
-                leapin.write(source_wat_command + " \n")
-
-                # Ligand(s) libraries (if any)
-                for amber_lib in ligands_lib_list:
-                    leapin.write("loadOff " + amber_lib + "\n")
-                for amber_frcmod in ligands_frcmod_list:
-                    leapin.write("loadamberparams " + amber_frcmod + "\n")
-
-                # Loading PDB file
-                leapin.write("mol = loadpdb " + self.stage_io_dict['in']['input_pdb_path'] + " \n")
-
-                # Generating box + adding water molecules
-                leapin.write(box_command + " mol " + self.water_type + " " + str(self.distance_to_molecule) + " " + str(self.closeness))
-                leapin.write(" iso \n") if self.iso else leapin.write("\n")
-
-                # Adding counterions
-                leapin.write(ions_command)
-
-                # Saving output PDB file, coordinates and topology
-                leapin.write("savepdb mol " + self.stage_io_dict['out']['output_pdb_path'] + " \n")
-                leapin.write("saveAmberParm mol " + self.stage_io_dict['out']['output_top_path'] + " " + self.stage_io_dict['out']['output_crd_path'] + "\n")
-                leapin.write("quit \n");
+            # Forcefields loaded by default:
+            # Protein: ff14SB (PARM99 + frcmod.ff99SB + frcmod.parmbsc0 + OL3 for RNA)
+            # leapin.write("source leaprc.protein.ff14SB \n")
+            # DNA: parmBSC1 (ParmBSC1 (ff99 + bsc0 + bsc1) for DNA. Ivani et al. Nature Methods 13: 55, 2016)
+            # leapin.write("source leaprc.DNA.bsc1 \n")
+            # Ligands: GAFF (General Amber Force field, J. Comput. Chem. 2004 Jul 15;25(9):1157-74)
+            # leapin.write("source leaprc.gaff \n")
+
+            # Forcefields loaded from input forcefield property
+            for t in self.forcefield:
+                leapin.write("source leaprc.{}\n".format(t))
+
+            # Additional Leap commands
+            for leap_commands in leap_source_list:
+                leapin.write("source " + leap_commands + "\n")
+
+            # Ions Type
+            if self.ions_type != "None":
+                leapin.write("loadamberparams frcmod." + self.ions_type + "\n")
+
+            # Additional Amber parameters
+            for amber_params in amber_params_list:
+                leapin.write("loadamberparams " + amber_params + "\n")
+
+            # Water Model loaded from input water_model property
+            leapin.write(source_wat_command + " \n")
+
+            # Ligand(s) libraries (if any)
+            for amber_lib in ligands_lib_list:
+                leapin.write("loadOff " + amber_lib + "\n")
+            for amber_frcmod in ligands_frcmod_list:
+                leapin.write("loadamberparams " + amber_frcmod + "\n")
+
+            # Loading PDB file
+            leapin.write("mol = loadpdb " + self.stage_io_dict['in']['input_pdb_path'] + " \n")
+
+            # Generating box + adding water molecules
+            leapin.write(box_command + " mol " + self.water_type + " " + str(self.distance_to_molecule))
+            leapin.write(" iso " + str(self.closeness) + "\n") if self.iso else leapin.write(" " + str(self.closeness) + "\n")
+
+            # Adding counterions
+            leapin.write(ions_command)
+
+            # Saving output PDB file, coordinates and topology
+            leapin.write("savepdb mol " + self.stage_io_dict['out']['output_pdb_path'] + " \n")
+            leapin.write("saveAmberParm mol " + self.stage_io_dict['out']['output_top_path'] + " " + self.stage_io_dict['out']['output_crd_path'] + "\n")
+            leapin.write("quit \n")
 
         # Command line
         self.cmd = [self.binary_path,
-               '-f', instructions_file_path
-               ]
+                    '-f', instructions_file_path
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -306,31 +307,33 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def leap_solvate(input_pdb_path: str, output_pdb_path: str,
-           output_top_path: str, output_crd_path: str,
-           input_lib_path: str = None, input_frcmod_path: str = None,
-           input_params_path: str = None, input_source_path: str = None,
-           properties: dict = None, **kwargs) -> int:
+                 output_top_path: str, output_crd_path: str,
+                 input_lib_path: str = None, input_frcmod_path: str = None,
+                 input_params_path: str = None, input_source_path: str = None,
+                 properties: dict = None, **kwargs) -> int:
     """Create :class:`LeapSolvate <leap.leap_solvate.LeapSolvate>`leap.leap_solvate.LeapSolvate class and
     execute :meth:`launch() <leap.leap_solvate.LeapSolvate.launch>` method"""
 
-    return LeapSolvate( input_pdb_path=input_pdb_path,
-                        input_lib_path=input_lib_path,
-                        input_frcmod_path=input_frcmod_path,
-                        input_params_path=input_params_path,
-                        input_source_path=input_source_path,
-                        output_pdb_path=output_pdb_path,
-                        output_top_path=output_top_path,
-                        output_crd_path=output_crd_path,
-                        properties=properties).launch()
+    return LeapSolvate(input_pdb_path=input_pdb_path,
+                       input_lib_path=input_lib_path,
+                       input_frcmod_path=input_frcmod_path,
+                       input_params_path=input_params_path,
+                       input_source_path=input_source_path,
+                       output_pdb_path=output_pdb_path,
+                       output_top_path=output_top_path,
+                       output_crd_path=output_crd_path,
+                       properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generating and solvating a system box for an AMBER MD system. using tLeap program from AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -344,19 +347,20 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output coordinates file (AMBER crd). Accepted formats: crd.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    leap_solvate(    input_pdb_path=args.input_pdb_path,
-                    input_lib_path=args.input_lib_path,
-                    input_frcmod_path=args.input_frcmod_path,
-                    input_params_path=args.input_params_path,
-                    input_source_path=args.input_source_path,
-                    output_pdb_path=args.output_pdb_path,
-                    output_top_path=args.output_top_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    leap_solvate(input_pdb_path=args.input_pdb_path,
+                 input_lib_path=args.input_lib_path,
+                 input_frcmod_path=args.input_frcmod_path,
+                 input_params_path=args.input_params_path,
+                 input_source_path=args.input_source_path,
+                 output_pdb_path=args.output_pdb_path,
+                 output_top_path=args.output_top_path,
+                 output_crd_path=args.output_crd_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/nab/nab_build_dna_structure.py` & `biobb_amber-4.0.0/biobb_amber/nab/nab_build_dna_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 
 """Module containing the NabBuildDNAStructure class and the command line interface."""
 import argparse
-import shutil
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.nab.common import *
+from biobb_amber.nab.common import check_output_path
+
 
 class NabBuildDNAStructure(BiobbObject):
     """
     | biobb_amber.nab.nab_build_dna_structure NabBuildDNAStructure
     | Wrapper of the `AmberTools (AMBER MD Package) nab tool <https://ambermd.org/AmberTools.php>`_ module.
     | Builds a 3D structure from a DNA sequence using nab (Nucleic Acid Builder) tool from the AmberTools MD package.
 
@@ -61,15 +61,15 @@
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             'in': {},
-            'out': { 'output_pdb_path': output_pdb_path }
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.sequence = properties.get('sequence', "GCGCGGCTGATAAACGAAAGC")
         self.helix_type = properties.get('helix_type', "lbdna")
         self.compiler = properties.get('compiler', "gcc")
@@ -80,30 +80,31 @@
         self.check_properties(properties)
         self.check_arguments()
 
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the NabBuildDNAStructure module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
-        #self.tmp_folder = fu.create_unique_dir()
-        #fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+        # self.tmp_folder = fu.create_unique_dir()
+        # fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         # create .nab file
         # molecule m;
         # m = fd_helix( "abdna", "aaaaaaaaaa", "dna" );
         # putpdb( "nuc.pdb", m, "-wwpdb");
 
         acid_type = 'dna'
@@ -117,37 +118,37 @@
             self.tmp_folder = None
         else:
             self.tmp_folder = fu.create_unique_dir()
             instructions_file = str(PurePath(self.tmp_folder).joinpath("nuc.nab"))
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             instructions_file_path = instructions_file
 
-        #instructions_file = str(PurePath(self.tmp_folder).joinpath("nuc.nab"))
+        # instructions_file = str(PurePath(self.tmp_folder).joinpath("nuc.nab"))
         with open(instructions_file, 'w') as nabin:
-                nabin.write("molecule m; \n")
-                nabin.write("m = fd_helix( \"" + self.helix_type + "\", \"" + self.sequence + "\", \"" + acid_type + "\" ); \n")
-                nabin.write("putpdb( \"" + self.stage_io_dict['out']['output_pdb_path'] + "\" , m, \"-wwpdb\");\n")
+            nabin.write("molecule m; \n")
+            nabin.write("m = fd_helix( \"" + self.helix_type + "\", \"" + self.sequence + "\", \"" + acid_type + "\" ); \n")
+            nabin.write("putpdb( \"" + self.stage_io_dict['out']['output_pdb_path'] + "\" , m, \"-wwpdb\");\n")
 
         # Command line
-        if self.container_path: 
+        if self.container_path:
             nuc_path = self.container_volume_path
             self.cmd = [self.binary_path,
-                '--compile', self.compiler,
-                '-Xlinker', self.linker,
-                instructions_file_path,
-                ' ; ' + nuc_path +'/nuc'
-                ]
-        else: 
+                        '--compile', self.compiler,
+                        '-Xlinker', self.linker,
+                        instructions_file_path,
+                        ' ; ' + nuc_path + '/nuc'
+                        ]
+        else:
             nuc_path = './' + self.tmp_folder
             self.cmd = [self.binary_path,
-                '--compiler', self.compiler,
-                '--linker', self.linker,
-                instructions_file_path,
-                ' ; ' + nuc_path +'/nuc'
-                ]
+                        '--compiler', self.compiler,
+                        '--linker', self.linker,
+                        instructions_file_path,
+                        ' ; ' + nuc_path + '/nuc'
+                        ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -160,21 +161,23 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def nab_build_dna_structure(output_pdb_path: str,
-           properties: dict = None, **kwargs) -> int:
+                            properties: dict = None, **kwargs) -> int:
     """Create :class:`NabBuildDNAStructure <nab.nab_build_dna_structure.NabBuildDNAStructure>`nab.nab_build_dna_structure.NabBuildDNAStructure class and
     execute :meth:`launch() <nab.nab_build_dna_structure.NabBuildDNAStructure.launch>` method"""
 
-    return NabBuildDNAStructure( output_pdb_path=output_pdb_path,
-                        properties=properties).launch()
+    return NabBuildDNAStructure(output_pdb_path=output_pdb_path,
+                                properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Building a 3D structure from a DNA sequence using nab.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -182,11 +185,12 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
     nab_build_dna_structure(output_pdb_path=args.output_pdb_path,
-             properties=properties)
+                            properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/parmed/parmed_cpinutil.py` & `biobb_amber-4.0.0/biobb_amber/parmed/parmed_cpinutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the ParmedCpinUtil class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.parmed.common import *
+from biobb_amber.parmed.common import check_input_path, check_output_path
+
 
 class ParmedCpinUtil(BiobbObject):
     """
     | biobb_amber ParmedCpinUtil
     | Wrapper of the `AmberTools (AMBER MD Package) parmed tool <https://ambermd.org/AmberTools.php>`_ module.
     | Creates a cpin file for constant pH simulations from an AMBER topology file using parmed tool from the AmberTools MD package.
 
@@ -66,17 +65,17 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_top_path': input_top_path },
-            'out': {    'output_cpin_path': output_cpin_path,
-                        'output_top_path': output_top_path }
+            'in': {'input_top_path': input_top_path},
+            'out': {'output_cpin_path': output_cpin_path,
+                    'output_top_path': output_top_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.resnames = properties.get('resnames')
         self.igb = properties.get('igb', 2)
         self.system = properties.get('system', "Unknown")
@@ -89,41 +88,42 @@
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], "input_top_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_cpin_path"] = check_output_path(self.io_dict["out"]["output_cpin_path"],"output_cpin_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"],"output_top_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cpin_path"] = check_output_path(self.io_dict["out"]["output_cpin_path"], "output_cpin_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"], "output_top_path", True, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the ParmedCpinUtil module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         # cpinutil.py -igb 2 -resname AS4 GL4 -p $1.prmtop -op $1.cpH.prmtop
         # cpinutil.py -p cln025.cpH.prmtop -igb 2 -system "CLN" -o cpin
 
         fu.log('Creating command line with instructions and required arguments', self.out_log, self.global_log)
 
         self.cmd = [self.binary_path,
-               '-p', self.stage_io_dict['in']['input_top_path'],
-               '-o', self.stage_io_dict['out']['output_cpin_path']
-               ]
+                    '-p', self.stage_io_dict['in']['input_top_path'],
+                    '-o', self.stage_io_dict['out']['output_cpin_path']
+                    ]
 
         if self.igb:
             self.cmd.append('-igb')
             self.cmd.append(str(self.igb))
 
         if self.system:
             self.cmd.append('-system')
@@ -150,24 +150,26 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def parmed_cpinutil(input_top_path: str, output_cpin_path: str,
-           output_top_path: str = None,
-           properties: dict = None, **kwargs) -> int:
+                    output_top_path: str = None,
+                    properties: dict = None, **kwargs) -> int:
     """Create :class:`ParmedCpinUtil <parmed.parmed_cpinutil.ParmedCpinUtil>`parmed.parmed_cpinutil.ParmedCpinUtil class and
     execute :meth:`launch() <parmed.parmed_cpinutil.ParmedCpinUtil.launch>` method"""
 
-    return ParmedCpinUtil( input_top_path=input_top_path,
-                        output_cpin_path=output_cpin_path,
-                        output_top_path=output_top_path,
-                        properties=properties).launch()
+    return ParmedCpinUtil(input_top_path=input_top_path,
+                          output_cpin_path=output_cpin_path,
+                          output_top_path=output_top_path,
+                          properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='create a cpin file for constant pH simulations from an AMBER topology file using parmed program from AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -176,14 +178,15 @@
     required_args.add_argument('--output_top_path', required=False, help='Output topology file (AMBER ParmTop). Accepted formats: top, parmtop, prmtop.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    parmed_cpinutil(   input_top_path=args.input_top_path,
-                            output_cpin_path=args.output_cpin_path,
-                            output_top_path=args.output_top_path,
-                            properties=properties)
+    parmed_cpinutil(input_top_path=args.input_top_path,
+                    output_cpin_path=args.output_cpin_path,
+                    output_top_path=args.output_top_path,
+                    properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/parmed/parmed_hmassrepartition.py` & `biobb_amber-4.0.0/biobb_amber/parmed/parmed_hmassrepartition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 
 """Module containing the ParmedHMassRepartition class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
+from pathlib import PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.parmed.common import *
+from biobb_amber.parmed.common import check_input_path, check_output_path
+
 
 class ParmedHMassRepartition(BiobbObject):
     """
     | biobb_amber ParmedHMassRepartition
     | Wrapper of the `AmberTools (AMBER MD Package) parmed tool <https://ambermd.org/AmberTools.php>`_ module.
     | Performs a Hydrogen Mass Repartition from an AMBER topology file using parmed tool from the AmberTools MD package.
 
@@ -54,16 +54,16 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_top_path': input_top_path },
-            'out': { 'output_top_path': output_top_path }
+            'in': {'input_top_path': input_top_path},
+            'out': {'output_top_path': output_top_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'parmed')
 
         # Check the properties
@@ -73,25 +73,26 @@
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], "input_top_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"],"output_top_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_top_path"] = check_output_path(self.io_dict["out"]["output_top_path"], "output_top_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the ParmedHMassRepartition module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder & Parmed configuration (instructions) file
         if self.container_path:
             instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("parmed.in"))
             instructions_file_path = str(PurePath(self.container_volume_path).joinpath("parmed.in"))
             self.tmp_folder = None
@@ -102,18 +103,18 @@
             instructions_file_path = instructions_file
 
         with open(instructions_file, 'w') as parmedin:
             parmedin.write("hmassrepartition\n")
             parmedin.write("outparm " + self.stage_io_dict['out']['output_top_path'] + "\n")
 
         self.cmd = [self.binary_path,
-               '-p', self.stage_io_dict['in']['input_top_path'],
-               '-i', instructions_file_path,
-               '-O' # Overwrite output files
-               ]
+                    '-p', self.stage_io_dict['in']['input_top_path'],
+                    '-i', instructions_file_path,
+                    '-O'  # Overwrite output files
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -124,23 +125,25 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def parmed_hmassrepartition(input_top_path: str,
-           output_top_path: str = None,
-           properties: dict = None, **kwargs) -> int:
+                            output_top_path: str = None,
+                            properties: dict = None, **kwargs) -> int:
     """Create :class:`ParmedHMassRepartition <parmed.parmed_hmassrepartition.ParmedHMassRepartition>`parmed.parmed_hmassrepartition.ParmedHMassRepartition class and
     execute :meth:`launch() <parmed.parmed_hmassrepartition.ParmedHMassRepartition.launch>` method"""
 
-    return ParmedHMassRepartition( input_top_path=input_top_path,
-                        output_top_path=output_top_path,
-                        properties=properties).launch()
+    return ParmedHMassRepartition(input_top_path=input_top_path,
+                                  output_top_path=output_top_path,
+                                  properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Performs a Hydrogen Mass Repartition from an AMBER topology file using parmed tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -148,13 +151,14 @@
     required_args.add_argument('--output_top_path', required=False, help='Output topology file (AMBER ParmTop). Accepted formats: top, parmtop, prmtop.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    parmed_hmassrepartition(   input_top_path=args.input_top_path,
+    parmed_hmassrepartition(input_top_path=args.input_top_path,
                             output_top_path=args.output_top_path,
                             properties=properties)
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/pdb4amber/pdb4amber_run.py` & `biobb_amber-4.0.0/biobb_amber/pdb4amber/pdb4amber_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the Pdb4amber class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.pdb4amber.common import *
+from biobb_amber.pdb4amber.common import check_input_path, check_output_path
+
 
 class Pdb4amberRun(BiobbObject):
     """
     | biobb_amber.pdb4amber.pdb4amber_run Pdb4amberRun
     | Wrapper of the `AmberTools (AMBER MD Package) pdb4amber tool <https://ambermd.org/AmberTools.php>`_ module.
     | Analyse PDB files and clean them for further usage, especially with the LEaP programs of Amber, using pdb4amber tool from the AmberTools MD package.
 
@@ -61,16 +60,16 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': { 'output_pdb_path': output_pdb_path }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.remove_hydrogens = properties.get('remove_hydrogens', False)
         self.remove_waters = properties.get('remove_waters', False)
         self.constant_pH = properties.get('constant_pH', False)
@@ -83,37 +82,38 @@
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_pdb_path"] = check_input_path(self.io_dict["in"]["input_pdb_path"], "input_pdb_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"],"output_pdb_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_pdb_path"] = check_output_path(self.io_dict["out"]["output_pdb_path"], "output_pdb_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the Pdb4amberRun module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
         # Command line
         # sander -O -i mdin/min.mdin -p $1.cpH.prmtop -c ph$i/$1.inpcrd -r ph$i/$1.min.rst7 -o ph$i/$1.min.o
         self.cmd = [self.binary_path,
-               '-i', self.stage_io_dict['in']['input_pdb_path'],
-               '-o', self.stage_io_dict['out']['output_pdb_path']
-               ]
+                    '-i', self.stage_io_dict['in']['input_pdb_path'],
+                    '-o', self.stage_io_dict['out']['output_pdb_path']
+                    ]
 
         if self.remove_hydrogens:
             self.cmd.append("-y ")
         if self.remove_waters:
             self.cmd.append("-d ")
         if self.constant_pH:
             self.cmd.append("--constantph ")
@@ -131,36 +131,39 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def pdb4amber_run(input_pdb_path: str, output_pdb_path: str,
-           properties: dict = None, **kwargs) -> int:
+                  properties: dict = None, **kwargs) -> int:
     """Create :class:`Pdb4amberRun <pdb4amber.pdb4amber_run.Pdb4amberRun>`pdb4amber.pdb4amber_run.Pdb4amberRun class and
     execute :meth:`launch() <pdb4amber.pdb4amber_run.Pdb4amberRun.launch>` method"""
 
-    return Pdb4amberRun( input_pdb_path=input_pdb_path,
+    return Pdb4amberRun(input_pdb_path=input_pdb_path,
                         output_pdb_path=output_pdb_path,
                         properties=properties).launch()
 
+
 def main():
     parser = argparse.ArgumentParser(description='Analyse PDB files and clean them for further usage, especially with the LEaP programs of Amber, using pdb4amber tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pdb_path', required=True, help='Input 3D structure PDB file. Accepted formats: pdb.')
     required_args.add_argument('--output_pdb_path', required=True, help='Output 3D structure PDB file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    pdb4amber_run(    input_pdb_path=args.input_pdb_path,
-                    output_pdb_path=args.output_pdb_path,
-                    properties=properties)
+    pdb4amber_run(input_pdb_path=args.input_pdb_path,
+                  output_pdb_path=args.output_pdb_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/pmemd/common.py` & `biobb_amber-4.0.0/biobb_amber/pmemd/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """ Common functions for package biobb_amber.pmemd """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 # CHECK OUTPUT PARAMETERS
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_top_path': ['top','prmtop','parmtop'],
-		'input_crd_path': ['crd','inpcrd','mdcrd','rst','rst7','netcdf','nc','ncrst'],
-		'input_mdin_path': ['mdin','txt','in'],
-		'input_cpin_path': ['cpin','txt','in'],
-		'input_ref_path': ['crd','inpcrd','mdcrd','rst','rst7','netcdf','nc','ncrst'],
-		'output_log_path': ['log','out','txt','o'],
-		'output_traj_path': ['trj', 'crd', 'mdcrd', 'x', 'netcdf', 'nc'],
-		'output_rst_path': ['rst', 'rst7','netcdf','nc','ncrst'],
-		'output_cpout_path': ['cpout'],
-		'output_cprst_path': ['cprst', 'rst', 'rst7'],
-		'output_mdinfo_path': ['mdinfo']
-	}
-	return ext in formats[argument]
+    """ Checks if file format is compatible """
+    formats = {
+        'input_top_path': ['top', 'prmtop', 'parmtop'],
+        'input_crd_path': ['crd', 'inpcrd', 'mdcrd', 'rst', 'rst7', 'netcdf', 'nc', 'ncrst'],
+        'input_mdin_path': ['mdin', 'txt', 'in'],
+        'input_cpin_path': ['cpin', 'txt', 'in'],
+        'input_ref_path': ['crd', 'inpcrd', 'mdcrd', 'rst', 'rst7', 'netcdf', 'nc', 'ncrst'],
+        'output_log_path': ['log', 'out', 'txt', 'o'],
+        'output_traj_path': ['trj', 'crd', 'mdcrd', 'x', 'netcdf', 'nc'],
+        'output_rst_path': ['rst', 'rst7', 'netcdf', 'nc', 'ncrst'],
+        'output_cpout_path': ['cpout'],
+        'output_cprst_path': ['cprst', 'rst', 'rst7'],
+        'output_mdinfo_path': ['mdinfo']
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_amber-3.9.0/biobb_amber/pmemd/pmemd_mdrun.py` & `biobb_amber-4.0.0/biobb_amber/pmemd/pmemd_mdrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
 """Module containing the PmemdMDRun class and the command line interface."""
 import argparse
-import shutil, re
-from pathlib import Path, PurePath
+import re
+from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.pmemd.common import *
+from biobb_amber.pmemd.common import check_input_path, check_output_path
+
 
 class PmemdMDRun(BiobbObject):
     """
     | biobb_amber PmemdMDRun
     | Wrapper of the `AmberTools (AMBER MD Package) pmemd tool <https://ambermd.org/AmberTools.php>`_ module.
     | Runs molecular dynamics using pmemd tool from the AMBER MD package.
 
@@ -74,25 +75,25 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_top_path': input_top_path,
-                    'input_crd_path': input_crd_path,
-                    'input_mdin_path': input_mdin_path,
-                    'input_ref_path': input_ref_path,
-                    'input_cpin_path': input_cpin_path },
-            'out': {    'output_log_path': output_log_path,
-                        'output_traj_path': output_traj_path,
-                        'output_rst_path': output_rst_path,
-                        'output_cpout_path': output_cpout_path,
-                        'output_cprst_path': output_cprst_path,
-                        'output_mdinfo_path': output_mdinfo_path }
+            'in': {'input_top_path': input_top_path,
+                   'input_crd_path': input_crd_path,
+                   'input_mdin_path': input_mdin_path,
+                   'input_ref_path': input_ref_path,
+                   'input_cpin_path': input_cpin_path},
+            'out': {'output_log_path': output_log_path,
+                    'output_traj_path': output_traj_path,
+                    'output_rst_path': output_rst_path,
+                    'output_cpout_path': output_cpout_path,
+                    'output_cprst_path': output_cprst_path,
+                    'output_mdinfo_path': output_mdinfo_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.simulation_type = properties.get('simulation_type', "minimization")
         self.binary_path = properties.get('binary_path', "pmemd")
         self.mdin = {k: str(v) for k, v in properties.get('mdin', dict()).items()}
@@ -113,20 +114,20 @@
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], "input_top_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_crd_path"] = check_input_path(self.io_dict["in"]["input_crd_path"], "input_crd_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_mdin_path"] = check_input_path(self.io_dict["in"]["input_mdin_path"], "input_mdin_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_cpin_path"] = check_input_path(self.io_dict["in"]["input_cpin_path"], "input_cpin_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_ref_path"] = check_input_path(self.io_dict["in"]["input_ref_path"], "input_ref_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"],"output_log_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_traj_path"] = check_output_path(self.io_dict["out"]["output_traj_path"],"output_traj_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_rst_path"] = check_output_path(self.io_dict["out"]["output_rst_path"],"output_rst_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_cpout_path"] = check_output_path(self.io_dict["out"]["output_cpout_path"],"output_cpout_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_cprst_path"] = check_output_path(self.io_dict["out"]["output_cprst_path"],"output_cprst_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_mdinfo_path"] = check_output_path(self.io_dict["out"]["output_mdinfo_path"],"output_mdinfo_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"], "output_log_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_traj_path"] = check_output_path(self.io_dict["out"]["output_traj_path"], "output_traj_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_rst_path"] = check_output_path(self.io_dict["out"]["output_rst_path"], "output_rst_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cpout_path"] = check_output_path(self.io_dict["out"]["output_cpout_path"], "output_cpout_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cprst_path"] = check_output_path(self.io_dict["out"]["output_cprst_path"], "output_cprst_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_mdinfo_path"] = check_output_path(self.io_dict["out"]["output_mdinfo_path"], "output_mdinfo_path", True, out_log, self.__class__.__name__)
 
     def create_mdin(self, path: str = None) -> str:
         """Creates an AMBER MD configuration file (mdin) using the properties file settings"""
         mdin_list = []
         mdin_firstPart = []
         mdin_middlePart = []
         mdin_lastPart = []
@@ -143,25 +144,25 @@
                 for line in input_params:
                     if '=' in line and not secondPart:
                         firstPart = False
                         mdin_middlePart.append(line.rstrip())
                     else:
                         if (firstPart):
                             mdin_firstPart.append(line.rstrip())
-                        elif(secondPart):
+                        elif (secondPart):
                             mdin_lastPart.append(line.rstrip())
                         else:
                             secondPart = True
                             mdin_lastPart.append(line.rstrip())
 
             for line in mdin_middlePart:
                 if ('!' in line or '#' in line) and not ('!@' in line or '!:' in line):
                     # Parsing lines with comments (#,!), e.g. :
                     # ntc=2, ntf=2, ! SHAKE, constrain lenghts of the bonds having H
-                    params = re.split('!|#',line)
+                    params = re.split('!|#', line)
                     for param in params[0].split(','):
                         if param.strip():
                             mdin_list.append("  " + param.strip() + " ! " + params[1])
                 elif ('@' in line or ':' in line):
                     # Parsing masks, e.g. :
                     # restraintmask = ":1-40@P,O5',C5',C4',C3',O3'", restraint_wt = 0.5
                     mylist = re.findall(r'(?:[^,"]|"(?:\\.|[^"])*")+', line)
@@ -173,15 +174,15 @@
                                 mdin_list.append("  " + param.strip())
 
         else:
             # MDIN parameters added by the biobb_amber module
             mdin_list.append("This mdin file has been created by the biobb_amber module from the BioBB library ")
 
             sim_type = self.properties.get('simulation_type', 'minimization')
-            #sim_type = self.mdin.get('simulation_type', 'minimization')
+            # sim_type = self.mdin.get('simulation_type', 'minimization')
             minimization = (sim_type == 'minimization')
             min_vacuo = (sim_type == 'min_vacuo')
             heat = (sim_type == 'heat')
             nvt = (sim_type == 'nvt')
             npt = (sim_type == 'npt')
             free = (sim_type == 'free')
             md = (nvt or npt or free or heat)
@@ -222,29 +223,29 @@
                 mdin_list.append("  gamma_ln = 5.0 ! BioBB simulation_type nvt")
                 mdin_list.append("  ntb = 1 ! BioBB simulation_type nvt")
                 mdin_list.append("  ntx = 5 ! BioBB simulation_type nvt")
             if heat:
                 mdin_list.append("  tempi = 0.0 ! BioBB simulation_type heat")
                 mdin_list.append("  temp0 = 300.0 ! BioBB simulation_type heat")
                 mdin_list.append("  irest = 0 ! BioBB simulation_type heat")
-                mdin_list.append("  ntb = 1 ! BioBB simulation_type heat") #periodic boundaries
+                mdin_list.append("  ntb = 1 ! BioBB simulation_type heat")  # periodic boundaries
                 mdin_list.append("  gamma_ln = 1.0 ! BioBB simulation_type heat")
-                #mdin_list.append("  nmropt = 1 ! BioBB simulation_type heat")
+                # mdin_list.append("  nmropt = 1 ! BioBB simulation_type heat")
 
-                #mdin_lastPart.append("/")
-                #mdin_lastPart.append("&wt")
-                #mdin_lastPart.append(" TYPE = 'TEMP0' ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" ISTEP1 = 1 ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" ISTEP2 = 4000 ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" VALUE1 = 10.0 ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" VALUE2 = 300.0 ! BioBB simulation_type heat")
-                #mdin_lastPart.append("/")
-                #mdin_lastPart.append("&wt")
-                #mdin_lastPart.append(" TYPE = 'END' ! BioBB simulation_type heat")
-                #mdin_lastPart.append("/")
+                # mdin_lastPart.append("/")
+                # mdin_lastPart.append("&wt")
+                # mdin_lastPart.append(" TYPE = 'TEMP0' ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" ISTEP1 = 1 ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" ISTEP2 = 4000 ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" VALUE1 = 10.0 ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" VALUE2 = 300.0 ! BioBB simulation_type heat")
+                # mdin_lastPart.append("/")
+                # mdin_lastPart.append("&wt")
+                # mdin_lastPart.append(" TYPE = 'END' ! BioBB simulation_type heat")
+                # mdin_lastPart.append("/")
 
         # Adding the rest of parameters in the config file to the mdin file
         # if the parameter has already been added replace the value
         parameter_keys = [parameter.split('=')[0].strip() for parameter in mdin_list]
         for k, v in self.mdin.items():
             config_parameter_key = str(k).strip()
             if config_parameter_key in parameter_keys:
@@ -276,38 +277,39 @@
     def launch(self):
         """Launches the execution of the PmemdMDRun module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
         self.tmp_folder = fu.create_unique_dir()
         fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
-        #if self.io_dict['in']['input_mdin_path']:
+        # if self.io_dict['in']['input_mdin_path']:
         #    self.output_mdin_path = self.io_dict['in']['input_mdin_path']
-        #else:
+        # else:
         #    self.output_mdin_path = self.create_mdin(path=str(Path(self.tmp_folder).joinpath("pmemd.mdin")))
         self.output_mdin_path = self.create_mdin(path=str(Path(self.tmp_folder).joinpath("pmemd.mdin")))
 
         # Command line
         # pmemd -O -i mdin/min.mdin -p $1.cpH.prmtop -c ph$i/$1.inpcrd -r ph$i/$1.min.rst7 -o ph$i/$1.min.o
         self.cmd = [self.binary_path,
-               '-O',
-               '-i', self.output_mdin_path,
-               '-p', self.io_dict['in']['input_top_path'],
-               '-c', self.io_dict['in']['input_crd_path'],
-               '-r', self.io_dict['out']['output_rst_path'],
-               '-o', self.io_dict['out']['output_log_path'],
-               '-x', self.io_dict['out']['output_traj_path']
-               ]
+                    '-O',
+                    '-i', self.output_mdin_path,
+                    '-p', self.io_dict['in']['input_top_path'],
+                    '-c', self.io_dict['in']['input_crd_path'],
+                    '-r', self.io_dict['out']['output_rst_path'],
+                    '-o', self.io_dict['out']['output_log_path'],
+                    '-x', self.io_dict['out']['output_traj_path']
+                    ]
 
         if self.io_dict['in']['input_ref_path']:
             self.cmd.append('-ref')
             self.cmd.append(self.io_dict['in']['input_ref_path'])
 
         if self.io_dict['in']['input_cpin_path']:
             self.cmd.append('-cpin')
@@ -349,35 +351,37 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def pmemd_mdrun(input_top_path: str, input_crd_path: str,
-            output_log_path: str, output_traj_path: str, output_rst_path: str,
-            input_mdin_path: str = None, input_cpin_path: str = None,
-            output_cpout_path: str = None, output_cprst_path: str = None,
-            output_mdinfo_path: str = None, input_ref_path: str=None,
-            properties: dict = None, **kwargs) -> int:
+                output_log_path: str, output_traj_path: str, output_rst_path: str,
+                input_mdin_path: str = None, input_cpin_path: str = None,
+                output_cpout_path: str = None, output_cprst_path: str = None,
+                output_mdinfo_path: str = None, input_ref_path: str = None,
+                properties: dict = None, **kwargs) -> int:
     """Create :class:`PmemdMDRun <pmemd.pmemd_mdrun.PmemdMDRun>`pmemd.pmemd_mdrun.PmemdMDRun class and
     execute :meth:`launch() <pmemd.pmemd_mdrun.PmemdMDRun.launch>` method"""
 
-    return PmemdMDRun( input_top_path=input_top_path,
-                    input_crd_path=input_crd_path,
-                    input_mdin_path=input_mdin_path,
-                    input_cpin_path=input_cpin_path,
-                    input_ref_path=input_ref_path,
-                    output_log_path=output_log_path,
-                    output_traj_path=output_traj_path,
-                    output_rst_path=output_rst_path,
-                    output_cpout_path=output_cpout_path,
-                    output_cprst_path=output_cprst_path,
-                    output_mdinfo_path=output_mdinfo_path,
-                    properties=properties).launch()
+    return PmemdMDRun(input_top_path=input_top_path,
+                      input_crd_path=input_crd_path,
+                      input_mdin_path=input_mdin_path,
+                      input_cpin_path=input_cpin_path,
+                      input_ref_path=input_ref_path,
+                      output_log_path=output_log_path,
+                      output_traj_path=output_traj_path,
+                      output_rst_path=output_rst_path,
+                      output_cpout_path=output_cpout_path,
+                      output_cprst_path=output_cprst_path,
+                      output_mdinfo_path=output_mdinfo_path,
+                      properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Running molecular dynamics using pmemd tool from the AMBER MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -394,22 +398,23 @@
     required_args.add_argument('--output_mdinfo_path', required=False, help='Output MD info. Accepted formats: mdinfo.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    pmemd_mdrun(    input_top_path=args.input_top_path,
-                    input_crd_path=args.input_crd_path,
-                    input_mdin_path=args.input_mdin_path,
-                    input_cpin_path=args.input_cpin_path,
-                    input_ref_path=args.input_ref_path,
-                    output_log_path=args.output_log_path,
-                    output_traj_path=args.output_traj_path,
-                    output_rst_path=args.output_rst_path,
-                    output_cpout_path=args.output_cpout_path,
-                    output_cprst_path=args.output_cprst_path,
-                    output_mdinfo_path=args.output_mdinfo_path,
-                    properties=properties)
+    pmemd_mdrun(input_top_path=args.input_top_path,
+                input_crd_path=args.input_crd_path,
+                input_mdin_path=args.input_mdin_path,
+                input_cpin_path=args.input_cpin_path,
+                input_ref_path=args.input_ref_path,
+                output_log_path=args.output_log_path,
+                output_traj_path=args.output_traj_path,
+                output_rst_path=args.output_rst_path,
+                output_cpout_path=args.output_cpout_path,
+                output_cprst_path=args.output_cprst_path,
+                output_mdinfo_path=args.output_mdinfo_path,
+                properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/process/process_mdout.py` & `biobb_amber-4.0.0/biobb_amber/process/process_mdout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
 """Module containing the ProcessMDOut class and the command line interface."""
 import argparse
 import shutil
 from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.process.common import *
+from biobb_amber.process.common import check_input_path, check_output_path
+
 
 class ProcessMDOut(BiobbObject):
     """
     | biobb_amber.process.process_mdout ProcessMDOut
     | Wrapper of the `AmberTools (AMBER MD Package) process_mdout tool <https://ambermd.org/AmberTools.php>`_ module.
     | Parses the AMBER (sander) md output file (log) and dumps statistics that can then be plotted. Using the process_mdout.pl tool from the AmberTools MD package.
 
@@ -59,16 +60,16 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_log_path': input_log_path },
-            'out': { 'output_dat_path': output_dat_path }
+            'in': {'input_log_path': input_log_path},
+            'out': {'output_dat_path': output_dat_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.terms = properties.get('terms', ["ETOT"])
         self.binary_path = properties.get('binary_path', 'process_mdout.perl')
 
@@ -79,39 +80,40 @@
     def check_data_params(self, out_log, err_log):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_log_path"] = check_input_path(self.io_dict["in"]["input_log_path"], "input_log_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"],"output_dat_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"], "output_dat_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the ProcessMDOut module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         if not self.container_path:
             self.tmp_folder = fu.create_unique_dir()
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             self.cmd = ['cd', self.tmp_folder, ';',
-                self.binary_path,
-                str(Path(self.stage_io_dict['in']['input_log_path']).resolve())
-            ]
+                        self.binary_path,
+                        str(Path(self.stage_io_dict['in']['input_log_path']).resolve())
+                        ]
         else:
             self.tmp_folder = None
             self.cmd = [self.binary_path,
-               self.stage_io_dict['in']['input_log_path']
-            ]
+                        self.stage_io_dict['in']['input_log_path']
+                        ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -133,16 +135,16 @@
                     for line in fp:
                         x = line.split()
                         if x:
                             if (len(x) > 1):
                                 ene_dict.setdefault(float(x[0]), {})[term] = x[1]
                             else:
                                 ene_dict.setdefault(float(x[0]), {})[term] = '-'
-                            
-            with open(self.io_dict['out']['output_dat_path'],'w') as fp_out:
+
+            with open(self.io_dict['out']['output_dat_path'], 'w') as fp_out:
                 fp_out.write("# TIME ")
                 for term in self.terms:
                     fp_out.write(term + " ")
                 fp_out.write("\n")
                 for key in sorted(ene_dict.keys()):
                     fp_out.write(str(key) + " ")
                     for term in self.terms:
@@ -159,36 +161,37 @@
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
 def process_mdout(input_log_path: str, output_dat_path: str,
-           properties: dict = None, **kwargs) -> int:
+                  properties: dict = None, **kwargs) -> int:
     """Create :class:`ProcessMDOut <process.process_mdout.ProcessMDOut>`process.process_mdout.ProcessMDOut class and
     execute :meth:`launch() <process.process_mdout.ProcessMDOut.launch>` method"""
 
-    return ProcessMDOut( input_log_path=input_log_path,
+    return ProcessMDOut(input_log_path=input_log_path,
                         output_dat_path=output_dat_path,
                         properties=properties).launch()
 
+
 def main():
     parser = argparse.ArgumentParser(description='Parses the AMBER (sander) MD output file (log) and dumps statistics that can then be plotted. Using the process_mdout.pl tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_log_path', required=True, help='AMBER (sander) MD output (log) file. Accepted formats: log, out, txt, o.')
     required_args.add_argument('--output_dat_path', required=True, help='Dat output file containing data from the specified terms along the MD process. File type: output. Accepted formats: dat, txt, csv.')
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
-    process_mdout(
-             input_log_path=args.input_log_path,
-             output_dat_path=args.output_dat_path,
-             properties=properties)
+    process_mdout(input_log_path=args.input_log_path,
+                  output_dat_path=args.output_dat_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/process/process_minout.py` & `biobb_amber-4.0.0/biobb_amber/process/process_minout.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import argparse
 import shutil
 from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.process.common import *
+from biobb_amber.process.common import check_input_path, check_output_path
+
 
 class ProcessMinOut(BiobbObject):
     """
     | biobb_amber.process.process_minout ProcessMinOut
     | Wrapper of the `AmberTools (AMBER MD Package) process_minout tool <https://ambermd.org/AmberTools.php>`_ module.
     | Parses the AMBER (sander) minimization output file (log) and dumps statistics that can then be plotted. Using the process_minout.pl tool from the AmberTools MD package.
 
@@ -59,16 +60,16 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_log_path': input_log_path },
-            'out': { 'output_dat_path': output_dat_path }
+            'in': {'input_log_path': input_log_path},
+            'out': {'output_dat_path': output_dat_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.terms = properties.get('terms', ["ENERGY"])
         self.binary_path = properties.get('binary_path', 'process_minout.perl')
 
@@ -79,39 +80,40 @@
     def check_data_params(self, out_log, out_err):
         """ Checks input/output paths correctness """
 
         # Check input(s)
         self.io_dict["in"]["input_log_path"] = check_input_path(self.io_dict["in"]["input_log_path"], "input_log_path", False, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"],"output_dat_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_dat_path"] = check_output_path(self.io_dict["out"]["output_dat_path"], "output_dat_path", False, out_log, self.__class__.__name__)
 
     @launchlogger
     def launch(self):
         """Launches the execution of the ProcessMinOut module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         if not self.container_path:
             self.tmp_folder = fu.create_unique_dir()
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             self.cmd = ['cd', self.tmp_folder, ';',
-                self.binary_path,
-                str(Path(self.stage_io_dict['in']['input_log_path']).resolve())
-            ]
+                        self.binary_path,
+                        str(Path(self.stage_io_dict['in']['input_log_path']).resolve())
+                        ]
         else:
             self.tmp_folder = None
             self.cmd = [self.binary_path,
-               self.stage_io_dict['in']['input_log_path']
-            ]
+                        self.stage_io_dict['in']['input_log_path']
+                        ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -129,20 +131,20 @@
 
             ene_dict = {}
             for term in self.terms:
                 with open(tmp + "/summary."+term) as fp:
                     for line in fp:
                         x = line.split()
                         if (x):
-                            if(len(x) > 1):
+                            if (len(x) > 1):
                                 ene_dict.setdefault(float(x[0]), {})[term] = x[1]
                             else:
                                 ene_dict.setdefault(float(x[0]), {})[term] = '-'
 
-            with open(self.io_dict['out']['output_dat_path'],'w') as fp_out:
+            with open(self.io_dict['out']['output_dat_path'], 'w') as fp_out:
                 fp_out.write("# TIME ")
                 for term in self.terms:
                     fp_out.write(term + " ")
                 fp_out.write("\n")
                 for key in sorted(ene_dict.keys()):
                     fp_out.write(str(key) + " ")
                     for term in self.terms:
@@ -157,22 +159,24 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def process_minout(input_log_path: str, output_dat_path: str,
-           properties: dict = None, **kwargs) -> int:
+                   properties: dict = None, **kwargs) -> int:
     """Create :class:`ProcessMinOut <process.process_mdout.ProcessMinOut>`process.process_mdout.ProcessMinOut class and
     execute :meth:`launch() <process.process_mdout.ProcessMinOut.launch>` method"""
 
-    return ProcessMinOut( input_log_path=input_log_path,
-                        output_dat_path=output_dat_path,
-                        properties=properties).launch()
+    return ProcessMinOut(input_log_path=input_log_path,
+                         output_dat_path=output_dat_path,
+                         properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Parses the AMBER (sander) minimization output file (log) and dumps statistics that can then be plotted. Using the process_minout.pl tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -181,12 +185,13 @@
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call
     process_minout(input_log_path=args.input_log_path,
-                    output_dat_path=args.output_dat_path,
-                    properties=properties)
+                   output_dat_path=args.output_dat_path,
+                   properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber/sander/common.py` & `biobb_amber-4.0.0/biobb_amber/leap/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-""" Common functions for package biobb_amber.sander """
+""" Common functions for package biobb_amber.leap """
 from pathlib import Path, PurePath
-import re
 from biobb_common.tools import file_utils as fu
 
+
 # CHECK INPUT PARAMETERS
 def check_input_path(path, argument, optional, out_log, classname):
-	""" Checks input file """
-	if optional and not path:
-		return None
-	if not Path(path).exists():
-		fu.log("Path: " + path)
-		fu.log("Path " + path + " --- " + classname + ': Unexisting %s file, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting %s file' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks input file """
+    if optional and not path:
+        return None
+    if not Path(path).exists():
+        fu.log(classname + ': Unexisting %s file, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting %s file' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
+# CHECK OUTPUT PARAMETERS
 def check_output_path(path, argument, optional, out_log, classname):
-	""" Checks output file """
-	if optional and not path:
-		return None
-	if PurePath(path).parent and not Path(PurePath(path).parent).exists():
-		fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
-		raise SystemExit(classname + ': Unexisting  %s folder' % argument)
-	file_extension = PurePath(path).suffix
-	if not is_valid_file(file_extension[1:], argument):
-		fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
-		raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
-	return path
+    """ Checks output file """
+    if optional and not path:
+        return None
+    if PurePath(path).parent and not Path(PurePath(path).parent).exists():
+        fu.log(classname + ': Unexisting  %s folder, exiting' % argument, out_log)
+        raise SystemExit(classname + ': Unexisting  %s folder' % argument)
+    file_extension = PurePath(path).suffix
+    if not is_valid_file(file_extension[1:], argument):
+        fu.log(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument), out_log)
+        raise SystemExit(classname + ': Format %s in  %s file is not compatible' % (file_extension[1:], argument))
+    return path
+
 
 def is_valid_file(ext, argument):
-	""" Checks if file format is compatible """
-	formats = {
-		'input_top_path': ['top','prmtop','parmtop'],
-		'input_crd_path': ['crd','inpcrd','mdcrd','rst','rst7','netcdf','nc','ncrst'],
-		'input_mdin_path': ['mdin','txt','in'],
-		'input_cpin_path': ['cpin','txt','in'],
-		'input_ref_path': ['crd','inpcrd','mdcrd','rst','rst7','netcdf','nc','ncrst'],
-		'output_log_path': ['log','out','txt','o'],
-		'output_traj_path': ['trj', 'crd', 'mdcrd', 'x', 'netcdf', 'nc'],
-		'output_rst_path': ['rst','rst7','netcdf','nc','ncrst'],
-		'output_cpout_path': ['cpout'],
-		'output_cprst_path': ['cprst', 'rst', 'rst7'],
-		'output_mdinfo_path': ['mdinfo']
-	}
-	return ext in formats[argument]
+    """ Checks if file format is compatible """
+    formats = {
+        'input_pdb_path': ['pdb'],
+        'input_lib_path': ['lib', 'zip'],
+        'input_frcmod_path': ['frcmod', 'zip'],
+        'input_params_path': ['in', 'leapin', 'txt', 'zip'],
+        'input_source_path': ['in', 'leapin', 'txt', 'zip'],
+        'output_pdb_path': ['pdb'],
+        'output_top_path': ['top', 'prmtop', 'parmtop'],
+        'output_crd_path': ['crd', 'mdcrd', 'inpcrd', 'rst', 'rst7']
+    }
+    return ext in formats[argument]
```

### Comparing `biobb_amber-3.9.0/biobb_amber/sander/sander_mdrun.py` & `biobb_amber-4.0.0/biobb_amber/sander/sander_mdrun.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python3
 
 """Module containing the SanderMDRun class and the command line interface."""
 import argparse
-import shutil, re
+import shutil
+import re
 from pathlib import Path, PurePath
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
-from biobb_amber.sander.common import *
+from biobb_amber.sander.common import check_input_path, check_output_path
+
 
 class SanderMDRun(BiobbObject):
     """
     | biobb_amber SanderMDRun
     | Wrapper of the `AmberTools (AMBER MD Package) sander tool <https://ambermd.org/AmberTools.php>`_ module.
     | Runs energy minimization, molecular dynamics, and NMR refinements using sander tool from the AmberTools MD package.
 
@@ -28,26 +30,27 @@
         output_cpout_path (str) (Optional): Output constant pH file (AMBER cpout). File type: output. `Sample file <https://github.com/bioexcel/biobb_amber/raw/master/biobb_amber/test/reference/sander/sander.cpout>`_. Accepted formats: cpout (edam:format_2330).
         output_cprst_path (str) (Optional): Output constant pH restart file (AMBER rstout). File type: output. `Sample file <https://github.com/bioexcel/biobb_amber/raw/master/biobb_amber/test/reference/sander/sander.cprst>`_. Accepted formats: cprst (edam:format_3886), rst (edam:format_3886), rst7 (edam:format_3886).
         output_mdinfo_path (str) (Optional): Output MD info. File type: output. `Sample file <https://github.com/bioexcel/biobb_amber/raw/master/biobb_amber/test/reference/sander/sander.mdinfo>`_. Accepted formats: mdinfo (edam:format_2330).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **mdin** (*dict*) - ({}) Sander MD run options specification. (Used if *input_mdin_path* is None)
             * **simulation_type** (*str*) - ("minimization") Default options for the mdin file. Each creates a different mdin file. Values: `minimization <https://biobb-amber.readthedocs.io/en/latest/_static/mdins/min.mdin>`_ (Runs an energy minimization), `min_vacuo <https://biobb-amber.readthedocs.io/en/latest/_static/mdins/min_vacuo.mdin>`_ (Runs an energy minimization in vacuo), `NVT <https://biobb-amber.readthedocs.io/en/latest/_static/mdins/nvt.mdin>`_ (Runs an NVT equilibration), `npt <https://biobb-amber.readthedocs.io/en/latest/_static/mdins/npt.mdin>`_ (Runs an NPT equilibration), `free <https://biobb-amber.readthedocs.io/en/latest/_static/mdins/free.mdin>`_ (Runs a MD simulation), `heat <https://biobb-amber.readthedocs.io/en/latest/_static/mdins/heat.mdin>`_ (Heats the MD system).
             * **binary_path** (*str*) - ("sander") sander binary path to be used.
+            * **direct_mdin** (*bool*) - (False) Use input_mdin_path as it is, skip file parsing.
             * **mpi_bin** (*str*) - (None) Path to the MPI runner. Usually "mpirun" or "srun".
             * **mpi_np** (*int*) - (0) [0~1000|1] Number of MPI processes. Usually an integer bigger than 1.
             * **mpi_flags** (*str*) - (None) Path to the MPI hostlist file.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
             * **container_image** (*str*) - ('afandiadib/ambertools:serial') Container image definition.
             * **container_volume_path** (*str*) - ('/tmp') Container volume path definition.
             * **container_working_dir** (*str*) - (None) Container working directory definition.
             * **container_user_id** (*str*) - (None) Container user_id definition.
             * **container_shell_path** (*str*) - ('/bin/bash') Path to default shell inside the container.
-            
+
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_amber.sander.sander_mdrun import sander_mdrun
             prop = {
                 'simulation_type' : 'minimization',
                 'mdin' : {
@@ -80,31 +83,33 @@
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_top_path': input_top_path,
-                    'input_crd_path': input_crd_path,
-                    'input_mdin_path': input_mdin_path,
-                    'input_ref_path': input_ref_path,
-                    'input_cpin_path': input_cpin_path },
-            'out': {    'output_log_path': output_log_path,
-                        'output_traj_path': output_traj_path,
-                        'output_rst_path': output_rst_path,
-                        'output_cpout_path': output_cpout_path,
-                        'output_cprst_path': output_cprst_path,
-                        'output_mdinfo_path': output_mdinfo_path }
+            'in': {'input_top_path': input_top_path,
+                   'input_crd_path': input_crd_path,
+                   'input_mdin_path': input_mdin_path,
+                   'input_ref_path': input_ref_path,
+                   'input_cpin_path': input_cpin_path},
+            'out': {'output_log_path': output_log_path,
+                    'output_traj_path': output_traj_path,
+                    'output_rst_path': output_rst_path,
+                    'output_cpout_path': output_cpout_path,
+                    'output_cprst_path': output_cprst_path,
+                    'output_mdinfo_path': output_mdinfo_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.simulation_type = properties.get('simulation_type', "minimization")
         self.binary_path = properties.get('binary_path', "sander")
+
+        self.direct_mdin = properties.get('direct_mdin', False)
         self.mdin = {k: str(v) for k, v in properties.get('mdin', dict()).items()}
 
         if 'restraintmask' in self.mdin and self.mdin['restraintmask'][0] != '"' and self.mdin['restraintmask'][-1] != '"':
             self.mdin['restraintmask'] = "\"" + self.mdin['restraintmask'] + "\""
 
         # Properties for MPI
         self.mpi_bin = properties.get('mpi_bin')
@@ -122,75 +127,76 @@
         self.io_dict["in"]["input_top_path"] = check_input_path(self.io_dict["in"]["input_top_path"], "input_top_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_crd_path"] = check_input_path(self.io_dict["in"]["input_crd_path"], "input_crd_path", False, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_mdin_path"] = check_input_path(self.io_dict["in"]["input_mdin_path"], "input_mdin_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_cpin_path"] = check_input_path(self.io_dict["in"]["input_cpin_path"], "input_cpin_path", True, out_log, self.__class__.__name__)
         self.io_dict["in"]["input_ref_path"] = check_input_path(self.io_dict["in"]["input_ref_path"], "input_ref_path", True, out_log, self.__class__.__name__)
 
         # Check output(s)
-        self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"],"output_log_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_traj_path"] = check_output_path(self.io_dict["out"]["output_traj_path"],"output_traj_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_rst_path"] = check_output_path(self.io_dict["out"]["output_rst_path"],"output_rst_path", False, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_cpout_path"] = check_output_path(self.io_dict["out"]["output_cpout_path"],"output_cpout_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_cprst_path"] = check_output_path(self.io_dict["out"]["output_cprst_path"],"output_cprst_path", True, out_log, self.__class__.__name__)
-        self.io_dict["out"]["output_mdinfo_path"] = check_output_path(self.io_dict["out"]["output_mdinfo_path"],"output_mdinfo_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_log_path"] = check_output_path(self.io_dict["out"]["output_log_path"], "output_log_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_traj_path"] = check_output_path(self.io_dict["out"]["output_traj_path"], "output_traj_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_rst_path"] = check_output_path(self.io_dict["out"]["output_rst_path"], "output_rst_path", False, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cpout_path"] = check_output_path(self.io_dict["out"]["output_cpout_path"], "output_cpout_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_cprst_path"] = check_output_path(self.io_dict["out"]["output_cprst_path"], "output_cprst_path", True, out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_mdinfo_path"] = check_output_path(self.io_dict["out"]["output_mdinfo_path"], "output_mdinfo_path", True, out_log, self.__class__.__name__)
 
     def create_mdin(self, path: str = None) -> str:
         """Creates an AMBER MD configuration file (mdin) using the properties file settings"""
         mdin_list = []
         mdin_firstPart = []
         mdin_middlePart = []
         mdin_lastPart = []
 
         self.output_mdin_path = path
 
         if self.io_dict['in']['input_mdin_path']:
             # MDIN parameters read from an input mdin file
-            mdin_firstPart.append("Mdin read from input file: " + self.stage_io_dict['in']['input_mdin_path'])
-            mdin_firstPart.append("and modified by the biobb_amber module from the BioBB library ")
-            with open(self.stage_io_dict['in']['input_mdin_path']) as input_params:
-                firstPart = True
-                secondPart = False
-                for line in input_params:
-                    if '=' in line and not secondPart:
-                        firstPart = False
-                        mdin_middlePart.append(line.rstrip())
-                    else:
-                        if (firstPart):
-                            mdin_firstPart.append(line.rstrip())
-                        elif(secondPart):
-                            mdin_lastPart.append(line.rstrip())
+            if (not self.direct_mdin):
+                mdin_firstPart.append("Mdin read from input file: " + self.stage_io_dict['in']['input_mdin_path'])
+                mdin_firstPart.append("and modified by the biobb_amber module from the BioBB library ")
+                with open(self.stage_io_dict['in']['input_mdin_path']) as input_params:
+                    firstPart = True
+                    secondPart = False
+                    for line in input_params:
+                        if '=' in line and not secondPart:
+                            firstPart = False
+                            mdin_middlePart.append(line.rstrip())
                         else:
-                            secondPart = True
-                            mdin_lastPart.append(line.rstrip())
-
-            for line in mdin_middlePart:
-                if ('!' in line or '#' in line) and not ('!@' in line or '!:' in line):
-                    # Parsing lines with comments (#,!), e.g. :
-                    # ntc=2, ntf=2, ! SHAKE, constrain lenghts of the bonds having H
-                    params = re.split('!|#',line)
-                    for param in params[0].split(','):
-                        if param.strip():
-                            mdin_list.append("  " + param.strip() + " ! " + params[1])
-                elif ('@' in line or ':' in line):
-                    # Parsing masks, e.g. :
-                    # restraintmask = ":1-40@P,O5',C5',C4',C3',O3'", restraint_wt = 0.5
-                    mylist = re.findall(r'(?:[^,"]|"(?:\\.|[^"])*")+', line)
-                    [mdin_list.append("  " + i.lstrip()) for i in mylist]
-                else:
-                    for param in line.split(','):
-                        if param.strip():
-                            if not param.strip().startswith('!'):
-                                mdin_list.append("  " + param.strip())
+                            if (firstPart):
+                                mdin_firstPart.append(line.rstrip())
+                            elif (secondPart):
+                                mdin_lastPart.append(line.rstrip())
+                            else:
+                                secondPart = True
+                                mdin_lastPart.append(line.rstrip())
+
+                for line in mdin_middlePart:
+                    if ('!' in line or '#' in line) and not ('!@' in line or '!:' in line):
+                        # Parsing lines with comments (#,!), e.g. :
+                        # ntc=2, ntf=2, ! SHAKE, constrain lenghts of the bonds having H
+                        params = re.split('!|#', line)
+                        for param in params[0].split(','):
+                            if param.strip():
+                                mdin_list.append("  " + param.strip() + " ! " + params[1])
+                    elif ('@' in line or ':' in line):
+                        # Parsing masks, e.g. :
+                        # restraintmask = ":1-40@P,O5',C5',C4',C3',O3'", restraint_wt = 0.5
+                        mylist = re.findall(r'(?:[^,"]|"(?:\\.|[^"])*")+', line)
+                        [mdin_list.append("  " + i.lstrip()) for i in mylist]
+                    else:
+                        for param in line.split(','):
+                            if param.strip():
+                                if not param.strip().startswith('!'):
+                                    mdin_list.append("  " + param.strip())
 
         else:
             # MDIN parameters added by the biobb_amber module
             mdin_list.append("This mdin file has been created by the biobb_amber module from the BioBB library ")
 
             sim_type = self.properties.get('simulation_type', 'minimization')
-            #sim_type = self.mdin.get('simulation_type', 'minimization')
+            # sim_type = self.mdin.get('simulation_type', 'minimization')
             minimization = (sim_type == 'minimization')
             min_vacuo = (sim_type == 'min_vacuo')
             heat = (sim_type == 'heat')
             nvt = (sim_type == 'nvt')
             npt = (sim_type == 'npt')
             free = (sim_type == 'free')
             md = (nvt or npt or free or heat)
@@ -231,105 +237,110 @@
                 mdin_list.append("  gamma_ln = 5.0 ! BioBB simulation_type nvt")
                 mdin_list.append("  ntb = 1 ! BioBB simulation_type nvt")
                 mdin_list.append("  ntx = 5 ! BioBB simulation_type nvt")
             if heat:
                 mdin_list.append("  tempi = 0.0 ! BioBB simulation_type heat")
                 mdin_list.append("  temp0 = 300.0 ! BioBB simulation_type heat")
                 mdin_list.append("  irest = 0 ! BioBB simulation_type heat")
-                mdin_list.append("  ntb = 1 ! BioBB simulation_type heat") #periodic boundaries
+                mdin_list.append("  ntb = 1 ! BioBB simulation_type heat")  # periodic boundaries
                 mdin_list.append("  gamma_ln = 1.0 ! BioBB simulation_type heat")
-                #mdin_list.append("  nmropt = 1 ! BioBB simulation_type heat")
+                # mdin_list.append("  nmropt = 1 ! BioBB simulation_type heat")
 
-                #mdin_lastPart.append("/")
-                #mdin_lastPart.append("&wt")
-                #mdin_lastPart.append(" TYPE = 'TEMP0' ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" ISTEP1 = 1 ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" ISTEP2 = 4000 ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" VALUE1 = 10.0 ! BioBB simulation_type heat")
-                #mdin_lastPart.append(" VALUE2 = 300.0 ! BioBB simulation_type heat")
-                #mdin_lastPart.append("/")
-                #mdin_lastPart.append("&wt")
-                #mdin_lastPart.append(" TYPE = 'END' ! BioBB simulation_type heat")
-                #mdin_lastPart.append("/")
-
-        # Adding the rest of parameters in the config file to the mdin file
-        # if the parameter has already been added replace the value
-        parameter_keys = [parameter.split('=')[0].strip() for parameter in mdin_list]
-        for k, v in self.mdin.items():
-            config_parameter_key = str(k).strip()
-            if config_parameter_key in parameter_keys:
-                mdin_list[parameter_keys.index(config_parameter_key)] = '  ' + config_parameter_key + ' = ' + str(v) + ' ! BioBB property'
-            else:
-                mdin_list.append('  ' + config_parameter_key + ' = '+str(v) + ' ! BioBB property')
+                # mdin_lastPart.append("/")
+                # mdin_lastPart.append("&wt")
+                # mdin_lastPart.append(" TYPE = 'TEMP0' ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" ISTEP1 = 1 ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" ISTEP2 = 4000 ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" VALUE1 = 10.0 ! BioBB simulation_type heat")
+                # mdin_lastPart.append(" VALUE2 = 300.0 ! BioBB simulation_type heat")
+                # mdin_lastPart.append("/")
+                # mdin_lastPart.append("&wt")
+                # mdin_lastPart.append(" TYPE = 'END' ! BioBB simulation_type heat")
+                # mdin_lastPart.append("/")
+
+        if (not self.direct_mdin):
+
+            # Adding the rest of parameters in the config file to the mdin file
+            # if the parameter has already been added replace the value
+            parameter_keys = [parameter.split('=')[0].strip() for parameter in mdin_list]
+            for k, v in self.mdin.items():
+                config_parameter_key = str(k).strip()
+                if config_parameter_key in parameter_keys:
+                    mdin_list[parameter_keys.index(config_parameter_key)] = '  ' + config_parameter_key + ' = ' + str(v) + ' ! BioBB property'
+                else:
+                    mdin_list.append('  ' + config_parameter_key + ' = '+str(v) + ' ! BioBB property')
 
-        # Writing MD configuration file (mdin)
-        with open(self.output_mdin_path, 'w') as mdin:
-            # Start of file keyword(s)
-            if mdin_firstPart:
-                for line in mdin_firstPart:
-                    mdin.write(line + '\n')
+            # Writing MD configuration file (mdin)
+            with open(self.output_mdin_path, 'w') as mdin:
+                # Start of file keyword(s)
+                if mdin_firstPart:
+                    for line in mdin_firstPart:
+                        mdin.write(line + '\n')
 
-            # MD config parameters
-            for line in mdin_list:
-                mdin.write(line + '\n')
-
-            # End of file keyword(s)
-            if mdin_lastPart:
-                for line in mdin_lastPart:
+                # MD config parameters
+                for line in mdin_list:
                     mdin.write(line + '\n')
-            else:
-                mdin.write("&end\n")
+
+                # End of file keyword(s)
+                if mdin_lastPart:
+                    for line in mdin_lastPart:
+                        mdin.write(line + '\n')
+                else:
+                    mdin.write("&end\n")
+        else:
+            # Copying generated output file to the final (user-given) file name
+            shutil.copy2(self.io_dict['in']['input_mdin_path'], self.output_mdin_path)
 
         return self.output_mdin_path
 
     @launchlogger
     def launch(self):
         """Launches the execution of the BuildLinearStructure module."""
 
         # check input/output paths and parameters
         self.check_data_params(self.out_log, self.err_log)
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Creating temporary folder
-        #self.tmp_folder = fu.create_unique_dir()
-        #fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+        # self.tmp_folder = fu.create_unique_dir()
+        # fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
-        #if self.io_dict['in']['input_mdin_path']:
+        # if self.io_dict['in']['input_mdin_path']:
         #    self.output_mdin_path = self.io_dict['in']['input_mdin_path']
-        #else:
+        # else:
         #    self.output_mdin_path = self.create_mdin(path=str(Path(self.tmp_folder).joinpath("sander.mdin")))
-        
-        #self.output_mdin_path = self.create_mdin(path=str(Path(self.tmp_folder).joinpath("sander.mdin")))
+        # self.output_mdin_path = self.create_mdin(path=str(Path(self.tmp_folder).joinpath("sander.mdin")))
 
         # Creating temporary folder & Sander configuration (instructions) file
         if self.container_path:
-            #instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
-            #instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
+            # instructions_file = str(PurePath(self.stage_io_dict['unique_dir']).joinpath("leap.in"))
+            # instructions_file_path = str(PurePath(self.container_volume_path).joinpath("leap.in"))
             instructions_file = self.create_mdin(path=str(Path(self.stage_io_dict['unique_dir']).joinpath("sander.mdin")))
             self.output_mdin_path = str(PurePath(self.container_volume_path).joinpath(PurePath(instructions_file).name))
             self.tmp_folder = None
         else:
             self.tmp_folder = fu.create_unique_dir()
             fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
             self.output_mdin_path = self.create_mdin(path=str(Path(self.tmp_folder).joinpath("sander.mdin")))
 
         # Command line
         # sander -O -i mdin/min.mdin -p $1.cpH.prmtop -c ph$i/$1.inpcrd -r ph$i/$1.min.rst7 -o ph$i/$1.min.o
         self.cmd = [self.binary_path,
-               '-O',
-               '-i', self.output_mdin_path,
-               '-p', self.stage_io_dict['in']['input_top_path'],
-               '-c', self.stage_io_dict['in']['input_crd_path'],
-               '-r', self.stage_io_dict['out']['output_rst_path'],
-               '-o', self.stage_io_dict['out']['output_log_path'],
-               '-x', self.stage_io_dict['out']['output_traj_path']
-               ]
+                    '-O',
+                    '-i', self.output_mdin_path,
+                    '-p', self.stage_io_dict['in']['input_top_path'],
+                    '-c', self.stage_io_dict['in']['input_crd_path'],
+                    '-r', self.stage_io_dict['out']['output_rst_path'],
+                    '-o', self.stage_io_dict['out']['output_log_path'],
+                    '-x', self.stage_io_dict['out']['output_traj_path']
+                    ]
 
         if self.io_dict['in']['input_ref_path']:
             self.cmd.append('-ref')
             self.cmd.append(self.stage_io_dict['in']['input_ref_path'])
 
         if self.io_dict['in']['input_cpin_path']:
             self.cmd.append('-cpin')
@@ -362,15 +373,15 @@
 
         # Copy files to host
         self.copy_to_host()
 
         # remove temporary folder(s)
         '''if self.remove_tmp:
             if self.container_path: self.tmp_files.append(self.stage_io_dict['unique_dir'])
-            else: 
+            else:
                 self.tmp_files.append(self.tmp_folder)
                 self.tmp_files.append("mdinfo")
             self.remove_tmp_files()'''
 
         self.tmp_files.extend([
             self.stage_io_dict.get("unique_dir"),
             "mdinfo",
@@ -378,75 +389,78 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def sander_mdrun(input_top_path: str, input_crd_path: str,
-            output_log_path: str, output_traj_path: str, output_rst_path: str,
-            input_mdin_path: str = None, input_cpin_path: str = None,
-            output_cpout_path: str = None, output_cprst_path: str = None,
-            output_mdinfo_path: str = None, input_ref_path: str=None,
-            properties: dict = None, **kwargs) -> int:
+                 output_log_path: str, output_traj_path: str, output_rst_path: str,
+                 input_mdin_path: str = None, input_cpin_path: str = None,
+                 output_cpout_path: str = None, output_cprst_path: str = None,
+                 output_mdinfo_path: str = None, input_ref_path: str = None,
+                 properties: dict = None, **kwargs) -> int:
     """Create :class:`SanderMDRun <sander.sander_mdrun.SanderMDRun>`sander.sander_mdrun.SanderMDRun class and
     execute :meth:`launch() <sander.sander_mdrun.SanderMDRun.launch>` method"""
 
-    return SanderMDRun( input_top_path=input_top_path,
-                    input_crd_path=input_crd_path,
-                    input_mdin_path=input_mdin_path,
-                    input_cpin_path=input_cpin_path,
-                    input_ref_path=input_ref_path,
-                    output_log_path=output_log_path,
-                    output_traj_path=output_traj_path,
-                    output_rst_path=output_rst_path,
-                    output_cpout_path=output_cpout_path,
-                    output_cprst_path=output_cprst_path,
-                    output_mdinfo_path=output_mdinfo_path,
-                    properties=properties).launch()
+    return SanderMDRun(input_top_path=input_top_path,
+                       input_crd_path=input_crd_path,
+                       input_mdin_path=input_mdin_path,
+                       input_cpin_path=input_cpin_path,
+                       input_ref_path=input_ref_path,
+                       output_log_path=output_log_path,
+                       output_traj_path=output_traj_path,
+                       output_rst_path=output_rst_path,
+                       output_cpout_path=output_cpout_path,
+                       output_cprst_path=output_cprst_path,
+                       output_mdinfo_path=output_mdinfo_path,
+                       properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Running energy minimization, molecular dynamics, and NMR refinements using sander tool from the AmberTools MD package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_top_path', required=True, help='Input topology file (AMBER ParmTop). Accepted formats: top, prmtop, parmtop.')
     required_args.add_argument('--input_crd_path', required=True, help='Input coordinates file (AMBER crd). Accepted formats: crd, mdcrd.')
-    #required_args.add_argument('--input_mdin_path', required=False, help='Input configuration file (MD run options) (AMBER mdin). Accepted formats: mdin, in, txt.')
+    # required_args.add_argument('--input_mdin_path', required=False, help='Input configuration file (MD run options) (AMBER mdin). Accepted formats: mdin, in, txt.')
     parser.add_argument('--input_mdin_path', required=False, help='Input configuration file (MD run options) (AMBER mdin). Accepted formats: mdin, in, txt.')
-    #required_args.add_argument('--input_cpin_path', required=False, help='Input constant pH file (AMBER cpin). Accepted formats: cpin.')
+    # required_args.add_argument('--input_cpin_path', required=False, help='Input constant pH file (AMBER cpin). Accepted formats: cpin.')
     parser.add_argument('--input_cpin_path', required=False, help='Input constant pH file (AMBER cpin). Accepted formats: cpin.')
-    #required_args.add_argument('--input_ref_path', required=False, help='Input reference coordinates for position restraints. Accepted formats: rst, rst7.')
+    # required_args.add_argument('--input_ref_path', required=False, help='Input reference coordinates for position restraints. Accepted formats: rst, rst7.')
     parser.add_argument('--input_ref_path', required=False, help='Input reference coordinates for position restraints. Accepted formats: rst, rst7.')
     required_args.add_argument('--output_log_path', required=True, help='Output log file. Accepted formats: log, out, txt.')
     required_args.add_argument('--output_traj_path', required=True, help='Output trajectory file. Accepted formats: trj, crd, mdcrd, x.')
     required_args.add_argument('--output_rst_path', required=True, help='Output restart file. Accepted formats: rst, rst7.')
-    #required_args.add_argument('--output_cpout_path', required=False, help='Output constant pH file (AMBER cpout). Accepted formats: cpout.')
+    # required_args.add_argument('--output_cpout_path', required=False, help='Output constant pH file (AMBER cpout). Accepted formats: cpout.')
     parser.add_argument('--output_cpout_path', required=False, help='Output constant pH file (AMBER cpout). Accepted formats: cpout.')
-    #required_args.add_argument('--output_cprst_path', required=False, help='Output constant pH restart file (AMBER rstout). Accepted formats: cprst.')
+    # required_args.add_argument('--output_cprst_path', required=False, help='Output constant pH restart file (AMBER rstout). Accepted formats: cprst.')
     parser.add_argument('--output_cprst_path', required=False, help='Output constant pH restart file (AMBER rstout). Accepted formats: cprst.')
-    #required_args.add_argument('--output_mdinfo_path', required=False, help='Output MD info. Accepted formats: mdinfo.')
+    # required_args.add_argument('--output_mdinfo_path', required=False, help='Output MD info. Accepted formats: mdinfo.')
     parser.add_argument('--output_mdinfo_path', required=False, help='Output MD info. Accepted formats: mdinfo.')
 
     args = parser.parse_args()
-    #config = args.config if args.config else None
+    # config = args.config if args.config else None
     args.config = args.config or "{}"
-    #properties = settings.ConfReader(config=config).get_prop_dic()
+    # properties = settings.ConfReader(config=config).get_prop_dic()
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    sander_mdrun(    input_top_path=args.input_top_path,
-                    input_crd_path=args.input_crd_path,
-                    input_mdin_path=args.input_mdin_path,
-                    input_cpin_path=args.input_cpin_path,
-                    input_ref_path=args.input_ref_path,
-                    output_log_path=args.output_log_path,
-                    output_traj_path=args.output_traj_path,
-                    output_rst_path=args.output_rst_path,
-                    output_cpout_path=args.output_cpout_path,
-                    output_cprst_path=args.output_cprst_path,
-                    output_mdinfo_path=args.output_mdinfo_path,
-                    properties=properties)
+    sander_mdrun(input_top_path=args.input_top_path,
+                 input_crd_path=args.input_crd_path,
+                 input_mdin_path=args.input_mdin_path,
+                 input_cpin_path=args.input_cpin_path,
+                 input_ref_path=args.input_ref_path,
+                 output_log_path=args.output_log_path,
+                 output_traj_path=args.output_traj_path,
+                 output_rst_path=args.output_rst_path,
+                 output_cpout_path=args.output_cpout_path,
+                 output_cprst_path=args.output_cprst_path,
+                 output_mdinfo_path=args.output_mdinfo_path,
+                 properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_amber-3.9.0/biobb_amber.egg-info/PKG-INFO` & `biobb_amber-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb-amber
-Version: 3.9.0
+Name: biobb_amber
+Version: 4.0.0
 Summary: Biobb_amber is a BioBB category for AMBER MD package.
 Home-page: https://github.com/bioexcel/biobb_amber
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_amber.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility MD Amber
```

### Comparing `biobb_amber-3.9.0/biobb_amber.egg-info/SOURCES.txt` & `biobb_amber-4.0.0/biobb_amber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_amber-3.9.0/biobb_amber.egg-info/entry_points.txt` & `biobb_amber-4.0.0/biobb_amber.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_amber-3.9.0/setup.py` & `biobb_amber-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_amber",
-    version="3.9.0",
+    version="4.0.0",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_amber is a BioBB category for AMBER MD package.",
     long_description="Biobb_amber allows setup and simulation of atomistic MD simulations using AMBER MD package and its associated AMBER tools.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility MD Amber",
     url="https://github.com/bioexcel/biobb_amber",
     project_urls={
         "Documentation": "http://biobb_amber.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==3.9.0'],
+    install_requires=['biobb_common==4.0.0'],
     python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "amber_to_pdb = biobb_amber.ambpdb.amber_to_pdb:main",
             "cestats_run = biobb_amber.cphstats.cestats_run:main",
             "cphstats_run = biobb_amber.cphstats.cphstats_run:main",
             "cpptraj_randomize_ions = biobb_amber.cpptraj.cpptraj_randomize_ions:main",
```

