# Comparing `tmp/cleancourt-0.7.6.tar.gz` & `tmp/cleancourt-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancourt-0.7.6.tar", last modified: Mon Apr  3 17:43:18 2023, max compression
+gzip compressed data, was "dist/cleancourt-0.7.7.tar", last modified: Wed Apr 12 15:18:54 2023, max compression
```

## Comparing `cleancourt-0.7.6.tar` & `cleancourt-0.7.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:43:18.000000 cleancourt-0.7.6/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-03 17:43:02.000000 cleancourt-0.7.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-03 17:43:18.000000 cleancourt-0.7.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-03 17:43:02.000000 cleancourt-0.7.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-03 17:43:18.000000 cleancourt-0.7.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-03 17:43:02.000000 cleancourt-0.7.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/check_spaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2406 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/clean_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/compare_companies.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/compute_ngrams.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/cosine_similarity.py
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/full_clean_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/integrate_output.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/parse_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/separate_parent_company.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-03 17:43:02.000000 cleancourt-0.7.6/src/cleancourt/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-03 17:43:18.000000 cleancourt-0.7.6/src/cleancourt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-12 15:18:39.000000 cleancourt-0.7.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-04-12 15:18:54.000000 cleancourt-0.7.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-12 15:18:39.000000 cleancourt-0.7.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-12 15:18:54.000000 cleancourt-0.7.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-12 15:18:39.000000 cleancourt-0.7.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/check_spaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2961 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/clean_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/compare_companies.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/compute_ngrams.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/cosine_similarity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/full_clean_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/integrate_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/parse_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/separate_parent_company.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-12 15:18:39.000000 cleancourt-0.7.7/src/cleancourt/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15468 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-12 15:18:54.000000 cleancourt-0.7.7/src/cleancourt.egg-info/top_level.txt
```

### Comparing `cleancourt-0.7.6/LICENSE.txt` & `cleancourt-0.7.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/PKG-INFO` & `cleancourt-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.6
+Version: 0.7.7
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.7.6/README.md` & `cleancourt-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/setup.py` & `cleancourt-0.7.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="cleancourt",
-    version="0.7.6",
+    version="0.7.7",
     description="a library for cleaning court docket entries",
     author="Logan Pratico",
     author_email="praticol@lsc.gov",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.9",
```

### Comparing `cleancourt-0.7.6/src/cleancourt/__init__.py` & `cleancourt-0.7.7/src/cleancourt/__init__.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/check_spaces.py` & `cleancourt-0.7.7/src/cleancourt/check_spaces.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/clean_data.py` & `cleancourt-0.7.7/src/cleancourt/clean_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,17 +52,26 @@
 
     string = re.sub(" corporation", " corp", string)  # shorten corporation to corp
     string = re.sub(" company", " co", string)  # shorten company to co
     string = re.sub(" maa?nage?ment", " mgmt", string)  # etc
     string = re.sub(" incorporated", " inc", string)
     string = re.sub(" apartment", " apt", string)
     string = re.sub(" square(\s|$|,)", " sq\\1", string)
+
+    string = re.sub("housing authy", "housing authority", string) # this replacement is being placed before any of the other housing authority replacements because "authy" appears in both PHA and RHA names
+    string = re.sub("housing authority, inc", "housing authority", string)
+
     string = re.sub("redevelopment and housing authority", "rha", string)
-    string = re.sub("redevelopment and housing auth\.?", "rha", string)
+    string = re.sub("redevelopment and housing auth.?", "rha", string)
     string = re.sub("redevelopment and housing", "rha", string)
+    string = re.sub("redevelopment housing authority", "rha", string)
+
+    string = re.sub("public housing authority", "pha", string)
+    string = re.sub("housing authority", "pha", string)
+    string = re.sub("housing and redevelopment authority", "pha", string)
 
     string = re.sub(" et\.?\s?al\.?$", "", string)
     string = re.sub(
         "p\.?c\.?$", "", string
     )  # Remove P.C. (Personal Corporation) abbreviation on the end of a name
 
     string = re.sub("\.", "", string)  # Remove any periods
```

### Comparing `cleancourt-0.7.6/src/cleancourt/compare_companies.py` & `cleancourt-0.7.7/src/cleancourt/compare_companies.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/cosine_similarity.py` & `cleancourt-0.7.7/src/cleancourt/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/filter_types.py` & `cleancourt-0.7.7/src/cleancourt/filter_types.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/full_clean_names.py` & `cleancourt-0.7.7/src/cleancourt/full_clean_names.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/integrate_output.py` & `cleancourt-0.7.7/src/cleancourt/integrate_output.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/parse_names.py` & `cleancourt-0.7.7/src/cleancourt/parse_names.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/separate_parent_company.py` & `cleancourt-0.7.7/src/cleancourt/separate_parent_company.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt/test_utils.py` & `cleancourt-0.7.7/src/cleancourt/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.6/src/cleancourt.egg-info/PKG-INFO` & `cleancourt-0.7.7/src/cleancourt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.6
+Version: 0.7.7
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.7.6/src/cleancourt.egg-info/SOURCES.txt` & `cleancourt-0.7.7/src/cleancourt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

