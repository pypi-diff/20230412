# Comparing `tmp/watchtower_browser_testing-0.1.4.tar.gz` & `tmp/watchtower_browser_testing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.1.4.tar", last modified: Sun Apr  2 19:05:08 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.2.0.tar", last modified: Wed Apr 12 09:53:22 2023, max compression
```

## Comparing `watchtower_browser_testing-0.1.4.tar` & `watchtower_browser_testing-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 19:05:08.744567 watchtower_browser_testing-0.1.4/
--rw-rw-rw-   0        0        0      310 2023-04-02 19:05:08.744567 watchtower_browser_testing-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-02 19:05:08.744567 watchtower_browser_testing-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 19:05:08.728974 watchtower_browser_testing-0.1.4/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      393 2023-04-01 18:08:23.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0       72 2023-04-01 17:37:20.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     6842 2023-04-02 19:04:58.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7697 2023-04-02 18:56:39.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-02 19:04:58.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-02 19:05:08.744567 watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-02 19:05:08.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-02 19:05:08.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 19:05:08.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-02 19:05:08.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-02 19:05:08.000000 watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 09:53:22.466011 watchtower_browser_testing-0.2.0/
+-rw-rw-rw-   0        0        0      310 2023-04-12 09:53:22.466011 watchtower_browser_testing-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:53:22.466011 watchtower_browser_testing-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:53:22.466011 watchtower_browser_testing-0.2.0/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-04-12 09:47:53.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     9236 2023-04-12 09:52:38.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 09:52:50.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:53:22.466011 watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-12 09:53:22.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-12 09:53:22.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:53:22.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 09:53:22.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 09:53:22.000000 watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.1.4/setup.py` & `watchtower_browser_testing-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.1.4/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.2.0/watchtower_browser_testing/tracking_validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,241 +1,272 @@
-import os
-import glob
-import importlib
-import inspect
+import re
+from urllib.parse import urlparse, parse_qs
+from http.cookies import SimpleCookie
 
-from playwright.sync_api import sync_playwright
+from cerberus import Validator
+import playwright.sync_api
 
-from watchtower_browser_testing.tracking_validation import EventQueue, RequestValidator
-from watchtower_browser_testing import exceptions
 from watchtower_browser_testing import config
 
 
-class TestContext(object):
+class ValidatorError(Exception): pass
 
-    def __init__(self):
 
-        self.scenario_context = {}
-        self.context = {}
+class RequestWrapper(object):
 
-    def get(self, key):
+    def __init__(self,
+                 request):
 
-        return self.scenario_context.get(key) or self.context.get(key)
+        self.request = request
+        self.errors = None
 
-    def set(self, key, value, level='test'):
+    @property
+    def url(self):
 
-        assert level in ('test', 'scenario'), '`level` should be test or scenario'
+        return self.request.url
 
-        if level == 'test':
-            self.context[key] = value
-            self.scenario_context.pop(key, None)
-        else:
-            self.scenario_context[key] = value
-            self.context.pop(key, None)
+    @property
+    def parsed_url(self):
+
+        return urlparse(self.url)
 
-    def reset_scenario_context(self):
+    @property
+    def parsed_qs(self):
 
-        self.scenario_context = {}
+        parsed_qs = parse_qs(self.parsed_url.query)
 
-    def reset_context(self):
+        for key, value in parsed_qs.items():
+            if isinstance(value, list):
+                if len(value) == 1:
+                    parsed_qs[key] = value[0]
+                elif len(value) == 0:
+                    parsed_qs.pop(key)
 
-        self.context = {}
+        return parsed_qs
 
+    @property
+    def headers(self):
 
-class TestResult(object):
+        return self.request.all_headers()
 
-    def __init__(self,
-                 test_name,
-                 browser,
-                 scenario=None,
-                 event=None,
-                 ok=True,
-                 errors=None,
-                 data=None):
-
-        self.test_name = test_name
-        self.scenario = scenario
-        self.event = event
-        self.browser = browser
-        self.ok = ok
-        self.errors = errors
-        self.data = data
+    @property
+    def cookies(self):
 
-    def as_dict(self):
+        cookies = SimpleCookie()
+        cookies.load(self.headers.get('cookie', ''))
+        return cookies
 
-        return {
-            'name': self.test_name,
-            'scenario': self.scenario,
-            'event': self.event,
-            'browser': self.browser,
-            'ok': self.ok,
-            'errors': self.errors,
-            'data': self.data
-        }
+    @property
+    def harvest_user_id(self):
 
+        cookies = self.cookies
 
-class TrackingTest(object):
+        if config.HARVEST_USER_SS_COOKIE_NAME in cookies:
+            return cookies[config.HARVEST_USER_SS_COOKIE_NAME].value
 
-    browsers = config.DEFAULT_BROWSERS
+        elif config.HARVEST_USER_WEB_COOKIE_NAME in cookies:
+            return cookies[config.HARVEST_USER_WEB_COOKIE_NAME].value
 
-    pipeline_pattern = config.DEFAULT_PIPELINE_PATTERN
+        elif not self.post_data_json is None and config.OLD_HARVEST_USER_ID_KEY in self.post_data_json:
+            return self.post_data_json[config.OLD_HARVEST_USER_ID_KEY]
 
-    def setUpInstance(self,
-                      playwright,
-                      browser,
-                      headless=False):
+        return None
 
-        self.app = getattr(playwright, browser)
-        self.browser = self.app.launch(headless=headless)
-        self.context = self.browser.new_context()
-        self.data_context = TestContext()
+    @property
+    def frame_url(self):
+        return self.request.frame.url
 
-    def tearDownInstance(self):
+    @property
+    def method(self):
+        return self.request.method
 
-        self.context.close()
-        self.browser.close()
+    @property
+    def post_data_json(self):
+        try:
+            return self.request.post_data_json
+        except playwright.sync_api.Error:
+            return None
+
+    def add_error(self,
+                  namespace,
+                  key,
+                  error):
+
+        namespace_errors = self.errors.get(namespace, {})
+        namespace_errors[key] = namespace_errors.get(key, []) + [error]
+        self.errors[namespace] = namespace_errors
+
+    def validate_query_string(self,
+                              validator):
+
+        if isinstance(validator, Validator):
+
+            validator.allow_unknown = True
+            if not validator.validate(self.parsed_qs):
+                self.errors['query_string'] = validator.errors
+
+        elif isinstance(validator, dict):
+
+            for key, value in validator.items():
+                actual_value = self.parsed_qs.get(key)
+                if actual_value is None:
+                    self.add_error('query_string', key, f'should have value "{value}", but was missing')
+                elif actual_value != value:
+                    self.add_error('query_string', key, f'should have value "{value}", not "{actual_value}"')
+        else:
+            raise ValidatorError('Query string validator should be a dict or Validator object')
 
-    def beforeEach(self):
+    @staticmethod
+    def build_validation_rule(value):
 
-        self.page = self.context.new_page()
-        self.data_context.reset_scenario_context()
+        return {
+            'type': {
+                'bool': 'boolean',
+                'bytes': 'binary',
+                'datetime.date': 'date',
+                'datetime.datetime': 'datetime',
+                'float': 'float',
+                'int': 'integer',
+                'str': 'string'
+            }[type(value).__name__],
+            'allowed': [value]
+        }
 
-    def afterEach(self):
+    def validate_body(self,
+                      validator):
 
-        self.page.close()
+        if isinstance(validator, dict):
 
-    def record_events(self):
+            validator = Validator({key: self.build_validation_rule(value) for key, value in validator.items()})
 
-        self.event_queue = EventQueue(url_pattern=self.pipeline_pattern)
-        self.page.on('request', self.event_queue.register)
+        if isinstance(validator, Validator):
 
-    def run(self,
-            browser=None,
-            headless=False,
-            report_data=None):
+            validator.allow_unknown = True
+            if not validator.validate(self.post_data_json):
+                self.errors['body'] = validator.errors
 
-        if browser is None:
-            browsers = self.browsers
         else:
-            browsers = [browser]
+            raise ValidatorError('Body validator should be a dict or Validator object')
 
-        self.results = []
-        report_data = report_data or {}
+    def is_valid(self,
+                 validators):
 
-        for browser in browsers:
+        self.errors = {}
 
-            with sync_playwright() as playwright:
+        if 'query_string' in validators:
 
-                self.setUpInstance(playwright, browser, headless=headless)
+            v = validators['query_string']
+            self.validate_query_string(v)
 
-                tests = [func for func in dir(self) if func.startswith(config.SCENARIO_METHOD_PREFIX)]
+        if 'body' in validators:
 
-                for test in tests:
+            v = validators['body']
+            self.validate_body(v)
 
-                    scenario = test[len(config.SCENARIO_METHOD_PREFIX):]
+        if not 'check_user_id' in validators or validators['check_user_id']:
 
-                    self.beforeEach()
+            if self.harvest_user_id is None:
+                self.add_error('general', 'harvest_user_id', 'No valid value found')
 
-                    getattr(self, test)()
-                    validation_setup = getattr(self, config.VALIDATION_METHOD_PREFIX + scenario)()
+        return len(self.errors) == 0
 
-                    for event, setup in validation_setup.items():
 
-                        validator = RequestValidator(**setup)
-                        validator.select(self.event_queue.requests)
+class RequestValidator(object):
 
-                        if validator.is_valid():
-                            self.result(browser=browser, scenario=scenario, event=event, ok=True,
-                                        data={'n_matched_requests': validator.n_matched_requests, **report_data})
-                        else:
-                            self.result(browser=browser, scenario=scenario, event=event, ok=False,
-                                        errors=validator.errors,
-                                        data={'n_matched_requests': validator.n_matched_requests, **report_data})
+    def __init__(self,
+                 selectors,
+                 validators,
+                 allow_multiple=False):
 
-                    self.afterEach()
+        self.selectors = selectors
+        self.validators = validators
 
-                self.tearDownInstance()
+        self.allow_multiple = allow_multiple
+        self.matched_requests = []
+        self.errors = None
 
-    def result(self,
-               browser,
-               scenario,
-               event,
-               ok,
-               errors=None,
-               data=None):
+    def is_valid(self):
 
-        self.results.append(
-            TestResult(
-                test_name=self.name,
-                scenario=scenario,
-                event=event,
-                browser=browser,
-                ok=ok,
-                errors=errors,
-                data=data)
-        )
+        self.errors = []
 
-    @property
-    def name(self):
+        if self.n_matched_requests == 0:
+            self.errors.append({'general': 'No matched requests found'})
+
+        for request in self.matched_requests:
+            if not request.is_valid(validators=self.validators):
+                self.errors.append(request.errors)
 
-        return self.__class__.__name__
+        if not self.allow_multiple and self.n_matched_requests > 1:
+            self.errors.append({'general': 'multiple matching requests are not allowed'})
+
+        return len(self.errors) == 0
 
     @property
-    def description(self):
+    def n_matched_requests(self):
+        return len(self.matched_requests)
 
-        return config.DEFAULT_TEST_DESCRIPTION
+    def select(self, requests):
 
+        for request_ in requests:
 
+            request = RequestWrapper(request=request_)
 
-class TestRunner(object):
+            if 'method' in self.selectors:
+                if request.method != self.selectors['method']:
+                    continue
 
-    def __init__(self,
-                 modules=None,
-                 directory=None):
+            if 'body' in self.selectors:
 
-        self.modules = modules
-        self.directory = directory
+                if not isinstance(request.post_data_json, dict):
+                    continue
 
-    def run_tests(self,
-                  headless=False,
-                  browser=None):
+                select = True
 
-        directory = self.directory or os.getcwd()
+                for key, value in self.selectors['body'].items():
+                    if request.post_data_json.get(key) != value:
+                        select = False
+                        break
 
-        mods = glob.glob(os.path.join(directory, "*.py"))
-        test_files = [os.path.basename(f)[:-3] for f in mods
-                      if os.path.isfile(f) and os.path.basename(f).startswith(config.TEST_FILE_PREFIX)]
+                if not select:
+                    continue
 
-        if self.modules:
+            if 'url' in self.selectors:
+                if not request.url.startswith(self.selectors['url']):
+                    continue
 
-            missing = set(self.modules) - set(test_files)
-            if len(missing) > 0:
-                raise exceptions.NotFoundError(f'Did not find test module(s): {", ".join(missing)}')
+            if 'frame_url' in self.selectors:
+                if not request.frame_url.startswith(self.selectors['frame_url']):
+                    continue
 
-            test_files = [tf for tf in test_files if tf in self.modules]
+            if 'query_string' in self.selectors:
+                select = True
+                for key, value in self.selectors['query_string'].items():
+                    if value not in request.parsed_qs.get(key, []):
+                        select = False
+                        break
 
-        results = []
+                if not select:
+                    continue
 
-        for test_file in test_files:
+            self.matched_requests.append(request)
 
-            mod = importlib.import_module(test_file)
+        return len(self.matched_requests) > 0
 
-            tests = []
-            for attr in dir(mod):
-                if inspect.isclass(getattr(mod, attr)) and issubclass(getattr(mod, attr), TrackingTest):
-                    if any(x.startswith(config.SCENARIO_METHOD_PREFIX) for x in dir(getattr(mod, attr))):
-                        tests.append({'file': test_file, 'class': getattr(mod, attr)})
 
-            for test in tests:
+class EventQueue(object):
 
-                test_instance = test['class']()
-                report_data = {'file': test_file}
-                test_instance.run(headless=headless,
-                                  browser=browser,
-                                  report_data=report_data)
-                results.extend(test_instance.results)
+    def __init__(self,
+                 url_patterns):
 
-        return results
+        self.url_patterns = url_patterns
+        self.requests = []
 
+    def register(self, request):
 
+        if self.registration_filter(request):
+            self.requests.append(request)
 
+    def registration_filter(self, request):
 
+        if not any(re.match(url_pattern, request.url) for url_pattern in self.url_patterns):
+            return False
+        return True
```

### Comparing `watchtower_browser_testing-0.1.4/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.2.0/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

