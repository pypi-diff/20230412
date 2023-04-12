# Comparing `tmp/fake_info_generation-0.0.1.tar.gz` & `tmp/fake_info_generation-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_info_generation-0.0.1.tar", last modified: Wed Apr 12 19:27:24 2023, max compression
+gzip compressed data, was "fake_info_generation-0.0.2.tar", last modified: Wed Apr 12 19:40:10 2023, max compression
```

## Comparing `fake_info_generation-0.0.1.tar` & `fake_info_generation-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:27:25.285225 fake_info_generation-0.0.1/
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 fake_info_generation-0.0.1/LICENSE
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3258 2023-04-12 19:27:25.280467 fake_info_generation-0.0.1/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)     2323 2023-04-12 13:04:48.000000 fake_info_generation-0.0.1/README.md
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:27:25.136019 fake_info_generation-0.0.1/fake_info_generation/
--rwxrwxrwx   0 manish    (1000) manish    (1000)      250 2023-04-12 19:25:09.000000 fake_info_generation-0.0.1/fake_info_generation/__init__.py
--rwxrwxrwx   0 manish    (1000) manish    (1000)     6746 2023-04-12 19:12:39.000000 fake_info_generation-0.0.1/fake_info_generation/main.py
-drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:27:25.256463 fake_info_generation-0.0.1/fake_info_generation.egg-info/
--rwxrwxrwx   0 manish    (1000) manish    (1000)     3258 2023-04-12 19:27:24.000000 fake_info_generation-0.0.1/fake_info_generation.egg-info/PKG-INFO
--rwxrwxrwx   0 manish    (1000) manish    (1000)      307 2023-04-12 19:27:24.000000 fake_info_generation-0.0.1/fake_info_generation.egg-info/SOURCES.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 19:27:24.000000 fake_info_generation-0.0.1/fake_info_generation.egg-info/dependency_links.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 19:27:24.000000 fake_info_generation-0.0.1/fake_info_generation.egg-info/requires.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       21 2023-04-12 19:27:24.000000 fake_info_generation-0.0.1/fake_info_generation.egg-info/top_level.txt
--rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 19:27:25.286734 fake_info_generation-0.0.1/setup.cfg
--rwxrwxrwx   0 manish    (1000) manish    (1000)     1147 2023-04-12 19:25:36.000000 fake_info_generation-0.0.1/setup.py
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:40:11.374432 fake_info_generation-0.0.2/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1073 2023-04-12 05:48:21.000000 fake_info_generation-0.0.2/LICENSE
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3256 2023-04-12 19:40:11.369430 fake_info_generation-0.0.2/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     2321 2023-04-12 19:32:49.000000 fake_info_generation-0.0.2/README.md
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:40:11.163704 fake_info_generation-0.0.2/fake_info_generation/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)      250 2023-04-12 19:25:09.000000 fake_info_generation-0.0.2/fake_info_generation/__init__.py
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     6746 2023-04-12 19:12:39.000000 fake_info_generation-0.0.2/fake_info_generation/main.py
+drwxrwxrwx   0 manish    (1000) manish    (1000)        0 2023-04-12 19:40:11.330425 fake_info_generation-0.0.2/fake_info_generation.egg-info/
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     3256 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/PKG-INFO
+-rwxrwxrwx   0 manish    (1000) manish    (1000)      307 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/SOURCES.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)        1 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/dependency_links.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       32 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/requires.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       21 2023-04-12 19:40:10.000000 fake_info_generation-0.0.2/fake_info_generation.egg-info/top_level.txt
+-rwxrwxrwx   0 manish    (1000) manish    (1000)       38 2023-04-12 19:40:11.375425 fake_info_generation-0.0.2/setup.cfg
+-rwxrwxrwx   0 manish    (1000) manish    (1000)     1147 2023-04-12 19:33:22.000000 fake_info_generation-0.0.2/setup.py
```

### Comparing `fake_info_generation-0.0.1/LICENSE` & `fake_info_generation-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_info_generation-0.0.1/PKG-INFO` & `fake_info_generation-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake_info_generation
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
 Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -29,20 +29,20 @@
 ---
 ### Usage 
 1 : Install the requirements library
 : [Faker](https://pypi.org/project/Faker/) and [phone-gen](https://pypi.org/project/phone-gen/)
 
 2 : Import the library
 ```
-from generate_data import generate_data_info
+from fake_info_generation import main
 ```
 
 3 : Call the function module
 ```
-generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
+main.generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
 ```
 
 4 : Response [ This response might change due to random generation ]
 ```
 {   'Address': [   '4711 Michael Canyon Suite 195\nGordonport, NV 01575',
                    '73989 Candace Course\nSouth Brian, ME 01819',
                    'Unit 7929 Box 8142\nDPO AA 71863'],
```

### Comparing `fake_info_generation-0.0.1/README.md` & `fake_info_generation-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 ---
 ### Usage 
 1 : Install the requirements library
 : [Faker](https://pypi.org/project/Faker/) and [phone-gen](https://pypi.org/project/phone-gen/)
 
 2 : Import the library
 ```
-from generate_data import generate_data_info
+from fake_info_generation import main
 ```
 
 3 : Call the function module
 ```
-generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
+main.generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
 ```
 
 4 : Response [ This response might change due to random generation ]
 ```
 {   'Address': [   '4711 Michael Canyon Suite 195\nGordonport, NV 01575',
                    '73989 Candace Course\nSouth Brian, ME 01819',
                    'Unit 7929 Box 8142\nDPO AA 71863'],
```

### Comparing `fake_info_generation-0.0.1/fake_info_generation/main.py` & `fake_info_generation-0.0.2/fake_info_generation/main.py`

 * *Files identical despite different names*

### Comparing `fake_info_generation-0.0.1/fake_info_generation.egg-info/PKG-INFO` & `fake_info_generation-0.0.2/fake_info_generation.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake-info-generation
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Fake Data Generator Package which can generate fake information based on the keys provided. You can customize the generation using the args.
 Home-page: https://gitlab.com/docsumo_dev/local_dev/manish-sharma/-/tree/exp/fake_data_extension?ref_type=heads
 Author: Manish Sharma
 Author-email: manish.sharma@docsumo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -29,20 +29,20 @@
 ---
 ### Usage 
 1 : Install the requirements library
 : [Faker](https://pypi.org/project/Faker/) and [phone-gen](https://pypi.org/project/phone-gen/)
 
 2 : Import the library
 ```
-from generate_data import generate_data_info
+from fake_info_generation import main
 ```
 
 3 : Call the function module
 ```
-generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
+main.generate_data_info(name_count=3, zip_count=3, address_count=3, region='IN')
 ```
 
 4 : Response [ This response might change due to random generation ]
 ```
 {   'Address': [   '4711 Michael Canyon Suite 195\nGordonport, NV 01575',
                    '73989 Candace Course\nSouth Brian, ME 01819',
                    'Unit 7929 Box 8142\nDPO AA 71863'],
```

### Comparing `fake_info_generation-0.0.1/setup.py` & `fake_info_generation-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setuptools.setup(
     name="fake_info_generation", 
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

