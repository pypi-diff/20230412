# Comparing `tmp/cycept-0.0.1.tar.gz` & `tmp/cycept-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycept-0.0.1.tar", last modified: Tue Apr 11 01:41:43 2023, max compression
+gzip compressed data, was "cycept-0.0.2.tar", last modified: Wed Apr 12 16:35:50 2023, max compression
```

## Comparing `cycept-0.0.1.tar` & `cycept-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-11 01:41:43.465021 cycept-0.0.1/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.1/LICENSE
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4244 2023-04-11 01:41:43.465021 cycept-0.0.1/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     2909 2023-04-09 17:51:03.000000 cycept-0.0.1/README.md
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-11 01:41:43.465021 cycept-0.0.1/cycept/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       77 2023-04-11 00:49:17.000000 cycept-0.0.1/cycept/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    27084 2023-04-10 22:23:09.000000 cycept-0.0.1/cycept/call.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    21245 2023-04-10 23:38:37.000000 cycept-0.0.1/cycept/core.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-11 01:41:43.465021 cycept-0.0.1/cycept/tests/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      109 2023-04-11 00:52:25.000000 cycept-0.0.1/cycept/tests/__init__.py
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     7356 2023-04-11 00:45:36.000000 cycept-0.0.1/cycept/tests/test_cycept.py
-drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-11 01:41:43.465021 cycept-0.0.1/cycept.egg-info/
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4244 2023-04-11 01:41:43.000000 cycept-0.0.1/cycept.egg-info/PKG-INFO
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      283 2023-04-11 01:41:43.000000 cycept-0.0.1/cycept.egg-info/SOURCES.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-04-11 01:41:43.000000 cycept-0.0.1/cycept.egg-info/dependency_links.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       99 2023-04-11 01:41:43.000000 cycept-0.0.1/cycept.egg-info/requires.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-04-11 01:41:43.000000 cycept-0.0.1/cycept.egg-info/top_level.txt
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1581 2023-04-11 01:36:31.000000 cycept-0.0.1/pyproject.toml
--rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-04-11 01:41:43.465021 cycept-0.0.1/setup.cfg
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.130908 cycept-0.0.2/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1068 2023-04-01 21:39:01.000000 cycept-0.0.2/LICENSE
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     5571 2023-04-12 16:35:50.130908 cycept-0.0.2/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     4236 2023-04-12 12:45:01.000000 cycept-0.0.2/README.md
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.126908 cycept-0.0.2/cycept/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       77 2023-04-11 00:49:17.000000 cycept-0.0.2/cycept/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    26018 2023-04-12 15:49:06.000000 cycept-0.0.2/cycept/call.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     2282 2023-04-12 12:46:27.000000 cycept-0.0.2/cycept/compile.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)    24974 2023-04-12 14:06:13.000000 cycept-0.0.2/cycept/core.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.130908 cycept-0.0.2/cycept/tests/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      618 2023-04-12 15:50:45.000000 cycept-0.0.2/cycept/tests/__init__.py
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     9385 2023-04-12 14:15:20.000000 cycept-0.0.2/cycept/tests/test_cycept.py
+drwxrwxr-x   0 jeppe     (1000) jeppe     (1000)        0 2023-04-12 16:35:50.130908 cycept-0.0.2/cycept.egg-info/
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     5571 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/PKG-INFO
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)      301 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        1 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       99 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/requires.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)        7 2023-04-12 16:35:50.000000 cycept-0.0.2/cycept.egg-info/top_level.txt
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)     1581 2023-04-12 16:17:29.000000 cycept-0.0.2/pyproject.toml
+-rw-rw-r--   0 jeppe     (1000) jeppe     (1000)       38 2023-04-12 16:35:50.130908 cycept-0.0.2/setup.cfg
```

### Comparing `cycept-0.0.1/LICENSE` & `cycept-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cycept-0.0.1/cycept/call.py` & `cycept-0.0.2/cycept/call.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import ast
 import collections
 import contextlib
-import distutils
 import inspect
 import itertools
-import os
 import pathlib
 import re
+import subprocess
 import sys
 import tempfile
-import traceback
+import time
 import typing
 import warnings
 import webbrowser
 
-import Cython.Build.Cythonize
-
 
 # Class for storing and dynamically handling
 # various aspects of the function call to be jitted.
 class FunctionCall:
 
     class Compiled(typing.NamedTuple):
         func: object
         module: object
         source: str
         html: str
 
+    class Time(typing.NamedTuple):
+        compile: float
+        total: float
+
     def __init__(self, func, args, kwargs):
         # Function and call arguments
         self.func = func
         self.args = args
         self.kwargs = kwargs
         # Properties to be lazily constructed
         self._func_name = None
@@ -48,14 +49,16 @@
         self._nonlocals = None
         # Record of inferred types of local variables
         self.locals_types = {}
         # Additional source lines to be included in the Cython extension module
         self.cython_module_lines = []
         # Compilation products
         self.compiled = None
+        # Time measurements
+        self.time = None
 
     # Name of function (with lambda functions renamed)
     @property
     def func_name(self):
         if self._func_name is not None:
             return self._func_name
         self._func_name = self.func.__name__
@@ -350,59 +353,74 @@
                 self.wrapped_any = False
                 self.tmp_any = False
             def wrap(self):
                 self.shape_attrs.clear()
                 self.wrapped_any = False
                 self.tmp_any = False
                 return self.visit(self.call.ast)
-            def wrap_node(self, node):
-                if not isinstance(node, ast.Name):
-                    return node
-                if node.id in self.names:
-                    node = ast.Name(**(vars(node) | {'id': f'{self.wrapper_func}({node.id})'}))
-                return node
-            # Unary and binary operators should always act on NumPy arrays
+            def wrap_node(self, node, kind=0):
+                def is_scalar(node):
+                    if isinstance(node, ast.Name):
+                        tp = self.call.types[node.id]
+                        if tp.startswith('cython.') and '[' not in tp:
+                            return True
+                    elif isinstance(node, ast.Constant):
+                        if isinstance(node.value, int):
+                            return True
+                    return False
+                n_nested_subscripts = 0
+                while isinstance(node, ast.Subscript):
+                    n_nested_subscripts += 1
+                    node_subscript = node
+                    node = node.value
+                if not isinstance(node, ast.Name) or node.id not in self.names:
+                    return
+                if n_nested_subscripts == 1:
+                    # Memoryview/array indexing arr[x].
+                    # If we can prove that x is a scalar
+                    # we use the memoryview as is.
+                    if isinstance(node_subscript.slice, ast.Tuple):
+                        if all(is_scalar(el) for el in node_subscript.slice.elts):
+                            return node
+                    elif is_scalar(node_subscript.slice):
+                        return node
+                # Wrap node
+                self.wrapped_any = True
+                if kind == 0:
+                    node.id = f'{self.wrapper_func}({node.id})'
+                elif kind == 1:
+                    self.tmp_any = True
+                    node.id = f'{self.tmp_name} = {self.wrapper_func}({node.id}); {self.tmp_name}'
             def visit_UnaryOp(self, node):
                 node = self.generic_visit(node)
-                operand = self.wrap_node(node.operand)
-                if operand is not node.operand:
-                    self.wrapped_any = True
-                    node = ast.UnaryOp(**(vars(node) | {'operand': operand}))
+                self.wrap_node(node.operand)
                 return node
             def visit_BinOp(self, node):
                 node = self.generic_visit(node)
-                left = self.wrap_node(node.left)
-                right = self.wrap_node(node.right)
-                if left is not node.left or right is not node.right:
-                    self.wrapped_any = True
-                    node = ast.BinOp(**(vars(node) | {'left': left, 'right': right}))
+                self.wrap_node(node.left)
+                self.wrap_node(node.right)
+                return node
+            def visit_Compare(self, node):
+                node = self.generic_visit(node)
+                self.wrap_node(node.left)
+                for comparator in node.comparators:
+                    self.wrap_node(comparator)
                 return node
-            # Augmented assignment should always be carried out
-            # on NumPy arrays.
             def visit_AugAssign(self, node):
                 node = self.generic_visit(node)
-                target = node.target
-                if not isinstance(target, ast.Name) or target.id not in self.names:
-                    return node
-                self.wrapped_any = True
-                self.tmp_any = True
-                expr = f'{self.tmp_name} = {self.wrapper_func}({target.id}); {self.tmp_name}'
-                target = ast.Name(**(vars(target) | {'id': expr}))
-                node.target = target
+                self.wrap_node(node.target, kind=1)
                 return node
             # Use NumPy arrays as arguments within function calls
             # if array_args is True.
             def visit_Call(self, node):
                 node = self.generic_visit(node)
                 if not self.array_args:
                     return node
-                args = [self.wrap_node(arg) for arg in node.args]
-                if any(arg_wrapped is not arg for arg, arg_wrapped in zip(args, node.args)):
-                    self.wrapped_any = True
-                    node = ast.Call(**(vars(node) | {'args': args}))
+                for arg in node.args:
+                    self.wrap_node(arg)
                 return node
             # NumPy arrays and Cython memory views generally share the same
             # attributes. One exception is 'shape', which for memoryviews
             # is meant to be used as memoryview.shape[i]. If the 'shape'
             # attribute is to be used without immediately indexing into it,
             # use a NumPy array instead of a memoryview.
             def visit_Subscript(self, node):
@@ -416,18 +434,15 @@
                     # Record usage of memoryview.shape[i]
                     self.shape_attrs.add(value)
                 node = self.generic_visit(node)
                 return node
             def visit_Attribute(self, node):
                 node = self.generic_visit(node)
                 if node not in self.shape_attrs:
-                    value = self.wrap_node(node.value)
-                    if value is not node.value:
-                        self.wrapped_any = True
-                        node = ast.Attribute(**(vars(node) | {'value': value}))
+                    self.wrap_node(node.value)
                 return node
         wrapper_func = '_cycept_asarray_'
         tmp_name = '_cycept_tmp_'
         array_wrapper = ArrayWrapper(self, names, array_args, wrapper_func, tmp_name)
         self._source = ast.unparse(array_wrapper.wrap())
         self._ast = None  # invalidate AST (cannot use the above as expressions are used as names)
         if not array_wrapper.wrapped_any:
@@ -529,106 +544,69 @@
         if ClosureVisitor(self).contains_closure():
             return False
         # No violations found
         return True
 
     # Method for handling Cythonization and C compilation
     def compile(self, optimizations, html, silent):
-        # Define context managers for temporarily hack into various
-        # objects during Cythonization and compilation.
-        @contextlib.contextmanager
-        def hack_os_environ():
-            cflags_in_environ = ('CFLAGS' in os.environ)
-            cflags = os.environ.get('CFLAGS', '')
-            os.environ['CFLAGS'] = ' '.join(optimizations)
-            yield
-            if cflags_in_environ:
-                os.environ['CFLAGS'] = cflags
-            else:
-                os.environ.pop('CFLAGS')
-        @contextlib.contextmanager
-        def hack_sys_argv():
-            module_path = get_module_path(dir_name)
-            sys_argv = sys.argv
-            sys.argv = list(
-                itertools.chain(
-                    [''],
-                    ['-i', '-3'],
-                    ['-q'] * silent,
-                    ['-a'] * html,
-                    [str(module_path.with_suffix('.pyx'))],
-                )
-            )
-            yield
-            sys.argv = sys_argv
+        # Cythonize and compile extension module within temporary directory.
+        # The compiled module is then imported (through hacking of sys.path)
+        # before it is removed from disk.
         @contextlib.contextmanager
         def hack_sys_path():
             sys.path.append(dir_name)
             yield
             sys.path.remove(dir_name)
-        @contextlib.contextmanager
-        def hack_distutils_spawn_log(silent):
-            class Printer:
-                def __init__(self, silent):
-                    self.silent = silent
-                def print(self, msg, *args, **kwargs):
-                    if not self.silent:
-                        print(msg)
-                def __getattr__(self, attr):
-                    return self.print
-            printer = Printer(silent)
-            module_names = ['spawn', 'dist']
-            loggers = {}
-            for module_name in module_names:
-                module = getattr(distutils, module_name)
-                if module_name is None:
-                    continue
-                logger = getattr(module, 'log')
-                if logger is None:
-                    continue
-                loggers[module_name] = logger
-                module.log = printer
-            yield
-            for module_name, logger in loggers.items():
-                module = getattr(distutils, module_name)
-                module.log = logger
-        # Cythonize and compile extension module within temporary directory,
-        # with arguments to Cython and the C compiler provided through hacking
-        # of sys.argv and os.environ. The compiled module is then imported
-        # (through hacking of sys.path) before it is removed from disk.
-        # If not compiling silently, we further hack distutils_spawn_log to
-        # print output to stdout.
         module_name = f'_cycept_module_{self.hash}'
-        get_module_path = lambda dir_name: pathlib.Path(dir_name) / module_name
         namespace = {}
         html_annotation = None
+        tempfile_kwargs = {}
+        if sys.version_info[:2] >= (3, 10):
+            tempfile_kwargs |= {'ignore_cleanup_errors': True}
         with (
-            tempfile.TemporaryDirectory() as dir_name,
-            hack_os_environ(),
-            hack_sys_argv(),
+            tempfile.TemporaryDirectory(**tempfile_kwargs) as dir_name,
             hack_sys_path(),
-            hack_distutils_spawn_log(silent),
         ):
-            module_path = get_module_path(dir_name)
             # Write Cython source to file
+            module_path = pathlib.Path(dir_name) / module_name
             module_path.with_suffix('.pyx').write_text(self.source, 'utf-8')
-            # Call Cython.Build.Cythonize.main(), which is equivalent
-            # to calling the cythonize script.
-            ok = True
-            try:
-                Cython.Build.Cythonize.main()
-            except BaseException:
-                ok = False
-                traceback.print_exc()
-            if not ok:
+            # Call Cython. We do so within a subprocess in order
+            # to capture stdout an stderr when running silently.
+            cmd = [
+                sys.executable,
+                '-c',
+                '; '.join([
+                    'import cycept.compile',
+                    'cycept.compile.compile({})'
+                    .format(', '.join([
+                        f'{str(module_path)!r}',
+                        f'{optimizations!r}',
+                        f'{html!r}',
+                    ]))
+                ]),
+            ]
+            run_kwargs = {}
+            if silent:
+                run_kwargs |= {
+                    'stdout': subprocess.PIPE,
+                    'stderr': subprocess.STDOUT,
+                    'text': True,
+                }
+            tic = time.perf_counter()
+            cproc = subprocess.run(cmd, **run_kwargs)
+            toc = time.perf_counter()
+            if cproc.returncode != 0:
                 if sys.flags.interactive:
                     # Do not remove the compilation files immediately when
                     # running interactively, allowing the user to inspect them.
                     input(f'Press Enter to clean up temporary build directory {dir_name} ')
-                raise OSError('Cythonization failed')
+                msg = ['Cythonization failed.']
+                if silent:
+                    msg += ['Subprocess output:', cproc.stdout]
+                raise OSError('\n'.join(msg))
             # Import function from compiled module into temporary namespace
             exec(f'import {module_name}', namespace)
             # Read in C source and annotated HTML
             source_c = module_path.with_suffix('.c').read_text('utf-8')
             path_html = module_path.with_suffix('.html')
             if path_html.is_file():
                 html_annotation = path_html.read_text('utf-8')
@@ -645,14 +623,16 @@
         # Store compilation products
         self.compiled = self.Compiled(
             func_compiled,
             module_compiled,
             source_c,
             html_annotation,
         )
+        # Return compilation time (in seconds)
+        return toc - tic
 
     # Method for viewing the annotated HTML
     def __call__(self, dir_name=None):
         if self.compiled is None or self.compiled.html is None:
             print(f'No Cython HTML annotation generated for {self.func_name}()')
             return
         if dir_name is None:
```

### Comparing `cycept-0.0.1/cycept/core.py` & `cycept-0.0.2/cycept/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import ast
 import collections
 import contextlib
 import dataclasses
 import functools
+import importlib
+import importlib.metadata
 import pathlib
 import re
 import sys
+import time
 import warnings
 
 import cython
 import numpy as np
 
 from .call import FunctionCall
 
 
-# Read current version from pyproject.toml
+# Get current version
 def get_version():
     version = '?.?.?'
-    # Get version from meta data on installed package
-    import importlib
-    try:
-        return importlib.metadata.version('cycept')
-    except importlib.metadata.PackageNotFoundError:
-        pass
-    # Look for pyproject.toml
+    # Get version from pyproject.toml
     def get_tomllib():
-        tomllib = None
-        try:
-            import tomllib
-        except ModuleNotFoundError:
+        toml_packages = ['tomllib', 'tomli', 'toml']
+        for name in toml_packages:
             try:
-                import toml as tomllib
+                return importlib.import_module(name)
             except ModuleNotFoundError:
-                warnings.warn(
-                    (
-                        f'For using Cycept with Python < 3.11 please install '
-                        f'the toml Python package:\n'
-                        f'    {sys.executable} -m pip install toml\n'
-                    ),
-                    RuntimeWarning,
-                )
-        return tomllib
+                pass
+        warnings.warn(
+            (
+                f'For using Cycept with Python < 3.11 please install '
+                f'the tomli Python package:\n'
+                f'    {sys.executable} -m pip install tomli\n'
+            ),
+            RuntimeWarning,
+        )
     path = pathlib.Path(__file__).resolve().parent
     while True:
-        path_pyproject = path / 'pyproject.toml'
-        if path_pyproject.is_file():
-            tomllib = get_tomllib()
-            if tomllib is not None:
+        if (path_pyproject := path / 'pyproject.toml').is_file():
+            if (tomllib := get_tomllib()) is not None:
                 info = tomllib.loads(path_pyproject.read_text('utf-8'))
-                version = info['project']['version']
+                if info['project']['name'] == 'cycept':
+                    return info['project']['version']
+                break
             break
         if path.parent == path:
             break
         path = path.parent
+    # Get version from meta data on installed package
+    try:
+        return importlib.metadata.version('cycept')
+    except ModuleNotFoundError:
+        pass
     return version
 __version__ = get_version()
 
 
 # Main JIT decorator function
 def jit(func=None, **options):
     """This decorator compiles a Python function to machine code using Cython
@@ -74,15 +74,15 @@
         options:
             compile: bool
                 Set to False to disable just-in-time compilation.
                 Default is True.
 
 
             silent: bool
-                Set to False to display compilation commands.
+                Set to False to display compilation messages.
                 Default value is True.
 
 
             html: bool
                 Set to True to produce HTML annotations of the compiled code.
                 View the HTMl using func.__cycept__().
                 Default value is False.
@@ -184,14 +184,45 @@
                 at all, making use of the defaults. Using
 
                     @jit(optimizations=False)
 
                 replaces all of the default optimizations with -O0.
 
 
+            integral: type | str
+                By default, Python ints are replaced with cython.Py_ssize_t.
+                These are not fully equivalent: while cython.Py_ssize_t is
+                typically 64-bit, Python ints are unbounded. If you prefer
+                to e.g. use 32-bit ints, set this option to e.g. np.int32:
+
+                    @jit(integral=np.int32)
+
+                To use the native int of the current machine, you can specify
+                any of cython.int, np.intc, 'int'. To use the (slow) Python
+                ints, specify integral=object.
+
+
+            floating: type | str
+                By default, Python floats are replaced with cython.double.
+                These are fully identical 64-bit floating-point numbers.
+                If you prefer to e.g. use 64-bit floats, set this option
+                to e.g. np.float32:
+
+                    @jit(floating=np.float32)
+
+
+            floating_complex: type | str
+                By default, Python complex floats are replaced with
+                cython.complex. These should be fully identical 128-bit (2×64)
+                complex floating-point numbers. If you prefer to e.g. use
+                64-bit (2×32) complex floats, set this option to e.g. np.complex64:
+
+                    @jit(floating_complex=np.complex64)
+
+
     Annotations
     -----------
         Types of variables are automatically inferred at runtime.
         Type annotations can be specified to manually set the types
         of specific variables, e.g.
 
             @jit
@@ -250,41 +281,64 @@
     silent=True,
     html=False,
     checks=False,
     clike=False,
     array_args=True,
     directives=None,
     optimizations=None,
+    integral=None,
+    floating=None,
+    floating_complex=None,
 ):
     if not compile:
         return func, None
     # Fetch function call object, implementing dynamic evaluation
     # of various attributes.
     call = fetch_function_call(func, args, kwargs)
     # If the call has already been transpiled and cached,
     # return immediately.
     if call.compiled is not None:
         return call.compiled.func, None
     # The function call object was not found in cache
+    tic = time.perf_counter()
+    # Populate global mappings of Cython types in accordance
+    # with user integral and floating specifications.
+    cython_types_user, cython_types_reverse_user = get_cython_types(
+        integral,
+        floating,
+        floating_complex,
+    )
+    cython_types.clear()
+    cython_types.update(cython_types_user)
+    cython_types_reverse.clear()
+    cython_types_reverse.update(cython_types_reverse_user)
+    # Print jitting message if not running silently
     if not silent:
         print(f'Jitting {call!r}')
     # Record types of passed arguments and locals. As a side effect,
     # the function is called and the return value obtained.
     record_types(call)
     result = record_locals(call)
     # Make sure that NumPy arrays are treated as such when necessary
     call.protect_arrays(array_args)
     # Convert Python function source into Cython module source
     directives = get_directives(directives, checks, clike)
     call.to_cython(directives)
     # Cythonize and compile
     optimizations = get_optimizations(optimizations)
-    call.compile(optimizations, html, silent)
+    time_compile = call.compile(optimizations, html, silent)
     # Store the function call object on the wrapper function
     wrapper.__cycept__[call.arguments_types] = call
+    # End and store time measurements
+    toc = time.perf_counter()
+    time_total = toc - tic
+    call.time = call.Time(time_compile, time_total)
+    if not silent:
+        print(f'Compilation time:   {call.time.compile:#.4g} s')
+        print(f'Total jitting time: {call.time.total:#.4g} s')
     # Return the result only
     return None, result
 
 
 # Function used to fetch FunctionCall instance from the global
 # cache or instantiating a new one if not found in the cache.
 def fetch_function_call(func, args=None, kwargs=None):
@@ -563,43 +617,31 @@
         return convert_to_cython_type(default, None)
     tp_str = getattr(tp, '__name__', getattr(tp, 'name', None))
     if tp_str is not None:
         return tp_str
     return str(tp)
 
 
-# Mapping of Python/NumPy types to str representations
-# of corresponding Cython types.
-cython_default_integral = 'cython.Py_ssize_t'  # typically 64-bit
-cython_types = collections.defaultdict(
-    lambda: 'object',
-    {
+# Function creating a mapping of Python/NumPy types
+# to str representations of corresponding Cython types.
+@functools.cache
+def get_cython_types(integral=None, floating=None, floating_complex=None):
+    if integral is None:
+        integral = cython_default_integral
+    if floating is None:
+        floating = cython_default_floating
+    if floating_complex is None:
+        floating_complex = cython_default_floating_complex
+    # Mapping of Cython types
+    cython_types = {
         # Python scalars
         bool: 'cython.bint',
-        int: cython_default_integral,
-        float: 'cython.double',
-        complex: 'cython.complex',
-        # NumPy signed integral scalars
-        np.int8: 'cython.schar',
-        np.int16: 'cython.short',
-        np.int32: 'cython.int',
-        np.int64: 'cython.longlong',
-        # NumPy unsigned integral scalars
-        np.uint8: 'cython.uchar',
-        np.uint16: 'cython.ushort',
-        np.uint32: 'cython.uint',
-        np.uint64: 'cython.ulonglong',
-        # NumPy floating scalars
-        np.float32: 'cython.float',
-        np.float64: 'cython.double',
-        np.longdouble: 'cython.longdouble',  # platform dependent
-        # NumPy complex floating scalars
-        np.complex64: 'cython.floatcomplex',  # Cython type may not be available at compile time
-        np.complex128: 'cython.doublecomplex',
-        np.complex256: 'cython.longdoublecomplex',  # Cython type may not be available at compile time; np.longdoublecomplex not defined
+        int: integral,
+        float: floating,
+        complex: floating_complex,
         # Python containers
         **{
             tp: tp.__name__
             for tp in [
                 bytearray,
                 bytes,
                 dict,
@@ -607,21 +649,62 @@
                 list,
                 object,
                 set,
                 str,
                 tuple,
             ]
         },
-    },
-)
-# Also create reverse mapping
-cython_types_reverse = collections.defaultdict(
-    lambda: object,
-    {name: tp for tp, name in cython_types.items()},
-)
-# Now add the Cython types themselves
-cython_types |= {
-    getattr(cython, name.removeprefix('cython.')): name
-    for tp, name in cython_types.items()
-    if name.startswith('cython.')
-}
+    }
+    # Add NumPy scalar types. Some NumPy types may not be
+    # available at runtime and some Cython types may not be
+    # available at compile time.
+    for name, val in {
+        # NumPy Boolean
+        'bool_': 'cython.uchar', # uchar is preferable to bint as otherwise Cython throws "ValueError: Buffer dtype mismatch, expected 'bint' but got 'bool'"
+        # NumPy signed integral scalars
+        'int8': 'cython.schar',
+        'int16': 'cython.short',
+        'int32': 'cython.int',
+        'int64': 'cython.longlong',
+        # NumPy unsigned integral scalars
+        'uint8': 'cython.uchar',
+        'uint16': 'cython.ushort',
+        'uint32': 'cython.uint',
+        'uint64': 'cython.ulonglong',
+        # NumPy floating scalars
+        'float32': 'cython.float',
+        'float64': 'cython.double',
+        'longdouble': 'cython.longdouble',  # platform dependent
+        # NumPy complex floating scalars
+        'complex64': 'cython.floatcomplex',
+        'complex128': 'cython.doublecomplex',
+        'complex256': 'cython.longdoublecomplex',  # numpy.longdoublecomplex not defined
+    }.items():
+        if (attr := getattr(np, name, None)) is not None:
+            cython_types[attr] = val
+    # Also create reverse mapping
+    cython_types_reverse = {
+        name: tp for tp, name in cython_types.items()
+    }
+    # Now add the Cython types themselves
+    cython_types |= {
+        getattr(cython, name.removeprefix('cython.')): name
+        for tp, name in cython_types.items()
+        if isinstance(name, str) and name.startswith('cython.')
+    }
+    # Ensure that the provided integral and floating types
+    # are resolved to str representation of Cython types.
+    cython_types[int] = cython_types.get(integral, integral)
+    cython_types[float] = cython_types.get(floating, floating)
+    cython_types[complex] = cython_types.get(floating_complex, floating_complex)
+    cython_types_reverse[cython_types[int]] = int
+    cython_types_reverse[cython_types[float]] = float
+    cython_types_reverse[cython_types[complex]] = complex
+    return cython_types, cython_types_reverse
+# Global mappings for the Cython types
+cython_types = collections.defaultdict(lambda: 'object')
+cython_types_reverse = collections.defaultdict(lambda: object)
+# Default integral and floating type to use
+cython_default_integral = 'cython.Py_ssize_t'       # typically 64-bit
+cython_default_floating = 'cython.double'           # 64-bit
+cython_default_floating_complex = 'cython.complex'  # should always be 128-bit
```

### Comparing `cycept-0.0.1/cycept/tests/test_cycept.py` & `cycept-0.0.2/cycept/tests/test_cycept.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from cycept import jit
+import re
+import sys
 
 import cython
 import numpy as np
+import pytest
+
+from cycept import jit, NdarrayTypeInfo
 
 
 def test_pass():
     @jit
     def f():
         pass
     assert f() is None
@@ -49,50 +53,66 @@
 
 def test_type_cython():
     @jit
     def f(a):
         b = [a]
         return 2*b.pop()
     f(True)
-    types = next(iter(f.__cycept__.values())).types
-    assert types == {'a': 'cython.bint', 'b': 'list', 'return': 'cython.Py_ssize_t'}
+    call = next(iter(f.__cycept__.values()))
+    assert call.types == {
+        'a': 'cython.bint',
+        'b': 'list',
+        'return': 'cython.Py_ssize_t',
+    }
 
 def test_type_array():
     @jit
     def f(a):
         b = a**0.5
         return b + 1j
-    f(np.arange(3))
-    call = next(iter(f.__cycept__.values()))
+    f(np.arange(3, dtype=np.int64))
+    key = next(iter(f.__cycept__))
+    assert isinstance(key[0], NdarrayTypeInfo)
+    call = f.__cycept__[key]
     assert call.locals_types['a'].dtype is np.int64
     assert call.locals_types['b'].dtype is np.float64
     assert call.locals_types['return'].dtype is np.complex128
-    assert call.types == {'a': 'cython.longlong[::1]', 'b': 'cython.double[::1]', 'return': 'cython.doublecomplex[::1]'}
+    assert call.types == {
+        'a': 'cython.longlong[::1]',
+        'b': 'cython.double[::1]',
+        'return': 'cython.doublecomplex[::1]',
+    }
 
 def test_type_annotation():
     @jit
     def f(a: int) -> float:
         b : object = [a]
         return 2*b.pop()
     f(True)
-    types = next(iter(f.__cycept__.values())).types
-    assert types == {'a': 'cython.Py_ssize_t', 'b': 'object', 'return': 'cython.double'}
+    call = next(iter(f.__cycept__.values()))
+    assert call.types == {
+        'a': 'cython.Py_ssize_t',
+        'b': 'object',
+        'return': 'cython.double',
+    }
 
 def test_manual():
     def f(a):
         return 2*a
     g = jit(f)
     assert f(1) == g(1)
-    assert next(iter(g.__cycept__.values())).types['return'] == 'cython.Py_ssize_t'
+    call = next(iter(g.__cycept__.values()))
+    assert call.types['return'] == 'cython.Py_ssize_t'
 
 def test_lambda():
     def test(f):
         g = jit(f)
         assert f(1) == g(1)
-        assert next(iter(g.__cycept__.values())).types['return'] == 'cython.Py_ssize_t'
+        call = next(iter(g.__cycept__.values()))
+        assert call.types['return'] == 'cython.Py_ssize_t'
     f = lambda a: 2*a
     test(f)
     test(lambda a: 2*a)
 
 def test_closure():
     @jit
     def f(a):
@@ -146,41 +166,45 @@
     assert g(b=5, a=1) == 11
 
 def test_arg_starargs():
     @jit
     def f(a, *args):
         return a + sum(args)
     f(1)
-    assert next(iter(f.__cycept__.values())).locals_types['args'] is tuple
+    call = next(iter(f.__cycept__.values()))
+    assert call.locals_types['args'] is tuple
     assert f(1) == 1
     assert f(a=0) == 0
     assert f(1, 2, 3, 4) == 10
     @jit
     def g(*args, a=1):
         return a + sum(args)
     g()
-    assert next(iter(g.__cycept__.values())).locals_types['args'] is tuple
+    call = next(iter(g.__cycept__.values()))
+    assert call.locals_types['args'] is tuple
     assert g() == 1
     assert g(2, 3, 4) == 10
     assert g(2, 3, 4, a=0) == 9
 
 def test_arg_starstarkwargs():
     @jit
     def f(a, **kwargs):
         return a + kwargs.get('b', 0) + kwargs.get('c', 0)
     f(1)
-    assert next(iter(f.__cycept__.values())).locals_types['kwargs'] is dict
+    call = next(iter(f.__cycept__.values()))
+    assert call.locals_types['kwargs'] is dict
     assert f(1) == 1
     assert f(a=0) == 0
     assert f(1, b=2, c=3) == 6
     @jit
     def g(a=1, **kwargs):
         return a + kwargs.get('b', 0) + kwargs.get('c', 0)
     g()
-    assert next(iter(g.__cycept__.values())).locals_types['kwargs'] is dict
+    call = next(iter(g.__cycept__.values()))
+    assert call.locals_types['kwargs'] is dict
     assert g() == 1
     assert g(b=2, c=3) == 6
     assert g(b=2, c=3, a=0) == 5
 
 def test_option_none():
     @jit()
     def f():
@@ -194,24 +218,25 @@
             return cython.compiled
         f()  # to compile
         assert f() is compile
 
 def test_option_silent(capfd):
     for silent in (False, True):
         @jit(silent=silent)
-        def f():
+        def f(a):
             pass
-        f()
+        f(np.linspace(0, 1, 3, dtype=np.float64))
         out, err = capfd.readouterr()
         if silent:
             assert out == ''
         else:
-            assert 'Jitting f()' in out  # Cycept
-            assert 'Compiling' in out    # Cython
-            assert '-O3' in out          # C compiler
+            assert 'Jitting f(a: double[::1])' in out       # Cycept
+            assert 'Compilation time' in out                # Cycept
+            assert 'Compiling' in out                       # Cython
+            assert re.search(r'cycept_module_\d+\.o', out)  # C compiler
 
 def test_option_html():
     for html in (False, True):
         @jit(html=html)
         def f():
             a = 1234
             pass
@@ -269,16 +294,87 @@
         @jit(directives={'cdivision': cdivision})
         def f(a, b):
             return a//b
         for _ in range(2):  # twice in order to use compiled function
             result = f(-1, 2)
         assert result == (0 if cdivision else -1)
 
+@pytest.mark.skipif(
+    re.search(r'(?<!dar)win', sys.platform.lower()),
+    reason=(
+        'CFLAGS optimizations does not work with MSVC, '
+        'which is probably the compiler used on Windows'
+    ),
+)
 def test_option_optimizations(capfd):
     for level, optimizations in enumerate([False, 1, '-O2', {'-O3': True}]):
         @jit(optimizations=optimizations, silent=False)
         def f():
             pass
         f()
         out, err = capfd.readouterr()
         assert f'-O{level}' in out
 
+def test_array_mutability():
+    @jit
+    def f(a):
+        a[0] += 1
+    a = np.zeros(3, dtype=int)
+    n = 3
+    for _ in range(n):
+        f(a)
+    assert a[0] == n
+
+def test_array_operations():
+    @jit
+    def f(a):
+        b = a + 1
+        return b
+    a = np.zeros(3, dtype=int)
+    for _ in range(2):
+        b = f(a)
+        assert b.sum() == 3
+
+def test_array_augmentation():
+    @jit
+    def f(a):
+        a += 1
+    a = np.zeros(3, dtype=int)
+    for _ in range(2):
+        f(a)
+    assert a.sum() == 6
+
+def test_array_slice_augmentation():
+    @jit
+    def f(a):
+        a[1:] += 1
+    a = np.zeros(3, dtype=int)
+    for _ in range(2):
+        f(a)
+    assert a.sum() == 4
+
+def test_array_element_augmentation():
+    @jit
+    def f(a, b):
+        a[b] += 1
+    a = np.zeros(3, dtype=int)
+    b = np.zeros(3, dtype=bool)
+    b[2] = True
+    for _ in range(2):
+        f(a, 1)  # should use memoryview for a
+        f(a, b)  # should use array for a
+    assert (a == [0, 2, 2]).all()
+    sourcelengths = [
+        len(call.compiled.source)
+        for call in f.__cycept__.values()
+    ]
+    assert sourcelengths[0] < sourcelengths[1]
+
+def test_array_comparison():
+    @jit
+    def f(a):
+        b = a < 2
+        return a >= b[0]
+    a = np.arange(3, dtype=int)
+    for _ in range(2):
+        assert f(a).sum() == 2
+
```

### Comparing `cycept-0.0.1/pyproject.toml` & `cycept-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cycept"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Jeppe Dakin", email="jeppe_dakin@hotmail.com"},
 ]
 description = "Effortless just-in-time compilation of Python functions, powered by Cython"
 readme = "README.md"
 requires-python = ">= 3.9"
 dependencies = [
     "cython >= 3.0.0b1",
     "numpy >= 1.20",
     "dill >= 0.3",
-    "toml >= 0.10.0; python_version < '3.11'",
+    "tomli >= 1.1.0; python_version < '3.11'",
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

