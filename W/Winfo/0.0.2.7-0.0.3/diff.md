# Comparing `tmp/Winfo-0.0.2.7.tar.gz` & `tmp/Winfo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.2.7.tar", last modified: Tue Apr 11 12:23:18 2023, max compression
+gzip compressed data, was "Winfo-0.0.3.tar", last modified: Tue Apr 11 23:29:04 2023, max compression
```

## Comparing `Winfo-0.0.2.7.tar` & `Winfo-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:23:18.224991 Winfo-0.0.2.7/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.7/LICENSE
--rw-rw-rw-   0        0        0     5833 2023-04-11 12:23:18.223994 Winfo-0.0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     5385 2023-04-11 12:19:53.000000 Winfo-0.0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 12:23:18.210994 Winfo-0.0.2.7/Winfo/
--rw-rw-rw-   0        0        0     2658 2023-04-10 14:29:58.000000 Winfo-0.0.2.7/Winfo/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.2.7/Winfo/cpu.py
--rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.2.7/Winfo/disk.py
--rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.2.7/Winfo/ethernet.py
--rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.2.7/Winfo/gpu.py
--rw-rw-rw-   0        0        0     1339 2023-04-11 12:16:05.000000 Winfo-0.0.2.7/Winfo/memory.py
--rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.2.7/Winfo/motherboard.py
--rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.2.7/Winfo/software.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:23:18.222992 Winfo-0.0.2.7/Winfo.egg-info/
--rw-rw-rw-   0        0        0     5833 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 12:23:18.000000 Winfo-0.0.2.7/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 12:23:18.224991 Winfo-0.0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-11 12:22:23.000000 Winfo-0.0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:29:04.118469 Winfo-0.0.3/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6160 2023-04-11 23:29:04.117469 Winfo-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5714 2023-04-11 23:13:18.000000 Winfo-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 23:29:04.107468 Winfo-0.0.3/Winfo/
+-rw-rw-rw-   0        0        0     2686 2023-04-11 23:02:28.000000 Winfo-0.0.3/Winfo/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.3/Winfo/cpu.py
+-rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.3/Winfo/disk.py
+-rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.3/Winfo/ethernet.py
+-rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.3/Winfo/gpu.py
+-rw-rw-rw-   0        0        0      628 2023-04-11 23:07:57.000000 Winfo-0.0.3/Winfo/internet.py
+-rw-rw-rw-   0        0        0     1339 2023-04-11 12:16:05.000000 Winfo-0.0.3/Winfo/memory.py
+-rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.3/Winfo/motherboard.py
+-rw-rw-rw-   0        0        0     1197 2023-04-10 14:38:42.000000 Winfo-0.0.3/Winfo/software.py
+drwxrwxrwx   0        0        0        0 2023-04-11 23:29:04.115470 Winfo-0.0.3/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     6160 2023-04-11 23:29:03.000000 Winfo-0.0.3/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-04-11 23:29:04.000000 Winfo-0.0.3/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 23:29:04.000000 Winfo-0.0.3/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 23:29:04.000000 Winfo-0.0.3/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 23:29:04.118469 Winfo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      675 2023-04-11 23:00:40.000000 Winfo-0.0.3/setup.py
```

### Comparing `Winfo-0.0.2.7/LICENSE` & `Winfo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/PKG-INFO` & `Winfo-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.7
+Version: 0.0.3
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -164,15 +164,29 @@
 
 ```
 Adapter 1
 Adapter 2
 Adapter 3
 
 ```
+### Internet Connection Information
 
+- Get public IP address
+- Check if you are connected to the internet
+
+```Python
+import Winfo
+
+print("My IP is " + Winfo.internet.publicIP())
+
+if Winfo.internet.isConnected():
+    print("I'm connected to the internet!")
+else:
+    print("I'm not connected to the internet :(")
+```
 ### Motherboard Information
 
 - Get Brandname of your Motherboard
 - Get Manufacturer of your Motherboard
 
 ```Python
 import Winfo
```

### Comparing `Winfo-0.0.2.7/README.md` & `Winfo-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,29 @@
 
 ```
 Adapter 1
 Adapter 2
 Adapter 3
 
 ```
+### Internet Connection Information
 
+- Get public IP address
+- Check if you are connected to the internet
+
+```Python
+import Winfo
+
+print("My IP is " + Winfo.internet.publicIP())
+
+if Winfo.internet.isConnected():
+    print("I'm connected to the internet!")
+else:
+    print("I'm not connected to the internet :(")
+```
 ### Motherboard Information
 
 - Get Brandname of your Motherboard
 - Get Manufacturer of your Motherboard
 
 ```Python
 import Winfo
```

### Comparing `Winfo-0.0.2.7/Winfo/__init__.py` & `Winfo-0.0.3/Winfo/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,7 +59,8 @@
 from Winfo import cpu
 from Winfo import gpu
 from Winfo import disk
 from Winfo import memory
 from Winfo import motherboard
 from Winfo import software
 from Winfo import ethernet
+from Winfo import internet
```

### Comparing `Winfo-0.0.2.7/Winfo/cpu.py` & `Winfo-0.0.3/Winfo/cpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/Winfo/disk.py` & `Winfo-0.0.3/Winfo/disk.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/Winfo/ethernet.py` & `Winfo-0.0.3/Winfo/ethernet.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/Winfo/gpu.py` & `Winfo-0.0.3/Winfo/gpu.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/Winfo/memory.py` & `Winfo-0.0.3/Winfo/memory.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/Winfo/software.py` & `Winfo-0.0.3/Winfo/software.py`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.7/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.3/Winfo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.7
+Version: 0.0.3
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -164,15 +164,29 @@
 
 ```
 Adapter 1
 Adapter 2
 Adapter 3
 
 ```
+### Internet Connection Information
 
+- Get public IP address
+- Check if you are connected to the internet
+
+```Python
+import Winfo
+
+print("My IP is " + Winfo.internet.publicIP())
+
+if Winfo.internet.isConnected():
+    print("I'm connected to the internet!")
+else:
+    print("I'm not connected to the internet :(")
+```
 ### Motherboard Information
 
 - Get Brandname of your Motherboard
 - Get Manufacturer of your Motherboard
 
 ```Python
 import Winfo
```

### Comparing `Winfo-0.0.2.7/setup.py` & `Winfo-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.2.7",
+    version="0.0.3",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
```

