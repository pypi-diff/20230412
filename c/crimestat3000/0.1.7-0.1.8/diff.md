# Comparing `tmp/crimestat3000-0.1.7.tar.gz` & `tmp/crimestat3000-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crimestat3000-0.1.7.tar", last modified: Sun Feb 19 15:04:41 2023, max compression
+gzip compressed data, was "crimestat3000-0.1.8.tar", last modified: Wed Apr 12 15:19:03 2023, max compression
```

## Comparing `crimestat3000-0.1.7.tar` & `crimestat3000-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-02-19 15:04:41.139118 crimestat3000-0.1.7/
--rw-rw-r--   0 sdf       (1000) sdf       (1000)    35148 2023-02-19 12:59:51.000000 crimestat3000-0.1.7/LICENSE
--rw-rw-r--   0 sdf       (1000) sdf       (1000)       33 2023-02-19 12:59:51.000000 crimestat3000-0.1.7/MANIFEST.in
--rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-02-19 15:04:41.139118 crimestat3000-0.1.7/PKG-INFO
--rw-rw-r--   0 sdf       (1000) sdf       (1000)     4076 2023-02-19 14:43:31.000000 crimestat3000-0.1.7/README.md
-drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-02-19 15:04:41.139118 crimestat3000-0.1.7/crimestat3000/
--rw-r--r--   0 sdf       (1000) sdf       (1000)       29 2022-12-02 21:22:11.000000 crimestat3000-0.1.7/crimestat3000/__init__.py
--rw-r--r--   0 sdf       (1000) sdf       (1000)     4493 2023-02-18 15:41:09.000000 crimestat3000-0.1.7/crimestat3000/helpers.py
--rw-r--r--   0 sdf       (1000) sdf       (1000)     4653 2023-02-18 15:40:36.000000 crimestat3000-0.1.7/crimestat3000/parse.py
-drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-02-19 15:04:41.139118 crimestat3000-0.1.7/crimestat3000.egg-info/
--rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-02-19 15:04:41.000000 crimestat3000-0.1.7/crimestat3000.egg-info/PKG-INFO
--rw-rw-r--   0 sdf       (1000) sdf       (1000)      296 2023-02-19 15:04:41.000000 crimestat3000-0.1.7/crimestat3000.egg-info/SOURCES.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)        1 2023-02-19 15:04:41.000000 crimestat3000-0.1.7/crimestat3000.egg-info/dependency_links.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)        7 2023-02-19 15:04:41.000000 crimestat3000-0.1.7/crimestat3000.egg-info/requires.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)       14 2023-02-19 15:04:41.000000 crimestat3000-0.1.7/crimestat3000.egg-info/top_level.txt
--rw-rw-r--   0 sdf       (1000) sdf       (1000)       38 2023-02-19 15:04:41.139118 crimestat3000-0.1.7/setup.cfg
--rw-rw-r--   0 sdf       (1000) sdf       (1000)      675 2023-02-19 14:46:46.000000 crimestat3000-0.1.7/setup.py
+drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)    35148 2023-02-19 12:59:51.000000 crimestat3000-0.1.8/LICENSE
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)       33 2023-02-19 12:59:51.000000 crimestat3000-0.1.8/MANIFEST.in
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/PKG-INFO
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)     4076 2023-02-19 14:43:31.000000 crimestat3000-0.1.8/README.md
+drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/crimestat3000/
+-rw-r--r--   0 sdf       (1000) sdf       (1000)       29 2022-12-02 21:22:11.000000 crimestat3000-0.1.8/crimestat3000/__init__.py
+-rw-r--r--   0 sdf       (1000) sdf       (1000)     4570 2023-04-12 15:09:35.000000 crimestat3000-0.1.8/crimestat3000/helpers.py
+-rw-r--r--   0 sdf       (1000) sdf       (1000)     4636 2023-04-12 15:03:59.000000 crimestat3000-0.1.8/crimestat3000/parse.py
+drwxrwxr-x   0 sdf       (1000) sdf       (1000)        0 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/crimestat3000.egg-info/
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)     4419 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/PKG-INFO
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)      296 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/SOURCES.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)        1 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/dependency_links.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)        7 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/requires.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)       14 2023-04-12 15:19:03.000000 crimestat3000-0.1.8/crimestat3000.egg-info/top_level.txt
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)       38 2023-04-12 15:19:03.935929 crimestat3000-0.1.8/setup.cfg
+-rw-rw-r--   0 sdf       (1000) sdf       (1000)      675 2023-04-12 15:18:47.000000 crimestat3000-0.1.8/setup.py
```

### Comparing `crimestat3000-0.1.7/LICENSE` & `crimestat3000-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crimestat3000-0.1.7/PKG-INFO` & `crimestat3000-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crimestat3000
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for parsing crime statistics reports (form 4-ЕГС) from crimestat.ru.
 Home-page: https://github.com/def-useful/crimestat3000
 Author: Sergey Bondarkov
 Author-email: rosebush@duck.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crimestat3000-0.1.7/README.md` & `crimestat3000-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `crimestat3000-0.1.7/crimestat3000/helpers.py` & `crimestat3000-0.1.8/crimestat3000/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     for k, v in spec_cases.items():
         if re.search(k, descr):
             return v
 
     article_group = re.search(
         r'(п\.\s*[«"]|ч\.\s*\d|ст\.\s*\d|\bглава\s+).*', descr)
     if article_group == None:
-        return re.search(r'строка\s*\d+\s*:', descr, re.IGNORECASE).group(0) + " no articles mentioned"
+        # return re.search(r'строка\s*\d+\s*:', descr, re.IGNORECASE).group(0) + " no articles mentioned"
+        return descr
     else:
         article = re.search(
             r"ст\.\s*(\d+(?:\s*[–,и\.]\s*\d+)*)\s*УП?К", article_group.group(0))
 
         if article:
             article = re.sub(r"\s*30\s*[,и]", "", article.group(1))
             article = re.sub(r"(,\s+|\s+и\s+)", r"|", article)
@@ -64,15 +65,16 @@
          "Республика Северная Осетия - Алания": "Республика Северная Осетия – Алания",
          "Республика Северная Осетия — Алания": "Республика Северная Осетия – Алания",
          "Ханты-Мансийский автономный округ - Югра": "Ханты-Мансийский автономный округ",
          "Ханты-Мансийский автономный округ –  Югра": "Ханты-Мансийский автономный округ"},
         inplace=True)
 
     districts_dict = {}
-
+    
+    d = 'Российская Федерация'
     for row in table.itertuples():
         if re.search(r"федераль", row.region, re.IGNORECASE):
             d = row.region
         else:
             districts_dict[row.region] = d
 
     table.insert(loc=1, column='federal_district',
```

### Comparing `crimestat3000-0.1.7/crimestat3000/parse.py` & `crimestat3000-0.1.8/crimestat3000/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         if re.search(sheet_filter[keep], short_descr):
             continue
 
         sheet_table = month_file.parse(
             sheet, usecols=f"B,{','.join(columns)}", index_col=0)
         sheet_table = sheet_table.loc[
-            'Центральный федеральный округ':'Транспорт России'][:-1].reset_index()
+            'Российская Федерация':'Транспорт России'][:-1].reset_index()
 
         if shorten_descr == True:
             descr = short_descr
 
         if len(columns) > 1:
             clmns = ['region']
             clmns.extend([f"{descr}_[{col}]" for col in columns])
```

### Comparing `crimestat3000-0.1.7/crimestat3000.egg-info/PKG-INFO` & `crimestat3000-0.1.8/crimestat3000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crimestat3000
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for parsing crime statistics reports (form 4-ЕГС) from crimestat.ru.
 Home-page: https://github.com/def-useful/crimestat3000
 Author: Sergey Bondarkov
 Author-email: rosebush@duck.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `crimestat3000-0.1.7/setup.py` & `crimestat3000-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 setup(
     author="Sergey Bondarkov",
     author_email="rosebush@duck.com",
     description="A tool for parsing crime statistics reports (form 4-ЕГС) from crimestat.ru.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     name="crimestat3000",
-    version="0.1.7",
+    version="0.1.8",
     url='https://github.com/def-useful/crimestat3000',
     packages=find_packages(include=["crimestat3000", "crimestat3000.*"]),
     install_requires=['pandas'],
     python_requires='>=3.7'
 )
```

