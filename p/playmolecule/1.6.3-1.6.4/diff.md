# Comparing `tmp/playmolecule-1.6.3.tar.gz` & `tmp/playmolecule-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.6.3.tar", last modified: Tue Apr 11 14:00:56 2023, max compression
+gzip compressed data, was "playmolecule-1.6.4.tar", last modified: Wed Apr 12 13:44:59 2023, max compression
```

## Comparing `playmolecule-1.6.3.tar` & `playmolecule-1.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:00:56.456857 playmolecule-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-11 14:00:44.000000 playmolecule-1.6.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 14:00:44.000000 playmolecule-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 14:00:56.456857 playmolecule-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 14:00:44.000000 playmolecule-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:00:56.456857 playmolecule-1.6.3/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32923 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-11 14:00:44.000000 playmolecule-1.6.3/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:00:56.456857 playmolecule-1.6.3/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 14:00:56.000000 playmolecule-1.6.3/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 14:00:44.000000 playmolecule-1.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:00:56.456857 playmolecule-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 14:00:44.000000 playmolecule-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:44:59.987275 playmolecule-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-12 13:44:49.000000 playmolecule-1.6.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 13:44:49.000000 playmolecule-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 13:44:59.987275 playmolecule-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-12 13:44:49.000000 playmolecule-1.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:44:59.987275 playmolecule-1.6.4/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-12 13:44:49.000000 playmolecule-1.6.4/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:44:59.987275 playmolecule-1.6.4/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 13:44:59.000000 playmolecule-1.6.4/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 13:44:49.000000 playmolecule-1.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:44:59.987275 playmolecule-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-12 13:44:49.000000 playmolecule-1.6.4/setup.py
```

### Comparing `playmolecule-1.6.3/LICENSE.md` & `playmolecule-1.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/PKG-INFO` & `playmolecule-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.3
+Version: 1.6.4
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.3/playmolecule/__init__.py` & `playmolecule-1.6.4/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/_test_funcs.py` & `playmolecule-1.6.4/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/config.py` & `playmolecule-1.6.4/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/datacenter.py` & `playmolecule-1.6.4/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/devutils.py` & `playmolecule-1.6.4/playmolecule/devutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
         newvals = []
         for val in ensurelist(value):  # Handling for list values
             # Download DataCenter files
             if isinstance(val, str) and val.startswith("dc://"):
                 ds = Dataset(val, _session=session)
                 dl_dir = os.path.join(indir, str(ds.datasetid))
                 val = ds.download(dl_dir)
-                input_args[name] = str(val)
+                newvals.append(val)
                 continue
             # Rebase file directories
             if val is not None and dtype in ("file", "Path"):
                 val = _rebase_file2(val, indir)
             newvals.append(val)
 
         if len(newvals) == 1:
@@ -1042,8 +1042,7 @@
             f.write(f"Unexpected error occurred in wrapper: {e}\n")
             traceback.print_exc(file=f)
 
         try:
             job._set_error()
         except Exception:
             pass
-
```

### Comparing `playmolecule-1.6.3/playmolecule/func2argparse.py` & `playmolecule-1.6.4/playmolecule/func2argparse.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/job.py` & `playmolecule-1.6.4/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/jsonlogger.py` & `playmolecule-1.6.4/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/local.py` & `playmolecule-1.6.4/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/playqueue.py` & `playmolecule-1.6.4/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/session.py` & `playmolecule-1.6.4/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule/utils.py` & `playmolecule-1.6.4/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.6.4/playmolecule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.3
+Version: 1.6.4
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.3/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.6.4/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.3/setup.py` & `playmolecule-1.6.4/setup.py`

 * *Files identical despite different names*

