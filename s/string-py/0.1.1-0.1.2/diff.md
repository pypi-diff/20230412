# Comparing `tmp/string_py-0.1.1.tar.gz` & `tmp/string_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "string_py-0.1.1.tar", last modified: Mon Apr 10 13:47:54 2023, max compression
+gzip compressed data, was "string_py-0.1.2.tar", last modified: Wed Apr 12 17:50:59 2023, max compression
```

## Comparing `string_py-0.1.1.tar` & `string_py-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 13:47:54.095958 string_py-0.1.1/
--rw-rw-rw-   0        0        0     1489 2023-04-10 13:47:54.094957 string_py-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-04-07 15:46:43.000000 string_py-0.1.1/README.md
--rw-rw-rw-   0        0        0      558 2023-04-10 13:47:51.000000 string_py-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 13:47:54.096960 string_py-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-04-10 13:47:51.000000 string_py-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 13:47:54.080945 string_py-0.1.1/string_py/
--rw-rw-rw-   0        0        0      171 2023-04-10 13:47:51.000000 string_py-0.1.1/string_py/__init__.py
--rw-rw-rw-   0        0        0    13185 2023-04-08 13:34:38.000000 string_py-0.1.1/string_py/string_py.py
-drwxrwxrwx   0        0        0        0 2023-04-10 13:47:54.091954 string_py-0.1.1/string_py.egg-info/
--rw-rw-rw-   0        0        0     1489 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 13:47:53.000000 string_py-0.1.1/string_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 17:50:59.390922 string_py-0.1.2/
+-rw-rw-rw-   0        0        0     1767 2023-04-12 17:50:59.388920 string_py-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2023-04-12 16:46:39.000000 string_py-0.1.2/README.md
+-rw-rw-rw-   0        0        0      683 2023-04-12 17:50:39.000000 string_py-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 17:50:59.390922 string_py-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-12 17:47:36.000000 string_py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:50:59.371905 string_py-0.1.2/string_py/
+-rw-rw-rw-   0        0        0      171 2023-04-12 17:45:17.000000 string_py-0.1.2/string_py/__init__.py
+-rw-rw-rw-   0        0        0    12676 2023-04-12 16:29:23.000000 string_py-0.1.2/string_py/string_py.py
+drwxrwxrwx   0        0        0        0 2023-04-12 17:50:59.385918 string_py-0.1.2/string_py.egg-info/
+-rw-rw-rw-   0        0        0     1767 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-12 17:50:59.000000 string_py-0.1.2/string_py.egg-info/top_level.txt
```

### Comparing `string_py-0.1.1/PKG-INFO` & `string_py-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: string_py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils for strings in python
 Home-page: https://github.com/BabyEntchen/string_py
 Author: BabyEntchen
 Author-email: BabyEntchen <baby_entchen@web.de>
 License: MIT
+Project-URL: GitHub, https://github.com/BabyEntchen/string_py
+Project-URL: Documentation, https://string-py.readthedocs.io
 Keywords: python,string,strings,utils,string utils,random,random strings,formatting,formatter
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # string_py
 
 
 [![PyPI](https://img.shields.io/pypi/v/string-py?style=flat-square)](https://pypi.org/project/string-py/)
+[![Documentation](https://readthedocs.org/projects/aioeasypillow/badge/?version=latest&style=flat-square)](https://string-py.readthedocs.io/en/latest/)
 
 A Python package to simplify working with strings
 
 ## Installation
 
 To install the library directly from PyPI you can just run the following command:
 ```shell
```

### Comparing `string_py-0.1.1/README.md` & `string_py-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # string_py
 
 
 [![PyPI](https://img.shields.io/pypi/v/string-py?style=flat-square)](https://pypi.org/project/string-py/)
+[![Documentation](https://readthedocs.org/projects/aioeasypillow/badge/?version=latest&style=flat-square)](https://string-py.readthedocs.io/en/latest/)
 
 A Python package to simplify working with strings
 
 ## Installation
 
 To install the library directly from PyPI you can just run the following command:
 ```shell
```

### Comparing `string_py-0.1.1/pyproject.toml` & `string_py-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -12,8 +12,12 @@
 requires-python = ">=3.10"
 keywords=['python', 'string', 'strings', 'utils', 'string utils', 'random', 'random strings', 'formatting', 'formatter']
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = []
-dynamic = ["version"]
+dynamic = ["version"]
+
+[project.urls]
+GitHub = "https://github.com/BabyEntchen/string_py"
+Documentation = "https://string-py.readthedocs.io"
```

### Comparing `string_py-0.1.1/setup.py` & `string_py-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 from pathlib import Path
 
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Utils for strings in python'
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 URL = "https://github.com/BabyEntchen/string_py"
+PROJECT_URLS = {
+    "Documentation": "https://string-py.readthedocs.io/en/latest/"
+},
 
 # Setting up
 setup(
     name="string_py",
     version=VERSION,
     author="BabyEntchen",
     author_email="<baby_entchen@web.de>",
     url=URL,
+    project_urls=PROJECT_URLS,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'string', 'strings', 'utils', 'string utils', 'random', 'random strings', 'formatting', 'formatter'],
     classifiers=[
```

### Comparing `string_py-0.1.1/string_py/string_py.py` & `string_py-0.1.2/string_py/string_py.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,114 +14,111 @@
     error = "\u001b[31m",
     basic = "\u001b[37m"
 
 
 class Printer:
     """Adds new print methods to work with.
 
-    Parameters
-    ----------
-    :param active:`True`
+    :param active: `True`
         If set to False, no more prints are executed. Exception: force Parameter is set to True.
+
     """
 
     def __init__(self, active: bool = True):
         self.active = active
 
     def time(self, args: str, dt: bool = True, force: bool = False, error: bool = False) -> None:
         """ Timestamp print: Print with the current day and time.
 
-        Parameters
-        ----------
-        :param args:`str`
+        :param args: `str`
             The text to print.
-        :param dt:`True`
+        :param dt: `True`
             Set to `False` to turn off timestamp.
-        :param force:`False`
+        :param force: `False`
             Set to `True` to print always, even if :class:`active` is set to False.
-        :param error:`False`
+        :param error: `False`
             Set to `True` to print always, even if :class:`active` is set to False, gets highlighted with red color.
+
         """
         if self.active or force or error:
             color = Color.error if error else Color.force if force else Color.basic
             if dt:
                 print(f"[{datetime.now().strftime('%d.%m | %H:%M:%S')}] {color}{args}\u001b[0m")
             else:
                 print(f"{color}{args}\u001b[0m")
 
     def slow(self, args: str, speed: float = 0.2, force: bool = False, error: bool = False) -> None:
         """Slow print: Char after char gets printed in a certain speed
 
-        Parameters
-        ----------
-        :param args:`str`
+        :param args: `str`
             The text to print.
-        :param speed:`0.1`
+        :param speed: `0.1`
             The speed in wich the chars will get printed out
-        :param force:`False`
+        :param force: `False`
             Set to `True` to print always, even if :class:`active` is set to False.
-        :param error:`False`
+        :param error: `False`
             Set to `True` to print always, even if :class:`active` is set to False, gets highlighted with red color.
+
         """
         if self.active or force or error:
             color = Color.error if error else Color.force if force else Color.basic
             for char in args:
                 print(color + char, end="")
                 sleep(speed)
 
     async def aio_slow(self, args: str, speed: float = 0.1, force: bool = False, error: bool = False) -> None:
         """Async slow print: Char after char gets printed in a certain speed
 
-        Parameters
-        ----------
-        :param args:`str`
+        :param args: `str`
             The text to print.
-        :param speed:`0.1`
+        :param speed: `0.1`
             The speed in wich the chars will get printed out
-        :param force:`False`
+        :param force: `False`
             Set to `True` to print always, even if :class:`active` is set to False.
-        :param error:`False`
+        :param error: `False`
             Set to `True` to print always, even if :class:`active` is set to False, gets highlighted with red color.
+
         """
         if self.active or force or error:
             color = Color.error if error else Color.force if force else Color.basic
             for char in args:
                 print(color + char, end="")
                 await aio_sleep(speed)
 
 
 class Str(str):
     """Functions to work with strings
 
-    Parameters
-    ----------
     :param values: `str`
         The value you want to work with
+
     """
 
-    def __init__(self, values: str):
-        self.values = values
-        self.chars = [*values]
+    def __init__(self, values: str | int):
+        self.values = str(values)
+        self.chars = [*self.values]
         self.ascii = {
             "ascii_lowercase": string.ascii_lowercase,
             "ascii_uppercase": string.ascii_uppercase,
             "digits": string.digits,
             "punctuation": string.punctuation
         }
 
     def generate(self, length: int = None, min_: int = None, max_: int = None) -> str:
         """Generate a random string out of :class:`values`
+
         :param length:
             Generate with certain length
         :param min_:
             Generate with random length, `max_` required
         :param max_:
             Generate with random length, `min_` required
         :return:
             Returns random string out of :class:`values` with length out of parameters
+
         """
         if (min_ is None and max_ is None) and length is None:
             raise AttributeError("min_ and max_ or length must have a value")
         elif length:
             return "".join(choices(self.chars, k=length))
         elif min_ is not None and max_ is not None:
             if min_ > max_:
@@ -129,68 +126,64 @@
             return "".join(choices(self.chars, k=randint(min_, max_)))
         else:
             raise AttributeError("min_ and max_ or length must have a value")
 
     def remove(self, *chars: str) -> str:
         """Remove chars from string
 
-        Parameters:
-        -----------
         :param chars:
             The chars you want to remove
+
         """
         for x in chars:
             self.values = self.values.replace(x, "")
         return self.values
 
     def split(self, each: int = None, chars: str = None) -> list[str]:
         """An extension of the built-in .split method. Also split on certain index
 
-        Parameters
-        ----------
         :param each:
             The index you want to split at
         :param chars:
             The char or word you want to split at
         :return:
             Returns list with splittet :class:`values`
+
         """
         if not each and not chars:
             raise AttributeError("each or chars must have a value")
         if each:
             return [self.values[i:i + each] for i in range(0, len(self.values), each)]
         else:
             return self.values.split(chars)
 
     def first(self, length: int = 1, remove=False) -> str:
         """A simplification for getting/removing the first chars in a string
 
-        Parameters:
-        -----------
         :param length:
             The amount of chars
         :param remove:
             If set to `True` removes `length` of :class:`values`
+
         """
         if len(self.values) < length:
             raise AttributeError("Length must be smaller then value")
         if remove:
             return self.values[length:]
         else:
             return self.values[:length]
 
     def last(self, length: int = 1, remove=False) -> str:
         """A simplification for getting/removing the last chars in a string
 
-        Parameters:
-        -----------
         :param length:
             The amount of chars
         :param remove:
             If set to `True` removes `length` of :class:`values`
+
         """
         if len(self.values) < length:
             raise AttributeError("Length must be smaller then value")
         if remove:
             return self.values[:-length]
         else:
             return self.values[-length:]
@@ -204,69 +197,65 @@
                 else:
                     gets[num] = char
         return gets
 
     def get_upper(self, chars: bool = True, index: bool = False) -> int | list[str] | dict[int, str]:
         """Get how many upper chars are in :class:`values`
 
-        Parameters
-        ----------
-        :param chars:`True`
+        :param chars: `True`
             If set to True, returns a list of all uppercase chars
             If set to False, returns the number of uppercase chars
-        :param index:`False`
+        :param index: `False`
             If set to True, also returns the Indexes of lower chars (`chars` MUST be `True`)
+
         """
         upper = self.__get("ascii_uppercase", index)
         return upper if chars else len(upper)
 
     def get_lower(self, chars: bool = True, index: bool = False) -> int | list[str] | dict[int, str]:
         """Get how many lower chars are in :class:`values`
 
-        Parameters
-        ----------
-        :param chars:`True`
+        :param chars: `True`
             If set to True, returns a list of all lower chars
             If set to False, returns the number of lower chars
-        :param index:`False`
+        :param index: `False`
             If set to True, also returns the Indexes of lower chars (`chars` MUST be `True`)
+
         """
         if not chars and index:
             raise AttributeError("If index is set to True, chars can't be False")
 
         lower = self.__get("ascii_lowercase", index)
         return lower if chars else len(lower)
 
     def get_numeric(self, chars: bool = True, index: bool = False) -> int | list[str] | dict[int, str]:
         """Get how many numeric chars are in :class:`values`
 
-        Parameters
-        ----------
-        :param chars:`True`
+        :param chars: `True`
             If set to True, returns a list of all numeric chars
             If set to False, returns the number of numeric chars
-        :param index:`False`
+        :param index: `False`
             If set to True, also returns the Indexes of numeric chars (`chars` MUST be `True`)
+
         """
         if not chars and index:
             raise AttributeError("If index is set to True, chars can't be False")
 
         numeric = self.__get("digits", index)
         return numeric if chars else len(numeric)
 
     def get_punctuation(self, chars: bool = True, index: bool = False) -> int | list[str] | dict[int, str]:
         """Get how many punctuation chars are in :class:`values`
 
-        Parameters
-        ----------
-        :param chars:`True`
+        :param chars: `True`
             If set to True, returns a list of all punctuation chars
             If set to False, returns the number of punctuation chars
-        :param index:`False`
+        :param index: `False`
             If set to True, also returns the Indexes of punctuation chars (`chars` MUST be `True`)
+
         """
         if not chars and index:
             raise AttributeError("If index is set to True, chars can't be False")
 
         punctuation = self.__get("punctuation", index)
         return punctuation if chars else len(punctuation)
 
@@ -274,60 +263,61 @@
 class Format:
     """Format texts"""
 
     @staticmethod
     def surround(values: str, char: str = "*") -> str:
         """Surround a text with chars
 
-        Parameters
-        ----------
-        :param values:`str`
+        :param values: `str`
             Text to surround
-        :param char:`*`
+        :param char: `*`
             Char to surround with
         :return:
             Returns a string with the text surrounded with certain chars
+
         """
         return f"{char * (len(values) + 4)}\n{char} {values} {char}\n{char * (len(values) + 4)}"
 
     @staticmethod
     def align(values: dict[str, str]):
         """Align a text
 
-        Parameters
-        ----------
-        :param values:`dict[str, str]`
+        :param values: `dict[str, str]`
             Texts to align {"Left side": "Right side"}
         :return:
             Returns a string with the key aligned left and the value right dependent from the keys
 
         Examples
         --------
-        values = {"Username:": "John", "Register Date:": "01.01.2001"}
-        Username:        John
-        Register Date:   01.01.2001
+
+        .. code-block::
+
+            values = {"Username:": "John", "Register Date:": "01.01.2001"}
+
+            Username:        John
+            Register Date:   01.01.2001
+
         """
         length = max([len(x) for x in list(values.keys())])
         aligned_text = ""
         for key in values:
             aligned_text += key + " " * ((length + 3) - len(key)) + values[key] + "\n"
         return aligned_text
 
     @staticmethod
     def table(values: list[list[str]], border: bool = True) -> str:
         """Create a table
 
-        Parameters
-        ----------
-        :param values:`list[list[str]]`
+        :param values: `list[list[str]]`
             The values to create the table with
-        :param border:`True`
+        :param border: `True`
             Set to `False` to remove the border
         :return:
             Returns the table as string
+
         """
 
         length = [max([len(str(x)) for x in column]) for column in zip(*values)]
         if border:
             table = "\u250C" + "\u2500" * (sum(length) + (3 * len(values) - 1)) + "\u2510\n"
             for index, row in enumerate(values):
                 table += "\u2502"
```

### Comparing `string_py-0.1.1/string_py.egg-info/PKG-INFO` & `string_py-0.1.2/string_py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: string-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: Utils for strings in python
 Home-page: https://github.com/BabyEntchen/string_py
 Author: BabyEntchen
 Author-email: BabyEntchen <baby_entchen@web.de>
 License: MIT
+Project-URL: GitHub, https://github.com/BabyEntchen/string_py
+Project-URL: Documentation, https://string-py.readthedocs.io
 Keywords: python,string,strings,utils,string utils,random,random strings,formatting,formatter
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # string_py
 
 
 [![PyPI](https://img.shields.io/pypi/v/string-py?style=flat-square)](https://pypi.org/project/string-py/)
+[![Documentation](https://readthedocs.org/projects/aioeasypillow/badge/?version=latest&style=flat-square)](https://string-py.readthedocs.io/en/latest/)
 
 A Python package to simplify working with strings
 
 ## Installation
 
 To install the library directly from PyPI you can just run the following command:
 ```shell
```

