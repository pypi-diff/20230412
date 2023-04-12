# Comparing `tmp/userlex-0.0.1.tar.gz` & `tmp/userlex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userlex-0.0.1.tar", last modified: Wed Apr  5 11:39:10 2023, max compression
+gzip compressed data, was "userlex-0.0.2.tar", last modified: Wed Apr 12 17:18:50 2023, max compression
```

## Comparing `userlex-0.0.1.tar` & `userlex-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 11:39:10.990861 userlex-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-04-05 11:39:10.990861 userlex-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-05 11:38:56.000000 userlex-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-05 11:39:10.990861 userlex-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-05 11:38:56.000000 userlex-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 11:39:10.990861 userlex-0.0.1/userlex/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-05 11:38:56.000000 userlex-0.0.1/userlex/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-05 11:38:56.000000 userlex-0.0.1/userlex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 11:39:10.990861 userlex-0.0.1/userlex/social_media/
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-05 11:38:56.000000 userlex-0.0.1/userlex/social_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2023-04-05 11:38:56.000000 userlex-0.0.1/userlex/social_media/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      583 2023-04-05 11:38:56.000000 userlex-0.0.1/userlex/social_media/instagram.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 11:39:10.990861 userlex-0.0.1/userlex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-04-05 11:39:10.000000 userlex-0.0.1/userlex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-04-05 11:39:10.000000 userlex-0.0.1/userlex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-05 11:39:10.000000 userlex-0.0.1/userlex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-05 11:39:10.000000 userlex-0.0.1/userlex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-05 11:39:10.000000 userlex-0.0.1/userlex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-05 11:39:10.000000 userlex-0.0.1/userlex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 17:18:50.704573 userlex-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-04-12 17:18:50.704573 userlex-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-12 17:18:36.000000 userlex-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 17:18:50.704573 userlex-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-04-12 17:18:36.000000 userlex-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 17:18:50.700573 userlex-0.0.2/userlex/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 17:18:50.700573 userlex-0.0.2/userlex/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 17:18:50.700573 userlex-0.0.2/userlex/social_media/
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2275 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/line.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/skype.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-12 17:18:36.000000 userlex-0.0.2/userlex/social_media/telegram.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 17:18:50.700573 userlex-0.0.2/userlex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      974 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-12 17:18:50.000000 userlex-0.0.2/userlex.egg-info/top_level.txt
```

### Comparing `userlex-0.0.1/PKG-INFO` & `userlex-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userlex
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to extract social media and other useful things
 Home-page: https://github.com/dvershinin/userlex
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `userlex-0.0.1/README.md` & `userlex-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `userlex-0.0.1/setup.py` & `userlex-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 """
 userlex
 """
-
 from setuptools import find_packages, setup
 import os
 
 install_requires = []
-tests_requires = ["pytest", "flake8"]
+tests_requires = ["pytest", "flake8", "pyyaml"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 base_dir = os.path.dirname(__file__)
 
 version = {}
@@ -30,13 +29,14 @@
     packages=find_packages(exclude=["tests"]),
     zip_safe=False,
     license="BSD",
     install_requires=install_requires,
     extras_require={
         "tests": install_requires + tests_requires,
     },
+    entry_points={"console_scripts": ["userlex = userlex.cli:main"]},
     tests_require=tests_requires,
     include_package_data=True,
     classifiers=[
         "Intended Audience :: Developers"
     ],
 )
```

### Comparing `userlex-0.0.1/userlex/social_media/instagram.py` & `userlex-0.0.2/userlex/social_media/instagram.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 
 from userlex.social_media import SocialMedia
 
 
 class Instagram(SocialMedia):
     PLATFORM_NAME = "instagram"
 
-    USERNAME_REGEX = re.compile(r'insta(?:gram)?:?\s+@(?P<username>\S+)\b', re.IGNORECASE)
+    USERNAME_REGEXES = [
+        r'insta(?:gram)?:?\s+@?(?P<username>\S+)\b',
+        r'\big\s*:\s+@?(?P<username>\w+)\b'
+    ]
 
     def __init__(self, username):
         self.username = username
 
     @property
     def url(self):
         return f"https://www.instagram.com/{self.username}/"
 
     @staticmethod
     def from_username(username):
         return Instagram(username)
 
     @staticmethod
     def matches_username(username):
-        return bool(Instagram.USERNAME_REGEX.fullmatch(username))
+        return bool(Instagram.USERNAME_REGEXES.fullmatch(username))
```

### Comparing `userlex-0.0.1/userlex.egg-info/PKG-INFO` & `userlex-0.0.2/userlex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userlex
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to extract social media and other useful things
 Home-page: https://github.com/dvershinin/userlex
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

