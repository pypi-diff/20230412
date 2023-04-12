# Comparing `tmp/universal_date_parser-0.0.2.tar.gz` & `tmp/universal_date_parser-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_date_parser-0.0.2.tar", last modified: Mon Mar 27 09:43:53 2023, max compression
+gzip compressed data, was "universal_date_parser-0.0.2.1.tar", last modified: Wed Apr 12 10:23:53 2023, max compression
```

## Comparing `universal_date_parser-0.0.2.tar` & `universal_date_parser-0.0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 guangyu    (501) staff       (20)        0 2023-03-27 09:43:53.432831 universal_date_parser-0.0.2/
--rw-r--r--   0 guangyu    (501) staff       (20)     2820 2023-03-27 09:43:53.432709 universal_date_parser-0.0.2/PKG-INFO
--rw-r--r--   0 guangyu    (501) staff       (20)     2360 2023-03-27 09:43:17.000000 universal_date_parser-0.0.2/README.md
--rw-r--r--   0 guangyu    (501) staff       (20)       38 2023-03-27 09:43:53.432868 universal_date_parser-0.0.2/setup.cfg
--rw-r--r--   0 guangyu    (501) staff       (20)      769 2023-03-27 09:43:39.000000 universal_date_parser-0.0.2/setup.py
-drwxr-xr-x   0 guangyu    (501) staff       (20)        0 2023-03-27 09:43:53.431975 universal_date_parser-0.0.2/universal_date_parser/
--rw-r--r--   0 guangyu    (501) staff       (20)       52 2023-03-27 09:09:12.000000 universal_date_parser-0.0.2/universal_date_parser/__init__.py
--rw-r--r--   0 guangyu    (501) staff       (20)    11126 2023-03-27 09:16:02.000000 universal_date_parser-0.0.2/universal_date_parser/parser.py
-drwxr-xr-x   0 guangyu    (501) staff       (20)        0 2023-03-27 09:43:53.432538 universal_date_parser-0.0.2/universal_date_parser.egg-info/
--rw-r--r--   0 guangyu    (501) staff       (20)     2820 2023-03-27 09:43:53.000000 universal_date_parser-0.0.2/universal_date_parser.egg-info/PKG-INFO
--rw-r--r--   0 guangyu    (501) staff       (20)      264 2023-03-27 09:43:53.000000 universal_date_parser-0.0.2/universal_date_parser.egg-info/SOURCES.txt
--rw-r--r--   0 guangyu    (501) staff       (20)        1 2023-03-27 09:43:53.000000 universal_date_parser-0.0.2/universal_date_parser.egg-info/dependency_links.txt
--rw-r--r--   0 guangyu    (501) staff       (20)       22 2023-03-27 09:43:53.000000 universal_date_parser-0.0.2/universal_date_parser.egg-info/top_level.txt
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:23:53.713487 universal_date_parser-0.0.2.1/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2903 2023-04-12 10:23:53.713372 universal_date_parser-0.0.2.1/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2441 2023-04-12 10:23:14.000000 universal_date_parser-0.0.2.1/README.md
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       38 2023-04-12 10:23:53.713520 universal_date_parser-0.0.2.1/setup.cfg
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      868 2023-04-12 10:23:14.000000 universal_date_parser-0.0.2.1/setup.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:23:53.712771 universal_date_parser-0.0.2.1/universal_date_parser/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       52 2023-03-27 13:43:32.000000 universal_date_parser-0.0.2.1/universal_date_parser/__init__.py
+-rw-r--r--   0 guangyuhe   (501) staff       (20)    11126 2023-03-27 13:43:32.000000 universal_date_parser-0.0.2.1/universal_date_parser/parser.py
+drwxr-xr-x   0 guangyuhe   (501) staff       (20)        0 2023-04-12 10:23:53.713209 universal_date_parser-0.0.2.1/universal_date_parser.egg-info/
+-rw-r--r--   0 guangyuhe   (501) staff       (20)     2903 2023-04-12 10:23:53.000000 universal_date_parser-0.0.2.1/universal_date_parser.egg-info/PKG-INFO
+-rw-r--r--   0 guangyuhe   (501) staff       (20)      264 2023-04-12 10:23:53.000000 universal_date_parser-0.0.2.1/universal_date_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)        1 2023-04-12 10:23:53.000000 universal_date_parser-0.0.2.1/universal_date_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 guangyuhe   (501) staff       (20)       22 2023-04-12 10:23:53.000000 universal_date_parser-0.0.2.1/universal_date_parser.egg-info/top_level.txt
```

### Comparing `universal_date_parser-0.0.2/PKG-INFO` & `universal_date_parser-0.0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal_date_parser
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A universal date parser to parse any kind of (possible) date strings.
 Home-page: https://github.com/guangyu-he/universal_date_parser
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -98,14 +98,20 @@
 
 ### v0.0.2
 
 #### update
 
 - description and setup updates
 
+### v0.0.2.1
+
+#### bug fix
+
+- fix long desc error in setup.py while installing 
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/universal_date_parser">GitHub</a>, you are
 welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: universal_date_parser Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: universal_date_parser Version: 0.0.2.1 Summary: A
 universal date parser to parse any kind of (possible) date strings. Home-page:
 https://github.com/guangyu-he/universal_date_parser Author: Guangyu He Author-
 email: me@heguangyu.net Classifier: Development Status :: 3 - Alpha Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown #
 Universal Date Parser an universal date parser for python, which can parse date
 string from different formats and localization (including Excel dates) into
@@ -26,11 +26,12 @@
 (date_format="%d.%m.%Y")) # >>> 06.07.1995 date_string = "06/07/1995" a =
 DateParser(date_string, locale="en_US") print(a.to_date_str()) # >>> 1995-06-07
 date_string = "06/07/1995" a = DateParser(date_string, date_format="%d/%m/%Y")
 print(a.to_date_str()) # >>> 1995-07-06 date_string = "Jun/06/1995" a =
 DateParser(date_string) print(a.to_date_str()) # >>> 1995-06-06 date_string =
 "06/Juni/1995" a = DateParser(date_string, locale="de_DE") print(a.to_date_str
 ()) # >>> 1995-06-06 ``` ## Updates Log ### v0.0.1 #### initial upload - first
-version ### v0.0.2 #### update - description and setup updates ## Support feel
+version ### v0.0.2 #### update - description and setup updates ### v0.0.2.1
+#### bug fix - fix long desc error in setup.py while installing ## Support feel
 free to check source code in GitHub, you are welcome to leave any comments.
 2022©Guangyu He, for further support please contact author.
 Email: me@heguangyu.net
```

### Comparing `universal_date_parser-0.0.2/README.md` & `universal_date_parser-0.0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,20 @@
 
 ### v0.0.2
 
 #### update
 
 - description and setup updates
 
+### v0.0.2.1
+
+#### bug fix
+
+- fix long desc error in setup.py while installing 
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/universal_date_parser">GitHub</a>, you are
 welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
```

#### html2text {}

```diff
@@ -20,11 +20,12 @@
 (date_format="%d.%m.%Y")) # >>> 06.07.1995 date_string = "06/07/1995" a =
 DateParser(date_string, locale="en_US") print(a.to_date_str()) # >>> 1995-06-07
 date_string = "06/07/1995" a = DateParser(date_string, date_format="%d/%m/%Y")
 print(a.to_date_str()) # >>> 1995-07-06 date_string = "Jun/06/1995" a =
 DateParser(date_string) print(a.to_date_str()) # >>> 1995-06-06 date_string =
 "06/Juni/1995" a = DateParser(date_string, locale="de_DE") print(a.to_date_str
 ()) # >>> 1995-06-06 ``` ## Updates Log ### v0.0.1 #### initial upload - first
-version ### v0.0.2 #### update - description and setup updates ## Support feel
+version ### v0.0.2 #### update - description and setup updates ### v0.0.2.1
+#### bug fix - fix long desc error in setup.py while installing ## Support feel
 free to check source code in GitHub, you are welcome to leave any comments.
 2022©Guangyu He, for further support please contact author.
 Email: me@heguangyu.net
```

### Comparing `universal_date_parser-0.0.2/setup.py` & `universal_date_parser-0.0.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
-with open('README.md') as fh:
-    long_description = fh.read()
+this_directory = Path(__file__).parent
+with open(this_directory / "README.md", encoding="utf-8") as f:
+    long_description = f.read()
 
 setup(
     name="universal_date_parser",
-    version="0.0.2",
+    version="0.0.2.1",
     author="Guangyu He",
     author_email="me@heguangyu.net",
     description="A universal date parser to parse any kind of (possible) date strings.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/guangyu-he/universal_date_parser",
     install_requires=[],
```

### Comparing `universal_date_parser-0.0.2/universal_date_parser/parser.py` & `universal_date_parser-0.0.2.1/universal_date_parser/parser.py`

 * *Files identical despite different names*

### Comparing `universal_date_parser-0.0.2/universal_date_parser.egg-info/PKG-INFO` & `universal_date_parser-0.0.2.1/universal_date_parser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universal-date-parser
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: A universal date parser to parse any kind of (possible) date strings.
 Home-page: https://github.com/guangyu-he/universal_date_parser
 Author: Guangyu He
 Author-email: me@heguangyu.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -98,14 +98,20 @@
 
 ### v0.0.2
 
 #### update
 
 - description and setup updates
 
+### v0.0.2.1
+
+#### bug fix
+
+- fix long desc error in setup.py while installing 
+
 ## Support
 
 feel free to check source code in <a href="https://github.com/guangyu-he/universal_date_parser">GitHub</a>, you are
 welcome
 to leave any comments.
 
 2022&copy;Guangyu He, for further support please contact author. <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: universal-date-parser Version: 0.0.2 Summary: A
+Metadata-Version: 2.1 Name: universal-date-parser Version: 0.0.2.1 Summary: A
 universal date parser to parse any kind of (possible) date strings. Home-page:
 https://github.com/guangyu-he/universal_date_parser Author: Guangyu He Author-
 email: me@heguangyu.net Classifier: Development Status :: 3 - Alpha Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown #
 Universal Date Parser an universal date parser for python, which can parse date
 string from different formats and localization (including Excel dates) into
@@ -26,11 +26,12 @@
 (date_format="%d.%m.%Y")) # >>> 06.07.1995 date_string = "06/07/1995" a =
 DateParser(date_string, locale="en_US") print(a.to_date_str()) # >>> 1995-06-07
 date_string = "06/07/1995" a = DateParser(date_string, date_format="%d/%m/%Y")
 print(a.to_date_str()) # >>> 1995-07-06 date_string = "Jun/06/1995" a =
 DateParser(date_string) print(a.to_date_str()) # >>> 1995-06-06 date_string =
 "06/Juni/1995" a = DateParser(date_string, locale="de_DE") print(a.to_date_str
 ()) # >>> 1995-06-06 ``` ## Updates Log ### v0.0.1 #### initial upload - first
-version ### v0.0.2 #### update - description and setup updates ## Support feel
+version ### v0.0.2 #### update - description and setup updates ### v0.0.2.1
+#### bug fix - fix long desc error in setup.py while installing ## Support feel
 free to check source code in GitHub, you are welcome to leave any comments.
 2022©Guangyu He, for further support please contact author.
 Email: me@heguangyu.net
```

