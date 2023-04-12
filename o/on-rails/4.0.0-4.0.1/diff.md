# Comparing `tmp/on_rails-4.0.0.tar.gz` & `tmp/on_rails-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "on_rails-4.0.0.tar", max compression
+gzip compressed data, was "on_rails-4.0.1.tar", max compression
```

## Comparing `on_rails-4.0.0.tar` & `on_rails-4.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-12 19:50:44.677832 on_rails-4.0.0/LICENSE
--rw-r--r--   0        0        0    14186 2023-04-12 19:50:44.677832 on_rails-4.0.0/README.md
--rw-r--r--   0        0        0    48141 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/Result.py
--rw-r--r--   0        0        0     2866 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetail.py
--rw-r--r--   0        0        0     1802 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/ErrorDetail.py
--rw-r--r--   0        0        0      808 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/BadRequestError.py
--rw-r--r--   0        0        0      819 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ConflictError.py
--rw-r--r--   0        0        0      840 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ExceptionError.py
--rw-r--r--   0        0        0      728 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ForbiddenError.py
--rw-r--r--   0        0        0      726 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/InternalError.py
--rw-r--r--   0        0        0     1227 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/NotFoundError.py
--rw-r--r--   0        0        0      880 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
--rw-r--r--   0        0        0      753 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ValidationError.py
--rw-r--r--   0        0        0      474 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/__init__.py
--rw-r--r--   0        0        0      573 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/CreatedDetail.py
--rw-r--r--   0        0        0      629 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
--rw-r--r--   0        0        0      831 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/PartialContentDetail.py
--rw-r--r--   0        0        0      188 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/SuccessDetail.py
--rw-r--r--   0        0        0      100 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/__init__.py
--rw-r--r--   0        0        0      135 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/__init__.py
--rw-r--r--   0        0        0     4867 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/_utility.py
--rw-r--r--   0        0        0     2085 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/decorator.py
--rw-r--r--   0        0        0     8011 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/test_helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 19:50:44.677832 on_rails-4.0.0/pyproject.toml
--rw-r--r--   0        0        0    14813 1970-01-01 00:00:00.000000 on_rails-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 20:37:44.960427 on_rails-4.0.1/LICENSE
+-rw-r--r--   0        0        0    14186 2023-04-12 20:37:44.960427 on_rails-4.0.1/README.md
+-rw-r--r--   0        0        0    48606 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/Result.py
+-rw-r--r--   0        0        0     2866 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetail.py
+-rw-r--r--   0        0        0     1802 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/ErrorDetail.py
+-rw-r--r--   0        0        0      808 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/Errors/BadRequestError.py
+-rw-r--r--   0        0        0      819 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/Errors/ConflictError.py
+-rw-r--r--   0        0        0      840 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/Errors/ExceptionError.py
+-rw-r--r--   0        0        0      728 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/ForbiddenError.py
+-rw-r--r--   0        0        0      726 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/InternalError.py
+-rw-r--r--   0        0        0     1227 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/NotFoundError.py
+-rw-r--r--   0        0        0      880 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/UnauthorizedError.py
+-rw-r--r--   0        0        0      753 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/ValidationError.py
+-rw-r--r--   0        0        0      474 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/__init__.py
+-rw-r--r--   0        0        0      573 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/CreatedDetail.py
+-rw-r--r--   0        0        0      629 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/NotModifiedDetail.py
+-rw-r--r--   0        0        0      831 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/PartialContentDetail.py
+-rw-r--r--   0        0        0      188 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/SuccessDetail.py
+-rw-r--r--   0        0        0      100 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/__init__.py
+-rw-r--r--   0        0        0     4867 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/_utility.py
+-rw-r--r--   0        0        0     2085 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/decorator.py
+-rw-r--r--   0        0        0     8011 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/test_helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 20:37:44.964428 on_rails-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14813 1970-01-01 00:00:00.000000 on_rails-4.0.1/PKG-INFO
```

### Comparing `on_rails-4.0.0/LICENSE` & `on_rails-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/README.md` & `on_rails-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/Result.py` & `on_rails-4.0.1/on_rails/Result.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,38 +330,43 @@
 
         return self.on_success_operate_when(condition_or_func, lambda: self.__fail_when(error_detail))
 
     # endregion
 
     # region on_fail
 
-    def on_fail(self, func: Callable, num_of_try: int = 1, try_only_on_exceptions=True):
+    def on_fail(self, func: Callable, num_of_try: int = 1, try_only_on_exceptions=True, none_means_success: bool = False):
         """
         If the result is not successful, call the function with the given arguments
 
         :param func: The function to call
 
         :param num_of_try: num_of_try is an optional parameter that specifies the number of times the function should be
         tried in case of failure. If the function fails on the first try, it will be retried num_of_try times. If num_of_try
         is not specified, the function will only be tried once, defaults to 1 (optional)
 
         :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
         exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
         function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
         :type try_only_on_exceptions: bool (optional)
 
+        :param none_means_success: A boolean parameter that determines whether a `None` output should be considered a
+        success or a failure. If `none_means_success` is `True`, then a `None` output will be considered a success and the
+        function will return a `Result.ok()` instance. If `none_means_success` is, defaults to True
+        :type none_means_success: bool (optional)
+
         :return: The result object is being returned.
         """
 
         if not is_func_valid(func):
             return Result.fail(ValidationError(message="The input function is not valid."))
         if self.success:
             return self
         return self.try_func(func, num_of_try, ignore_previous_error=True,
-                             try_only_on_exceptions=try_only_on_exceptions, none_means_success=False)
+                             try_only_on_exceptions=try_only_on_exceptions, none_means_success=none_means_success)
 
     def on_fail_add_more_data(self, object_or_func: Union[Any, Callable], ignore_errors: bool = False):
         """
         This function adds more data to an error detail object, and returns the original object or a new one
         with the added data.
 
         :param object_or_func: The parameter `object_or_fuc` can be either an object or a function.
@@ -439,15 +444,16 @@
         :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
         exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
         function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
         :type try_only_on_exceptions: bool (optional)
         :param ignore_errors: If it is false, it will return the error result when the result of the function fails, otherwise it will be ignored.
         :return: an instance of the class that it belongs to (presumably named `self`).
         """
-        result = self.on_fail(func, num_of_try, try_only_on_exceptions)
+
+        result = self.on_fail(func, num_of_try, try_only_on_exceptions, none_means_success=True)
         if result.success or ignore_errors:
             return self  # ignore result
         return result
 
     def on_fail_raise_exception(self, exception_type: Optional[type] = None):
         """
         Request to raise the exception when the previous function failed.
```

### Comparing `on_rails-4.0.0/on_rails/ResultDetail.py` & `on_rails-4.0.1/on_rails/ResultDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/ErrorDetail.py` & `on_rails-4.0.1/on_rails/ResultDetails/ErrorDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/BadRequestError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/BadRequestError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/ConflictError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/ConflictError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/ExceptionError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/ExceptionError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/ForbiddenError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/ForbiddenError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/InternalError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/InternalError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/NotFoundError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/NotFoundError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/UnauthorizedError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/UnauthorizedError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Errors/ValidationError.py` & `on_rails-4.0.1/on_rails/ResultDetails/Errors/ValidationError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Success/CreatedDetail.py` & `on_rails-4.0.1/on_rails/ResultDetails/Success/CreatedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Success/NotModifiedDetail.py` & `on_rails-4.0.1/on_rails/ResultDetails/Success/NotModifiedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/Success/PartialContentDetail.py` & `on_rails-4.0.1/on_rails/ResultDetails/Success/PartialContentDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/ResultDetails/SuccessDetail.py` & `on_rails-4.0.1/on_rails/ResultDetails/SuccessDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/_utility.py` & `on_rails-4.0.1/on_rails/_utility.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/decorator.py` & `on_rails-4.0.1/on_rails/decorator.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/on_rails/test_helpers.py` & `on_rails-4.0.1/on_rails/test_helpers.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.0/pyproject.toml` & `on_rails-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "on_rails"
-version = "4.0.0"
+version = "4.0.1"
 description = "Simple and powerful Railway Oriented library for python"
 authors = ["Payadel <payadelteam@gmail.com>"]
 readme = "README.md"
 license = "GPLV3"
 repository = "https://github.com/Payadel/on_rails"
 keywords = ["railway oriented","functional programming", "error handling"]
 packages = [{ include = "on_rails" }]
```

### Comparing `on_rails-4.0.0/PKG-INFO` & `on_rails-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: on-rails
-Version: 4.0.0
+Version: 4.0.1
 Summary: Simple and powerful Railway Oriented library for python
 Home-page: https://github.com/Payadel/on_rails
 License: GPLV3
 Keywords: railway oriented,functional programming,error handling
 Author: Payadel
 Author-email: payadelteam@gmail.com
 Requires-Python: >=3.10,<4.0
```

