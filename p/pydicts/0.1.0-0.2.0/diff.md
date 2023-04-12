# Comparing `tmp/pydicts-0.1.0.tar.gz` & `tmp/pydicts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicts-0.1.0.tar", max compression
+gzip compressed data, was "pydicts-0.2.0.tar", max compression
```

## Comparing `pydicts-0.1.0.tar` & `pydicts-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.1.0/LICENSE
--rw-r--r--   0        0        0      187 2023-04-10 16:27:20.112887 pydicts-0.1.0/README.md
--rw-r--r--   0        0        0      143 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/__init__.py
--rw-r--r--   0        0        0     8707 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/lod.py
--rw-r--r--   0        0        0     1093 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/row_column_value.py
--rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/tests/__init__.py
--rw-r--r--   0        0        0      350 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/tests/test_lod.py
--rw-r--r--   0        0        0      458 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/tests/test_year_month_value.py
--rw-r--r--   0        0        0     3307 2023-04-10 16:27:20.112887 pydicts-0.1.0/pydicts/year_month_value.py
--rw-r--r--   0        0        0      331 2023-04-10 16:27:20.112887 pydicts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 pydicts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2044 2023-04-12 05:43:21.075383 pydicts-0.2.0/README.md
+-rw-r--r--   0        0        0      143 2023-04-12 05:41:59.410380 pydicts-0.2.0/pydicts/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.2.0/pydicts/classes.py
+-rw-r--r--   0        0        0     5382 2023-04-12 05:11:39.114325 pydicts-0.2.0/pydicts/lod.py
+-rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.2.0/pydicts/lod_xyv.py
+-rw-r--r--   0        0        0     3199 2023-04-12 05:34:00.504366 pydicts-0.2.0/pydicts/lod_ymv.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.2.0/pydicts/tests/__init__.py
+-rw-r--r--   0        0        0      913 2023-04-12 05:37:22.137372 pydicts-0.2.0/pydicts/tests/test_lod.py
+-rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.2.0/pydicts/tests/test_lod_ymv.py
+-rw-r--r--   0        0        0      407 2023-04-12 05:46:36.401389 pydicts-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 pydicts-0.2.0/PKG-INFO
```

### Comparing `pydicts-0.1.0/LICENSE` & `pydicts-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicts-0.1.0/pydicts/year_month_value.py` & `pydicts-0.2.0/pydicts/lod_ymv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-
-
 from datetime import date
-from pydicts.lod import lod2dict, lod_min_value, lod_max_value, lod2dict_tuple
+from pydicts import lod
 
 
 ## Converts a tipical groyp by lor with year, month, value into an other lor with year, 1, 2, 3 .... 12, total 
-def lod_year_month_value_transposition(ld, key_year="year", key_month="month", key_value="value"):
+def lod_ymv_transposition(ld, key_year="year", key_month="month", key_value="value"):
     if len(ld)==0:
        return []
 
     if not key_year in ld[0] or not key_month in ld[0] or not key_value in ld[0]:
-        print("Keys names are not correct in dictionary in lod_year_month_value_transposition function")
+        print("Keys names are not correct in dictionary in lod_ymv_transposition function")
         return None
 
-    min_year=lod_min_value(ld, key_year)
-    max_year=lod_max_value(ld, key_year)
+    min_year=lod.lod_min_value(ld, key_year)
+    max_year=lod.lod_max_value(ld, key_year)
     #Initialize result
     r=[]
     for year in range(min_year,max_year+1):
         r.append({"year": year, "m1":0, "m2":0,  "m3":0, "m4":0, "m5":0, "m6":0, "m7":0, "m8":0, "m9":0, "m10":0, "m11":0, "m12":0, "total":0})
 
     #Assign values
     for d in ld:
@@ -27,17 +25,17 @@
     #Calculate totals
     for year in range(min_year,max_year+1):
         d=r[year-min_year]
         d["total"]=d["m1"]+d["m2"]+d["m3"]+d["m4"]+d["m5"]+d["m6"]+d["m7"]+d["m8"]+d["m9"]+d["m10"]+d["m11"]+d["m12"]
 
     return r
 
-def lod_year_month_value_transposition_sum(lymv_a, lymv_b):
+def lod_ymv_transposition_sum(lymv_a, lymv_b):
     """
-        Sums to lod_year_month_value_transpositions
+        Sums to lod_ymv_transpositions
     """
     def get_younger(year, field):
         if year in d_younger:
             return d_younger[year][field]
         else:
             return 0
     
@@ -46,15 +44,15 @@
     if len(lymv_b)==0:
         return lymv_a
     year_lymv_a=lymv_a[0]["year"]
     year_lymv_b=lymv_b[0]["year"]
     print(year_lymv_a, year_lymv_b)
     older=lymv_a if year_lymv_a<year_lymv_b else lymv_b
     younger=lymv_a if year_lymv_a>year_lymv_b else lymv_b
-    d_younger=lod2dict(younger, "year")
+    d_younger=lod.lod2dod(younger, "year")
     r=[]
     for d in older:
         new={}
         new["year"]=d["year"]
         new["m1"]=d["m1"]+get_younger(d["year"],"m1")
         new["m2"]=d["m2"]+get_younger(d["year"],"m2")
         new["m3"]=d["m3"]+get_younger(d["year"],"m3")
@@ -68,16 +66,16 @@
         new["m11"]=d["m11"]+get_younger(d["year"],"m11")
         new["m12"]=d["m12"]+get_younger(d["year"],"m12")
         new["total"]=d["total"]+get_younger(d["year"],"total")
         r.append(new)
     return r
 
 ## Converts a tipical groyp by lor with year, month (normaly extracted from db to fill empty values)
-def lod_year_month_value_filling(lod, year_from, year_to=date.today().year, fill_value=0, key_year="year", key_month="month", key_value="value"):
-    ld_tuple=lod2dict_tuple(lod, key_year, key_month)
+def lod_ymv_filling(lod, year_from, year_to=date.today().year, fill_value=0, key_year="year", key_month="month", key_value="value"):
+    ld_tuple=lod.lod2dod_tuple(lod, key_year, key_month)
     for year in range(year_from,year_to+1):
         for month in range (1,13):
             if not (key_year,key_month) in ld_tuple:
                 ld_tuple[(key_year,key_month)]={key_year: year, key_month: month, key_value:fill_value}
     r=[]
     for d in ld_tuple.values:
         r.append(d)
```

