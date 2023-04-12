# Comparing `tmp/st_config-0.0.2.tar.gz` & `tmp/st_config-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st_config-0.0.2.tar", last modified: Fri Apr  7 12:54:17 2023, max compression
+gzip compressed data, was "dist/st_config-0.0.3.tar", last modified: Wed Apr 12 09:15:00 2023, max compression
```

## Comparing `st_config-0.0.2.tar` & `st_config-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-07 12:54:17.000000 st_config-0.0.2/
--rw-r--r--   0 nezah      (501) staff       (20)      424 2023-04-07 12:54:17.000000 st_config-0.0.2/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 st_config-0.0.2/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-07 12:54:17.000000 st_config-0.0.2/sconf/
--rw-r--r--   0 nezah      (501) staff       (20)     1192 2023-04-07 12:50:25.000000 st_config-0.0.2/sconf/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-07 12:54:17.000000 st_config-0.0.2/st_config.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      424 2023-04-07 12:54:17.000000 st_config-0.0.2/st_config.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-07 12:54:17.000000 st_config-0.0.2/st_config.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-07 12:54:17.000000 st_config-0.0.2/st_config.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-07 12:54:17.000000 st_config-0.0.2/st_config.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       25 2023-04-07 12:34:19.000000 st_config-0.0.2/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      559 2023-04-07 12:52:06.000000 st_config-0.0.2/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-07 12:54:17.000000 st_config-0.0.2/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:15:00.000000 st_config-0.0.3/
+-rw-r--r--   0 nezah      (501) staff       (20)      424 2023-04-12 09:15:00.000000 st_config-0.0.3/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 st_config-0.0.3/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:15:00.000000 st_config-0.0.3/sconf/
+-rw-r--r--   0 nezah      (501) staff       (20)     1438 2023-04-12 09:14:12.000000 st_config-0.0.3/sconf/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      424 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       25 2023-04-07 12:34:19.000000 st_config-0.0.3/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      559 2023-04-12 09:14:58.000000 st_config-0.0.3/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-12 09:15:00.000000 st_config-0.0.3/setup.cfg
```

### Comparing `st_config-0.0.2/LICENSE` & `st_config-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `st_config-0.0.2/sconf/__init__.py` & `st_config-0.0.3/sconf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import os
 import sys
 import json
+import logging
 
+logger = logging.getLogger(__name__)
 
 class Config(object):
     def __new__(cls, *args, **kwargs):
         if not hasattr(cls, "_instance"):
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, filename="config.json"):
         cls = type(self)
         if not hasattr(cls, "_init"):
-            context_root = os.path.dirname(os.path.abspath(sys.modules['__main__'].__file__))
-            config_file = f"{context_root}/{filename}"
+            env_path = os.getenv("RIGGER_CONFIG_PATH")
+            if env_path is not None:
+                config_file = f"{env_path}/{filename}"
+            else:
+                context_root = os.path.dirname(os.path.abspath(sys.modules['__main__'].__file__))
+                config_file = f"{context_root}/{filename}"
 
             with open(config_file, encoding="UTF-8") as json_file:
                 self.json_data = json.load(json_file)
-                print(f"Loading config.json for [{self.json_data.get('ENV')}] from {config_file}")
+                logger.info(f"Loading config.json for [{self.json_data.get('ENV')}] from {config_file}")
             cls._init = True
 
     def cfg(self, *keys):
         tmp = self.json_data
         try:
             for key in keys:
                 tmp = tmp.get(key)
         except Exception as ex:
-            print(f"exception : {ex}")
+            logger.exception(f"exception : {ex}", ex)
             return None
 
         return tmp
 
 
 if __name__ == "__main__":
     x = Config()
```

### Comparing `st_config-0.0.2/setup.py` & `st_config-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_config",
-    version="0.0.2",
+    version="0.0.3",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="Singleton config for python",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/singleton-config",
     packages=setuptools.find_packages(),
```

