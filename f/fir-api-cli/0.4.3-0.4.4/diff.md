# Comparing `tmp/fir-api-cli-0.4.3.tar.gz` & `tmp/fir-api-cli-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fir-api-cli-0.4.3.tar", last modified: Tue Mar 14 13:26:50 2023, max compression
+gzip compressed data, was "fir-api-cli-0.4.4.tar", last modified: Wed Apr 12 06:07:31 2023, max compression
```

## Comparing `fir-api-cli-0.4.3.tar` & `fir-api-cli-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 13:26:50.657304 fir-api-cli-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1888 2023-03-14 13:26:50.657304 fir-api-cli-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1442 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 13:26:50.647304 fir-api-cli-0.4.3/fir_api_cli/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-03-14 13:19:43.000000 fir-api-cli-0.4.3/fir_api_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/fir_api_cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    12450 2023-03-14 13:19:43.000000 fir-api-cli-0.4.3/fir_api_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/fir_api_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/fir_api_cli/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     7544 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/fir_api_cli/fir.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2023-03-14 12:54:55.000000 fir-api-cli-0.4.3/fir_api_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 13:26:50.657304 fir-api-cli-0.4.3/fir_api_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1888 2023-03-14 13:26:50.000000 fir-api-cli-0.4.3/fir_api_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-03-14 13:26:50.000000 fir-api-cli-0.4.3/fir_api_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 13:26:50.000000 fir-api-cli-0.4.3/fir_api_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-03-14 13:26:50.000000 fir-api-cli-0.4.3/fir_api_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-03-14 13:26:50.000000 fir-api-cli-0.4.3/fir_api_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-14 13:26:50.000000 fir-api-cli-0.4.3/fir_api_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-03-14 13:19:43.000000 fir-api-cli-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-14 13:26:50.657304 fir-api-cli-0.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:07:31.380808 fir-api-cli-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-03-14 12:54:55.000000 fir-api-cli-0.4.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-12 06:07:31.380808 fir-api-cli-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-12 06:01:05.000000 fir-api-cli-0.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:07:31.380808 fir-api-cli-0.4.4/fir_api_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-12 06:01:05.000000 fir-api-cli-0.4.4/fir_api_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-03-14 12:54:55.000000 fir-api-cli-0.4.4/fir_api_cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12450 2023-03-14 13:19:43.000000 fir-api-cli-0.4.4/fir_api_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2023-03-14 12:54:55.000000 fir-api-cli-0.4.4/fir_api_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-03-14 12:54:55.000000 fir-api-cli-0.4.4/fir_api_cli/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     7544 2023-03-14 12:54:55.000000 fir-api-cli-0.4.4/fir_api_cli/fir.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2023-03-14 12:54:55.000000 fir-api-cli-0.4.4/fir_api_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:07:31.380808 fir-api-cli-0.4.4/fir_api_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-04-12 06:07:31.000000 fir-api-cli-0.4.4/fir_api_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-12 06:07:31.000000 fir-api-cli-0.4.4/fir_api_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 06:07:31.000000 fir-api-cli-0.4.4/fir_api_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-12 06:07:31.000000 fir-api-cli-0.4.4/fir_api_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-04-12 06:07:31.000000 fir-api-cli-0.4.4/fir_api_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-12 06:07:31.000000 fir-api-cli-0.4.4/fir_api_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-04-12 06:01:05.000000 fir-api-cli-0.4.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 06:07:31.380808 fir-api-cli-0.4.4/setup.cfg
```

### Comparing `fir-api-cli-0.4.3/LICENSE` & `fir-api-cli-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fir-api-cli-0.4.3/PKG-INFO` & `fir-api-cli-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fir-api-cli
-Version: 0.4.3
+Version: 0.4.4
 Summary: Package for exploring and downloading data from the FIR API service.
 Author-email: "Earth Observation Operation Center (FOK)" <fok@lechnerkozpont.hu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 valid FIR eFöld registration.
 
 More information at: https://efold.gov.hu/
 
 ## Installation
 
 ```bash
-pip install fir-cli
+pip install fir-api-cli
 ```
 
 
 ## Usage
 
 Get some help:
```

### Comparing `fir-api-cli-0.4.3/README.md` & `fir-api-cli-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 valid FIR eFöld registration.
 
 More information at: https://efold.gov.hu/
 
 ## Installation
 
 ```bash
-pip install fir-cli
+pip install fir-api-cli
 ```
 
 
 ## Usage
 
 Get some help:
```

### Comparing `fir-api-cli-0.4.3/fir_api_cli/cli.py` & `fir-api-cli-0.4.4/fir_api_cli/cli.py`

 * *Files identical despite different names*

### Comparing `fir-api-cli-0.4.3/fir_api_cli/config.py` & `fir-api-cli-0.4.4/fir_api_cli/config.py`

 * *Files identical despite different names*

### Comparing `fir-api-cli-0.4.3/fir_api_cli/constants.py` & `fir-api-cli-0.4.4/fir_api_cli/constants.py`

 * *Files identical despite different names*

### Comparing `fir-api-cli-0.4.3/fir_api_cli/fir.py` & `fir-api-cli-0.4.4/fir_api_cli/fir.py`

 * *Files identical despite different names*

### Comparing `fir-api-cli-0.4.3/fir_api_cli/utils.py` & `fir-api-cli-0.4.4/fir_api_cli/utils.py`

 * *Files identical despite different names*

### Comparing `fir-api-cli-0.4.3/fir_api_cli.egg-info/PKG-INFO` & `fir-api-cli-0.4.4/fir_api_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fir-api-cli
-Version: 0.4.3
+Version: 0.4.4
 Summary: Package for exploring and downloading data from the FIR API service.
 Author-email: "Earth Observation Operation Center (FOK)" <fok@lechnerkozpont.hu>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -22,15 +22,15 @@
 valid FIR eFöld registration.
 
 More information at: https://efold.gov.hu/
 
 ## Installation
 
 ```bash
-pip install fir-cli
+pip install fir-api-cli
 ```
 
 
 ## Usage
 
 Get some help:
```

### Comparing `fir-api-cli-0.4.3/pyproject.toml` & `fir-api-cli-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fir-api-cli"
-version = "0.4.3"
+version = "0.4.4"
 description = "Package for exploring and downloading data from the FIR API service."
 authors = [{ name="Earth Observation Operation Center (FOK)", email="fok@lechnerkozpont.hu" }]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

