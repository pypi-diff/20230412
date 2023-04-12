# Comparing `tmp/nonebot-plugin-clock-0.7.2.tar.gz` & `tmp/nonebot-plugin-clock-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-clock-0.7.2.tar", last modified: Wed Apr 12 10:24:51 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.7.3.tar", last modified: Wed Apr 12 10:33:48 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.7.2.tar` & `nonebot-plugin-clock-0.7.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:24:51.214804 nonebot-plugin-clock-0.7.2/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.2/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      299 2023-04-12 10:24:51.214549 nonebot-plugin-clock-0.7.2/PKG-INFO
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:24:51.212102 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     5674 2023-04-12 10:13:10.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1820 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:24:51.214193 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      299 2023-04-12 10:24:51.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      331 2023-04-12 10:24:51.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-12 10:24:51.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 10:24:51.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-12 10:24:51.000000 nonebot-plugin-clock-0.7.2/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-12 10:24:51.214930 nonebot-plugin-clock-0.7.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-12 10:24:14.000000 nonebot-plugin-clock-0.7.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:33:48.000000 nonebot-plugin-clock-0.7.3/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.3/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.7.3/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-12 10:33:48.000000 nonebot-plugin-clock-0.7.3/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1284 2023-04-12 10:23:52.000000 nonebot-plugin-clock-0.7.3/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:33:48.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     5674 2023-04-12 10:13:10.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1820 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-12 10:33:48.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-12 10:33:47.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-12 10:33:47.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-12 10:33:47.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 10:33:47.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-12 10:33:47.000000 nonebot-plugin-clock-0.7.3/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.7.3/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-12 10:33:48.000000 nonebot-plugin-clock-0.7.3/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-12 10:33:36.000000 nonebot-plugin-clock-0.7.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nonebot-plugin-clock-0.7.2/LICENSE` & `nonebot-plugin-clock-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.7.2/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.7.3/nonebot_plugin_clock/database.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.7.2/setup.py` & `nonebot-plugin-clock-0.7.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.7.2',
+    version='0.7.3',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

