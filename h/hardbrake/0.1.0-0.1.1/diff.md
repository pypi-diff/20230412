# Comparing `tmp/hardbrake-0.1.0.tar.gz` & `tmp/hardbrake-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardbrake-0.1.0.tar", last modified: Wed Apr 12 14:54:26 2023, max compression
+gzip compressed data, was "hardbrake-0.1.1.tar", last modified: Wed Apr 12 14:57:17 2023, max compression
```

## Comparing `hardbrake-0.1.0.tar` & `hardbrake-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:54:26.836010 hardbrake-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-12 14:54:01.000000 hardbrake-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 14:54:26.836010 hardbrake-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      940 2023-04-12 14:54:01.000000 hardbrake-0.1.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)      517 2023-04-12 14:54:01.000000 hardbrake-0.1.0/hardbrake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:54:26.836010 hardbrake-0.1.0/hardbrake.egg-info/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 14:54:26.000000 hardbrake-0.1.0/hardbrake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      340 2023-04-12 14:54:26.000000 hardbrake-0.1.0/hardbrake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:54:26.000000 hardbrake-0.1.0/hardbrake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-04-12 14:54:26.000000 hardbrake-0.1.0/hardbrake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-12 14:54:26.000000 hardbrake-0.1.0/hardbrake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-12 14:54:01.000000 hardbrake-0.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 14:54:26.836010 hardbrake-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      502 2023-04-12 14:54:01.000000 hardbrake-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:54:26.836010 hardbrake-0.1.0/src/
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/app.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/event.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/file.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/loader.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/logger.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/manager.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/prompts.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-04-12 14:54:01.000000 hardbrake-0.1.0/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:57:17.214648 hardbrake-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-12 14:56:42.000000 hardbrake-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 14:57:17.214648 hardbrake-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      940 2023-04-12 14:56:42.000000 hardbrake-0.1.1/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      517 2023-04-12 14:56:42.000000 hardbrake-0.1.1/hardbrake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:57:17.210648 hardbrake-0.1.1/hardbrake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      340 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-12 14:57:17.000000 hardbrake-0.1.1/hardbrake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-04-12 14:56:42.000000 hardbrake-0.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 14:57:17.214648 hardbrake-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      502 2023-04-12 14:56:42.000000 hardbrake-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 14:57:17.214648 hardbrake-0.1.1/src/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2270 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/app.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/event.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/file.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/loader.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/prompts.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-04-12 14:56:42.000000 hardbrake-0.1.1/src/utils.py
```

### Comparing `hardbrake-0.1.0/LICENSE` & `hardbrake-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/README.md` & `hardbrake-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/hardbrake` & `hardbrake-0.1.1/hardbrake`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/src/app.py` & `hardbrake-0.1.1/src/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,7 +81,9 @@
   if has_update(current_version, latest_version):
     logger.print(f"New version of {package_name} available: {latest_version}")
     answer = prompts.ask_boolean(f"Do you want to update? ({current_version} -> {latest_version})")
 
     if answer:
       cmd = f"pip install --upgrade {package_name}"
       os.system(cmd)
+  else:
+    logger.success(f"You are using the latest version of {package_name} ({current_version})")
```

### Comparing `hardbrake-0.1.0/src/event.py` & `hardbrake-0.1.1/src/event.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/src/file.py` & `hardbrake-0.1.1/src/file.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/src/loader.py` & `hardbrake-0.1.1/src/loader.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/src/manager.py` & `hardbrake-0.1.1/src/manager.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/src/prompts.py` & `hardbrake-0.1.1/src/prompts.py`

 * *Files identical despite different names*

### Comparing `hardbrake-0.1.0/src/utils.py` & `hardbrake-0.1.1/src/utils.py`

 * *Files identical despite different names*

