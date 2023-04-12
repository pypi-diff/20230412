# Comparing `tmp/on_rails-3.1.0.tar.gz` & `tmp/on_rails-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "on_rails-3.1.0.tar", max compression
+gzip compressed data, was "on_rails-4.0.0.tar", max compression
```

## Comparing `on_rails-3.1.0.tar` & `on_rails-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-10 20:21:28.797593 on_rails-3.1.0/LICENSE
--rw-r--r--   0        0        0    14186 2023-04-10 20:21:28.797593 on_rails-3.1.0/README.md
--rw-r--r--   0        0        0    37998 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/Result.py
--rw-r--r--   0        0        0     2866 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetail.py
--rw-r--r--   0        0        0     1504 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetails/ErrorDetail.py
--rw-r--r--   0        0        0      808 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetails/Errors/BadRequestError.py
--rw-r--r--   0        0        0      819 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetails/Errors/ConflictError.py
--rw-r--r--   0        0        0      840 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetails/Errors/ExceptionError.py
--rw-r--r--   0        0        0      728 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py
--rw-r--r--   0        0        0      726 2023-04-10 20:21:28.797593 on_rails-3.1.0/on_rails/ResultDetails/Errors/InternalError.py
--rw-r--r--   0        0        0     1227 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Errors/NotFoundError.py
--rw-r--r--   0        0        0      880 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
--rw-r--r--   0        0        0      753 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Errors/ValidationError.py
--rw-r--r--   0        0        0      474 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Errors/__init__.py
--rw-r--r--   0        0        0      573 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Success/CreatedDetail.py
--rw-r--r--   0        0        0      629 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
--rw-r--r--   0        0        0      831 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py
--rw-r--r--   0        0        0      188 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/Success/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/SuccessDetail.py
--rw-r--r--   0        0        0      100 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/ResultDetails/__init__.py
--rw-r--r--   0        0        0      135 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/__init__.py
--rw-r--r--   0        0        0     4780 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/_utility.py
--rw-r--r--   0        0        0     1760 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/decorator.py
--rw-r--r--   0        0        0     7444 2023-04-10 20:21:28.801593 on_rails-3.1.0/on_rails/test_helpers.py
--rw-r--r--   0        0        0      722 2023-04-10 20:21:28.801593 on_rails-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    14813 1970-01-01 00:00:00.000000 on_rails-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 19:50:44.677832 on_rails-4.0.0/LICENSE
+-rw-r--r--   0        0        0    14186 2023-04-12 19:50:44.677832 on_rails-4.0.0/README.md
+-rw-r--r--   0        0        0    48141 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/Result.py
+-rw-r--r--   0        0        0     2866 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetail.py
+-rw-r--r--   0        0        0     1802 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/ErrorDetail.py
+-rw-r--r--   0        0        0      808 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/BadRequestError.py
+-rw-r--r--   0        0        0      819 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ConflictError.py
+-rw-r--r--   0        0        0      840 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ExceptionError.py
+-rw-r--r--   0        0        0      728 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ForbiddenError.py
+-rw-r--r--   0        0        0      726 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/InternalError.py
+-rw-r--r--   0        0        0     1227 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/NotFoundError.py
+-rw-r--r--   0        0        0      880 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
+-rw-r--r--   0        0        0      753 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/ValidationError.py
+-rw-r--r--   0        0        0      474 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Errors/__init__.py
+-rw-r--r--   0        0        0      573 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/CreatedDetail.py
+-rw-r--r--   0        0        0      629 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
+-rw-r--r--   0        0        0      831 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/PartialContentDetail.py
+-rw-r--r--   0        0        0      188 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/Success/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/SuccessDetail.py
+-rw-r--r--   0        0        0      100 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/ResultDetails/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/__init__.py
+-rw-r--r--   0        0        0     4867 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/_utility.py
+-rw-r--r--   0        0        0     2085 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/decorator.py
+-rw-r--r--   0        0        0     8011 2023-04-12 19:50:44.677832 on_rails-4.0.0/on_rails/test_helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 19:50:44.677832 on_rails-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14813 1970-01-01 00:00:00.000000 on_rails-4.0.0/PKG-INFO
```

### Comparing `on_rails-3.1.0/LICENSE` & `on_rails-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/README.md` & `on_rails-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/Result.py` & `on_rails-4.0.0/on_rails/Result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Callable, Generic, List, Optional, TypeVar, Union
+from typing import (Any, Callable, Coroutine, Generic, List, Optional, TypeVar,
+                    Union)
 
 from on_rails._utility import (await_func, generate_error,
                                get_num_of_function_parameters, is_func_valid)
 from on_rails.ResultDetail import ResultDetail
 from on_rails.ResultDetails.ErrorDetail import ErrorDetail
 from on_rails.ResultDetails.Errors.ValidationError import ValidationError
 from on_rails.ResultDetails.SuccessDetail import SuccessDetail
@@ -29,15 +30,23 @@
         self.value = value
 
     def __str__(self) -> str:
         result = f"success: {self.success}\n"
         if self.value:
             result += f"Value: {self.value}\n"
         if self.detail:
-            result += f"Detail:\n{self.detail}\n"
+            result += f"Detail:\n{str(self.detail)}\n"
+        return result
+
+    def __repr__(self):
+        result = f"success: {self.success}\n"
+        if self.value:
+            result += f"Value: {self.value}\n"
+        if self.detail:
+            result += f"Detail:\n{repr(self.detail)}\n"
         return result
 
     # region Static Methods
 
     @staticmethod
     def ok(value: Optional[T] = None, detail: Optional[ResultDetail] = None):
         """
@@ -66,22 +75,25 @@
     def convert_to_result(value: Any, none_means_success: bool = True):
         """
         The function converts a given output to a Result object, where None can indicate success or failure depending on the
         value of a boolean parameter.
 
         :param value: The output parameter is of type Any, which means it can be any Python object
         :type value: Any
+
         :param none_means_success: A boolean parameter that determines whether a `None` output should be considered a
         success or a failure. If `none_means_success` is `True`, then a `None` output will be considered a success and the
         function will return a `Result.ok()` instance. If `none_means_success` is, defaults to True
         :type none_means_success: bool (optional)
+
         :return: The function `convert_to_result` returns a `Result` object. If the `output` parameter is `None`, it returns
         a `Result` object with a success status if `none_means_success` is `True`, otherwise it returns a `Result` object
         with a failure status. If the `output` parameter is already a `Result` object, it returns it as is. Otherwise,
         """
+
         if value is None:
             return Result.ok() if none_means_success else Result.fail()
         if isinstance(value, Result):
             return value
         return Result.ok(value)
 
     # endregion
@@ -115,14 +127,15 @@
         :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
         exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
         function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
         :type try_only_on_exceptions: bool (optional)
 
         :return: The method `on_success` returns either self or the result of given function.
         """
+
         if not self.success:
             return self
 
         return self.__call_func(func, optional_args=[self.value, self],
                                 num_of_try=num_of_try, try_only_on_exceptions=try_only_on_exceptions)
 
     def on_success_add_more_data(self, object_or_func: Union[Any, Callable], ignore_errors: bool = False):
@@ -240,39 +253,71 @@
         If condition not pass, returns previous Result object.
         """
         if not self.success:
             return self
         return self.__operate_when(condition_or_func, func, [self.value, self],
                                    num_of_try, try_only_on_exceptions, break_rails)
 
-    def on_success_break(self, condition_or_func: Union[Callable, bool]):
+    def on_success_break_rails(self, condition_or_func: Union[Callable, bool] = True):
         """
-        The function raises a BreakRails exception if a given condition is true.
+        The function raises a BreakRailsException if a given condition is true.
+        The BreakRailsException breaks all chaining functions and can catch by
+        @def_result decorator or functions that supports `try_func` like on_success, etc
 
         :param condition_or_func: The parameter `condition_or_func` can be either a callable function or a boolean value.
         It is used to determine whether to break chaining of functions or not. If it is a callable function, it
         will be called with two optional arguments: the value and the result of the previous operation.
         :type condition_or_func: Union[Callable, bool]
 
         :return: If `condition_or_func` is callable function and fails, it returns error result.
         Otherwise, raise BreakRails exception
 
-        :raise BreakRails
+        :raise BreakRailsException
         """
+
         if not self.success:
             return self
 
         result = self.__is_condition_pass(condition_or_func, [self.value, self])
         if not result.success:
             return result  # return error result
         if not result.value:  # The condition is not true
             return self
 
         self.__break_rails()
-        return Result.fail(ErrorDetail(message="The BreakRails exception not raised."))  # pragma: no cover
+        return Result.fail(ErrorDetail(message="The BreakRailsException not raised."))  # pragma: no cover
+
+    def on_success_break_function(self, condition_or_func: Union[Callable, bool] = True):
+        """
+        The function raises a BreakFunctionException if a given condition is true.
+        The BreakFunctionException breaks all chaining functions and can catch by
+        @def_result decorator or functions that supports `try_func` like on_success, etc
+
+        :param condition_or_func: The parameter `condition_or_func` can be either a callable function or a boolean value.
+        It is used to determine whether to break chaining of functions or not. If it is a callable function, it
+        will be called with two optional arguments: the value and the result of the previous operation.
+        :type condition_or_func: Union[Callable, bool]
+
+        :return: If `condition_or_func` is callable function and fails, it returns error result.
+        Otherwise, raise BreakRails exception
+
+        :raise BreakFunctionException
+        """
+
+        if not self.success:
+            return self
+
+        result = self.__is_condition_pass(condition_or_func, [self.value, self])
+        if not result.success:
+            return result  # return error result
+        if not result.value:  # The condition is not true
+            return self
+
+        self.__break_function()
+        return Result.fail(ErrorDetail(message="The BreakFunctionException not raised."))  # pragma: no cover
 
     def on_success_fail_when(self, condition_or_func: Union[Callable, bool],
                              error_detail: Optional[ErrorDetail] = None):
         """
         If the previous result is successful and condition is true, return a failure result with the given error detail
 
         :param condition_or_func: The condition or function that needs to be checked before calling the main function. It
@@ -302,20 +347,21 @@
         :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
         exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
         function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
         :type try_only_on_exceptions: bool (optional)
 
         :return: The result object is being returned.
         """
+
         if not is_func_valid(func):
             return Result.fail(ValidationError(message="The input function is not valid."))
         if self.success:
             return self
         return self.try_func(func, num_of_try, ignore_previous_error=True,
-                             try_only_on_exceptions=try_only_on_exceptions)
+                             try_only_on_exceptions=try_only_on_exceptions, none_means_success=False)
 
     def on_fail_add_more_data(self, object_or_func: Union[Any, Callable], ignore_errors: bool = False):
         """
         This function adds more data to an error detail object, and returns the original object or a new one
         with the added data.
 
         :param object_or_func: The parameter `object_or_fuc` can be either an object or a function.
@@ -446,36 +492,59 @@
 
         :return: If condition pass, returns result of function as Result object.
         If condition not pass, returns previous Result object.
         """
 
         if self.success:
             return self
-        return self.__operate_when(condition_or_func, func, [self],
-                                   num_of_try, try_only_on_exceptions, break_rails)
+        return self.__operate_when(condition_or_func, func, [self], num_of_try,
+                                   try_only_on_exceptions, break_rails, none_means_success=False)
 
-    def on_fail_break(self, condition_or_func: Union[Callable, bool]):
+    def on_fail_break_rails(self, condition_or_func: Union[Callable, bool] = True):
         """
-        The function raises a BreakRails exception if a given condition is true.
+        The function raises a BreakRailsException if a given condition is true.
+        The BreakRailsException breaks all chaining functions and can catch by
+        @def_result decorator or functions that supports `try_func` like on_success, etc
 
         :param condition_or_func: The parameter `condition_or_func` can be either a callable function or a boolean value.
         It is used to determine whether to break chaining of functions or not. If it is a callable function, it
         will be called with two optional arguments: the value and the result of the previous operation.
         :type condition_or_func: Union[Callable, bool]
 
         :return: If `condition_or_func` is callable function and fails, it returns error result.
-        Otherwise, raise BreakRails exception
+        Otherwise, raise BreakRailsException
 
-        :raise BreakRails
+        :raise BreakRailsException
         """
+
         if self.success:
             return self
 
         return self.break_rails(condition_or_func)
 
+    def on_fail_break_function(self, condition_or_func: Union[Callable, bool] = True):
+        """
+        The function raises a BreakFunctionException if a given condition is true.
+
+        :param condition_or_func: The parameter `condition_or_func` can be either a callable function or a boolean value.
+        It is used to determine whether to break chaining of functions or not. If it is a callable function, it
+        will be called with two optional arguments: the value and the result of the previous operation.
+        :type condition_or_func: Union[Callable, bool]
+
+        :return: If `condition_or_func` is callable function and fails, it returns error result.
+        Otherwise, raise BreakFunctionException
+
+        :raise BreakFunctionException
+        """
+
+        if self.success:
+            return self
+
+        return self.break_function(condition_or_func)
+
     # endregion
 
     def fail_when(self, condition_or_func: Union[Callable, bool],
                   error_detail: Optional[ErrorDetail] = None, add_prev_detail: bool = False):
         """
         If the condition is true, return a failure result with the given error detail
 
@@ -531,50 +600,64 @@
 
         return self.__operate_when(condition_or_func=condition_or_func,
                                    func=func, optional_args=[self],
                                    num_of_try=num_of_try, try_only_on_exceptions=try_only_on_exceptions,
                                    break_rails=break_rails)
 
     def try_func(self, func: Callable, num_of_try: int = 1,
-                 ignore_previous_error: bool = False, try_only_on_exceptions: bool = True):
+                 ignore_previous_error: bool = False, try_only_on_exceptions: bool = True,
+                 none_means_success: bool = True):
         """
         The function `try_func` attempts to execute a given function with a specified number of tries and handles errors.
 
         :param func: `func` is a function object that will be executed by the `try_func` method. It is the main parameter of
         the method and must be provided for the method to work
+
         :param num_of_try: The number of times the function should be attempted before returning a failure result. The
         default value is 1, meaning the function will be attempted once, defaults to 1 (optional)
+
         :param ignore_previous_error: By default, if the previous function fails, the Result is
          passed as a parameter to the new function. That is, the new function must accept
          1 parameter. If skip_previous_error is True, the new function can be with or without parameters.
         :type ignore_previous_error: bool (optional)
         the error.
 
-    :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
-    exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
-    function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
-    :type try_only_on_exceptions: bool (optional)
+        :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
+        exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
+        function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
+        :type try_only_on_exceptions: bool (optional)
 
-    :return: a `Result` object.
-        :return: an instance of the `Result` class, which contains either a successful result or an error message.
+        :param none_means_success: A boolean parameter that determines whether a `None` output should be considered a
+        success or a failure. If `none_means_success` is `True`, then a `None` output will be considered a success and the
+        function will return a `Result.ok()` instance. If `none_means_success` is, defaults to True
+        :type none_means_success: bool (optional)
+
+        :return: a `Result` object.
+            :return: an instance of the `Result` class, which contains either a successful result or an error message.
         """
+
         if not is_func_valid(func):
             return Result.fail(ValidationError(message="The input function is not valid."))
 
-        num_of_function_params = get_num_of_function_parameters(func)
+        result = _get_num_of_function_parameters(func)
+        if not result.success:
+            return result
+        num_of_function_params = result.value
 
         if num_of_function_params == 0:
             if self.success or ignore_previous_error:
-                return try_func(func, num_of_try=num_of_try, try_only_on_exceptions=try_only_on_exceptions)
+                return try_func(func, num_of_try=num_of_try, try_only_on_exceptions=try_only_on_exceptions,
+                                none_means_success=none_means_success)
             return Result.fail(ValidationError(
                 message="The previous function failed. "
                         "The new function does not have a parameter to get the previous result. "
                         "Either define a function that accepts a parameter or set skip_previous_error to True."))
         if num_of_function_params == 1:
-            return try_func(lambda: func(self), num_of_try=num_of_try, try_only_on_exceptions=try_only_on_exceptions)
+            return try_func(lambda: func(self), num_of_try=num_of_try,
+                            try_only_on_exceptions=try_only_on_exceptions, none_means_success=none_means_success)
         return Result.fail(ValidationError(
             message=f"{func.__name__}() takes {num_of_function_params} arguments. It cannot be executed."))
 
     def finally_tee(self, func: Callable, num_of_try: int = 1, try_only_on_exceptions: bool = True):
         """
         Whether the previous operation was successful or not, this function is executed.
         If the `func` result is successful, the previous result will be returned.
@@ -593,53 +676,90 @@
         should only be retried if an exception is raised or not.
         """
         result = self.__call_func(func, [self], num_of_try, try_only_on_exceptions)
         if result.success:
             return self
         return result
 
-    def break_rails(self, condition_or_func: Union[Callable, bool]):
+    def break_rails(self, condition_or_func: Union[Callable, bool] = True):
         """
-        The function raises a BreakRails exception if a given condition is true.
+        The function raises a BreakRailsException if a given condition is true.
+        The BreakRailsException breaks all chaining functions and can catch by
+        @def_result decorator or functions that supports `try_func` like on_success, etc
 
         :param condition_or_func: The parameter `condition_or_func` can be either a callable function or a boolean value.
         It is used to determine whether to break chaining of functions or not. If it is a callable function, it
         will be called with previous result as optional parameter.
         :type condition_or_func: Union[Callable, bool]
 
         :return: If `condition_or_func` is callable function and fails, it returns error result.
         Otherwise, raise BreakRails exception
 
         :raise BreakRails
         """
+
         result = self.__is_condition_pass(condition_or_func, [self])
         if not result.success:
             return result  # return error result
         if not result.value:  # The condition is not true
             return self
 
         self.__break_rails()
         return Result.fail(ErrorDetail(message="The BreakRails exception not raised."))  # pragma: no cover
 
+    def break_function(self, condition_or_func: Union[Callable, bool] = True):
+        """
+        The function raises a BreakFunctionException if a given condition is true.
+        The BreakFunctionException breaks a function to reach @def_result decorator
+        or catches manually.
+        Important: functions like try_func, on_success, ..., can not (should not) capture this exception.
+        Because if this function catch this, the exception can not break all function codes.
+
+        :param condition_or_func: The parameter `condition_or_func` can be either a callable function or a boolean value.
+        It is used to determine whether to break function or not. If it is a callable function, it
+        will be called with previous result as optional parameter.
+        :type condition_or_func: Union[Callable, bool]
+
+        :return: If `condition_or_func` is callable function and fails, it returns error result.
+        Otherwise, raise BreakFunctionException
+
+        :raise BreakFunctionException
+        """
+
+        result = self.__is_condition_pass(condition_or_func, [self])
+        if not result.success:
+            return result  # return error result
+        if not result.value:  # The condition is not true
+            return self
+
+        self.__break_function()
+        return Result.fail(ErrorDetail(message="The BreakFunctionException not raised."))  # pragma: no cover
+
     # region private methods
 
     @staticmethod
     def __call_func(func: callable, optional_args: List[Any] = None,
-                    num_of_try: int = 1, try_only_on_exceptions: bool = False):
+                    num_of_try: int = 1, try_only_on_exceptions: bool = False, none_means_success: bool = True):
         if not is_func_valid(func):
             return Result.fail(ValidationError(message="The input function is not valid."))
 
         optional_args = optional_args if optional_args else []
-        num_of_function_params = get_num_of_function_parameters(func)
+
+        result = _get_num_of_function_parameters(func)
+        if not result.success:
+            return result
+        num_of_function_params = result.value
+
         if num_of_function_params > len(optional_args):
             return Result.fail(ValidationError(
                 message=f"{func.__name__}() takes {num_of_function_params} arguments. It cannot be executed. "
                         f"maximum of {len(optional_args)} parameters is acceptable."))
 
-        return try_func(lambda: func(*optional_args[:num_of_function_params]), num_of_try, try_only_on_exceptions)
+        return try_func(lambda: func(*optional_args[:num_of_function_params]),
+                        num_of_try, try_only_on_exceptions, none_means_success=none_means_success)
 
     def __is_condition_pass(self, condition_or_func: Union[Callable, bool],
                             optional_args: List[Any] = None,
                             num_of_try: int = 1, try_only_on_exceptions: bool = True):
         """
         This function checks if a given condition or function is true or false and returns a result accordingly.
         If `condition_or_func` is a boolean value, it returns condition.
@@ -660,84 +780,194 @@
             return result
         if result.value is not None and isinstance(result.value, bool):
             return Result.ok(result.value)
         return Result.ok(True)
 
     def __operate_when(self, condition_or_func: Union[Callable, bool],
                        func: Callable, optional_args: List[Any] = None,
-                       num_of_try: int = 1, try_only_on_exceptions=True, break_rails: bool = False):
+                       num_of_try: int = 1, try_only_on_exceptions=True, break_rails: bool = False,
+                       none_means_success: bool = True):
         result = self.__is_condition_pass(condition_or_func, optional_args, num_of_try, try_only_on_exceptions)
         if not result.success:
             return result  # Return error result
         if not result.value:  # The condition is not true
             return self
-        return self.__call_func(func, optional_args, num_of_try, try_only_on_exceptions) \
+        return self.__call_func(func, optional_args, num_of_try,
+                                try_only_on_exceptions, none_means_success=none_means_success) \
             .break_rails(break_rails)
 
     def __break_rails(self):
         raise BreakRailsException(result=self)
 
+    def __break_function(self):
+        raise BreakFunctionException(result=self)
+
     # endregion
 
 
-def try_func(func: Callable, num_of_try: int = 1, try_only_on_exceptions: bool = True) -> Result:
+def try_func(func: Callable, num_of_try: int = 1, try_only_on_exceptions: bool = True,
+             none_means_success: bool = True) -> Result:
     """
     The function `try_func` attempts to execute a given function with a specified number of tries and handles errors.
 
     :param func: The input function that needs to be executed
     :param num_of_try: The number of times the input function will be attempted to execute in case of failure. The default
     value is 1, meaning the function will be executed only once by default, defaults to 1 (optional)
     :return: a `Result` object. The `Result` object can either be a successful result or a failed result with an
     `ValidationError` object containing information about the error.
 
     :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
     exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
     function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
     :type try_only_on_exceptions: bool (optional)
+
+    :param none_means_success: A boolean parameter that determines whether a `None` output should be considered a
+        success or a failure. If `none_means_success` is `True`, then a `None` output will be considered a success and the
+        function will return a `Result.ok()` instance. If `none_means_success` is, defaults to True
+    :type none_means_success: bool (optional)
+
     :return: a `Result` object.
     """
+
     if not is_func_valid(func):
         return Result.fail(ValidationError(message="The input function is not valid."))
 
-    num_of_function_params = get_num_of_function_parameters(func)
+    result = _get_num_of_function_parameters(func)
+    if not result.success:
+        return result
+    num_of_function_params = result.value
+
     if num_of_function_params > 0:
         return Result.fail(ValidationError(
             message=f"{func.__name__}() takes {num_of_function_params} arguments. It cannot be executed."))
 
     errors = []
     for _ in range(num_of_try):
         try:
             result = await_func(func)
+            result = Result.convert_to_result(result, none_means_success=none_means_success)
+            if result.success or try_only_on_exceptions:
+                return result
+            if result.detail:
+                errors.append(result.detail)
+        except BreakFunctionException:
+            raise  # Must be captured and managed in @def_result decorator.
+        except BreakRailsException as e:
+            return e.result
+        except Exception as e:
+            errors.append(e)
+
+    error_detail = generate_error(errors, num_of_try)
+    return Result.fail(error_detail)
+
+
+async def try_func_async(func_async: Callable, num_of_try: int = 1, try_only_on_exceptions: bool = True) -> Result:
+    """
+    The function `try_func` attempts to execute a given function with a specified number of tries and handles errors.
+
+    :param func_async: The input function that needs to be executed
+    :param num_of_try: The number of times the input function will be attempted to execute in case of failure. The default
+    value is 1, meaning the function will be executed only once by default, defaults to 1 (optional)
+    :return: a `Result` object. The `Result` object can either be a successful result or a failed result with an
+    `ValidationError` object containing information about the error.
+
+    :param try_only_on_exceptions: A boolean parameter that determines whether the function should only be retried if an
+    exception is raised. If set to True, the function will only be retried if an exception is raised. If set to False, the
+    function will be retried regardless of whether an exception is raised or Result is not success, defaults to True
+    :type try_only_on_exceptions: bool (optional)
+
+    :return: a `Result` object.
+    """
+
+    if not is_func_valid(func_async):
+        return Result.fail(ValidationError(message="The input function is not valid."))
+
+    result = _get_num_of_function_parameters(func_async)
+    if not result.success:
+        return result
+    num_of_function_params = result.value
+
+    if num_of_function_params > 0:
+        return Result.fail(ValidationError(
+            message=f"{func_async.__name__}() takes {num_of_function_params} arguments. It cannot be executed."))
+
+    errors = []
+    for _ in range(num_of_try):
+        try:
+            result = func_async()
+            if isinstance(result, Coroutine):
+                result = await result
             result = Result.convert_to_result(result)
             if result.success or try_only_on_exceptions:
                 return result
             if result.detail:
                 errors.append(result.detail)
+        except BreakFunctionException:
+            raise  # Must be captured and managed in @def_result decorator.
+        except BreakRailsException as e:
+            return e.result
         except Exception as e:
             errors.append(e)
 
     error_detail = generate_error(errors, num_of_try)
     return Result.fail(error_detail)
 
 
+def _get_num_of_function_parameters(func: Callable):
+    try:
+        return Result.ok(get_num_of_function_parameters(func))
+    except Exception:
+        return Result.fail(ErrorDetail(title="Function Parameter Detection Error",
+                                       message=f"Can not recognize the number of function ({func.__name__}) "
+                                               f"parameters. You can wrap your built-in function with a python "
+                                               f"function like `lambda`.", code=400))
+
+
 # The class `BreakRails` defines an exception that takes a `Result` object as input.
 class BreakRailsException(Exception):
     """
     An exception for break fast chaining of functions.
     It stores the last result.
     """
+
     result: Result
 
     def __init__(self, result: Result):
         """
         This function initializes an object with a non-null and valid instance of the Result class.
 
         :param result: The `result` parameter is an instance of the `Result` class. The constructor checks if
         the `result` parameter is not `None` and is an instance of the `Result` class
         :type result: Result
         """
+
+        super().__init__()
+        if result is None:
+            raise ValueError("The result cannot be None")
+        if not isinstance(result, Result):
+            raise ValueError("The result must be an instance of Result")
+        self.result = result
+
+
+class BreakFunctionException(Exception):
+    """
+    An exception for break fast function.
+    It only catches by @def_result decorator and stores the last result.
+    """
+
+    result: Result
+
+    def __init__(self, result: Result):
+        """
+        This function initializes an object with a non-null and valid instance of the Result class.
+
+        :param result: The `result` parameter is an instance of the `Result` class. The constructor checks if
+        the `result` parameter is not `None` and is an instance of the `Result` class
+        :type result: Result
+        """
+
         super().__init__()
         if result is None:
             raise ValueError("The result cannot be None")
         if not isinstance(result, Result):
             raise ValueError("The result must be an instance of Result")
         self.result = result
```

### Comparing `on_rails-3.1.0/on_rails/ResultDetail.py` & `on_rails-4.0.0/on_rails/ResultDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/ErrorDetail.py` & `on_rails-4.0.0/on_rails/ResultDetails/ErrorDetail.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,13 +34,22 @@
         self.errors[key] = value
 
     def __str__(self):
         error_details = super().__str__()
 
         if self.errors is not None:
             error_details += "Errors: " + str(self.errors) + "\n"
+        if self.exception:
+            error_details += "Exception: " + str(self.exception) + "\n"
+
+        return error_details
 
+    def __repr__(self):
+        error_details = super().__str__()
+
+        if self.errors is not None:
+            error_details += "Errors: " + str(self.errors) + "\n"
         if self.exception:
             error_details += "Exception: " + str(self.exception) + "\n"
         error_details += "Stack trace: " + ''.join(self.stack_trace.format()) + "\n"
 
         return error_details
```

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/BadRequestError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/BadRequestError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/ConflictError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/ConflictError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/ExceptionError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/ExceptionError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/ForbiddenError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/InternalError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/InternalError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/NotFoundError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/NotFoundError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/UnauthorizedError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Errors/ValidationError.py` & `on_rails-4.0.0/on_rails/ResultDetails/Errors/ValidationError.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Success/CreatedDetail.py` & `on_rails-4.0.0/on_rails/ResultDetails/Success/CreatedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py` & `on_rails-4.0.0/on_rails/ResultDetails/Success/NotModifiedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py` & `on_rails-4.0.0/on_rails/ResultDetails/Success/PartialContentDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/ResultDetails/SuccessDetail.py` & `on_rails-4.0.0/on_rails/ResultDetails/SuccessDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-3.1.0/on_rails/_utility.py` & `on_rails-4.0.0/on_rails/_utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import asyncio
 import inspect
 from asyncio import AbstractEventLoop
-from typing import Any, Coroutine, List
+from typing import Any, Callable, Coroutine, List
 
 from on_rails.ResultDetails.ErrorDetail import ErrorDetail
 
 
-def get_num_of_function_parameters(func: callable) -> int:
+def get_num_of_function_parameters(func: Callable) -> int:
     """
     Returns the number of parameters of a given function.
 
     :param func: The `func` is a function object for which we want to determine the number of parameters it
     takes
     :return: Returns the number of parameters that the function takes.
     """
-    return len(inspect.signature(func).parameters)
+    try:
+        return len(inspect.signature(func).parameters)
+    except ValueError:
+        return func.__code__.co_argcount
 
 
-def is_async(func: callable):
+def is_async(func: Callable):
     """
     The function checks if a given function is a coroutine function
 
     :param func: func is a parameter that represents a function. If the function is a coroutine function
     :return: Returns a boolean value indicating whether the
     function is a coroutine function or not. If the argument is not a function, it returns `False`.
     """
```

### Comparing `on_rails-3.1.0/on_rails/test_helpers.py` & `on_rails-4.0.0/on_rails/test_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 from on_rails.Result import Result
 from on_rails.ResultDetail import ResultDetail
 from on_rails.ResultDetails.ErrorDetail import ErrorDetail
 
 
 def assert_result(test_class: unittest.TestCase, target_result: Result, expected_success: bool,
-                  expected_detail: Optional[ResultDetail] = None, expected_value: Optional[Any] = None) -> None:
+                  expected_detail: Optional[ResultDetail] = None, expected_value: Optional[Any] = None,
+                  print_detail_if_failed=True) -> None:
     """
     This function asserts that the given result matches the expected success, detail, and value.
 
     :param test_class: The test class that is calling this function. This is typically a subclass of
     unittest.TestCase
     :type test_class: unittest.TestCase
 
@@ -25,17 +26,18 @@
 
     :param expected_detail: The expected value of `detail`. It will check with `result.detail`
     :type expected_detail: Optional[ResultDetail]
 
     :param expected_value: The expected value of `value`. It will check with `result.value`
     :type expected_value: Optional[Any]
     """
-    test_class.assertEqual(expected_success, target_result.success, msg="success")
-    test_class.assertEqual(expected_detail, target_result.detail, msg="detail")
+    test_class.assertEqual(expected_success, target_result.success,
+                           msg=f"success {target_result if print_detail_if_failed else ''}")
     test_class.assertEqual(expected_value, target_result.value, msg="value")
+    test_class.assertEqual(expected_detail, target_result.detail, msg="detail")
 
 
 def assert_result_with_type(test_class: unittest.TestCase, target_result: Result, expected_success: bool,
                             expected_detail_type=None, expected_value: Optional[Any] = None) -> None:
     """
     This function asserts the success, detail type, and value of a given result object.
 
@@ -53,14 +55,15 @@
 
     :param expected_detail_type: The `detail_type` parameter is an optional argument that
     specifies the expected type of the `detail`
 
     :param expected_value: The expected value of `value`. It will check with `result.value`
     :type expected_value: Optional[Any]
     """
+    test_class.assertTrue(isinstance(target_result, Result), msg="Target must be an instance of Result")
     test_class.assertEqual(expected_success, target_result.success, msg="success")
     test_class.assertTrue(isinstance(target_result.detail, expected_detail_type), msg="detail type")
     test_class.assertEqual(expected_value, target_result.value, msg="value")
 
 
 def assert_result_detail(test_class: unittest.TestCase, target_result_detail: ResultDetail, expected_title: str,
                          expected_message: Optional[str] = None, expected_code: Optional[int] = None,
@@ -85,14 +88,16 @@
     :type expected_code: Optional[int]
 
     :param expected_more_data: The expected value of `more_data`. It will check with `result_detail.more_data
     :type expected_more_data: Optional[List[Any]]
     """
     if expected_more_data is None:
         expected_more_data = []
+    test_class.assertTrue(isinstance(target_result_detail, ResultDetail),
+                          msg="Target must be an instance of ResultDetail")
     test_class.assertEqual(expected_title, target_result_detail.title, msg="title")
     test_class.assertEqual(expected_message, target_result_detail.message, msg="message")
     test_class.assertEqual(expected_code, target_result_detail.code, msg="code")
 
     test_class.assertIsNotNone(target_result_detail.more_data, msg="more data")  # It should never be None.
     test_class.assertEqual(expected_more_data, target_result_detail.more_data, msg="more data")
 
@@ -129,14 +134,16 @@
     :type expected_errors: Optional[Dict[str, str]]
 
     :param expected_exception: The expected exception that should be present in the error detail
     :type expected_exception: Optional[Exception]
     """
     if expected_more_data is None:
         expected_more_data = []
+    test_class.assertTrue(isinstance(target_error_detail, ErrorDetail),
+                          msg=f"Target ({type(target_error_detail).__name__}) must be an instance of ErrorDetail")
     assert_result_detail(test_class=test_class, target_result_detail=target_error_detail,
                          expected_title=expected_title, expected_message=expected_message, expected_code=expected_code,
                          expected_more_data=expected_more_data)
     test_class.assertEqual(expected_errors, target_error_detail.errors, msg="errors")
     test_class.assertEqual(expected_exception, target_error_detail.exception, msg="exception")
 
     test_class.assertTrue(target_error_detail.stack_trace, msg="stack trace")
```

### Comparing `on_rails-3.1.0/pyproject.toml` & `on_rails-4.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "on_rails"
-version = "3.1.0"
+version = "4.0.0"
 description = "Simple and powerful Railway Oriented library for python"
 authors = ["Payadel <payadelteam@gmail.com>"]
 readme = "README.md"
 license = "GPLV3"
 repository = "https://github.com/Payadel/on_rails"
 keywords = ["railway oriented","functional programming", "error handling"]
 packages = [{ include = "on_rails" }]
```

### Comparing `on_rails-3.1.0/PKG-INFO` & `on_rails-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: on-rails
-Version: 3.1.0
+Version: 4.0.0
 Summary: Simple and powerful Railway Oriented library for python
 Home-page: https://github.com/Payadel/on_rails
 License: GPLV3
 Keywords: railway oriented,functional programming,error handling
 Author: Payadel
 Author-email: payadelteam@gmail.com
 Requires-Python: >=3.10,<4.0
```

