# Comparing `tmp/watchtower_browser_testing-0.2.3.tar.gz` & `tmp/watchtower_browser_testing-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.2.3.tar", last modified: Wed Apr 12 12:02:57 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.2.4.tar", last modified: Wed Apr 12 13:23:30 2023, max compression
```

## Comparing `watchtower_browser_testing-0.2.3.tar` & `watchtower_browser_testing-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/
--rw-rw-rw-   0        0        0      310 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:02:57.559282 watchtower_browser_testing-0.2.3/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0    10082 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-12 12:02:23.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/
+-rw-rw-rw-   0        0        0      310 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0    11517 2023-04-12 13:23:18.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 13:23:18.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 13:23:30.424163 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 13:23:30.000000 watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.2.3/setup.py` & `watchtower_browser_testing-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.3/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.2.4/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.3/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.2.4/watchtower_browser_testing/testsuite.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 import importlib.util
 import inspect
 import sys
 import types
 import functools
 
 from playwright.sync_api import sync_playwright
+import marko
 
 from watchtower_browser_testing.tracking_validation import EventQueue, RequestValidator
 from watchtower_browser_testing import exceptions
 from watchtower_browser_testing import config
 
+markdown = marko.Markdown()
+
 class TestContext(object):
 
     def __init__(self):
 
         self.scenario_context = {}
         self.context = {}
 
@@ -219,86 +222,125 @@
         )
 
     @property
     def name(self):
 
         return self.__class__.__name__
 
-    @property
-    def description(self):
+    @classmethod
+    def scenario_methods(cls):
+
+        return [x for x in dir(cls) if x.startswith(config.SCENARIO_METHOD_PREFIX)]
+
+    def md_description(self):
 
-        return config.DEFAULT_TEST_DESCRIPTION
+        md = markdown.parse(self.__doc__)
 
+        for scenario_method in self.scenario_methods():
+            md.children.extend(markdown.parse(getattr(self, scenario_method).__doc__).children)
 
+        return md
 
-class TestRunner(object):
+
+class MeasurementPlan(object):
 
     def __init__(self,
                  modules=None,
                  directory=None):
 
         self.modules = modules
         self.directory = directory
 
-    def run_tests(self,
-                  headless=False,
-                  browser=None,
-                  gtm_web_preview_link=None,
-                  tag_assistant_path=None):
-
-        if not gtm_web_preview_link is None and not re.match(config.GTM_WEB_PREVIEW_LINK_REGEX, gtm_web_preview_link):
-            raise exceptions.InvalidInputError(f'This does not look like a valid gtm-preview link: {gtm_web_preview_link}')
-
-        if not gtm_web_preview_link is None and browser != 'chromium':
-            raise exceptions.InvalidInputError(f'Debugging with GTM preview only works in chromium, not {browser}')
-
-        if not gtm_web_preview_link is None:
-            tag_assistant_path = tag_assistant_path or config.DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION
-            if not (os.path.isdir(tag_assistant_path)
-                    and os.path.isfile(os.path.join(tag_assistant_path, 'manifest.json'))):
-                raise exceptions.InvalidInputError(f'No tag assistant extension found at {tag_assistant_path}')
+    def get_tests(self):
 
         directory = self.directory or os.getcwd()
 
         mods = glob.glob(os.path.join(directory, '*.py'))
         test_modules = [os.path.basename(f)[:-3] for f in mods
-                      if os.path.isfile(f) and os.path.basename(f).startswith(config.TEST_FILE_PREFIX)]
+                        if os.path.isfile(f) and os.path.basename(f).startswith(config.TEST_FILE_PREFIX)]
 
         if self.modules:
 
             missing = set(self.modules) - set(test_modules)
             if len(missing) > 0:
                 raise exceptions.NotFoundError(f'Did not find test module(s): {", ".join(missing)}')
 
             test_modules = [tf for tf in test_modules if tf in self.modules]
 
-        results = []
+        tests = []
 
         for module_name in test_modules:
 
             spec = importlib.util.spec_from_file_location(module_name, os.path.join(directory, module_name + '.py'))
             module = importlib.util.module_from_spec(spec)
             sys.modules[module_name] = module
             spec.loader.exec_module(module)
 
-            tests = []
             for attr in dir(module):
                 if inspect.isclass(getattr(module, attr)) and issubclass(getattr(module, attr), TrackingTest):
                     if any(x.startswith(config.SCENARIO_METHOD_PREFIX) for x in dir(getattr(module, attr))):
                         tests.append({'module': module_name, 'class': getattr(module, attr)})
 
-            for test in tests:
+        missing_validation_methods = []
+        for test in tests:
+            for method in dir(test['class']):
+                if method.startswith(config.SCENARIO_METHOD_PREFIX):
+                    scenario = method[len(config.SCENARIO_METHOD_PREFIX):]
+                    if not hasattr(test['class'], config.VALIDATION_METHOD_PREFIX + scenario):
+                        missing_validation_methods.append(
+                            test['module'] +
+                            '.' + test['class'].__name__ +
+                            '.' + config.VALIDATION_METHOD_PREFIX + scenario)
+
+        if len(missing_validation_methods) > 0:
+            raise exceptions.NotFoundError(
+                f'The following validation methods are missing: {", ".join(missing_validation_methods)}')
 
-                test_instance = test['class']()
-                report_data = {'module': module_name}
-                test_instance.run(headless=headless,
-                                  browser=browser,
-                                  gtm_web_preview_link=gtm_web_preview_link,
-                                  tag_assistant_path=tag_assistant_path,
-                                  report_data=report_data)
-                results.extend(test_instance.results)
+        return tests
+
+    def run_tests(self,
+                  headless=False,
+                  browser=None,
+                  gtm_web_preview_link=None,
+                  tag_assistant_path=None):
+
+        if not gtm_web_preview_link is None and not re.match(config.GTM_WEB_PREVIEW_LINK_REGEX, gtm_web_preview_link):
+            raise exceptions.InvalidInputError(f'This does not look like a valid gtm-preview link: {gtm_web_preview_link}')
+
+        if not gtm_web_preview_link is None and browser != 'chromium':
+            raise exceptions.InvalidInputError(f'Debugging with GTM preview only works in chromium, not {browser}')
+
+        if not gtm_web_preview_link is None:
+            tag_assistant_path = tag_assistant_path or config.DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION
+            if not (os.path.isdir(tag_assistant_path)
+                    and os.path.isfile(os.path.join(tag_assistant_path, 'manifest.json'))):
+                raise exceptions.InvalidInputError(f'No tag assistant extension found at {tag_assistant_path}')
+
+        tests = self.get_tests()
+
+        results = []
+        for test in tests:
+
+            test_instance = test['class']()
+            report_data = {'module': test['module']}
+            test_instance.run(headless=headless,
+                              browser=browser,
+                              gtm_web_preview_link=gtm_web_preview_link,
+                              tag_assistant_path=tag_assistant_path,
+                              report_data=report_data)
+            results.extend(test_instance.results)
 
         return results
 
+    def md_description(self):
+
+        tests = self.get_tests()
+
+        md = markdown.parse(self.__doc__)
+
+        for test in tests:
+            md.children.extend(test.md_description().children)
+
+        return md
```

### Comparing `watchtower_browser_testing-0.2.3/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.2.4/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.2.4/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

