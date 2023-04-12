# Comparing `tmp/sroll-0.2.9.5.tar.gz` & `tmp/sroll-0.2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sroll-0.2.9.5.tar", last modified: Fri Apr  7 10:17:09 2023, max compression
+gzip compressed data, was "dist/sroll-0.2.9.6.tar", last modified: Wed Apr 12 13:38:23 2023, max compression
```

## Comparing `sroll-0.2.9.5.tar` & `sroll-0.2.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-07 10:17:09.000000 sroll-0.2.9.5/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       38 2023-04-07 10:17:09.000000 sroll-0.2.9.5/setup.cfg
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       46 2023-01-26 14:13:59.000000 sroll-0.2.9.5/MANIFEST.in
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      787 2023-04-07 10:16:59.000000 sroll-0.2.9.5/setup.py
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll.egg-info/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)        1 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll.egg-info/dependency_links.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      253 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll.egg-info/SOURCES.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       21 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll.egg-info/requires.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll.egg-info/PKG-INFO
--rw-r--r--   0 tfoulqui (205105) droos    (10042)       14 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll.egg-info/top_level.txt
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll_package/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)     8278 2023-04-07 10:14:52.000000 sroll-0.2.9.5/sroll_package/set_env.py
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      142 2023-01-26 14:13:59.000000 sroll-0.2.9.5/sroll_package/__init__.py
-drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-07 10:17:09.000000 sroll-0.2.9.5/sroll_package/static/
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      793 2023-03-29 12:59:48.000000 sroll-0.2.9.5/sroll_package/static/requirements.txt
--rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-07 10:17:09.000000 sroll-0.2.9.5/PKG-INFO
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       38 2023-04-12 13:38:23.000000 sroll-0.2.9.6/setup.cfg
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       46 2023-01-26 14:13:59.000000 sroll-0.2.9.6/MANIFEST.in
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      787 2023-04-12 13:38:13.000000 sroll-0.2.9.6/setup.py
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll.egg-info/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)        1 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/dependency_links.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      253 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll.egg-info/SOURCES.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       21 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/requires.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/PKG-INFO
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)       14 2023-04-12 13:38:22.000000 sroll-0.2.9.6/sroll.egg-info/top_level.txt
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll_package/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)     8266 2023-04-12 13:37:43.000000 sroll-0.2.9.6/sroll_package/set_env.py
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      142 2023-01-26 14:13:59.000000 sroll-0.2.9.6/sroll_package/__init__.py
+drwxr-xr-x   0 tfoulqui (205105) droos    (10042)        0 2023-04-12 13:38:23.000000 sroll-0.2.9.6/sroll_package/static/
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      793 2023-03-29 12:59:48.000000 sroll-0.2.9.6/sroll_package/static/requirements.txt
+-rw-r--r--   0 tfoulqui (205105) droos    (10042)      506 2023-04-12 13:38:23.000000 sroll-0.2.9.6/PKG-INFO
```

### Comparing `sroll-0.2.9.5/setup.py` & `sroll-0.2.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 
 
 
 setuptools.setup(
     name='sroll',
-    version='0.2.9.5',    
+    version='0.2.9.6',    
     description='Python package for SRoll installation',    
     url='https://gitlab.ifremer.fr/iaocea/srollex.git',
     author='Theo Foulquier',
     author_email='tfoulqui@ifremer.fr',
     license='BSD 2-clause',
     include_package_data = True,
     packages=['sroll_package'],
```

### Comparing `sroll-0.2.9.5/sroll_package/set_env.py` & `sroll-0.2.9.6/sroll_package/set_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,28 +19,28 @@
   mapout =str(path)+"/MAP/"+str(name)+"_maps/"
   vecout = str(path)+"/VEC/"+str(name)+"_vecs/"
   
   os.system('mkdir -p '+str(mapout))
   os.system('mkdir -p '+str(vecout))
   
   # Read in the file
-  with open(str(path)+"/srollex/sroll4/unit_test_"+str(name)+".py", 'r') as file :
+  with open(str(path)+"/srollex/sroll4/test"+str(name)+".py", 'r') as file :
     filedata = file.read()
 
   # Replace the target string
   filedata = filedata.replace('Out_MAP = ','Out_MAP = ["'+str(mapout)+'Nside%s_%s"%(Nside,i) for i in bolo_map]')
   filedata = filedata.replace('Out_VEC = ','Out_VEC = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_Offset = ','Out_Offset = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_Offset_corr = ','Out_Offset_corr = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_xi2 = ','Out_xi2 = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
   filedata = filedata.replace('Out_xi2_corr = ','Out_xi2_corr = ["'+str(vecout)+'Nside%s_%s"%(Nside,i) for i in bolo]')
 
 
   # Write the file out again
-  with open(str(path)+"/srollex/sroll4/unit_test_"+str(name)+".py", 'w') as file:
+  with open(str(path)+"/srollex/sroll4/test"+str(name)+".py", 'w') as file:
     file.write(filedata)
 
   
 # -------------------------------------------------------
 def clone_repository(path):
   """
     Clone SRoll repository from git using path given
```

### Comparing `sroll-0.2.9.5/sroll_package/static/requirements.txt` & `sroll-0.2.9.6/sroll_package/static/requirements.txt`

 * *Files identical despite different names*

