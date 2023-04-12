# Comparing `tmp/ImaginaryInfo-0.0.1.tar.gz` & `tmp/ImaginaryInfo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImaginaryInfo-0.0.1.tar", last modified: Wed Apr 12 12:04:22 2023, max compression
+gzip compressed data, was "ImaginaryInfo-0.0.2.tar", last modified: Wed Apr 12 13:05:14 2023, max compression
```

## Comparing `ImaginaryInfo-0.0.1.tar` & `ImaginaryInfo-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 12:04:22.423211 ImaginaryInfo-0.0.1/
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 12:04:22.382559 ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3220 2023-04-12 12:04:22.000000 ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)      210 2023-04-12 12:04:22.000000 ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/SOURCES.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 12:04:22.000000 ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/dependency_links.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 12:04:22.000000 ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/requires.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 12:04:22.000000 ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/top_level.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 ImaginaryInfo-0.0.1/LICENSE
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3220 2023-04-12 12:04:22.420159 ImaginaryInfo-0.0.1/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)     2328 2023-04-12 07:15:48.000000 ImaginaryInfo-0.0.1/README.md
--rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 12:04:22.423211 ImaginaryInfo-0.0.1/setup.cfg
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1142 2023-04-12 12:04:11.000000 ImaginaryInfo-0.0.1/setup.py
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 13:05:14.646823 ImaginaryInfo-0.0.2/
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 13:05:14.626514 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3215 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)      210 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/dependency_links.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/requires.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 13:05:14.000000 ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/top_level.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 ImaginaryInfo-0.0.2/LICENSE
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3215 2023-04-12 13:05:14.643802 ImaginaryInfo-0.0.2/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     2323 2023-04-12 13:04:48.000000 ImaginaryInfo-0.0.2/README.md
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 13:05:14.647818 ImaginaryInfo-0.0.2/setup.cfg
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1142 2023-04-12 13:05:01.000000 ImaginaryInfo-0.0.2/setup.py
```

### Comparing `ImaginaryInfo-0.0.1/ImaginaryInfo.egg-info/PKG-INFO` & `ImaginaryInfo-0.0.2/ImaginaryInfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImaginaryInfo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
 Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ---
 ### Usage 
 1 : Install the requirements library
 : [Faker](https://pypi.org/project/Faker/) and [phone-gen](https://pypi.org/project/phone-gen/)
 
 2 : Import the library
 ```
-from fake_data_generate import generate_data_info
+from generate_data import generate_data_info
 ```
 
 3 : Call the function module
 ```
 generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
 ```
```

### Comparing `ImaginaryInfo-0.0.1/LICENSE` & `ImaginaryInfo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ImaginaryInfo-0.0.1/PKG-INFO` & `ImaginaryInfo-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ImaginaryInfo
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
 Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 ---
 ### Usage 
 1 : Install the requirements library
 : [Faker](https://pypi.org/project/Faker/) and [phone-gen](https://pypi.org/project/phone-gen/)
 
 2 : Import the library
 ```
-from fake_data_generate import generate_data_info
+from generate_data import generate_data_info
 ```
 
 3 : Call the function module
 ```
 generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
 ```
```

### Comparing `ImaginaryInfo-0.0.1/README.md` & `ImaginaryInfo-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ---
 ### Usage 
 1 : Install the requirements library
 : [Faker](https://pypi.org/project/Faker/) and [phone-gen](https://pypi.org/project/phone-gen/)
 
 2 : Import the library
 ```
-from fake_data_generate import generate_data_info
+from generate_data import generate_data_info
 ```
 
 3 : Call the function module
 ```
 generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
 ```
```

### Comparing `ImaginaryInfo-0.0.1/setup.py` & `ImaginaryInfo-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="ImaginaryInfo", 
-    version="0.0.1",
+    version="0.0.2",
     author="Manish Sharma",
     author_email="manish.sharma@docsumo.com",
     description="A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=["Faker==18.4.0", "phone-gen==2.2.25"],
     url="https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads",
```

