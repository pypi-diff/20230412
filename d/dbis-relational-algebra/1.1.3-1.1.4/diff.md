# Comparing `tmp/dbis-relational-algebra-1.1.3.tar.gz` & `tmp/dbis-relational-algebra-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-algebra-1.1.3.tar", last modified: Tue Mar 28 21:10:55 2023, max compression
+gzip compressed data, was "dbis-relational-algebra-1.1.4.tar", last modified: Wed Apr 12 19:19:37 2023, max compression
```

## Comparing `dbis-relational-algebra-1.1.3.tar` & `dbis-relational-algebra-1.1.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.879277 dbis-relational-algebra-1.1.3/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4848 2023-03-28 21:10:55.879277 dbis-relational-algebra-1.1.3/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4356 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.877277 dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4848 2023-03-28 21:10:55.000000 dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1910 2023-03-28 21:10:55.000000 dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-03-28 21:10:55.000000 dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       39 2023-03-28 21:10:55.000000 dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       19 2023-03-28 21:10:55.000000 dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/top_level.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      719 2023-03-28 21:10:38.000000 dbis-relational-algebra-1.1.3/pyproject.toml
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.877277 dbis-relational-algebra-1.1.3/relational_algebra/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1564 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.877277 dbis-relational-algebra-1.1.3/relational_algebra/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1888 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.878276 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1700 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1712 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1704 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1709 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1701 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.878276 dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1258 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      642 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1255 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.878276 dbis-relational-algebra-1.1.3/relational_algebra/operators/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1302 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/CrossProduct.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2059 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Difference.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1899 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Division.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1912 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Intersection.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1269 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/LeftSemiJoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2858 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/NaturalJoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4029 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Operator.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1023 2023-03-28 21:10:38.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Projection.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10290 2023-03-28 21:10:38.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Relation.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4036 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Rename.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1277 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/RightSemiJoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      860 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Selection.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1178 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/ThetaJoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2036 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/Union.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/relational_algebra/operators/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-03-28 21:10:55.879277 dbis-relational-algebra-1.1.3/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-03-28 21:10:55.879277 dbis-relational-algebra-1.1.3/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6151 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_comparators.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1321 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_connectives.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1046 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_crossproduct.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1452 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_difference.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      884 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_division.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1502 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_intersection.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      694 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_leftsemijoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1573 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_naturaljoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      555 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_projection.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      270 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_relation.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2017 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_rename.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      696 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_rightsemijoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      985 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_selection.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1870 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_sql_basic.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5071 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_sql_complex.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2716 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_thetajoin.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1518 2023-03-28 21:00:05.000000 dbis-relational-algebra-1.1.3/tests/test_union.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.418269 dbis-relational-algebra-1.1.4/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4848 2023-04-12 19:19:37.418269 dbis-relational-algebra-1.1.4/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4356 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.416269 dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4848 2023-04-12 19:19:37.000000 dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1910 2023-04-12 19:19:37.000000 dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-12 19:19:37.000000 dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       39 2023-04-12 19:19:37.000000 dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       19 2023-04-12 19:19:37.000000 dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/top_level.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      719 2023-04-12 19:19:10.000000 dbis-relational-algebra-1.1.4/pyproject.toml
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.416269 dbis-relational-algebra-1.1.4/relational_algebra/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1564 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.416269 dbis-relational-algebra-1.1.4/relational_algebra/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1888 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.417269 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1700 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1712 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1704 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1709 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1701 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.417269 dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1258 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      642 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1254 2023-04-12 19:19:10.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.417269 dbis-relational-algebra-1.1.4/relational_algebra/operators/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1302 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/CrossProduct.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2059 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Difference.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1899 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Division.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1912 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Intersection.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1269 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/LeftSemiJoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2858 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/NaturalJoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4029 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Operator.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1021 2023-04-12 19:19:10.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Projection.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10290 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Relation.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4036 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Rename.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1277 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/RightSemiJoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      860 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Selection.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1182 2023-04-12 19:19:10.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/ThetaJoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2036 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/Union.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/relational_algebra/operators/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-12 19:19:37.418269 dbis-relational-algebra-1.1.4/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-12 19:19:37.418269 dbis-relational-algebra-1.1.4/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6151 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_comparators.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1321 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_connectives.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1046 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_crossproduct.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1452 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_difference.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      884 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_division.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1502 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_intersection.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      694 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_leftsemijoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1573 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_naturaljoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      555 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_projection.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      270 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_relation.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2017 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_rename.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      696 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_rightsemijoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      985 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_selection.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1870 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_sql_basic.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     5071 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_sql_complex.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2716 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_thetajoin.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1518 2023-04-12 19:11:04.000000 dbis-relational-algebra-1.1.4/tests/test_union.py
```

### Comparing `dbis-relational-algebra-1.1.3/LICENSE` & `dbis-relational-algebra-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/PKG-INFO` & `dbis-relational-algebra-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-algebra
-Version: 1.1.3
+Version: 1.1.4
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-algebra
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-algebra-1.1.3/README.md` & `dbis-relational-algebra-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/PKG-INFO` & `dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-algebra
-Version: 1.1.3
+Version: 1.1.4
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-algebra
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-algebra-1.1.3/dbis_relational_algebra.egg-info/SOURCES.txt` & `dbis-relational-algebra-1.1.4/dbis_relational_algebra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/pyproject.toml` & `dbis-relational-algebra-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-relational-algebra"
-version = "1.1.3"
+version = "1.1.4"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/__init__.py` & `dbis-relational-algebra-1.1.4/relational_algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/Formula.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/Formula.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/Equals.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/Equals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/GreaterEquals.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/GreaterEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/GreaterThan.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/GreaterThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/LessEquals.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/LessEquals.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/atoms/LessThan.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/atoms/LessThan.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/And.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/And.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/Not.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/Not.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/formulas/conenctives/Or.py` & `dbis-relational-algebra-1.1.4/relational_algebra/formulas/conenctives/Or.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,14 @@
         if isinstance(self.children[1], Or):
             right = (
                 f"{self.children[1].children[0]} \\land {self.children[1].children[1]}"
             )
         elif not isinstance(self.children[1], ra.Not | ra.ATOM_TYPES):
             right = f"({right})"
 
-        return f"{left} \\land {right}"
+        return f"{left} \\lor {right}"
 
     @typechecked
     def to_series(self, relation: ra.Relation) -> pd.Series:
         return self.children[0].to_series(relation) | self.children[1].to_series(
             relation
         )
```

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/CrossProduct.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/CrossProduct.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Difference.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Difference.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Division.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Division.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Intersection.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Intersection.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/LeftSemiJoin.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/LeftSemiJoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/NaturalJoin.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/NaturalJoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Operator.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Operator.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Projection.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Projection.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,13 +24,13 @@
             attr = list()
             attr.append(attributes)
             attributes = attr
         self.attributes = attributes
 
     @typechecked
     def __repr__(self) -> str:
-        return f"\\prod_{{{','.join(self.attributes)}}}({self.children[0]})"
+        return f"\\pi_{{{','.join(self.attributes)}}}({self.children[0]})"
 
     @typechecked
     def evaluate(self, sql_con: Optional[sqlite3.Connection] = None) -> ra.Relation:
         child_relation = self.children[0].evaluate(sql_con)
         return child_relation[tuple(self.attributes)]
```

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Relation.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Relation.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Rename.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Rename.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/RightSemiJoin.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/RightSemiJoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Selection.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Selection.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/ThetaJoin.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/ThetaJoin.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         if isinstance(right_child, str):
             right_child = ra.Relation(right_child)
         super().__init__(children=[left_child, right_child])
         self.formula = formula
 
     @typechecked
     def __repr__(self) -> str:
-        return f"({self.children[0]} \\bowtie_{self.formula} {self.children[1]})"
+        return f"({self.children[0]} \\bowtie_{{{self.formula}}} {self.children[1]})"
 
     @typechecked
     def evaluate(self, sql_con: Optional[sqlite3.Connection] = None) -> ra.Relation:
         left_relation = self.children[0].evaluate(sql_con)
         right_relation = self.children[1].evaluate(sql_con)
         return ra.Selection(
             ra.CrossProduct(left_relation, right_relation), self.formula
```

### Comparing `dbis-relational-algebra-1.1.3/relational_algebra/operators/Union.py` & `dbis-relational-algebra-1.1.4/relational_algebra/operators/Union.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_comparators.py` & `dbis-relational-algebra-1.1.4/tests/test_comparators.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_connectives.py` & `dbis-relational-algebra-1.1.4/tests/test_connectives.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_crossproduct.py` & `dbis-relational-algebra-1.1.4/tests/test_crossproduct.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_difference.py` & `dbis-relational-algebra-1.1.4/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_division.py` & `dbis-relational-algebra-1.1.4/tests/test_division.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_intersection.py` & `dbis-relational-algebra-1.1.4/tests/test_intersection.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_leftsemijoin.py` & `dbis-relational-algebra-1.1.4/tests/test_leftsemijoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_naturaljoin.py` & `dbis-relational-algebra-1.1.4/tests/test_naturaljoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_projection.py` & `dbis-relational-algebra-1.1.4/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_rename.py` & `dbis-relational-algebra-1.1.4/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_rightsemijoin.py` & `dbis-relational-algebra-1.1.4/tests/test_rightsemijoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_selection.py` & `dbis-relational-algebra-1.1.4/tests/test_selection.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_sql_basic.py` & `dbis-relational-algebra-1.1.4/tests/test_sql_basic.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_sql_complex.py` & `dbis-relational-algebra-1.1.4/tests/test_sql_complex.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_thetajoin.py` & `dbis-relational-algebra-1.1.4/tests/test_thetajoin.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-algebra-1.1.3/tests/test_union.py` & `dbis-relational-algebra-1.1.4/tests/test_union.py`

 * *Files identical despite different names*

