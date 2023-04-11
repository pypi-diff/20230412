# Comparing `tmp/print_position-1.0.0.tar.gz` & `tmp/print_position-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "print_position-1.0.0.tar", last modified: Sat Mar 25 08:30:51 2023, max compression
+gzip compressed data, was "print_position-1.0.1.tar", last modified: Tue Apr 11 22:36:58 2023, max compression
```

## Comparing `print_position-1.0.0.tar` & `print_position-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-03-25 08:30:51.074586 print_position-1.0.0/
--rw-r--r--   0 pranav    (1000) pranav    (1001)     1068 2023-03-25 04:34:20.000000 print_position-1.0.0/LICENSE
--rw-r--r--   0 pranav    (1000) pranav    (1001)        0 2023-03-21 18:48:05.000000 print_position-1.0.0/MANIFEST.in
--rw-r--r--   0 pranav    (1000) pranav    (1001)     2537 2023-03-25 08:30:51.074586 print_position-1.0.0/PKG-INFO
--rw-r--r--   0 pranav    (1000) pranav    (1001)     1897 2023-03-25 08:29:13.000000 print_position-1.0.0/README.md
--rw-r--r--   0 pranav    (1000) pranav    (1001)       84 2023-03-25 06:34:30.000000 print_position-1.0.0/pyproject.toml
--rw-r--r--   0 pranav    (1000) pranav    (1001)      766 2023-03-25 08:30:51.075586 print_position-1.0.0/setup.cfg
-drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-03-25 08:30:51.069586 print_position-1.0.0/src/
-drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-03-25 08:30:51.072586 print_position-1.0.0/src/printPosition/
--rw-r--r--   0 pranav    (1000) pranav    (1001)        0 2023-03-25 06:39:08.000000 print_position-1.0.0/src/printPosition/__init__.py
--rw-r--r--   0 pranav    (1000) pranav    (1001)      318 2023-03-25 08:28:34.000000 print_position-1.0.0/src/printPosition/printPosition.py
-drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-03-25 08:30:51.074586 print_position-1.0.0/src/print_position.egg-info/
--rw-r--r--   0 pranav    (1000) pranav    (1001)     2537 2023-03-25 08:30:51.000000 print_position-1.0.0/src/print_position.egg-info/PKG-INFO
--rw-r--r--   0 pranav    (1000) pranav    (1001)      287 2023-03-25 08:30:51.000000 print_position-1.0.0/src/print_position.egg-info/SOURCES.txt
--rw-r--r--   0 pranav    (1000) pranav    (1001)        1 2023-03-25 08:30:51.000000 print_position-1.0.0/src/print_position.egg-info/dependency_links.txt
--rw-r--r--   0 pranav    (1000) pranav    (1001)       14 2023-03-25 08:30:51.000000 print_position-1.0.0/src/print_position.egg-info/top_level.txt
+drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-04-11 22:36:58.478293 print_position-1.0.1/
+-rw-r--r--   0 pranav    (1000) pranav    (1001)     1068 2023-03-25 04:34:20.000000 print_position-1.0.1/LICENSE
+-rw-r--r--   0 pranav    (1000) pranav    (1001)        0 2023-03-21 18:48:05.000000 print_position-1.0.1/MANIFEST.in
+-rw-r--r--   0 pranav    (1000) pranav    (1001)     2859 2023-04-11 22:36:58.478293 print_position-1.0.1/PKG-INFO
+-rw-r--r--   0 pranav    (1000) pranav    (1001)     2220 2023-04-11 22:30:46.000000 print_position-1.0.1/README.md
+-rw-r--r--   0 pranav    (1000) pranav    (1001)       84 2023-03-25 06:34:30.000000 print_position-1.0.1/pyproject.toml
+-rw-r--r--   0 pranav    (1000) pranav    (1001)      766 2023-04-11 22:36:58.479292 print_position-1.0.1/setup.cfg
+drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-04-11 22:36:58.474293 print_position-1.0.1/src/
+drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-04-11 22:36:58.477293 print_position-1.0.1/src/printPosition/
+-rw-r--r--   0 pranav    (1000) pranav    (1001)        0 2023-03-25 06:39:08.000000 print_position-1.0.1/src/printPosition/__init__.py
+-rw-r--r--   0 pranav    (1000) pranav    (1001)      318 2023-03-25 08:28:34.000000 print_position-1.0.1/src/printPosition/printPosition.py
+drwxr-xr-x   0 pranav    (1000) pranav    (1001)        0 2023-04-11 22:36:58.478293 print_position-1.0.1/src/print_position.egg-info/
+-rw-r--r--   0 pranav    (1000) pranav    (1001)     2859 2023-04-11 22:36:58.000000 print_position-1.0.1/src/print_position.egg-info/PKG-INFO
+-rw-r--r--   0 pranav    (1000) pranav    (1001)      287 2023-04-11 22:36:58.000000 print_position-1.0.1/src/print_position.egg-info/SOURCES.txt
+-rw-r--r--   0 pranav    (1000) pranav    (1001)        1 2023-04-11 22:36:58.000000 print_position-1.0.1/src/print_position.egg-info/dependency_links.txt
+-rw-r--r--   0 pranav    (1000) pranav    (1001)       14 2023-04-11 22:36:58.000000 print_position-1.0.1/src/print_position.egg-info/top_level.txt
```

### Comparing `print_position-1.0.0/LICENSE` & `print_position-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `print_position-1.0.0/PKG-INFO` & `print_position-1.0.1/src/print_position.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,82 @@
 Metadata-Version: 2.1
-Name: print_position
-Version: 1.0.0
+Name: print-position
+Version: 1.0.1
 Summary: A cool python package to add the line number and file name in the print statements.
 Home-page: https://github.com/ps428/PrintPosition-pip
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Project-URL: Bug Tracker, https://github.com/ps428/PrintPosition-pip/issues
 Project-URL: repository, https://github.com/ps428/PrintPosition-pip
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Print Position
+
 A cool python package to add the file name and line number in the print statements. This small tool can be very helpful in debugging big Python projects.
 
+[Here](https://pypi.org/project/print-position/) is the project on pypi.
+
+The current download stas are:
+[![Downloads](https://static.pepy.tech/badge/print-position)](https://pepy.tech/project/print-position)
+[![Downloads](https://static.pepy.tech/badge/print-position/month)](https://pepy.tech/project/print-position)
+
+
 ## Motivation
-To debug the Python code present in multiple files, it becomes difficult to track down the print statement calls in the different files. This small pip package can be highly useful in such cases, one can simply use the custom print statement defined in this package and see the filename and line number of the print call.
+
+To debug the Python code present in multiple files, it becomes difficult to track down the print statement calls in the different files. This small pip package can be highly useful in such cases, one can simply use the custom print statement defined in this package and see the filename and line number of the print calls.
 
 ## How to install?
+
 Just install the package using the command:
+
 ```
 pip3 install print_position
 ```
 
+
 ## Usage
+
 Simply add this import statement on top of your python file to see the file name and line number of each print statement.
+
 ```
-from printPosition.printPosition import printPosition as print 
+from printPosition.printPosition import printPosition as print
 ```
+
 A simple example is (test.py):
+
 ```
-from printPosition.printPosition import printPosition as print 
+from printPosition.printPosition import printPosition as print
 print("Test on line 2 from test.py")
 print("Test on line 3 from test.py")
 
-
-
 print("Test on line 7 from test.py")
 ```
-\
-The output is shown as:
 
+
+The output is shown as:
 ```
 @file_name:line_number
 print_data
 ```
 
+
 I believe this would be very helpful in tracking down errors during debugging, **especially when you are working with someone else's code**.
 
 # Contact me
+
 To raise any **issues/requests** you may refer the issue page [here](https://github.com/ps428/PrintPosition-pip/issues).
-\
+
 You may **mail me** here on my [mail id](mailto:pranav.bhawan@gmail.com).
-\
+
 Feel free to **connect with me** on [my LinkedIn](https://www.linkedin.com/in/ps428).
-\
+
 Please do check out my other projects on my **GitHub** [here](http://www.github.com/ps428).
-\
+
 Also I have made many cool Firefox Add ons. They are pretty useful, you may want to check them out [here](https://addons.mozilla.org/en-US/firefox/user/17277929/).
-\
-\
+
 If you like my work, you may want to [buy me a book here](https://www.buymeacoffee.com/ps428).
+
```

### Comparing `print_position-1.0.0/README.md` & `print_position-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,66 @@
 # Print Position
+
 A cool python package to add the file name and line number in the print statements. This small tool can be very helpful in debugging big Python projects.
 
+[Here](https://pypi.org/project/print-position/) is the project on pypi.
+
+The current download stas are:
+[![Downloads](https://static.pepy.tech/badge/print-position)](https://pepy.tech/project/print-position)
+[![Downloads](https://static.pepy.tech/badge/print-position/month)](https://pepy.tech/project/print-position)
+
+
 ## Motivation
-To debug the Python code present in multiple files, it becomes difficult to track down the print statement calls in the different files. This small pip package can be highly useful in such cases, one can simply use the custom print statement defined in this package and see the filename and line number of the print call.
+
+To debug the Python code present in multiple files, it becomes difficult to track down the print statement calls in the different files. This small pip package can be highly useful in such cases, one can simply use the custom print statement defined in this package and see the filename and line number of the print calls.
 
 ## How to install?
+
 Just install the package using the command:
+
 ```
 pip3 install print_position
 ```
 
+
 ## Usage
+
 Simply add this import statement on top of your python file to see the file name and line number of each print statement.
+
 ```
-from printPosition.printPosition import printPosition as print 
+from printPosition.printPosition import printPosition as print
 ```
+
 A simple example is (test.py):
+
 ```
-from printPosition.printPosition import printPosition as print 
+from printPosition.printPosition import printPosition as print
 print("Test on line 2 from test.py")
 print("Test on line 3 from test.py")
 
-
-
 print("Test on line 7 from test.py")
 ```
-\
-The output is shown as:
 
+
+The output is shown as:
 ```
 @file_name:line_number
 print_data
 ```
 
+
 I believe this would be very helpful in tracking down errors during debugging, **especially when you are working with someone else's code**.
 
 # Contact me
+
 To raise any **issues/requests** you may refer the issue page [here](https://github.com/ps428/PrintPosition-pip/issues).
-\
+
 You may **mail me** here on my [mail id](mailto:pranav.bhawan@gmail.com).
-\
+
 Feel free to **connect with me** on [my LinkedIn](https://www.linkedin.com/in/ps428).
-\
+
 Please do check out my other projects on my **GitHub** [here](http://www.github.com/ps428).
-\
+
 Also I have made many cool Firefox Add ons. They are pretty useful, you may want to check them out [here](https://addons.mozilla.org/en-US/firefox/user/17277929/).
-\
-\
-If you like my work, you may want to [buy me a book here](https://www.buymeacoffee.com/ps428).
+
+If you like my work, you may want to [buy me a book here](https://www.buymeacoffee.com/ps428).
+
```

### Comparing `print_position-1.0.0/setup.cfg` & `print_position-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = print_position
-version = 1.0.0
+version = 1.0.1
 author = Pranav Soni
 author_email = pranav.bhawan@gmail.com
 description = A cool python package to add the line number and file name in the print statements.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/ps428/PrintPosition-pip
 project_urls =
```

### Comparing `print_position-1.0.0/src/print_position.egg-info/PKG-INFO` & `print_position-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,82 @@
 Metadata-Version: 2.1
-Name: print-position
-Version: 1.0.0
+Name: print_position
+Version: 1.0.1
 Summary: A cool python package to add the line number and file name in the print statements.
 Home-page: https://github.com/ps428/PrintPosition-pip
 Author: Pranav Soni
 Author-email: pranav.bhawan@gmail.com
 Project-URL: Bug Tracker, https://github.com/ps428/PrintPosition-pip/issues
 Project-URL: repository, https://github.com/ps428/PrintPosition-pip
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Print Position
+
 A cool python package to add the file name and line number in the print statements. This small tool can be very helpful in debugging big Python projects.
 
+[Here](https://pypi.org/project/print-position/) is the project on pypi.
+
+The current download stas are:
+[![Downloads](https://static.pepy.tech/badge/print-position)](https://pepy.tech/project/print-position)
+[![Downloads](https://static.pepy.tech/badge/print-position/month)](https://pepy.tech/project/print-position)
+
+
 ## Motivation
-To debug the Python code present in multiple files, it becomes difficult to track down the print statement calls in the different files. This small pip package can be highly useful in such cases, one can simply use the custom print statement defined in this package and see the filename and line number of the print call.
+
+To debug the Python code present in multiple files, it becomes difficult to track down the print statement calls in the different files. This small pip package can be highly useful in such cases, one can simply use the custom print statement defined in this package and see the filename and line number of the print calls.
 
 ## How to install?
+
 Just install the package using the command:
+
 ```
 pip3 install print_position
 ```
 
+
 ## Usage
+
 Simply add this import statement on top of your python file to see the file name and line number of each print statement.
+
 ```
-from printPosition.printPosition import printPosition as print 
+from printPosition.printPosition import printPosition as print
 ```
+
 A simple example is (test.py):
+
 ```
-from printPosition.printPosition import printPosition as print 
+from printPosition.printPosition import printPosition as print
 print("Test on line 2 from test.py")
 print("Test on line 3 from test.py")
 
-
-
 print("Test on line 7 from test.py")
 ```
-\
-The output is shown as:
 
+
+The output is shown as:
 ```
 @file_name:line_number
 print_data
 ```
 
+
 I believe this would be very helpful in tracking down errors during debugging, **especially when you are working with someone else's code**.
 
 # Contact me
+
 To raise any **issues/requests** you may refer the issue page [here](https://github.com/ps428/PrintPosition-pip/issues).
-\
+
 You may **mail me** here on my [mail id](mailto:pranav.bhawan@gmail.com).
-\
+
 Feel free to **connect with me** on [my LinkedIn](https://www.linkedin.com/in/ps428).
-\
+
 Please do check out my other projects on my **GitHub** [here](http://www.github.com/ps428).
-\
+
 Also I have made many cool Firefox Add ons. They are pretty useful, you may want to check them out [here](https://addons.mozilla.org/en-US/firefox/user/17277929/).
-\
-\
+
 If you like my work, you may want to [buy me a book here](https://www.buymeacoffee.com/ps428).
+
```

