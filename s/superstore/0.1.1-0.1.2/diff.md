# Comparing `tmp/superstore-0.1.1.tar.gz` & `tmp/superstore-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superstore-0.1.1.tar", last modified: Tue Sep 20 16:43:54 2022, max compression
+gzip compressed data, was "superstore-0.1.2.tar", last modified: Wed Apr 12 02:18:21 2023, max compression
```

## Comparing `superstore-0.1.1.tar` & `superstore-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 timkpaine   (502) staff       (20)        0 2022-09-20 16:43:54.471154 superstore-0.1.1/
--rw-r--r--   0 timkpaine   (502) staff       (20)      108 2022-09-20 16:00:22.000000 superstore-0.1.1/AUTHORS
--rw-r--r--   0 timkpaine   (502) staff       (20)    11352 2022-09-20 16:00:22.000000 superstore-0.1.1/LICENSE
--rw-r--r--   0 timkpaine   (502) staff       (20)      340 2022-09-20 16:11:02.000000 superstore-0.1.1/MANIFEST.in
--rw-r--r--   0 timkpaine   (502) staff       (20)     1077 2022-09-20 16:11:02.000000 superstore-0.1.1/Makefile
--rw-r--r--   0 timkpaine   (502) staff       (20)     1470 2022-09-20 16:43:54.471217 superstore-0.1.1/PKG-INFO
--rw-r--r--   0 timkpaine   (502) staff       (20)      816 2022-09-20 16:00:22.000000 superstore-0.1.1/README.md
--rw-r--r--   0 timkpaine   (502) staff       (20)      395 2022-09-20 16:00:22.000000 superstore-0.1.1/pyproject.toml
--rw-r--r--   0 timkpaine   (502) staff       (20)      575 2022-09-20 16:43:54.471479 superstore-0.1.1/setup.cfg
--rw-r--r--   0 timkpaine   (502) staff       (20)     1729 2022-09-20 16:43:43.000000 superstore-0.1.1/setup.py
-drwxr-xr-x   0 timkpaine   (502) staff       (20)        0 2022-09-20 16:43:54.470329 superstore-0.1.1/superstore/
--rw-r--r--   0 timkpaine   (502) staff       (20)     1791 2022-09-20 16:43:43.000000 superstore-0.1.1/superstore/__init__.py
-drwxr-xr-x   0 timkpaine   (502) staff       (20)        0 2022-09-20 16:43:54.471068 superstore-0.1.1/superstore/tests/
--rw-r--r--   0 timkpaine   (502) staff       (20)      117 2022-09-20 16:00:22.000000 superstore-0.1.1/superstore/tests/test_superstore.py
-drwxr-xr-x   0 timkpaine   (502) staff       (20)        0 2022-09-20 16:43:54.470969 superstore-0.1.1/superstore.egg-info/
--rw-r--r--   0 timkpaine   (502) staff       (20)     1470 2022-09-20 16:43:54.000000 superstore-0.1.1/superstore.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (502) staff       (20)      341 2022-09-20 16:43:54.000000 superstore-0.1.1/superstore.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (502) staff       (20)        1 2022-09-20 16:43:54.000000 superstore-0.1.1/superstore.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (502) staff       (20)        1 2022-09-20 16:04:11.000000 superstore-0.1.1/superstore.egg-info/not-zip-safe
--rw-r--r--   0 timkpaine   (502) staff       (20)      244 2022-09-20 16:43:54.000000 superstore-0.1.1/superstore.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (502) staff       (20)       11 2022-09-20 16:43:54.000000 superstore-0.1.1/superstore.egg-info/top_level.txt
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-12 02:18:21.871612 superstore-0.1.2/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      108 2023-04-12 02:10:37.000000 superstore-0.1.2/AUTHORS
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-12 02:10:37.000000 superstore-0.1.2/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      340 2023-04-12 02:10:37.000000 superstore-0.1.2/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1077 2023-04-12 02:10:37.000000 superstore-0.1.2/Makefile
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1450 2023-04-12 02:18:21.871673 superstore-0.1.2/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      816 2023-04-12 02:10:37.000000 superstore-0.1.2/README.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)      395 2023-04-12 02:10:37.000000 superstore-0.1.2/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)      575 2023-04-12 02:18:21.871905 superstore-0.1.2/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1728 2023-04-12 02:18:15.000000 superstore-0.1.2/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-12 02:18:21.870797 superstore-0.1.2/superstore/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      357 2023-04-12 02:18:15.000000 superstore-0.1.2/superstore/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2325 2023-04-12 02:10:37.000000 superstore-0.1.2/superstore/superstore.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-12 02:18:21.871518 superstore-0.1.2/superstore/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1303 2023-04-12 02:10:37.000000 superstore-0.1.2/superstore/tests/test_superstore.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2023-04-12 02:18:21.871413 superstore-0.1.2/superstore.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1450 2023-04-12 02:18:21.000000 superstore-0.1.2/superstore.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      366 2023-04-12 02:18:21.000000 superstore-0.1.2/superstore.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-12 02:18:21.000000 superstore-0.1.2/superstore.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-12 02:18:21.000000 superstore-0.1.2/superstore.egg-info/not-zip-safe
+-rw-r--r--   0 timkpaine   (501) staff       (20)      243 2023-04-12 02:18:21.000000 superstore-0.1.2/superstore.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       11 2023-04-12 02:18:21.000000 superstore-0.1.2/superstore.egg-info/top_level.txt
```

### Comparing `superstore-0.1.1/LICENSE` & `superstore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superstore-0.1.1/Makefile` & `superstore-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `superstore-0.1.1/PKG-INFO` & `superstore-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: superstore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Categorical data generator
 Home-page: https://github.com/timkpaine/superstore
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: finance data
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -38,9 +37,7 @@
 
 `python setup.py install`
 
 ## License
 
 This software is licensed under the Apache 2.0 license. See the
 [LICENSE](LICENSE) and [AUTHORS](AUTHORS) files for details.
-
-
```

### Comparing `superstore-0.1.1/README.md` & `superstore-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `superstore-0.1.1/setup.cfg` & `superstore-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 commit = True
 tag = False
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
```

### Comparing `superstore-0.1.1/setup.py` & `superstore-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 requires = [
     "Faker>=1.0.1",
     "finance-enums>=0.1.0",
     "pandas>=0.23.4",
 ]
 
 requires_dev = requires + [
-    "black>=20.",
+    "black>=22",
     "bump2version>=1.0.0",
     "check-manifest",
     "flake8>=3.7.8",
     "flake8-black>=0.2.1",
     "pytest>=4.3.0",
     "pytest-cov>=2.6.1",
     "pytest-rerunfailures>=10.1",
 ]
 
 setup(
     name=name,
-    version="0.1.1",
+    version="0.1.2",
     description="Categorical data generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timkpaine/{name}".format(name=name),
     author="Tim Paine",
     author_email="t.paine154@gmail.com",
     license="Apache 2.0",
```

### Comparing `superstore-0.1.1/superstore/__init__.py` & `superstore-0.1.2/superstore/superstore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-# *****************************************************************************
-#
-# Copyright (c) 2021, the superstore authors.
-#
-# This file is part of the superstore library, distributed under the terms of
-# the Apache License 2.0.  The full license can be found in the LICENSE file.
-#
-
-__version__ = "0.1.1"
-
 import pandas as pd
 import finance_enums
 from faker import Faker
 from random import random, randint, choice
 
 fake = Faker()
 
@@ -24,15 +14,14 @@
         dat["Order ID"] = fake.ein()
         dat["Order Date"] = fake.date_this_year()
         dat["Ship Date"] = fake.date_between_dates(dat["Order Date"]).strftime(
             "%Y-%m-%d"
         )
         dat["Order Date"] = dat["Order Date"].strftime("%Y-%m-%d")
         dat["Ship Mode"] = choice(["First Class", "Standard Class", "Second Class"])
-        dat["Ship Mode"] = choice(["First Class", "Standard Class", "Second Class"])
         dat["Customer ID"] = fake.license_plate()
         dat["Segment"] = choice(["A", "B", "C", "D"])
         dat["Country"] = "US"
         dat["City"] = fake.city()
         dat["State"] = fake.state()
         dat["Postal Code"] = fake.zipcode()
         dat["Region"] = choice(["Region %d" % i for i in range(5)])
@@ -43,7 +32,32 @@
         dat["Sub-Category"] = industry
         dat["Sales"] = randint(1, 100) * 100
         dat["Quantity"] = randint(1, 100) * 10
         dat["Discount"] = round(random() * 100, 2)
         dat["Profit"] = round(random() * 1000, 2)
         data.append(dat)
     return pd.DataFrame(data)
+
+
+def employees(count=1000):
+    data = []
+    for id in range(count):
+        dat = {}
+        dat["Row ID"] = id
+        dat["Employee ID"] = fake.unique.license_plate()
+        dat["First Name"] = fake.first_name()
+        dat["Surname"] = fake.last_name()
+        dat["Prefix"] = fake.prefix()
+        dat["Suffix"] = fake.suffix()
+        dat["Phone Number"] = fake.unique.phone_number()
+        dat["Email"] = fake.safe_email()
+        dat["SSN"] = fake.ssn()
+        dat["Street"] = fake.street_address()
+        dat["City"] = fake.city()
+        dat["Postal Code"] = fake.zipcode()
+        dat["Region"] = choice(["Region %d" % i for i in range(5)])
+        dat["State"] = fake.state()
+        dat["Country"] = "US"
+        dat["Start Date"] = fake.date_between()  # 30yrs ago to today
+        dat["Date of Birth"] = fake.date_of_birth(minimum_age=18, maximum_age=70)
+        data.append(dat)
+    return pd.DataFrame(data)
```

### Comparing `superstore-0.1.1/superstore.egg-info/PKG-INFO` & `superstore-0.1.2/superstore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: superstore
-Version: 0.1.1
+Version: 0.1.2
 Summary: Categorical data generator
 Home-page: https://github.com/timkpaine/superstore
 Author: Tim Paine
 Author-email: t.paine154@gmail.com
 License: Apache 2.0
 Keywords: finance data
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
@@ -38,9 +37,7 @@
 
 `python setup.py install`
 
 ## License
 
 This software is licensed under the Apache 2.0 license. See the
 [LICENSE](LICENSE) and [AUTHORS](AUTHORS) files for details.
-
-
```

