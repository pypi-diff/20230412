# Comparing `tmp/TransLiter-0.1.2.tar.gz` & `tmp/TransLiter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TransLiter-0.1.2.tar", last modified: Sat Apr  8 00:38:20 2023, max compression
+gzip compressed data, was "TransLiter-0.2.0.tar", last modified: Wed Apr 12 04:46:37 2023, max compression
```

## Comparing `TransLiter-0.1.2.tar` & `TransLiter-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-08 00:38:20.490754 TransLiter-0.1.2/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-04-07 00:09:21.000000 TransLiter-0.1.2/LICENSE
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1795 2023-04-08 00:38:20.490616 TransLiter-0.1.2/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1447 2023-04-08 00:37:29.000000 TransLiter-0.1.2/README.md
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-08 00:38:20.489754 TransLiter-0.1.2/TransLiter/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       77 2023-04-08 00:33:07.000000 TransLiter-0.1.2/TransLiter/__init__.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     3264 2023-04-07 00:09:21.000000 TransLiter-0.1.2/TransLiter/jp_list.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1892 2023-04-07 00:09:21.000000 TransLiter-0.1.2/TransLiter/ko_jamo.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1062 2023-04-08 00:33:00.000000 TransLiter-0.1.2/TransLiter/transliter_jp.py
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      691 2023-04-08 00:32:59.000000 TransLiter-0.1.2/TransLiter/transliter_ko.py
-drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-08 00:38:20.490427 TransLiter-0.1.2/TransLiter.egg-info/
--rw-r--r--   0 hoyeolkim   (501) staff       (20)     1795 2023-04-08 00:38:20.000000 TransLiter-0.1.2/TransLiter.egg-info/PKG-INFO
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      351 2023-04-08 00:38:20.000000 TransLiter-0.1.2/TransLiter.egg-info/SOURCES.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-08 00:38:20.000000 TransLiter-0.1.2/TransLiter.egg-info/dependency_links.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-08 00:38:20.000000 TransLiter-0.1.2/TransLiter.egg-info/not-zip-safe
--rw-r--r--   0 hoyeolkim   (501) staff       (20)        9 2023-04-08 00:38:20.000000 TransLiter-0.1.2/TransLiter.egg-info/requires.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-04-08 00:38:20.000000 TransLiter-0.1.2/TransLiter.egg-info/top_level.txt
--rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-04-08 00:38:20.490795 TransLiter-0.1.2/setup.cfg
--rw-r--r--   0 hoyeolkim   (501) staff       (20)      627 2023-04-08 00:19:53.000000 TransLiter-0.1.2/setup.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-12 04:46:37.162894 TransLiter-0.2.0/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1067 2023-04-07 00:09:21.000000 TransLiter-0.2.0/LICENSE
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3915 2023-04-12 04:46:37.162762 TransLiter-0.2.0/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3565 2023-04-12 04:38:49.000000 TransLiter-0.2.0/README.md
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-12 04:46:37.161845 TransLiter-0.2.0/TransLiter/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       77 2023-04-12 04:43:48.000000 TransLiter-0.2.0/TransLiter/__init__.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3264 2023-04-07 00:09:21.000000 TransLiter-0.2.0/TransLiter/jp_list.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1116 2023-04-12 00:32:24.000000 TransLiter-0.2.0/TransLiter/ko_jamo.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     1973 2023-04-12 04:44:11.000000 TransLiter-0.2.0/TransLiter/transliter_jp.py
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     2360 2023-04-12 04:44:08.000000 TransLiter-0.2.0/TransLiter/transliter_ko.py
+drwxr-xr-x   0 hoyeolkim   (501) staff       (20)        0 2023-04-12 04:46:37.162568 TransLiter-0.2.0/TransLiter.egg-info/
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)     3915 2023-04-12 04:46:37.000000 TransLiter-0.2.0/TransLiter.egg-info/PKG-INFO
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      351 2023-04-12 04:46:37.000000 TransLiter-0.2.0/TransLiter.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-12 04:46:37.000000 TransLiter-0.2.0/TransLiter.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)        1 2023-04-12 04:46:37.000000 TransLiter-0.2.0/TransLiter.egg-info/not-zip-safe
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       16 2023-04-12 04:46:37.000000 TransLiter-0.2.0/TransLiter.egg-info/requires.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       11 2023-04-12 04:46:37.000000 TransLiter-0.2.0/TransLiter.egg-info/top_level.txt
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)       38 2023-04-12 04:46:37.162941 TransLiter-0.2.0/setup.cfg
+-rw-r--r--   0 hoyeolkim   (501) staff       (20)      647 2023-04-12 04:39:36.000000 TransLiter-0.2.0/setup.py
```

### Comparing `TransLiter-0.1.2/LICENSE` & `TransLiter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TransLiter-0.1.2/TransLiter/jp_list.py` & `TransLiter-0.2.0/TransLiter/jp_list.py`

 * *Files identical despite different names*

### Comparing `TransLiter-0.1.2/setup.py` & `TransLiter-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='TransLiter',
     python_requires='>=3.6',
-    version='0.1.2',
+    version='0.2.0',
     url='https://github.com/elibooklover/TransLiter',
     license='MIT',
     author='Hoyeol Kim',
     author_email='elibooklover@gmail.com',
-    description='TransLiter transliterates multilingual text to English.',
+    description='TransLiter transliterates multilingual text into English.',
     packages=['TransLiter', ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
     include_package_data=True,
     install_requires=[
+        "pandas",
         "pykakasi"
     ]
 )
```

