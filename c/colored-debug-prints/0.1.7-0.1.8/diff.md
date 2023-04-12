# Comparing `tmp/colored_debug_prints-0.1.7.tar.gz` & `tmp/colored_debug_prints-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colored_debug_prints-0.1.7.tar", last modified: Sun Apr  2 18:12:28 2023, max compression
+gzip compressed data, was "colored_debug_prints-0.1.8.tar", last modified: Wed Apr 12 17:58:46 2023, max compression
```

## Comparing `colored_debug_prints-0.1.7.tar` & `colored_debug_prints-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 18:12:28.893799 colored_debug_prints-0.1.7/
--rw-rw-rw-   0        0        0      533 2023-04-02 18:12:28.892797 colored_debug_prints-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-02 18:12:28.883793 colored_debug_prints-0.1.7/colored_debug_prints/
--rw-rw-rw-   0        0        0      254 2023-04-02 18:12:20.000000 colored_debug_prints-0.1.7/colored_debug_prints/__init__.py
--rw-rw-rw-   0        0        0      361 2023-03-29 14:49:38.000000 colored_debug_prints-0.1.7/colored_debug_prints/colored_prints.py
--rw-rw-rw-   0        0        0     1308 2023-03-29 14:19:21.000000 colored_debug_prints-0.1.7/colored_debug_prints/print_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-02 18:12:28.890794 colored_debug_prints-0.1.7/colored_debug_prints.egg-info/
--rw-rw-rw-   0        0        0      533 2023-04-02 18:12:28.000000 colored_debug_prints-0.1.7/colored_debug_prints.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-02 18:12:28.000000 colored_debug_prints-0.1.7/colored_debug_prints.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 18:12:28.000000 colored_debug_prints-0.1.7/colored_debug_prints.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-02 18:12:28.000000 colored_debug_prints-0.1.7/colored_debug_prints.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-02 18:12:28.000000 colored_debug_prints-0.1.7/colored_debug_prints.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 18:12:28.893799 colored_debug_prints-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-04-02 18:12:04.000000 colored_debug_prints-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:58:46.566419 colored_debug_prints-0.1.8/
+-rw-rw-rw-   0        0        0      546 2023-04-12 17:58:46.566419 colored_debug_prints-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 17:58:46.555415 colored_debug_prints-0.1.8/colored_debug_prints/
+-rw-rw-rw-   0        0        0      254 2023-04-02 18:12:20.000000 colored_debug_prints-0.1.8/colored_debug_prints/__init__.py
+-rw-rw-rw-   0        0        0      361 2023-03-29 14:49:38.000000 colored_debug_prints-0.1.8/colored_debug_prints/colored_prints.py
+-rw-rw-rw-   0        0        0     1575 2023-04-12 17:57:30.000000 colored_debug_prints-0.1.8/colored_debug_prints/print_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:58:46.565419 colored_debug_prints-0.1.8/colored_debug_prints.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-04-12 17:58:46.000000 colored_debug_prints-0.1.8/colored_debug_prints.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-12 17:58:46.000000 colored_debug_prints-0.1.8/colored_debug_prints.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:58:46.000000 colored_debug_prints-0.1.8/colored_debug_prints.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 17:58:46.000000 colored_debug_prints-0.1.8/colored_debug_prints.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-12 17:58:46.000000 colored_debug_prints-0.1.8/colored_debug_prints.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:58:46.567402 colored_debug_prints-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-04-12 17:58:31.000000 colored_debug_prints-0.1.8/setup.py
```

### Comparing `colored_debug_prints-0.1.7/PKG-INFO` & `colored_debug_prints-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: colored_debug_prints
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple colored debug prints
-Author: Leon
+Author: Mistercoolertyper
 Author-email: leonwagner09@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `colored_debug_prints-0.1.7/colored_debug_prints/print_utils.py` & `colored_debug_prints-0.1.8/colored_debug_prints/print_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
     def error(self, textToPrint, extraData=None):
         if (extraData != None):
             print(f"{Fore.RED}[*] {textToPrint} {Fore.LIGHTBLACK_EX}({extraData}){Fore.RESET}")
         else:
             print(f"{Fore.RED}[*] {textToPrint}{Fore.RESET}")
 
+    def success(self, textToPrint, extraData=None):
+        if (extraData != None):
+            print(f"{Fore.GREEN}[*] {textToPrint} {Fore.LIGHTBLACK_EX}({extraData}){Fore.RESET}")
+        else:
+            print(f"{Fore.GREEN}[*] {textToPrint}{Fore.RESET}")
+
 if (__name__ == "__main__"):
     prints = debugPrints()
     prints.info("Hello World!")
     prints.info("Hello World!", "But this is the 2nd print!")
     prints.warn("Hello World, but this is a warning!")
     prints.warn("Hello World, but this is a warning!", "but with extra text")
     prints.error("Hello World, but this is an error!")
```

### Comparing `colored_debug_prints-0.1.7/colored_debug_prints.egg-info/PKG-INFO` & `colored_debug_prints-0.1.8/colored_debug_prints.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: colored-debug-prints
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple colored debug prints
-Author: Leon
+Author: Mistercoolertyper
 Author-email: leonwagner09@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `colored_debug_prints-0.1.7/setup.py` & `colored_debug_prints-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.7' 
+VERSION = '0.1.8' 
 DESCRIPTION = 'Simple colored debug prints'
 LONG_DESCRIPTION = 'Colored print functions like info, warn and error'
 
 setup(
         name="colored_debug_prints", 
         version=VERSION,
-        author="Leon",
+        author="Mistercoolertyper",
         author_email="leonwagner09@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=["colorama"],
         
         keywords=['python', 'first package'],
```

