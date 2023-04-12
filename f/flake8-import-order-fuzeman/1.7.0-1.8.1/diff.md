# Comparing `tmp/flake8-import-order-fuzeman-1.7.0.tar.gz` & `tmp/flake8-import-order-fuzeman-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\flake8-import-order-fuzeman-1.7.0.tar", last modified: Sun Jan  7 23:36:45 2018, max compression
+gzip compressed data, was "flake8-import-order-fuzeman-1.8.1.tar", last modified: Wed Apr 12 00:27:06 2023, max compression
```

## Comparing `flake8-import-order-fuzeman-1.7.0.tar` & `flake8-import-order-fuzeman-1.8.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2018-01-07 23:36:45.000000 flake8-import-order-fuzeman-1.7.0/
-drwxrwxrwx   0        0        0        0 2018-01-07 23:36:45.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/
--rw-rw-rw-   0        0        0        1 2018-01-07 23:36:44.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2018-01-07 23:36:44.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     5812 2018-01-07 23:36:44.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       26 2018-01-07 23:36:44.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/requires.txt
--rw-rw-rw-   0        0        0      368 2018-01-07 23:36:44.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       28 2018-01-07 23:36:44.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6322 2018-01-07 23:29:46.000000 flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.py
--rw-rw-rw-   0        0        0     5812 2018-01-07 23:36:45.000000 flake8-import-order-fuzeman-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3416 2018-01-07 23:33:27.000000 flake8-import-order-fuzeman-1.7.0/README.rst
--rw-rw-rw-   0        0        0       74 2018-01-07 23:36:45.000000 flake8-import-order-fuzeman-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1751 2018-01-07 23:33:40.000000 flake8-import-order-fuzeman-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:27:06.316589 flake8-import-order-fuzeman-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-12 00:26:52.000000 flake8-import-order-fuzeman-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-12 00:27:06.316589 flake8-import-order-fuzeman-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-12 00:26:52.000000 flake8-import-order-fuzeman-1.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:27:06.316589 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-12 00:27:06.000000 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-12 00:27:06.000000 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:27:06.000000 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 00:27:06.000000 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 00:27:06.000000 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-12 00:26:52.000000 flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-12 00:27:06.316589 flake8-import-order-fuzeman-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:26:52.000000 flake8-import-order-fuzeman-1.8.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flake8-import-order-fuzeman-1.7.0/flake8_import_order_fuzeman.py` & `flake8-import-order-fuzeman-1.8.1/flake8_import_order_fuzeman.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,201 +1,200 @@
-from flake8_import_order import (
-    IMPORT_3RD_PARTY, IMPORT_APP, IMPORT_APP_PACKAGE,
-    IMPORT_APP_RELATIVE, IMPORT_FUTURE, IMPORT_STDLIB,
-    ClassifiedImport
-)
-from flake8_import_order.checker import ImportOrderChecker
-from flake8_import_order.styles import Error, Style, lookup_entry_point
-import ast
-import textwrap
-import unittest
-
-IMPORT_EXTERNAL_SET = {IMPORT_STDLIB, IMPORT_3RD_PARTY}
-
-__all__ = 'Fuzeman',
-
-
-class Fuzeman(Style):
-    from_importable_standard_librarires = frozenset([
-        'argparse',
-        'collections',
-        'contextlib',
-        'copy',
-        'datetime',
-        'decimal',
-        'json',
-        'pkgutil',
-        'pprint',
-        'subprocess',
-        'tempfile',
-        'threading',
-        'typing'
-    ])
-
-    @staticmethod
-    def name_key(identifier):
-        name = identifier.lstrip('_')
-        hidden = name != identifier
-
-        if not name:
-            return 2, hidden
-        elif name.isupper():
-            return 0, hidden  # constants e.g. CONSTANT_NAME
-        elif name[0].isupper():
-            return 1, hidden  # classes e.g. ClassName
-        else:
-            return 2, hidden  # normal variables e.g. normal_names
-
-    @staticmethod
-    def module_key(name):
-        return name.lower(), name
-
-    @classmethod
-    def sorted_names(cls, names):
-        return sorted(names, key=cls.name_key)
-
-    @classmethod
-    def import_key(cls, import_):
-        modules = [cls.module_key(module) for module in import_.modules]
-        names = [cls.name_key(name) for name in import_.names]
-
-        group = import_.type
-
-        # Reorder import types
-        if group in (IMPORT_APP, IMPORT_APP_PACKAGE):
-            group += IMPORT_APP_RELATIVE
-        elif group == IMPORT_FUTURE:
-            group += IMPORT_APP + IMPORT_APP_RELATIVE + 10
-        elif group == IMPORT_3RD_PARTY:
-            group = IMPORT_STDLIB
-
-        # Order `import ...` below `from ... import ...`
-        if not import_.is_from:
-            group -= 5
-
-        return -group, -import_.level, modules, names
-
-    @classmethod
-    def same_section(cls, previous, current):
-        return (
-            # Both imports match
-            current.type == previous.type or
-
-            # Both imports are external (stdlib, or third-party)
-            (previous.type in IMPORT_EXTERNAL_SET and current.type in IMPORT_EXTERNAL_SET) or
-
-            # Both imports are relative
-            {previous.type, current.type} <= {IMPORT_APP, IMPORT_APP_RELATIVE}
-        )
-
-    def check(self):
-        for i in self.nodes:
-            if not isinstance(i, ClassifiedImport):
-                continue
-
-            mod = i.modules[0]
-
-            if i.type == IMPORT_STDLIB and i.is_from and mod not in self.from_importable_standard_librarires:
-                yield Error(i.lineno, 'I901',
-                            'A standard library is imported using '
-                            '"from {0} import ..." statement. Should be '
-                            '"import {0}" instead.'.format(mod))
-            elif i.type in (IMPORT_APP, IMPORT_APP_PACKAGE) and not i.is_from:
-                yield Error(i.lineno, 'I902',
-                            'An app module is imported using "import {0}"'
-                            ' statement. Should be "from {0} import ..."'
-                            ' instead.'.format(mod))
-        for error in super(Fuzeman, self).check():
-            yield error
-
-
-class TestCase(unittest.TestCase):
-    def assert_error_codes(self, expected_error_codes, filename, code):
-        tree = ast.parse(code, filename or '<stdin>')
-
-        checker = ImportOrderChecker(filename, tree)
-        checker.lines = code.splitlines(True)
-        checker.options = {
-            'application_import_names': ['myapp', 'tests'],
-            'import_order_style': lookup_entry_point('fuzeman'),
-        }
-
-        errors = list(checker.check_order())
-
-        self.assertEquals(
-            frozenset(expected_error_codes),
-            frozenset(error.code for error in errors)
-        )
-
-    def test_itself(self):
-        with open(__file__) as f:
-            code = f.read()
-
-        self.assert_error_codes([], __file__, code)
-
-    def make_test(expected_error_codes, code):
-        def test_func(self):
-            self.assert_error_codes(expected_error_codes, None, textwrap.dedent(code))
-
-        return test_func
-
-    test_valid_1 = make_test([], '''
-        from __future__ import absolute_import
-
-        from myapp import something
-        from myapp.helpers import get_view
-        from myapp.views import *
-        from ...deepest import a
-        from ..deeper import b
-        from .a import this, that
-        from .z import This, That
-
-        from pkg_resources import (SOURCE_DIST, EntryPoint, Requirement, get_provider)
-        from typing import Optional
-        import arrow
-        import datetime
-        import sys
-    ''')
-
-    test_constants_must_be_former_than_classes = make_test(['I101'], '''
-        from pkg_resources import EntryPoint, SOURCE_DIST
-    ''')
-
-    test_classes__must_be_former_than_normal_names = make_test(['I101'], '''
-        from pkg_resources import get_provider, Requirement
-    ''')
-
-    test_deeper_relative_imports_must_be_latter = make_test(['I100'], '''
-        from ..deeper import b
-        from ...deepest import a
-    ''')
-
-    test_app_imports_must_be_former_than_relative_imports = \
-        make_test(['I100'], '''
-            from .rel import a
-            from myapp import b
-        ''')
-
-    test_standard_libraries_must_not_be_from_import = make_test(['I901'], '''
-        from sys import argv
-    ''')
-
-    test_typing_is_only_exception_able_to_be_from_import = make_test([], '''
-        from typing import Sequence
-        import typing
-    ''')
-
-    test_from_typing_must_be_former_than_import_typing = make_test(
-        ['I100'],
-        '''
-        import typing
-        from typing import Sequence
-        '''
-    )
-
-    test_can_import_3rd_parties = make_test([], '''
-        import pkg_resources
-    ''')
-
-    test_apps_must_be_from_import = make_test(['I902'], '''
-        import myapp
-    ''')
+from flake8_import_order import (
+    ImportType,
+    ClassifiedImport
+)
+from flake8_import_order.checker import ImportOrderChecker
+from flake8_import_order.styles import Error, Style, lookup_entry_point
+import ast
+import textwrap
+import unittest
+
+IMPORT_EXTERNAL_SET = {ImportType.STDLIB, ImportType.THIRD_PARTY}
+
+__all__ = 'Fuzeman',
+
+
+class Fuzeman(Style):
+    from_importable_standard_librarires = frozenset([
+        'argparse',
+        'collections',
+        'contextlib',
+        'copy',
+        'datetime',
+        'decimal',
+        'json',
+        'pkgutil',
+        'pprint',
+        'subprocess',
+        'tempfile',
+        'threading',
+        'typing'
+    ])
+
+    @staticmethod
+    def name_key(identifier):
+        name = identifier.lstrip('_')
+        hidden = name != identifier
+
+        if not name:
+            return 2, hidden
+        elif name.isupper():
+            return 0, hidden  # constants e.g. CONSTANT_NAME
+        elif name[0].isupper():
+            return 1, hidden  # classes e.g. ClassName
+        else:
+            return 2, hidden  # normal variables e.g. normal_names
+
+    @staticmethod
+    def module_key(name):
+        return name.lower(), name
+
+    @classmethod
+    def sorted_names(cls, names):
+        return sorted(names, key=cls.name_key)
+
+    @classmethod
+    def import_key(cls, import_):
+        modules = [cls.module_key(module) for module in import_.modules]
+        names = [cls.name_key(name) for name in import_.names]
+
+        group = import_.type
+
+        # Reorder import types
+        if group in (ImportType.APPLICATION, ImportType.APPLICATION_PACKAGE):
+            group += ImportType.APPLICATION_RELATIVE
+        elif group == ImportType.FUTURE:
+            group += ImportType.APPLICATION + ImportType.APPLICATION_RELATIVE + 10
+        elif group == ImportType.THIRD_PARTY:
+            group = ImportType.STDLIB
+
+        # Order `import ...` below `from ... import ...`
+        if not import_.is_from:
+            group -= 5
+
+        return -group, -import_.level, modules, names
+
+    @classmethod
+    def same_section(cls, previous, current):
+        return (
+            # Both imports match
+            current.type == previous.type or
+
+            # Both imports are external (stdlib, or third-party)
+            (previous.type in IMPORT_EXTERNAL_SET and current.type in IMPORT_EXTERNAL_SET) or
+
+            # Both imports are relative
+            {previous.type, current.type} <= {ImportType.APPLICATION, ImportType.APPLICATION_RELATIVE}
+        )
+
+    def check(self):
+        for i in self.nodes:
+            if not isinstance(i, ClassifiedImport):
+                continue
+
+            mod = i.modules[0]
+
+            if i.type == ImportType.STDLIB and i.is_from and mod not in self.from_importable_standard_librarires:
+                yield Error(i.lineno, 'I901',
+                            'A standard library is imported using '
+                            '"from {0} import ..." statement. Should be '
+                            '"import {0}" instead.'.format(mod))
+            elif i.type in (ImportType.APPLICATION, ImportType.APPLICATION_PACKAGE) and not i.is_from:
+                yield Error(i.lineno, 'I902',
+                            'An app module is imported using "import {0}"'
+                            ' statement. Should be "from {0} import ..."'
+                            ' instead.'.format(mod))
+        for error in super(Fuzeman, self).check():
+            yield error
+
+
+class TestCase(unittest.TestCase):
+    def assert_error_codes(self, expected_error_codes, filename, code):
+        tree = ast.parse(code, filename or '<stdin>')
+
+        checker = ImportOrderChecker(filename, tree)
+        checker.lines = code.splitlines(True)
+        checker.options = {
+            'application_import_names': ['myapp', 'tests'],
+            'import_order_style': lookup_entry_point('fuzeman'),
+        }
+
+        errors = list(checker.check_order())
+
+        self.assertEqual(
+            frozenset(expected_error_codes),
+            frozenset(error.code for error in errors)
+        )
+
+    def test_itself(self):
+        with open(__file__) as f:
+            code = f.read()
+
+        self.assert_error_codes([], __file__, code)
+
+    def make_test(expected_error_codes, code):
+        def test_func(self):
+            self.assert_error_codes(expected_error_codes, None, textwrap.dedent(code))
+
+        return test_func
+
+    test_valid_1 = make_test([], '''
+        from __future__ import absolute_import
+
+        from myapp import something
+        from myapp.helpers import get_view
+        from myapp.views import *
+        from ...deepest import a
+        from ..deeper import b
+        from .a import this, that
+        from .z import This, That
+
+        from pkg_resources import (SOURCE_DIST, EntryPoint, Requirement, get_provider)
+        from typing import Optional
+        import arrow
+        import datetime
+        import sys
+    ''')
+
+    test_constants_must_be_former_than_classes = make_test(['I101'], '''
+        from pkg_resources import EntryPoint, SOURCE_DIST
+    ''')
+
+    test_classes__must_be_former_than_normal_names = make_test(['I101'], '''
+        from pkg_resources import get_provider, Requirement
+    ''')
+
+    test_deeper_relative_imports_must_be_latter = make_test(['I100'], '''
+        from ..deeper import b
+        from ...deepest import a
+    ''')
+
+    test_app_imports_must_be_former_than_relative_imports = \
+        make_test(['I100'], '''
+            from .rel import a
+            from myapp import b
+        ''')
+
+    test_standard_libraries_must_not_be_from_import = make_test(['I901'], '''
+        from sys import argv
+    ''')
+
+    test_typing_is_only_exception_able_to_be_from_import = make_test([], '''
+        from typing import Sequence
+        import typing
+    ''')
+
+    test_from_typing_must_be_former_than_import_typing = make_test(
+        ['I100'],
+        '''
+        import typing
+        from typing import Sequence
+        '''
+    )
+
+    test_can_import_3rd_parties = make_test([], '''
+        import pkg_resources
+    ''')
+
+    test_apps_must_be_from_import = make_test(['I902'], '''
+        import myapp
+    ''')
```

