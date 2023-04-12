# Comparing `tmp/crimestat3000-0.1.8.tar.gz` & `tmp/crimestat3000-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crimestat3000-0.1.8.tar", last modified: Wed Apr 12 15:19:03 2023, max compression
+gzip compressed data, was "crimestat3000-0.1.9.tar", last modified: Wed Apr 12 16:08:18 2023, max compression
```

## Comparing `crimestat3000-0.1.8.tar` & `crimestat3000-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/
--rw-rw-r--   0 sdf       (1000) sdf       (1000)    35148 2023-02-19 12:59:51.000000 crimestat3000-0.1.8/LICENSE
--rw-rw-r--   0 sdf       (1000) sdf       (1000)       33 2023-02-19 12:59:51.000000 crimestat3000-0.1.8/MANIFEST.in
--rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/PKG-INFO
--rw-rw-r--   0 sdf       (1000) sdf       (1000)     4076 2023-02-19 14:43:31.000000 crimestat3000-0.1.8/README.md
-drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/crimestat3000/
--rw-r--r--   0 sdf       (1000) sdf       (1000)       29 2022-12-02 21:22:11.000000 crimestat3000-0.1.8/crimestat3000/__init__.py
--rw-r--r--   0 sdf       (1000) sdf       (1000)     4570 2023-04-12 15:09:35.000000 crimestat3000-0.1.8/crimestat3000/helpers.py
--rw-r--r--   0 sdf       (1000) sdf       (1000)     4636 2023-04-12 15:03:59.000000 crimestat3000-0.1.8/crimestat3000/parse.py
-drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/crimestat3000.egg-info/
--rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/PKG-INFO
--rw-rw-r--   0 sdf       (1000) sdf       (1000)      296 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/SOURCES.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)        1 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/dependency_links.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)        7 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/requires.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)       14 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/top_level.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)       38 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/setup.cfg
--rw-rw-r--   0 sdf       (1000) sdf       (1000)      675 2023-04-12 15:18:47.000000 crimestat3000-0.1.8/setup.py
+drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 16:08:18.822806 crimestat3000-0.1.9/
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)    35148 2023-02-19 12:59:51.000000 crimestat3000-0.1.9/LICENSE
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)       33 2023-02-19 12:59:51.000000 crimestat3000-0.1.9/MANIFEST.in
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-04-12 16:08:18.822806 crimestat3000-0.1.9/PKG-INFO
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)     4076 2023-02-19 14:43:31.000000 crimestat3000-0.1.9/README.md
+drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 16:08:18.822806 crimestat3000-0.1.9/crimestat3000/
+-rw-r--r--   0 sdf       (1000) sdf       (1000)       29 2022-12-02 21:22:11.000000 crimestat3000-0.1.9/crimestat3000/__init__.py
+-rw-r--r--   0 sdf       (1000) sdf       (1000)     4570 2023-04-12 16:05:01.000000 crimestat3000-0.1.9/crimestat3000/helpers.py
+-rw-r--r--   0 sdf       (1000) sdf       (1000)     4650 2023-04-12 16:04:37.000000 crimestat3000-0.1.9/crimestat3000/parse.py
+drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 16:08:18.822806 crimestat3000-0.1.9/crimestat3000.egg-info/
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-04-12 16:08:18.000000 crimestat3000-0.1.9/crimestat3000.egg-info/PKG-INFO
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)      296 2023-04-12 16:08:18.000000 crimestat3000-0.1.9/crimestat3000.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)        1 2023-04-12 16:08:18.000000 crimestat3000-0.1.9/crimestat3000.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)        7 2023-04-12 16:08:18.000000 crimestat3000-0.1.9/crimestat3000.egg-info/requires.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)       14 2023-04-12 16:08:18.000000 crimestat3000-0.1.9/crimestat3000.egg-info/top_level.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)       38 2023-04-12 16:08:18.822806 crimestat3000-0.1.9/setup.cfg
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)      675 2023-04-12 16:08:00.000000 crimestat3000-0.1.9/setup.py
```

### Comparing `crimestat3000-0.1.8/LICENSE` & `crimestat3000-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crimestat3000-0.1.8/PKG-INFO` & `crimestat3000-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crimestat3000
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for parsing crime statistics reports (form 4-ЕГС) from crimestat.ru.
 Home-page: https://github.com/def-useful/crimestat3000
 Author: Sergey Bondarkov
 Author-email: rosebush@duck.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crimestat3000-0.1.8/README.md` & `crimestat3000-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `crimestat3000-0.1.8/crimestat3000/helpers.py` & `crimestat3000-0.1.9/crimestat3000/helpers.py`

 * *Files identical despite different names*

### Comparing `crimestat3000-0.1.8/crimestat3000/parse.py` & `crimestat3000-0.1.9/crimestat3000/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             sheet_table = districts_to_column(sheet_table)
         except:
             print(f"problem with:\nsheet {sheet}, {month}-{year}")
             raise Exception
         if len(month_table) == 0:
             month_table = sheet_table.copy()
         else:
-            month_table = pd.merge(month_table, sheet_table)
+            month_table = pd.merge(month_table, sheet_table, how = 'left')
 
     month_table['period_end'] = pd.to_datetime(f"{year}-{month}-01")
     month_table.sort_values(['region', 'period_end'], inplace=True)
     month_table = rearrange_columns(month_table)
 
     return month_table
```

### Comparing `crimestat3000-0.1.8/crimestat3000.egg-info/PKG-INFO` & `crimestat3000-0.1.9/crimestat3000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crimestat3000
-Version: 0.1.8
+Version: 0.1.9
 Summary: A tool for parsing crime statistics reports (form 4-ЕГС) from crimestat.ru.
 Home-page: https://github.com/def-useful/crimestat3000
 Author: Sergey Bondarkov
 Author-email: rosebush@duck.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crimestat3000-0.1.8/setup.py` & `crimestat3000-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 setup(
     author="Sergey Bondarkov",
     author_email="rosebush@duck.com",
     description="A tool for parsing crime statistics reports (form 4-ЕГС) from crimestat.ru.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="crimestat3000",
-    version="0.1.8",
+    version="0.1.9",
     url='https://github.com/def-useful/crimestat3000',
     packages=find_packages(include=["crimestat3000", "crimestat3000.*"]),
     install_requires=['pandas'],
     python_requires='>=3.7'
 )
```

