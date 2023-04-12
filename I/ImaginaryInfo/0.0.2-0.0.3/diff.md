# Comparing `tmp/ImaginaryInfo-0.0.2.tar.gz` & `tmp/ImaginaryInfo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImaginaryInfo-0.0.2.tar", last modified: Wed Apr 12 13:05:14 2023, max compression
+gzip compressed data, was "ImaginaryInfo-0.0.3.tar", last modified: Wed Apr 12 18:15:40 2023, max compression
```

## Comparing `ImaginaryInfo-0.0.2.tar` & `ImaginaryInfo-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,10 @@
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 13:05:14.646823 ImaginaryInfo-0.0.2/
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 13:05:14.626514 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3215 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)      210 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/SOURCES.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/dependency_links.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/requires.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/top_level.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 ImaginaryInfo-0.0.2/LICENSE
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3215 2023-04-12 13:05:14.643802 ImaginaryInfo-0.0.2/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)     2323 2023-04-12 13:04:48.000000 ImaginaryInfo-0.0.2/README.md
--rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 13:05:14.647818 ImaginaryInfo-0.0.2/setup.cfg
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1142 2023-04-12 13:05:01.000000 ImaginaryInfo-0.0.2/setup.py
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 18:15:42.108914 ImaginaryInfo-0.0.3/
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 18:15:42.070333 ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3193 2023-04-12 18:15:41.000000 ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)      192 2023-04-12 18:15:41.000000 ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 18:15:41.000000 ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 18:15:41.000000 ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/requires.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 18:15:41.000000 ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/top_level.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3193 2023-04-12 18:15:42.104393 ImaginaryInfo-0.0.3/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 18:15:42.108914 ImaginaryInfo-0.0.3/setup.cfg
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1227 2023-04-12 18:14:33.000000 ImaginaryInfo-0.0.3/setup.py
```

### Comparing `ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/PKG-INFO` & `ImaginaryInfo-0.0.3/ImaginaryInfo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImaginaryInfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
 Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ### Fake data Generator Library
 ---
 ### Description
 - This library intends to generate Fake Information based on the keys provided and count associated with them
 - You can generate "n" number of information using this library
 - This library internally uses `Faker` and `Phone-gen` library
```

### Comparing `ImaginaryInfo-0.0.2/PKG-INFO` & `ImaginaryInfo-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImaginaryInfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
 Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ### Fake data Generator Library
 ---
 ### Description
 - This library intends to generate Fake Information based on the keys provided and count associated with them
 - You can generate "n" number of information using this library
 - This library internally uses `Faker` and `Phone-gen` library
```

### Comparing `ImaginaryInfo-0.0.2/setup.py` & `ImaginaryInfo-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("/mnt/g/Users/Manish/Desktop/docsumo_dev/data_scaling/manish-sharma/fake_data_package/README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="ImaginaryInfo", 
-    version="0.0.2",
+    version="0.0.3",
     author="Manish Sharma",
     author_email="manish.sharma@docsumo.com",
     description="A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=["Faker==18.4.0", "phone-gen==2.2.25"],
     url="https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads",
```

