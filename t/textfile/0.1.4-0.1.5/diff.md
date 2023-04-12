# Comparing `tmp/textfile-0.1.4.tar.gz` & `tmp/textfile-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textfile-0.1.4.tar", max compression
+gzip compressed data, was "textfile-0.1.5.tar", max compression
```

## Comparing `textfile-0.1.4.tar` & `textfile-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     2008 2021-07-03 02:34:48.987537 textfile-0.1.4/README.rst
--rw-r--r--   0        0        0      841 2021-07-03 01:49:01.218165 textfile-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6559 2021-07-03 02:12:30.633080 textfile-0.1.4/textfile/__init__.py
--rw-r--r--   0        0        0     2727 2021-07-03 02:35:40.801895 textfile-0.1.4/setup.py
--rw-r--r--   0        0        0     2741 2021-07-03 02:35:40.802124 textfile-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2008 2023-04-12 02:41:26.016481 textfile-0.1.5/README.rst
+-rw-r--r--   0        0        0      981 2023-04-12 02:54:55.375118 textfile-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6576 2023-04-12 02:42:59.060848 textfile-0.1.5/textfile/__init__.py
+-rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 textfile-0.1.5/PKG-INFO
```

### Comparing `textfile-0.1.4/README.rst` & `textfile-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `textfile-0.1.4/pyproject.toml` & `textfile-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "textfile"
-version = "0.1.4"
+version = "0.1.5"
 description = "Functions that enables us to write out or read from with text file in shorter syntax."
 authors = ["kenjimaru <kendimaru2@gmail.com>"]
 maintainers = ["kenjimaru <kendimaru2@gmail.com>"]
 readme = 'README.rst'
 repository = 'https://github.com/kendimaru/textfile'
 homepage = 'https://jimaru.site/textfile/'
 keywords = ['text', 'file', 'oneline', 'write', 'read']
@@ -12,19 +12,22 @@
 
 classifiers=[
     'License :: OSI Approved :: MIT License',
 
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^7.3.0"
 Sphinx = "^4.0.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `textfile-0.1.4/textfile/__init__.py` & `textfile-0.1.5/textfile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 import re
 
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 _ENCODING = 'utf-8'
 
 
 def write(file, s, overwrite=True):
     """ Open file for write mode, write string to it, then close.
 
     Write string to file in ``utf-8`` encoding.
@@ -90,17 +90,17 @@
 
     This code will append "str to append" to the end of the content of ``a.txt`` file.
     """
     file = Path(file)
 
     if not file.exists():
         write(file, s)
-
-    with open(file, 'a', encoding=_ENCODING) as appender:
-        appender.write(s)
+    else:
+        with open(file, 'a', encoding=_ENCODING) as appender:
+            appender.write(s)
 
 
 def prepend(file, s):
     raise NotImplemented()
 
 
 def insert(file, s, line):
```

### Comparing `textfile-0.1.4/setup.py` & `textfile-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,119 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: textfile
+Version: 0.1.5
+Summary: Functions that enables us to write out or read from with text file in shorter syntax.
+Home-page: https://jimaru.site/textfile/
+License: MIT
+Keywords: text,file,oneline,write,read
+Author: kenjimaru
+Author-email: kendimaru2@gmail.com
+Maintainer: kenjimaru
+Maintainer-email: kendimaru2@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Project-URL: Repository, https://github.com/kendimaru/textfile
+Description-Content-Type: text/x-rst
 
-packages = \
-['textfile']
 
-package_data = \
-{'': ['*']}
+Wrapper functions of codes of text file operation that are very commonly seen.
+By using ``textfile``, readability of our program will be improve!
 
-setup_kwargs = {
-    'name': 'textfile',
-    'version': '0.1.4',
-    'description': 'Functions that enables us to write out or read from with text file in shorter syntax.',
-    'long_description': '\nWrapper functions of codes of text file operation that are very commonly seen.\nBy using ``textfile``, readability of our program will be improve!\n\nInstall\n-------\n\n.. code-block:: Shell\n\n    > pip install textfile\n\n\nVery basic usage\n----------------\n\nCreate file and write text to it.\n\n.. code-block:: python\n\n    >>> import textfile\n    >>> textfile.write("a.txt", "any string value")\n\nRead text from text file.\n\n.. code-block:: python\n\n    >>> import textfile\n    >>> textfile.read("a.txt")\n    "any string value"\n\nUse cases\n---------\n\nWrite string to text file:\n\n.. code-block:: python\n\n    textfile.write("somefile.txt", "any string value")\n\nRead entire string from text file:\n\n.. code-block::\n\n    textfile.read("somefile.txt")\n\nReplace string in text file:\n\n.. code-block::\n\n    textfile.replace("somefile.txt", "replaced", "replacement")\n\nAppend string to text file:\n\n.. code-block::\n\n    textfile.append("somefile.txt", "text to append")\n\nInsert string to text file:\n\n.. code-block::\n\n    textfile.insert("somefile.txt", "text to insert", line=10)\n\n\nJust a implementation of facade pattern\n---------------------------------------\n\n``textfile`` wraps python algorithms that are very commonly used\nin the purpose of to more simplify basic operations.\n\nThis is just a facade pattern.\n\nThe side effect of simplify the interface of text file operation, gets less flexibility.\nFurther more, it becomes hard to do speed tuning.\n\nBut I think that those are not a matter in almost all situations of our programming.\n\nWe should pay more attention to code readability!\n\nI courage you to use ``textfile`` as much as possible you can.\nIf you do so, the readability of your code will increase, and will suppress many bugs.\n\n\nIs this document written in strange English?\n--------------------------------------------\nKenjimaru, the author of this document, I am Japanese and am not familiar to English.\n\nIf you read this document, and find anything should be fixed, feel free to contact me,\nand I will appreciate.\n\n',
-    'author': 'kenjimaru',
-    'author_email': 'kendimaru2@gmail.com',
-    'maintainer': 'kenjimaru',
-    'maintainer_email': 'kendimaru2@gmail.com',
-    'url': 'https://jimaru.site/textfile/',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
-}
+Install
+-------
+
+.. code-block:: Shell
+
+    > pip install textfile
+
+
+Very basic usage
+----------------
+
+Create file and write text to it.
+
+.. code-block:: python
+
+    >>> import textfile
+    >>> textfile.write("a.txt", "any string value")
+
+Read text from text file.
+
+.. code-block:: python
+
+    >>> import textfile
+    >>> textfile.read("a.txt")
+    "any string value"
+
+Use cases
+---------
+
+Write string to text file:
+
+.. code-block:: python
+
+    textfile.write("somefile.txt", "any string value")
+
+Read entire string from text file:
+
+.. code-block::
+
+    textfile.read("somefile.txt")
+
+Replace string in text file:
+
+.. code-block::
+
+    textfile.replace("somefile.txt", "replaced", "replacement")
+
+Append string to text file:
+
+.. code-block::
+
+    textfile.append("somefile.txt", "text to append")
+
+Insert string to text file:
+
+.. code-block::
+
+    textfile.insert("somefile.txt", "text to insert", line=10)
+
+
+Just a implementation of facade pattern
+---------------------------------------
+
+``textfile`` wraps python algorithms that are very commonly used
+in the purpose of to more simplify basic operations.
+
+This is just a facade pattern.
+
+The side effect of simplify the interface of text file operation, gets less flexibility.
+Further more, it becomes hard to do speed tuning.
+
+But I think that those are not a matter in almost all situations of our programming.
+
+We should pay more attention to code readability!
+
+I courage you to use ``textfile`` as much as possible you can.
+If you do so, the readability of your code will increase, and will suppress many bugs.
+
+
+Is this document written in strange English?
+--------------------------------------------
+Kenjimaru, the author of this document, I am Japanese and am not familiar to English.
+
+If you read this document, and find anything should be fixed, feel free to contact me,
+and I will appreciate.
 
 
-setup(**setup_kwargs)
```

