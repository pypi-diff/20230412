# Comparing `tmp/st_config-0.0.3.tar.gz` & `tmp/st_config-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/st_config-0.0.3.tar", last modified: Wed Apr 12 09:15:00 2023, max compression
+gzip compressed data, was "dist/st_config-0.0.4.tar", last modified: Wed Apr 12 09:17:08 2023, max compression
```

## Comparing `st_config-0.0.3.tar` & `st_config-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:15:00.000000 st_config-0.0.3/
--rw-r--r--   0 nezah      (501) staff       (20)      424 2023-04-12 09:15:00.000000 st_config-0.0.3/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 st_config-0.0.3/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:15:00.000000 st_config-0.0.3/sconf/
--rw-r--r--   0 nezah      (501) staff       (20)     1438 2023-04-12 09:14:12.000000 st_config-0.0.3/sconf/__init__.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      424 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-12 09:15:00.000000 st_config-0.0.3/st_config.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       25 2023-04-07 12:34:19.000000 st_config-0.0.3/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      559 2023-04-12 09:14:58.000000 st_config-0.0.3/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-12 09:15:00.000000 st_config-0.0.3/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:17:08.000000 st_config-0.0.4/
+-rw-r--r--   0 nezah      (501) staff       (20)      470 2023-04-12 09:17:08.000000 st_config-0.0.4/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1068 2023-04-07 12:34:51.000000 st_config-0.0.4/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:17:08.000000 st_config-0.0.4/sconf/
+-rw-r--r--   0 nezah      (501) staff       (20)     1430 2023-04-12 09:17:08.000000 st_config-0.0.4/sconf/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      470 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-12 09:17:08.000000 st_config-0.0.4/st_config.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       71 2023-04-12 09:17:08.000000 st_config-0.0.4/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      559 2023-04-12 09:17:08.000000 st_config-0.0.4/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-12 09:17:08.000000 st_config-0.0.4/setup.cfg
```

### Comparing `st_config-0.0.3/LICENSE` & `st_config-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_config-0.0.3/sconf/__init__.py` & `st_config-0.0.4/sconf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         if not hasattr(cls, "_instance"):
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, filename="config.json"):
         cls = type(self)
         if not hasattr(cls, "_init"):
-            env_path = os.getenv("RIGGER_CONFIG_PATH")
+            env_path = os.getenv("SCONF_PATH")
             if env_path is not None:
                 config_file = f"{env_path}/{filename}"
             else:
                 context_root = os.path.dirname(os.path.abspath(sys.modules['__main__'].__file__))
                 config_file = f"{context_root}/{filename}"
 
             with open(config_file, encoding="UTF-8") as json_file:
```

### Comparing `st_config-0.0.3/setup.py` & `st_config-0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st_config",
-    version="0.0.3",
+    version="0.0.4",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="Singleton config for python",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/singleton-config",
     packages=setuptools.find_packages(),
```

