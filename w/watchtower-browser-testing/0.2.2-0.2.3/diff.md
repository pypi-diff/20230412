# Comparing `tmp/watchtower_browser_testing-0.2.2.tar.gz` & `tmp/watchtower_browser_testing-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.2.2.tar", last modified: Wed Apr 12 10:28:07 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.2.3.tar", last modified: Wed Apr 12 12:02:57 2023, max compression
```

## Comparing `watchtower_browser_testing-0.2.2.tar` & `watchtower_browser_testing-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:28:07.303743 watchtower_browser_testing-0.2.2/
--rw-rw-rw-   0        0        0      310 2023-04-12 10:28:07.302779 watchtower_browser_testing-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 10:28:07.303743 watchtower_browser_testing-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:28:07.293744 watchtower_browser_testing-0.2.2/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      522 2023-04-12 09:47:53.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 10:27:57.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-12 10:27:57.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:28:07.300742 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-12 10:28:07.000000 watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/
+-rw-rw-rw-   0        0        0      310 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:02:57.559282 watchtower_browser_testing-0.2.3/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      143 2023-04-01 17:58:47.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      526 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0    10082 2023-04-12 11:53:39.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-12 12:02:23.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-12 12:02:57.577987 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 12:02:57.000000 watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.2.2/setup.py` & `watchtower_browser_testing-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.2/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.2.3/watchtower_browser_testing/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 SCENARIO_METHOD_PREFIX = 'scenario_'
 VALIDATION_METHOD_PREFIX = 'validation_'
 DEFAULT_TEST_DESCRIPTION = ''
 DEFAULT_BROWSERS = ['chromium', 'firefox', 'webkit']
 HARVEST_USER_SS_COOKIE_NAME = '_harvest_ss_user'
 HARVEST_USER_WEB_COOKIE_NAME = '_harvest_web_user'
 OLD_HARVEST_USER_ID_KEY = 'oldHarvestUserId'
-GTM_PREVIEW_LINK_REGEX = r'^https://tagassistant[.]google[.]com/.*'
+GTM_WEB_PREVIEW_LINK_REGEX = r'^https://tagassistant[.]google[.]com/.*'
 DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION = r'tag_assistant'
```

### Comparing `watchtower_browser_testing-0.2.2/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.2.3/watchtower_browser_testing/testsuite.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,35 +87,35 @@
     browsers = config.DEFAULT_BROWSERS
 
     pipeline_patterns = [config.DEFAULT_PIPELINE_PATTERN]
 
     def setUpInstance(self,
                       playwright,
                       browser,
-                      gtm_preview_link=None,
+                      gtm_web_preview_link=None,
                       tag_assistant_path=None,
                       headless=False):
 
         self.app = getattr(playwright, browser)
 
-        if gtm_preview_link and re.match(config.GTM_PREVIEW_LINK_REGEX, gtm_preview_link):
+        if gtm_web_preview_link and re.match(config.GTM_WEB_PREVIEW_LINK_REGEX, gtm_web_preview_link):
             self.browser = None
             tag_assistant_path is tag_assistant_path or config.DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION
             args = [
                 f'--disable-extensions-except={tag_assistant_path}',
                 f'--load-extension={tag_assistant_path}']
             if headless:
                 args.append('--headless=new')
             self.context = self.app.launch_persistent_context(
                 '',
                 headless=False,
                 args=args
             )
             self.ta_page = self.context.new_page()
-            self.ta_page.goto(gtm_preview_link)
+            self.ta_page.goto(gtm_web_preview_link)
             with self.ta_page.expect_popup() as page_info:
                 self.ta_page.get_by_role("button", name="Connect").click()
             self.page = page_info.value
             self.ta_page.get_by_role("button", name="Continue", exact=True).click()
             self.page.close()
             func = functools.partial(new_page_from_gtm, ta_page=self.ta_page)
             self.context.new_page = types.MethodType(func, self.context)
@@ -145,15 +145,15 @@
 
         self.event_queue = EventQueue(url_patterns=self.pipeline_patterns)
         self.page.on('request', self.event_queue.register)
 
     def run(self,
             browser=None,
             headless=False,
-            gtm_preview_link=None,
+            gtm_web_preview_link=None,
             tag_assistant_path=None,
             report_data=None):
 
         if browser is None:
             browsers = self.browsers
         else:
             browsers = [browser]
@@ -163,15 +163,15 @@
 
         for browser in browsers:
 
             with sync_playwright() as playwright:
 
                 self.setUpInstance(playwright,
                                    browser,
-                                   gtm_preview_link=gtm_preview_link,
+                                   gtm_web_preview_link=gtm_web_preview_link,
                                    tag_assistant_path=tag_assistant_path,
                                    headless=headless)
 
                 tests = [func for func in dir(self) if func.startswith(config.SCENARIO_METHOD_PREFIX)]
 
                 for test in tests:
 
@@ -238,24 +238,24 @@
 
         self.modules = modules
         self.directory = directory
 
     def run_tests(self,
                   headless=False,
                   browser=None,
-                  gtm_preview_link=None,
+                  gtm_web_preview_link=None,
                   tag_assistant_path=None):
 
-        if not gtm_preview_link is None and not re.match(config.GTM_PREVIEW_LINK_REGEX, gtm_preview_link):
-            raise exceptions.InvalidInputError(f'This does not look like a valid gtm-preview link: {gtm_preview_link}')
+        if not gtm_web_preview_link is None and not re.match(config.GTM_WEB_PREVIEW_LINK_REGEX, gtm_web_preview_link):
+            raise exceptions.InvalidInputError(f'This does not look like a valid gtm-preview link: {gtm_web_preview_link}')
 
-        if not gtm_preview_link is None and browser != 'chromium':
+        if not gtm_web_preview_link is None and browser != 'chromium':
             raise exceptions.InvalidInputError(f'Debugging with GTM preview only works in chromium, not {browser}')
 
-        if not gtm_preview_link is None:
+        if not gtm_web_preview_link is None:
             tag_assistant_path = tag_assistant_path or config.DEFAULT_PATH_TO_TAG_ASSISTANT_EXTENSION
             if not (os.path.isdir(tag_assistant_path)
                     and os.path.isfile(os.path.join(tag_assistant_path, 'manifest.json'))):
                 raise exceptions.InvalidInputError(f'No tag assistant extension found at {tag_assistant_path}')
 
         directory = self.directory or os.getcwd()
 
@@ -288,15 +288,15 @@
 
             for test in tests:
 
                 test_instance = test['class']()
                 report_data = {'module': module_name}
                 test_instance.run(headless=headless,
                                   browser=browser,
-                                  gtm_preview_link=gtm_preview_link,
+                                  gtm_web_preview_link=gtm_web_preview_link,
                                   tag_assistant_path=tag_assistant_path,
                                   report_data=report_data)
                 results.extend(test_instance.results)
 
         return results
```

### Comparing `watchtower_browser_testing-0.2.2/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.2.3/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.2.2/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.2.3/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

