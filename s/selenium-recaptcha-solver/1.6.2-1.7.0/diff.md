# Comparing `tmp/selenium-recaptcha-solver-1.6.2.tar.gz` & `tmp/selenium-recaptcha-solver-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-recaptcha-solver-1.6.2.tar", last modified: Wed Apr 12 10:33:03 2023, max compression
+gzip compressed data, was "selenium-recaptcha-solver-1.7.0.tar", last modified: Wed Apr  5 10:14:07 2023, max compression
```

## Comparing `selenium-recaptcha-solver-1.6.2.tar` & `selenium-recaptcha-solver-1.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 10:33:03.984895 selenium-recaptcha-solver-1.6.2/
--rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     3501 2023-04-12 10:33:03.984895 selenium-recaptcha-solver-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     3075 2023-03-25 19:51:06.000000 selenium-recaptcha-solver-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 10:33:03.976571 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/
--rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/__init__.py
--rw-rw-rw-   0        0        0      971 2023-04-12 10:28:50.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/delay_config.py
--rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/exceptions.py
--rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/services.py
--rw-rw-rw-   0        0        0     8996 2023-04-12 10:29:28.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/solver.py
-drwxrwxrwx   0        0        0        0 2023-04-12 10:33:03.983574 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/
--rw-rw-rw-   0        0        0     3501 2023-04-12 10:33:03.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-04-12 10:33:03.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 10:33:03.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-12 10:33:03.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-12 10:33:03.000000 selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 10:33:03.984895 selenium-recaptcha-solver-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-04-12 10:30:22.000000 selenium-recaptcha-solver-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-05 10:14:07.242616 selenium-recaptcha-solver-1.7.0/
+-rw-rw-rw-   0        0        0     1095 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3501 2023-04-05 10:14:07.242616 selenium-recaptcha-solver-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3075 2023-03-25 19:51:06.000000 selenium-recaptcha-solver-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-05 10:14:07.235616 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/
+-rw-rw-rw-   0        0        0      170 2023-02-21 21:45:09.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/__init__.py
+-rw-rw-rw-   0        0        0     1702 2023-03-25 19:51:06.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/delay_config.py
+-rw-rw-rw-   0        0        0       48 2023-01-08 17:39:18.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/exceptions.py
+-rw-rw-rw-   0        0        0     7838 2023-02-11 09:55:38.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/services.py
+-rw-rw-rw-   0        0        0     9587 2023-04-05 09:59:38.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/solver.py
+drwxrwxrwx   0        0        0        0 2023-04-05 10:14:07.241617 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/
+-rw-rw-rw-   0        0        0     3501 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-05 10:14:07.000000 selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-05 10:14:07.242616 selenium-recaptcha-solver-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-04-05 10:13:09.000000 selenium-recaptcha-solver-1.7.0/setup.py
```

### Comparing `selenium-recaptcha-solver-1.6.2/LICENSE` & `selenium-recaptcha-solver-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.6.2/PKG-INFO` & `selenium-recaptcha-solver-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.6.2
+Version: 1.7.0
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
```

### Comparing `selenium-recaptcha-solver-1.6.2/README.md` & `selenium-recaptcha-solver-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/services.py` & `selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/services.py`

 * *Files identical despite different names*

### Comparing `selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver/solver.py` & `selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver/solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         self._driver.switch_to.frame(iframe)
 
         checkbox = self._driver.find_element(
             by='id',
             value='recaptcha-anchor',
         )
 
+        if self._delay_config:
+            self._delay_config.delay_before_click_checkbox()
+
         self._js_click(checkbox)
 
         if self._delay_config:
             self._delay_config.delay_after_click_checkbox()
 
         if checkbox.get_attribute('aria-checked') == 'true':
             return
@@ -106,28 +109,34 @@
         # Locate captcha audio button and click it via JavaScript
         audio_button = self._wait_for_element(
             by=By.ID,
             locator='recaptcha-audio-button',
             timeout=10,
         )
 
+        if self._delay_config:
+            self._delay_config.delay_before_click_audio_button()
+
         self._js_click(audio_button)
 
         if self._delay_config:
             self._delay_config.delay_after_click_audio_button()
 
         self._solve_audio_challenge()
 
         # Locate verify button and click it via JavaScript
         verify_button = self._wait_for_element(
             by=By.ID,
             locator='recaptcha-verify-button',
             timeout=5,
         )
 
+        if self._delay_config:
+            self._delay_config.delay_before_click_verify_button()
+
         self._js_click(verify_button)
 
         if self._delay_config:
             self._delay_config.delay_after_click_verify_button()
 
         try:
             self._wait_for_element(
@@ -141,14 +150,17 @@
             # Locate verify button again to avoid stale element reference and click it via JavaScript
             second_verify_button = self._wait_for_element(
                 by=By.ID,
                 locator='recaptcha-verify-button',
                 timeout=5,
             )
 
+            if self._delay_config:
+                self._delay_config.delay_before_click_verify_button()
+
             self._js_click(second_verify_button)
 
             if self._delay_config:
                 self._delay_config.delay_after_click_verify_button()
 
         except TimeoutException:
             pass
@@ -204,16 +216,22 @@
         for path in tmp_files:
             if os.path.exists(path):
                 os.remove(path)
 
         # Write transcribed text to iframe's input box
         response_textbox = self._driver.find_element(By.ID, 'audio-response')
 
+        if self._delay_config:
+            self._delay_config.delay_before_type_answer()
+
         self._human_type(element=response_textbox, text=recognized_text)
 
+        if self._delay_config:
+            self._delay_config.delay_after_type_answer()
+
     def _js_click(self, element: WebElement) -> None:
         """
         Perform click on given web element using JavaScript.
 
         :param element: web element to click
         """
```

### Comparing `selenium-recaptcha-solver-1.6.2/selenium_recaptcha_solver.egg-info/PKG-INFO` & `selenium-recaptcha-solver-1.7.0/selenium_recaptcha_solver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-recaptcha-solver
-Version: 1.6.2
+Version: 1.7.0
 Home-page: https://github.com/thicccat688/selenium-recaptcha-solver
 Download-URL: https://pypi.org/project/selenium-recaptcha-solver
 Author: Tomás Perestrelo
 Author-email: tomasperestrelo21@gmail.com
 License: MIT
 Keywords: python,captcha,speech recognition,selenium,web automation
 Description-Content-Type: text/markdown
```

