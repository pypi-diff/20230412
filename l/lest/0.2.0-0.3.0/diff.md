# Comparing `tmp/lest-0.2.0.tar.gz` & `tmp/lest-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lest-0.2.0.tar", last modified: Sat Apr  8 07:43:27 2023, max compression
+gzip compressed data, was "lest-0.3.0.tar", last modified: Wed Apr 12 07:24:13 2023, max compression
```

## Comparing `lest-0.2.0.tar` & `lest-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.602996 lest-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1334 2023-04-08 07:43:27.601003 lest-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      831 2023-04-08 07:35:21.000000 lest-0.2.0/README.md
--rw-rw-rw-   0        0        0      493 2023-04-08 07:42:33.000000 lest-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 07:43:27.602996 lest-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.579984 lest-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.591990 lest-0.2.0/src/lest/
--rw-rw-rw-   0        0        0      223 2023-04-04 11:03:08.000000 lest-0.2.0/src/lest/__init__.py
--rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.2.0/src/lest/registerer.py
--rw-rw-rw-   0        0        0     1997 2023-04-08 07:38:46.000000 lest-0.2.0/src/lest/runner.py
-drwxrwxrwx   0        0        0        0 2023-04-08 07:43:27.598991 lest-0.2.0/src/lest.egg-info/
--rw-rw-rw-   0        0        0     1334 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-08 07:43:27.000000 lest-0.2.0/src/lest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.557674 lest-0.3.0/
+-rw-rw-rw-   0        0        0     1084 2023-04-04 11:05:14.000000 lest-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1143 2023-04-12 07:24:13.556673 lest-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2023-04-12 06:56:59.000000 lest-0.3.0/README.md
+-rw-rw-rw-   0        0        0      493 2023-04-12 07:20:31.000000 lest-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:24:13.557674 lest-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.521158 lest-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.548670 lest-0.3.0/src/lest/
+-rw-rw-rw-   0        0        0      371 2023-04-12 06:57:45.000000 lest-0.3.0/src/lest/__init__.py
+-rw-rw-rw-   0        0        0      911 2023-04-12 07:13:46.000000 lest-0.3.0/src/lest/assertions.py
+-rw-rw-rw-   0        0        0      312 2023-04-03 11:04:41.000000 lest-0.3.0/src/lest/registerer.py
+-rw-rw-rw-   0        0        0     2128 2023-04-11 08:52:17.000000 lest-0.3.0/src/lest/runner.py
+-rw-rw-rw-   0        0        0      184 2023-04-11 08:52:17.000000 lest-0.3.0/src/lest/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:13.554673 lest-0.3.0/src/lest.egg-info/
+-rw-rw-rw-   0        0        0     1143 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-12 07:24:13.000000 lest-0.3.0/src/lest.egg-info/top_level.txt
```

### Comparing `lest-0.2.0/LICENSE` & `lest-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lest-0.2.0/README.md` & `lest-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,40 +13,37 @@
 ## Usage
 
 ### Example:
 
 Code:
 
 ```python
-from lest import register, run
+from lest import register, run, setup
+from lest.assertions import assert_eq
+
+
+@setup
+def my_setup():
+    print('Setup ran!')
 
 
 @register
 def test_adding_two_and_two():
-    assert 2 + 2 == 4
+    assert_eq(2 + 2, 4)
 
 
 @register
 def some_error_test():
-    assert 2 + 2 == 5
+    assert_eq(2 + 2, 5)  # AssertionError
+
+
+@register
+def some_more_error():
+    assert_eq(a + 2, 4)  # NameError
 
 
 run()
 ```
 
-Output: (To visible the highlighting, run on the command line)
+Output (to visible the highlighting, it's a print-screen):
 
-```text
-Running [test_adding_two_and_two]... OK
-Running [some_error_test]... FAILED:
-Traceback (most recent call last):
-  File "E:\vladimir\Python\lest\src\lest\runner.py", line 23, in run
-    func()
-  File "E:\vladimir\Python\lest\src\test.py", line 11, in some_error_test
-    assert 2 + 2 == 5
-AssertionError
-
-Run 2 tests:
-   + Successful: 1
-   + Failed: 1
-   + Time elapsed: 0.000
-```
+![](result.png)
```

### Comparing `lest-0.2.0/src/lest/runner.py` & `lest-0.3.0/src/lest/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 
         # information
         self.successful = 0
         self.failed = 0
         self.elapsed = 0
         self.errors = 0
 
-    def run(self, funcs: list[Callable]) -> None:
+    def run(self, funcs: list[Callable], setup: Callable | None = None) -> None:
+        if setup is None:
+            setup = lambda: ...  # Empty function.
         for func in funcs:
             print(f'Running [{func.__name__}]... ', end='')
             start = perf_counter()
+            setup()
             try:
                 func()
             except AssertionError:
                 self.elapsed += perf_counter() - start
                 self.console.print('[red]FAILED:[/red]')
                 self.console.print(f'[red]{traceback.format_exc()}[/red]')
                 self.failed += 1
```

