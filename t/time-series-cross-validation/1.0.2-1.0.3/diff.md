# Comparing `tmp/time_series_cross_validation-1.0.2.tar.gz` & `tmp/time_series_cross_validation-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series_cross_validation-1.0.2.tar", last modified: Tue Apr 11 21:14:35 2023, max compression
+gzip compressed data, was "time_series_cross_validation-1.0.3.tar", last modified: Wed Apr 12 13:45:44 2023, max compression
```

## Comparing `time_series_cross_validation-1.0.2.tar` & `time_series_cross_validation-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:14:35.466142 time_series_cross_validation-1.0.2/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 20:55:29.000000 time_series_cross_validation-1.0.2/LICENCE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-11 21:14:35.462142 time_series_cross_validation-1.0.2/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       35 2023-04-11 20:55:44.000000 time_series_cross_validation-1.0.2/README.md
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 21:14:35.466142 time_series_cross_validation-1.0.2/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      784 2023-04-11 21:14:16.000000 time_series_cross_validation-1.0.2/setup.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:14:35.462142 time_series_cross_validation-1.0.2/time_series_cross_validation/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       56 2023-04-11 21:13:00.000000 time_series_cross_validation-1.0.2/time_series_cross_validation/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     6143 2023-04-11 21:14:00.000000 time_series_cross_validation-1.0.2/time_series_cross_validation/time_series_cross_validation.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 21:14:35.462142 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      391 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       32 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       29 2023-04-11 21:14:35.000000 time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/top_level.txt
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 20:55:29.000000 time_series_cross_validation-1.0.3/LICENSE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       35 2023-04-11 20:55:44.000000 time_series_cross_validation-1.0.3/README.md
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      784 2023-04-12 13:45:17.000000 time_series_cross_validation-1.0.3/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/time_series_cross_validation/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       56 2023-04-11 21:13:00.000000 time_series_cross_validation-1.0.3/time_series_cross_validation/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     6185 2023-04-12 13:45:01.000000 time_series_cross_validation-1.0.3/time_series_cross_validation/time_series_cross_validation.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-12 13:45:44.591994 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      561 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      391 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       32 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       29 2023-04-12 13:45:44.000000 time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/top_level.txt
```

### Comparing `time_series_cross_validation-1.0.2/LICENCE.txt` & `time_series_cross_validation-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `time_series_cross_validation-1.0.2/PKG-INFO` & `time_series_cross_validation-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: time_series_cross_validation
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for cross-validating time series
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep time series cross validation data science
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
-License-File: LICENCE.txt
+License-File: LICENSE.txt
 
 Library for cross-validating time series
```

### Comparing `time_series_cross_validation-1.0.2/setup.py` & `time_series_cross_validation-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='time_series_cross_validation',
-    version='1.0.2',
+    version='1.0.3',
     description='Library for cross-validating time series',
     long_description = 'Library for cross-validating time series',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['time_series_cross_validation'],
     license = 'MIT',
```

### Comparing `time_series_cross_validation-1.0.2/time_series_cross_validation/time_series_cross_validation.py` & `time_series_cross_validation-1.0.3/time_series_cross_validation/time_series_cross_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,20 +106,20 @@
             print('Interrupted process!')
             return None
     
     def view_folds(self, _format='%m-%d-%y'):
         plt.figure(figsize=(16, 6))
         plt.xticks(rotation=90)
         df = pd.DataFrame(self.folds).T
-        for row in range(len(df)):
-            plt.text(df.loc[row, 'begin'], row + 0.05, df.loc[row, 'begin'].strftime(format=_format), ha='center')
-            plt.hlines(row, df.loc[row, 'begin'], df.loc[row, 'split'], 'b')
-            plt.text(df.loc[row, 'split'], row + 0.05, df.loc[row, 'split'].strftime(format=_format), ha='center')
-            plt.hlines(row, df.loc[row, 'split'], df.loc[row, 'end'], 'r')
-            plt.text(df.loc[row, 'end'], row + 0.05, df.loc[row, 'end'].strftime(format=_format), ha='center')
+        for k_fold in df.index:
+            plt.text(df.loc[k_fold, 'begin'], k_fold + 0.05, df.loc[k_fold, 'begin'].strftime(format=_format), ha='center')
+            plt.hlines(k_fold, df.loc[k_fold, 'begin'], df.loc[k_fold, 'split'], 'b')
+            plt.text(df.loc[k_fold, 'split'], k_fold + 0.05, df.loc[k_fold, 'split'].strftime(format=_format), ha='center')
+            plt.hlines(k_fold, df.loc[k_fold, 'split'], df.loc[k_fold, 'end'], 'r')
+            plt.text(df.loc[k_fold, 'end'], k_fold + 0.05, df.loc[k_fold, 'end'].strftime(format=_format), ha='center')
         return None
             
     def validate(self, X, y, time_series, model=None, metrics_function=None):
         cronometer = self.Cronometer()
         cronometer.start()
 
         for k_fold, fold in self.folds.items():
```

### Comparing `time_series_cross_validation-1.0.2/time_series_cross_validation.egg-info/PKG-INFO` & `time_series_cross_validation-1.0.3/time_series_cross_validation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: time-series-cross-validation
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for cross-validating time series
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep time series cross validation data science
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
-License-File: LICENCE.txt
+License-File: LICENSE.txt
 
 Library for cross-validating time series
```

