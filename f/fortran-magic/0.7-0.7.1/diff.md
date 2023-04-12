# Comparing `tmp/fortran-magic-0.7.tar.gz` & `tmp/fortran-magic-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fortran-magic-0.7.tar", last modified: Sun Mar 13 15:37:02 2016, max compression
+gzip compressed data, was "fortran-magic-0.7.1.tar", last modified: Wed Apr 12 15:35:28 2023, max compression
```

## Comparing `fortran-magic-0.7.tar` & `fortran-magic-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2016-03-13 15:37:02.000000 fortran-magic-0.7/
--rw-rw-r--   0 tin       (1000) tin       (1000)     1827 2016-03-13 15:23:32.000000 fortran-magic-0.7/CHANGES.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)    13712 2016-03-13 15:19:25.000000 fortran-magic-0.7/fortranmagic.py
--rw-rw-r--   0 tin       (1000) tin       (1000)     5475 2016-03-13 15:37:02.000000 fortran-magic-0.7/PKG-INFO
-drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2016-03-13 15:37:02.000000 fortran-magic-0.7/fortran_magic.egg-info/
--rw-rw-r--   0 tin       (1000) tin       (1000)     5475 2016-03-13 15:37:02.000000 fortran-magic-0.7/fortran_magic.egg-info/PKG-INFO
--rw-rw-r--   0 tin       (1000) tin       (1000)       13 2016-03-13 15:37:02.000000 fortran-magic-0.7/fortran_magic.egg-info/top_level.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)        1 2016-03-13 15:37:02.000000 fortran-magic-0.7/fortran_magic.egg-info/dependency_links.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       14 2016-03-13 15:37:02.000000 fortran-magic-0.7/fortran_magic.egg-info/requires.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)      243 2016-03-13 15:37:02.000000 fortran-magic-0.7/fortran_magic.egg-info/SOURCES.txt
--rw-rw-r--   0 tin       (1000) tin       (1000)       59 2016-03-13 15:37:02.000000 fortran-magic-0.7/setup.cfg
--rw-rw-r--   0 tin       (1000) tin       (1000)     1121 2016-03-13 15:36:07.000000 fortran-magic-0.7/setup.py
--rw-rw-r--   0 tin       (1000) tin       (1000)     1674 2015-12-02 12:22:08.000000 fortran-magic-0.7/README.rst
--rw-rw-r--   0 tin       (1000) tin       (1000)       38 2015-12-02 12:00:26.000000 fortran-magic-0.7/MANIFEST.in
+drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/
+-rw-rw-r--   0 tin       (1000) tin       (1000)     2479 2023-04-12 15:34:29.000000 fortran-magic-0.7.1/CHANGES.rst
+-rw-rw-r--   0 tin       (1000) tin       (1000)     1491 2023-04-12 15:25:00.000000 fortran-magic-0.7.1/LICENSE
+-rw-rw-r--   0 tin       (1000) tin       (1000)       38 2023-04-12 15:25:00.000000 fortran-magic-0.7.1/MANIFEST.in
+-rw-rw-r--   0 tin       (1000) tin       (1000)     5017 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/PKG-INFO
+-rw-rw-r--   0 tin       (1000) tin       (1000)     1674 2023-04-12 15:25:00.000000 fortran-magic-0.7.1/README.rst
+drwxrwxr-x   0 tin       (1000) tin       (1000)        0 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/fortran_magic.egg-info/
+-rw-rw-r--   0 tin       (1000) tin       (1000)     5017 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/PKG-INFO
+-rw-rw-r--   0 tin       (1000) tin       (1000)      251 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/SOURCES.txt
+-rw-rw-r--   0 tin       (1000) tin       (1000)        1 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/dependency_links.txt
+-rw-rw-r--   0 tin       (1000) tin       (1000)       14 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/requires.txt
+-rw-rw-r--   0 tin       (1000) tin       (1000)       13 2023-04-12 15:35:28.000000 fortran-magic-0.7.1/fortran_magic.egg-info/top_level.txt
+-rw-rw-r--   0 tin       (1000) tin       (1000)    13133 2023-04-12 15:26:50.000000 fortran-magic-0.7.1/fortranmagic.py
+-rw-rw-r--   0 tin       (1000) tin       (1000)       38 2023-04-12 15:35:28.216755 fortran-magic-0.7.1/setup.cfg
+-rw-rw-r--   0 tin       (1000) tin       (1000)     1171 2023-04-12 15:35:23.000000 fortran-magic-0.7.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fortran-magic-0.7/CHANGES.rst` & `fortran-magic-0.7.1/CHANGES.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 
 Changelog
 =========
 
-0.7 / 2016-03-13
+0.7.1 / 2022-04-12
+------------------
+
+- Synchronize version number in fortranmagic.py & setup.py (TBD, TBD, https://github.com/Serge3leo)
+
+- Patch fortran source in compiled object. (029d890, 2020-08-01, https://github.com/mgaitan)
+
+- Fix deprecation warning (3667bc1, 2017-08-18, https://github.com/guihigashi)
+  [IPython.utils.path removed from IPython 8.x] 
+
+- Simplify f2py execution. (d8a058f, 2016-06-04, https://github.com/QuLogic)
+  Don't change directories, and don't mangle `sys.argv`. The former can be
+  specified directly in the `Popen` constructor, and the latter is cruft
+  from when the f2py module was imported directly.
+
+
+0.7 / 2016-03-13 
 ----------------
 
-- Fix cross compatibility with older NumPy and Python 3.
+- Fix cross compatibility with older NumPy and Python 3. (15ab10c)
 
 Thanks to `Elliott Sales de Andrade`_ for this contribution
 
 .. _Elliott Sales de Andrade: https://github.com/QuLogic
 
 
 0.6 / 2015-12-02
@@ -17,15 +33,15 @@
 
 - Decode text before printing
 - Call f2py module instead of binary (numpy >=1.10 is mandatory)
 - Check if f2py command failed
 
 Thanks to `Juan Luis Cano Rodríguez`_ for this contribution
 
-.. _Juan Luis Cano Rodriguez: https://github.com/Juanlu001
+.. _Juan Luis Cano Rodríguez: https://github.com/Juanlu001
 
 
 0.5 / 2015-01-21
 ----------------
 
 - Call f2py via subprocess. It fixes problems finding fortran compilers under Windows. (Thanks to `David Powell`_ )
 
@@ -71,8 +87,8 @@
 - Improved documentation
 
 .. _Bradley Froehle: https://github.com/bfroehle
 
 0.1 / 2013-09-08
 ----------------
 
-- First public release
+- First public release
```

### Comparing `fortran-magic-0.7/fortranmagic.py` & `fortran-magic-0.7.1/fortranmagic.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     import md5 as hashlib
 
 from IPython.core.error import UsageError
 from IPython.core.magic import Magics, magics_class, line_magic, cell_magic
 from IPython.core import display, magic_arguments
 from IPython.utils import py3compat
 from IPython.utils.io import capture_output
-from IPython.utils.path import get_ipython_cache_dir
+from IPython.paths import get_ipython_cache_dir
 import numpy as np
 from numpy.f2py import f2py2e
 from numpy.distutils import fcompiler
 from distutils.core import Distribution
 from distutils.ccompiler import compiler_class
 from distutils.command.build_ext import build_ext
 from distutils.version import LooseVersion
 
 
-__version__ = '0.6.1'
+__version__ = '0.7.1'
 fcompiler.load_all_fcompiler_classes()
 
 
 def compose(*decorators):
     """Helper to compose decorators::
 
         @a
@@ -144,76 +144,65 @@
         super(FortranMagics, self).__init__(shell=shell)
         self._reloads = {}
         self._code_cache = {}
         self._lib_dir = os.path.join(get_ipython_cache_dir(), 'fortran')
         if not os.path.exists(self._lib_dir):
             os.makedirs(self._lib_dir)
 
-    def _import_all(self, module, verbosity=0):
+    def _import_all(self, module, verbosity=0, code=''):
         imported = []
         for k, v in module.__dict__.items():
             if not k.startswith('__'):
+                v.__source__ = code
                 self.shell.push({k: v})
                 imported.append(k)
         if verbosity > 0 and imported:
             print("\nOk. The following fortran objects "
                   "are ready to use: %s" % ", ".join(imported))
 
     def _run_f2py(self, argv, show_captured=False, verbosity=0):
         """
-        Here we directly call the numpy.f2py.f2py2e.run_compile() entry point,
-        after some small amount of setup to get sys.argv and the current
-        working directory set appropriately.
+        Here we directly call the numpy.f2py module or the f2py executable.
         """
-        old_argv = sys.argv
-        old_cwd = os.getcwdu() if sys.version_info[0] == 2 else os.getcwd()
-        try:
-            if np.__version__ < LooseVersion('1.10.0'):
-                if sys.version_info[0] >= 3:
-                    sys.argv = ['f2py3']
-                else:
-                    sys.argv = ['f2py']
+        if np.__version__ < LooseVersion('1.10.0'):
+            if sys.version_info[0] >= 3:
+                command = ['f2py3']
             else:
-                sys.argv = [sys.executable, '-m', 'numpy.f2py']
-            sys.argv += map(str, argv)
+                command = ['f2py']
+        else:
+            command = [sys.executable, '-m', 'numpy.f2py']
+        command += map(str, argv)
 
-            if verbosity > 1:
-                print("Running...\n   %s" % ' '.join(sys.argv))
+        if verbosity > 1:
+            print("Running...\n   %s" % ' '.join(command))
 
-            os.chdir(self._lib_dir)
+        with capture_output() as captured:
+            # subprocess.call(command)
+            # Refactor subprocess call to work with jupyterhub
+            try:
+                p = Popen(command, stdout=PIPE, stderr=PIPE, stdin=PIPE,
+                          cwd=self._lib_dir)
+            except OSError as e:
+                if e.errno == errno.ENOENT:
+                    print("Couldn't find program: %r" % command[0])
+                    return
+                else:
+                    raise
             try:
-                with capture_output() as captured:
-                    #subprocess.call(sys.argv)
-                    # Refactor subprocess call to work with jupyterhub
-                    try:
-                      p = Popen(sys.argv, stdout=PIPE, stderr=PIPE, stdin=PIPE)
-                    except OSError as e:
-                      if e.errno == errno.ENOENT:
-                        print("Couldn't find program: %r" % sys.argv[0])
-                        return
-                      else:
-                        raise
-                    try:
-                      out, err = p.communicate(input=None)
-                    except:
-                      pass
-                    if err:
-                      sys.stderr.write(err.decode())
-                      sys.stderr.flush()
-                if show_captured or verbosity > 2:
-                    if out:
-                      sys.stdout.write(out.decode())
-                      sys.stdout.flush()
-                    captured()
-            except SystemExit as e:
-                captured()
-                raise UsageError(str(e))
-        finally:
-            sys.argv = old_argv
-            os.chdir(old_cwd)
+                out, err = p.communicate(input=None)
+            except:
+                pass
+            if err:
+                sys.stderr.write(err.decode())
+                sys.stderr.flush()
+        if show_captured or verbosity > 2:
+            if out:
+                sys.stdout.write(out.decode())
+                sys.stdout.flush()
+            captured()
 
         return p.returncode
 
     @magic_arguments.magic_arguments()
     @magic_arguments.argument(
         '--resources', action="store_true",
         help="""List system resources found by system_info.py.
@@ -376,15 +365,15 @@
         res = self._run_f2py(f2py_args + ['-m', module_name, '-c', f90_file],
                              verbosity=args.verbosity)
         if res != 0:
            raise RuntimeError("f2py failed, see output")
 
         self._code_cache[key] = module_name
         module = imp.load_dynamic(module_name, module_path)
-        self._import_all(module, verbosity=args.verbosity)
+        self._import_all(module, verbosity=args.verbosity, code=code)
 
     @property
     def so_ext(self):
         """The extension suffix for compiled modules."""
         try:
             return self._so_ext
         except AttributeError:
```

### Comparing `fortran-magic-0.7/setup.py` & `fortran-magic-0.7.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 from setuptools import setup
 
 long_description = (open('README.rst').read() + '\n\n' +
                     open('CHANGES.rst').read())
 
 setup(
     name='fortran-magic',
-    version='0.7',
+    version='0.7.1',
     description='An extension for IPython that help to use Fortran in '
                 'your interactive session.',
     long_description=long_description,
+    long_description_content_type="text/x-rst",
     author='Martin Gaitan',
     author_email='gaitan@gmail.com',
     url='https://github.com/mgaitan/fortran_magic',
     license='BSD',
     keywords="ipython notebook fortran f2py science",
     py_modules=['fortranmagic'],
     install_requires=['ipython', 'numpy'],
```

### Comparing `fortran-magic-0.7/README.rst` & `fortran-magic-0.7.1/README.rst`

 * *Files identical despite different names*

