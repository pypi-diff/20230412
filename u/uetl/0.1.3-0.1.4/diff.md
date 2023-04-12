# Comparing `tmp/uetl-0.1.3.tar.gz` & `tmp/uetl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uetl-0.1.3.tar", last modified: Wed Apr 12 14:44:59 2023, max compression
+gzip compressed data, was "uetl-0.1.4.tar", last modified: Wed Apr 12 15:13:37 2023, max compression
```

## Comparing `uetl-0.1.3.tar` & `uetl-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 14:44:59.488400 uetl-0.1.3/
--rw-rw-r--   0 andre     (1000) andre     (1000)     1070 2023-04-12 14:37:49.000000 uetl-0.1.3/LICENSE
--rw-rw-r--   0 andre     (1000) andre     (1000)       29 2023-04-12 14:37:49.000000 uetl-0.1.3/MANIFEST.in
--rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-12 14:44:59.488400 uetl-0.1.3/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)     2763 2023-04-12 14:37:49.000000 uetl-0.1.3/README.md
--rw-rw-r--   0 andre     (1000) andre     (1000)       38 2023-04-12 14:44:59.488400 uetl-0.1.3/setup.cfg
--rw-rw-r--   0 andre     (1000) andre     (1000)     1055 2023-04-12 14:42:36.000000 uetl-0.1.3/setup.py
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 14:44:59.488400 uetl-0.1.3/src/
-drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 14:44:59.488400 uetl-0.1.3/src/uetl.egg-info/
--rw-rw-r--   0 andre     (1000) andre     (1000)     3179 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/PKG-INFO
--rw-rw-r--   0 andre     (1000) andre     (1000)      209 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/SOURCES.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        1 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/dependency_links.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)      116 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/requires.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)        5 2023-04-12 14:44:59.000000 uetl-0.1.3/src/uetl.egg-info/top_level.txt
--rw-rw-r--   0 andre     (1000) andre     (1000)    14560 2023-04-12 14:37:49.000000 uetl-0.1.3/src/uetl.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 15:13:37.506958 uetl-0.1.4/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1799 2023-04-12 14:37:49.000000 uetl-0.1.4/.gitignore
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1070 2023-04-12 14:37:49.000000 uetl-0.1.4/LICENSE
+-rw-rw-r--   0 andre     (1000) andre     (1000)       29 2023-04-12 14:37:49.000000 uetl-0.1.4/MANIFEST.in
+-rw-rw-r--   0 andre     (1000) andre     (1000)      702 2023-04-12 14:37:49.000000 uetl-0.1.4/Makefile
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3216 2023-04-12 15:13:37.506958 uetl-0.1.4/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)     2763 2023-04-12 14:37:49.000000 uetl-0.1.4/README.md
+-rw-rw-r--   0 andre     (1000) andre     (1000)       24 2023-04-12 14:37:49.000000 uetl-0.1.4/requirements.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)       38 2023-04-12 15:13:37.506958 uetl-0.1.4/setup.cfg
+-rw-rw-r--   0 andre     (1000) andre     (1000)     1055 2023-04-12 15:13:19.000000 uetl-0.1.4/setup.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 15:13:37.506958 uetl-0.1.4/src/
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 15:13:37.506958 uetl-0.1.4/src/uetl.egg-info/
+-rw-rw-r--   0 andre     (1000) andre     (1000)     3216 2023-04-12 15:13:37.000000 uetl-0.1.4/src/uetl.egg-info/PKG-INFO
+-rw-rw-r--   0 andre     (1000) andre     (1000)      273 2023-04-12 15:13:37.000000 uetl-0.1.4/src/uetl.egg-info/SOURCES.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        1 2023-04-12 15:13:37.000000 uetl-0.1.4/src/uetl.egg-info/dependency_links.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)      116 2023-04-12 15:13:37.000000 uetl-0.1.4/src/uetl.egg-info/requires.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)        5 2023-04-12 15:13:37.000000 uetl-0.1.4/src/uetl.egg-info/top_level.txt
+-rw-rw-r--   0 andre     (1000) andre     (1000)    14541 2023-04-12 15:11:36.000000 uetl-0.1.4/src/uetl.py
+drwxrwxr-x   0 andre     (1000) andre     (1000)        0 2023-04-12 15:13:37.506958 uetl-0.1.4/tests/
+-rwxrwxr-x   0 andre     (1000) andre     (1000)      398 2023-04-12 14:37:49.000000 uetl-0.1.4/tests/test_uetl.py
+-rw-rw-r--   0 andre     (1000) andre     (1000)       69 2023-04-12 14:37:49.000000 uetl-0.1.4/tox.ini
```

### Comparing `uetl-0.1.3/LICENSE` & `uetl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uetl-0.1.3/PKG-INFO` & `uetl-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: uetl
-Version: 0.1.3
+Version: 0.1.4
 Summary: Minimalist python ETL library.
 Home-page: https://github.com/andrespp/uetl
 Author: Andre Pereira
 Author-email: andrespp@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -137,7 +139,9 @@
 ```
 
 [MSSql ODBC Driver](https://learn.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16)
 
 ## Issues
 
 If you have any problems with or questions about this image, please contact me through a [GitHub issue](https://github.com/andrespp/uetl/issues).
+
+
```

### Comparing `uetl-0.1.3/README.md` & `uetl-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `uetl-0.1.3/setup.py` & `uetl-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='uetl',
-    version='0.1.3',
+    version='0.1.4',
     description='Minimalist python ETL library.',
     py_modules=["uetl"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
                  "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent",
     ],
```

### Comparing `uetl-0.1.3/src/uetl.egg-info/PKG-INFO` & `uetl-0.1.4/src/uetl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: uetl
-Version: 0.1.3
+Version: 0.1.4
 Summary: Minimalist python ETL library.
 Home-page: https://github.com/andrespp/uetl
 Author: Andre Pereira
 Author-email: andrespp@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -137,7 +139,9 @@
 ```
 
 [MSSql ODBC Driver](https://learn.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16)
 
 ## Issues
 
 If you have any problems with or questions about this image, please contact me through a [GitHub issue](https://github.com/andrespp/uetl/issues).
+
+
```

### Comparing `uetl-0.1.3/src/uetl.py` & `uetl-0.1.4/src/uetl.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,21 +132,20 @@
         """
         conn = self.get_conn()
         if conn == -1: # DBMS Unreachable!
             return False
         else:
             cur = conn.cursor()
             cur.execute(
-                text(
-                    """ select exists(
-                        select *
-                        from information_schema.tables
-                        where table_name=%s
-                       )
-                       """, (table_name,)
+                text(f"""
+                        select exists(
+                            select * from information_schema.tables
+                            where table_name={table_name}
+                        )
+                    """
                 )
             )
             status = cur.fetchone()[0]
             conn.close()
         return status
 
     def create_tables(self, tables, verbose=False):
```

