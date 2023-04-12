# Comparing `tmp/fake_info_generation-0.0.2.tar.gz` & `tmp/fake_info_generation-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_info_generation-0.0.2.tar", last modified: Wed Apr 12 19:40:10 2023, max compression
+gzip compressed data, was "fake_info_generation-0.0.3.tar", last modified: Wed Apr 12 19:43:44 2023, max compression
```

## Comparing `fake_info_generation-0.0.2.tar` & `fake_info_generation-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:40:11.374432 fake_info_generation-0.0.2/
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 fake_info_generation-0.0.2/LICENSE
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3256 2023-04-12 19:40:11.369430 fake_info_generation-0.0.2/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)     2321 2023-04-12 19:32:49.000000 fake_info_generation-0.0.2/README.md
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:40:11.163704 fake_info_generation-0.0.2/fake_info_generation/
--rwxrwxrwx   0 manish    (1000) manish    (1000)      250 2023-04-12 19:25:09.000000 fake_info_generation-0.0.2/fake_info_generation/__init__.py
--rwxrwxrwx   0 manish    (1000) manish    (1000)     6746 2023-04-12 19:12:39.000000 fake_info_generation-0.0.2/fake_info_generation/main.py
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:40:11.330425 fake_info_generation-0.0.2/fake_info_generation.egg-info/
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3256 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)      307 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/SOURCES.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/dependency_links.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/requires.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       21 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/top_level.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 19:40:11.375425 fake_info_generation-0.0.2/setup.cfg
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1147 2023-04-12 19:33:22.000000 fake_info_generation-0.0.2/setup.py
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:43:45.684212 fake_info_generation-0.0.3/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 fake_info_generation-0.0.3/LICENSE
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3250 2023-04-12 19:43:45.677173 fake_info_generation-0.0.3/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     2321 2023-04-12 19:32:49.000000 fake_info_generation-0.0.3/README.md
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:43:45.466045 fake_info_generation-0.0.3/fake_info_generation/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)      250 2023-04-12 19:25:09.000000 fake_info_generation-0.0.3/fake_info_generation/__init__.py
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     6746 2023-04-12 19:12:39.000000 fake_info_generation-0.0.3/fake_info_generation/main.py
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:43:45.635808 fake_info_generation-0.0.3/fake_info_generation.egg-info/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3250 2023-04-12 19:43:44.000000 fake_info_generation-0.0.3/fake_info_generation.egg-info/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)      307 2023-04-12 19:43:44.000000 fake_info_generation-0.0.3/fake_info_generation.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 19:43:44.000000 fake_info_generation-0.0.3/fake_info_generation.egg-info/dependency_links.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 19:43:44.000000 fake_info_generation-0.0.3/fake_info_generation.egg-info/requires.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       21 2023-04-12 19:43:44.000000 fake_info_generation-0.0.3/fake_info_generation.egg-info/top_level.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 19:43:45.685722 fake_info_generation-0.0.3/setup.cfg
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1141 2023-04-12 19:43:28.000000 fake_info_generation-0.0.3/setup.py
```

### Comparing `fake_info_generation-0.0.2/LICENSE` & `fake_info_generation-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_info_generation-0.0.2/PKG-INFO` & `fake_info_generation-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fake_info_generation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
-Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
+Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_lib?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fake_info_generation-0.0.2/README.md` & `fake_info_generation-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fake_info_generation-0.0.2/fake_info_generation/main.py` & `fake_info_generation-0.0.3/fake_info_generation/main.py`

 * *Files identical despite different names*

### Comparing `fake_info_generation-0.0.2/fake_info_generation.egg-info/PKG-INFO` & `fake_info_generation-0.0.3/fake_info_generation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fake-info-generation
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
-Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
+Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_lib?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fake_info_generation-0.0.2/setup.py` & `fake_info_generation-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="fake_info_generation", 
-    version="0.0.2",
+    version="0.0.3",
     author="Manish Sharma",
     author_email="manish.sharma@docsumo.com",
     description="A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=["Faker==18.4.0", "phone-gen==2.2.25"],
-    url="https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads",
+    url="https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_lib?ref_type=heads",
     packages=['fake_info_generation'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

