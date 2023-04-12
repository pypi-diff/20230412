# Comparing `tmp/djackal-0.5.0.tar.gz` & `tmp/djackal-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djackal-0.5.0.tar", max compression
+gzip compressed data, was "djackal-0.5.3.tar", max compression
```

## Comparing `djackal-0.5.0.tar` & `djackal-0.5.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1068 2021-04-27 09:26:04.461893 djackal-0.5.0/LICENSE
--rw-r--r--   0        0        0      484 2022-01-14 07:38:42.023715 djackal-0.5.0/README.md
--rw-r--r--   0        0        0        0 2021-04-27 10:13:03.376108 djackal-0.5.0/djackal/__init__.py
--rw-r--r--   0        0        0      118 2021-04-28 13:22:14.818993 djackal-0.5.0/djackal/apps.py
--rw-r--r--   0        0        0      541 2021-11-23 06:18:24.021837 djackal-0.5.0/djackal/erra.py
--rw-r--r--   0        0        0     2614 2022-04-16 11:25:48.492286 djackal-0.5.0/djackal/exceptions.py
--rw-r--r--   0        0        0      227 2021-02-25 12:42:37.423177 djackal-0.5.0/djackal/expressions.py
--rw-r--r--   0        0        0       34 2021-04-29 09:48:08.913022 djackal-0.5.0/djackal/fields/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-12 16:24:40.909639 djackal-0.5.0/djackal/fields/json_field.py
--rw-r--r--   0        0        0      655 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/filters.py
--rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.345990 djackal-0.5.0/djackal/initializer.py
--rw-r--r--   0        0        0      161 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/loaders.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.0/djackal/management/__init__.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.0/djackal/management/commands/__init__.py
--rw-r--r--   0        0        0      370 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/management/commands/init.py
--rw-r--r--   0        0        0       36 2023-02-01 05:48:44.579388 djackal-0.5.0/djackal/model_mixins/__init__.py
--rw-r--r--   0        0        0     1222 2023-01-30 07:23:30.657224 djackal-0.5.0/djackal/model_mixins/extra_mixin.py
--rw-r--r--   0        0        0     2243 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/pagination.py
--rw-r--r--   0        0        0     2699 2022-04-16 11:25:48.492286 djackal-0.5.0/djackal/permissions.py
--rw-r--r--   0        0        0     1606 2021-06-28 06:44:58.185826 djackal-0.5.0/djackal/serializers.py
--rw-r--r--   0        0        0     3106 2023-02-13 09:29:41.681975 djackal-0.5.0/djackal/settings.py
--rw-r--r--   0        0        0     1638 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/shortcuts.py
--rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/__init__.py
--rw-r--r--   0        0        0      126 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/apps.py
--rw-r--r--   0        0        0      404 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/migrations/__init__.py
--rw-r--r--   0        0        0      658 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/models.py
--rw-r--r--   0        0        0      760 2022-06-01 07:29:12.961130 djackal-0.5.0/djackal/tests.py
--rw-r--r--   0        0        0      512 2021-04-28 14:13:50.279047 djackal-0.5.0/djackal/utils.py
--rw-r--r--   0        0        0       79 2021-04-27 10:23:21.074040 djackal-0.5.0/djackal/views/__init__.py
--rw-r--r--   0        0        0    13636 2023-04-12 16:24:40.865637 djackal-0.5.0/djackal/views/base.py
--rw-r--r--   0        0        0     3316 2021-04-28 14:02:19.921014 djackal-0.5.0/djackal/views/generics.py
--rw-r--r--   0        0        0      379 2021-12-15 14:11:54.023043 djackal-0.5.0/djackal/views/handler.py
--rw-r--r--   0        0        0     2217 2023-02-13 09:40:58.569400 djackal-0.5.0/djackal/views/mixins.py
--rw-r--r--   0        0        0      574 2023-04-12 16:24:40.905638 djackal-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.0/tests/model_mixins/__init__.py
--rw-r--r--   0        0        0     2360 2023-02-01 05:48:23.658496 djackal-0.5.0/tests/model_mixins/test_extra_mixin.py
--rw-r--r--   0        0        0      515 2021-04-27 10:01:21.653305 djackal-0.5.0/tests/models.py
--rw-r--r--   0        0        0      494 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/settings.py
--rw-r--r--   0        0        0      770 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_erra.py
--rw-r--r--   0        0        0     3665 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_exceptions.py
--rw-r--r--   0        0        0      631 2021-04-29 09:49:02.876011 djackal-0.5.0/tests/test_fields.py
--rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.353990 djackal-0.5.0/tests/test_initializer.py
--rw-r--r--   0        0        0      260 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_loaders.py
--rw-r--r--   0        0        0     4139 2023-01-05 11:28:45.245418 djackal-0.5.0/tests/test_query_filter.py
--rw-r--r--   0        0        0      871 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_settings.py
--rw-r--r--   0        0        0     2808 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_shortcuts.py
--rw-r--r--   0        0        0      924 2021-04-28 14:13:50.263048 djackal-0.5.0/tests/test_utils.py
--rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 djackal-0.5.0/setup.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 djackal-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-04-27 09:26:04.461893 djackal-0.5.3/LICENSE
+-rw-r--r--   0        0        0      484 2022-01-14 07:38:42.023715 djackal-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2021-04-27 10:13:03.376108 djackal-0.5.3/djackal/__init__.py
+-rw-r--r--   0        0        0      118 2021-04-28 13:22:14.818993 djackal-0.5.3/djackal/apps.py
+-rw-r--r--   0        0        0      541 2021-11-23 06:18:24.021837 djackal-0.5.3/djackal/erra.py
+-rw-r--r--   0        0        0     2614 2022-04-16 11:25:48.492286 djackal-0.5.3/djackal/exceptions.py
+-rw-r--r--   0        0        0      227 2021-02-25 12:42:37.423177 djackal-0.5.3/djackal/expressions.py
+-rw-r--r--   0        0        0       34 2021-04-29 09:48:08.913022 djackal-0.5.3/djackal/fields/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-12 16:24:40.909639 djackal-0.5.3/djackal/fields/json_field.py
+-rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.345990 djackal-0.5.3/djackal/initializer.py
+-rw-r--r--   0        0        0      161 2022-06-01 07:29:57.471726 djackal-0.5.3/djackal/loaders.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.3/djackal/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.3/djackal/management/commands/__init__.py
+-rw-r--r--   0        0        0      370 2021-06-17 15:10:32.349990 djackal-0.5.3/djackal/management/commands/init.py
+-rw-r--r--   0        0        0       36 2023-02-01 05:48:44.579388 djackal-0.5.3/djackal/model_mixins/__init__.py
+-rw-r--r--   0        0        0     1222 2023-01-30 07:23:30.657224 djackal-0.5.3/djackal/model_mixins/extra_mixin.py
+-rw-r--r--   0        0        0     2243 2022-06-01 07:29:57.471726 djackal-0.5.3/djackal/pagination.py
+-rw-r--r--   0        0        0     2699 2022-04-16 11:25:48.492286 djackal-0.5.3/djackal/permissions.py
+-rw-r--r--   0        0        0     2785 2023-04-12 18:33:20.643759 djackal-0.5.3/djackal/query_filter.py
+-rw-r--r--   0        0        0     1606 2021-06-28 06:44:58.185826 djackal-0.5.3/djackal/serializers.py
+-rw-r--r--   0        0        0     2953 2023-04-12 18:33:08.143971 djackal-0.5.3/djackal/settings.py
+-rw-r--r--   0        0        0     1638 2022-06-01 07:29:57.471726 djackal-0.5.3/djackal/shortcuts.py
+-rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.3/djackal/storage/__init__.py
+-rw-r--r--   0        0        0      126 2021-06-17 15:10:32.349990 djackal-0.5.3/djackal/storage/apps.py
+-rw-r--r--   0        0        0      404 2021-06-17 15:10:32.349990 djackal-0.5.3/djackal/storage/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.3/djackal/storage/migrations/__init__.py
+-rw-r--r--   0        0        0      658 2021-06-17 15:10:32.349990 djackal-0.5.3/djackal/storage/models.py
+-rw-r--r--   0        0        0      760 2022-06-01 07:29:12.961130 djackal-0.5.3/djackal/tests.py
+-rw-r--r--   0        0        0      751 2023-04-12 17:11:13.292868 djackal-0.5.3/djackal/utils.py
+-rw-r--r--   0        0        0       79 2021-04-27 10:23:21.074040 djackal-0.5.3/djackal/views/__init__.py
+-rw-r--r--   0        0        0    11194 2023-04-12 18:28:58.288679 djackal-0.5.3/djackal/views/base.py
+-rw-r--r--   0        0        0     3316 2021-04-28 14:02:19.921014 djackal-0.5.3/djackal/views/generics.py
+-rw-r--r--   0        0        0      379 2021-12-15 14:11:54.023043 djackal-0.5.3/djackal/views/handler.py
+-rw-r--r--   0        0        0     2217 2023-02-13 09:40:58.569400 djackal-0.5.3/djackal/views/mixins.py
+-rw-r--r--   0        0        0      574 2023-04-12 19:03:26.047283 djackal-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.3/tests/model_mixins/__init__.py
+-rw-r--r--   0        0        0     2360 2023-02-01 05:48:23.658496 djackal-0.5.3/tests/model_mixins/test_extra_mixin.py
+-rw-r--r--   0        0        0      515 2021-04-27 10:01:21.653305 djackal-0.5.3/tests/models.py
+-rw-r--r--   0        0        0      494 2022-06-01 07:29:57.471726 djackal-0.5.3/tests/settings.py
+-rw-r--r--   0        0        0      770 2022-06-01 07:29:57.471726 djackal-0.5.3/tests/test_erra.py
+-rw-r--r--   0        0        0     3665 2022-06-01 07:29:57.471726 djackal-0.5.3/tests/test_exceptions.py
+-rw-r--r--   0        0        0      631 2021-04-29 09:49:02.876011 djackal-0.5.3/tests/test_fields.py
+-rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.353990 djackal-0.5.3/tests/test_initializer.py
+-rw-r--r--   0        0        0      260 2022-06-01 07:29:57.471726 djackal-0.5.3/tests/test_loaders.py
+-rw-r--r--   0        0        0     4139 2023-01-05 11:28:45.245418 djackal-0.5.3/tests/test_query_filter.py
+-rw-r--r--   0        0        0      899 2023-04-12 18:32:31.632601 djackal-0.5.3/tests/test_settings.py
+-rw-r--r--   0        0        0     2808 2022-06-01 07:29:57.471726 djackal-0.5.3/tests/test_shortcuts.py
+-rw-r--r--   0        0        0     1365 2023-04-12 17:11:32.692297 djackal-0.5.3/tests/test_utils.py
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 djackal-0.5.3/setup.py
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 djackal-0.5.3/PKG-INFO
```

### Comparing `djackal-0.5.0/LICENSE` & `djackal-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/erra.py` & `djackal-0.5.3/djackal/erra.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/exceptions.py` & `djackal-0.5.3/djackal/exceptions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/fields/json_field.py` & `djackal-0.5.3/djackal/fields/json_field.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/initializer.py` & `djackal-0.5.3/djackal/initializer.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/model_mixins/extra_mixin.py` & `djackal-0.5.3/djackal/model_mixins/extra_mixin.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/pagination.py` & `djackal-0.5.3/djackal/pagination.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/permissions.py` & `djackal-0.5.3/djackal/permissions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/serializers.py` & `djackal-0.5.3/djackal/serializers.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/settings.py` & `djackal-0.5.3/djackal/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from importlib import import_module
 
 from django.conf import settings
 from django.test.signals import setting_changed
 
-default_param_func = 'djackal.param_funcs.DefaultParamFunc'
-
 DEFAULTS = {
     'PAGE_SIZE': 10,
     'MAX_PAGE_SIZE': 100,
 
     'DEFAULT_PAGINATION_CLASS': 'djackal.pagination.PageNumberPagination',
 
     'EXCEPTION_HANDLER': 'djackal.views.handler.exception_handler',
 
     'DEFAULT_NONE_VALUES': ([], {}, '', None),
 
     'INITIALIZER': None,
 
-    'PARAM_FUNC_CLASSES': [
-        default_param_func,
-    ],
-
     'SINGLE_APP': False,
     'SINGLE_APP_NAME': None,
 }
 
 IMPORT_STRINGS = [
-    'PARAM_FUNC_CLASSES',
-
     'DEFAULT_PAGINATION_CLASS',
-
     'EXCEPTION_HANDLER',
 ]
 
 
 class DjackalSettings:
     def __init__(self, custom_settings=None, defaults=None, import_strings=None):
         if custom_settings:
```

### Comparing `djackal-0.5.0/djackal/shortcuts.py` & `djackal-0.5.3/djackal/shortcuts.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/storage/models.py` & `djackal-0.5.3/djackal/storage/models.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/tests.py` & `djackal-0.5.3/djackal/tests.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/views/base.py` & `djackal-0.5.3/djackal/views/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,36 @@
 from puty import purify
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
+from djackal import query_filter
 from djackal.exceptions import NotFound
-from djackal.filters import DefaultFilterFunc
 from djackal.settings import djackal_settings
-from djackal.shortcuts import gen_q
-from djackal.utils import value_mapper, isiter
+from djackal.utils import value_mapper
 
 
 class QueryMixin:
     lookup_map = {}
-    filter_map = {}
-    search_map = {}
     extra_map = {}
     ordering_map = {}
 
-    search_keyword_key = 'search_keyword'
-    search_type_key = 'search_type'
     ordering_key = 'ordering'
     ordering_default = None
 
-    custom_action_prefix = '@'
+    filter_schema = {}
 
     user_field = None
     bind_user_field = None
-    filter_func_class = DefaultFilterFunc
-
-    def get_filter_func_instance(self):
-        return self.filter_func_class()
-
-    def filter_func_action(self, name, value):
-        instance = self.get_filter_func_instance()
-        return instance.action(name, value)
 
     def get_lookup_map(self, **additional):
         d = self.lookup_map or dict()
         return {**d, **additional}
 
-    def get_filter_map(self, **additional):
-        d = self.filter_map or dict()
-        return {**d, **additional}
-
-    def get_search_map(self, **additional):
-        d = self.search_map or dict()
+    def get_filter_schema(self, **additional):
+        d = self.filter_schema or dict()
         return {**d, **additional}
 
     def get_extra_map(self, **additional):
         d = self.extra_map or dict()
         return {**d, **additional}
 
     def get_ordering_map(self, **additional):
@@ -73,103 +56,49 @@
         return queryset.filter(**{user_field: self.request.user})
 
     def query_by_extra_map(self, queryset, extra_map=None):
         if extra_map is None:
             extra_map = self.get_extra_map()
         return queryset.filter(**extra_map)
 
-    def query_by_filter_map(self, queryset, filter_map=None):
-        params = self.request.query_params
-        if filter_map is None:
-            filter_map = self.get_filter_map()
-
-        for map_key, map_value in filter_map.items():
-            if map_key.endswith('[]') and hasattr(params, 'getlist'):
-                value = params.getlist(map_key)
-            else:
-                value = params.get(map_key)
-            if value in [None, '', []]:
-                continue
-
-            split_key = map_key.split(':')
-            if len(split_key) == 2:
-                value = self.filter_func_action(split_key[1], value)
-
-            if map_value.startswith(self.custom_action_prefix):
-                keyword = map_value.replace(self.custom_action_prefix, '')
-                queryset = self.query_by_filter_action(queryset, keyword, value)
-                continue
-            if isiter(map_value):
-                queryset = queryset.filter(*gen_q(value, *map_value))
-            else:
-                queryset = queryset.filter(**{map_value: value})
-        return queryset
+    def query_by_filter_schema(self, queryset, filter_schema=None):
+        params = self.get_query_params_dict()
+        if filter_schema is None:
+            filter_schema = self.get_filter_schema()
 
-    def query_by_search_map(self, queryset, search_map=None):
-        if search_map is None:
-            search_map = self.get_search_map()
-
-        params = self.request.query_params
-        search_type = params.get(self.search_type_key)
-        search_keyword = params.get(self.search_keyword_key)
-        map_value = search_map.get(search_type, 'all')
-
-        if not search_keyword or not map_value:
-            return queryset
-
-        if map_value.startswith(self.custom_action_prefix):
-            keyword = map_value.replace(self.custom_action_prefix, '')
-            return self.query_by_search_action(queryset, keyword, search_keyword)
-        if isiter(map_value):
-            return queryset.filter(gen_q(search_keyword, *map_value))
-        else:
-            return queryset.filter(**{map_value: search_keyword})
+        return query_filter.filtering(queryset, params, filter_schema)
 
     def query_by_ordering(self, queryset, order_map=None):
         if order_map is None:
             order_map = self.get_ordering_map()
 
-        params = self.request.query_params
+        params = self.get_query_params_dict()
         param_value = params.get(self.ordering_key)
 
         if order_map is not None:
             order_value = order_map.get(param_value)
         else:
             order_value = param_value
 
         if not order_value:
             if not self.ordering_default:
                 return queryset
             order_value = self.ordering_default
 
-        if order_value.start_with(self.custom_action_prefix):
-            keyword = order_value.replace(self.custom_action_prefix, '')
-            return self.query_by_order_action(queryset, keyword)
-
         order_by = order_value.split(',')
         return queryset.order_by(*order_by)
 
-    def query_by_filter_action(self, queryset, keyword, value):
-        return queryset
-
-    def query_by_search_action(self, queryset, keyword, value):
-        return queryset
-
-    def query_by_order_action(self, queryset, keyword):
-        return queryset
-
     def get_filtered_queryset(self, queryset=None):
         if queryset is None:
             queryset = self.get_queryset()
 
         queryset = self.query_by_user(queryset)
         queryset = self.query_by_lookup_map(queryset)
         queryset = self.query_by_extra_map(queryset)
-        queryset = self.query_by_filter_map(queryset)
-        queryset = self.query_by_search_map(queryset)
+        queryset = self.query_by_filter_schema(queryset)
         queryset = self.query_by_ordering(queryset)
 
         return queryset
 
     def get_object(self, queryset=None):
         if queryset is None:
             queryset = self.get_queryset()
@@ -206,14 +135,37 @@
             return None
         return self.paginator.paginate_queryset(queryset, self.request, view=self)
 
     def get_paginated_meta(self):
         return self.paginator.get_paginated_meta()
 
 
+class DataPurifyMixin:
+    data_schema = None
+    query_params_schema = None
+
+    def get_purified_data(self, key=None, many=False):
+        schema = self.get_data_schema(key)
+        return purify(self.request.data, schema, many=many)
+
+    def get_data_schema(self, key=None):
+        if key in self.data_schema:
+            return self.data_schema[key]
+        return self.data_schema
+
+    def get_purified_query_params(self, key=None, many=False):
+        schema = self.get_query_params_schema(key)
+        return purify(self.get_query_params_dict(), schema, many=many)
+
+    def get_query_params_schema(self, key=None):
+        if key in self.query_params_schema:
+            return self.query_params_schema[key]
+        return self.query_params_schema
+
+
 class BaseDjackalAPIView(APIView):
     default_permission_classes = ()
     default_authentication_classes = ()
 
     result_root = 'result'
     result_meta = 'meta'
 
@@ -288,28 +240,29 @@
         self.kwargs = kwargs
         request = self.initialize_request(request, *args, **kwargs)
         self.request = request
         self.headers = self.default_response_headers
 
         try:
             self.initial(request, *args, **kwargs)
+
             if request.method.lower() in self.http_method_names:
                 handler = getattr(self, request.method.lower(),
                                   self.http_method_not_allowed)
             else:
                 handler = self.http_method_not_allowed
+
             self.pre_method_call(request, *args, **kwargs)
             response = handler(request, *args, **kwargs)
             self.post_method_call(request, response, *args, **kwargs)
 
         except Exception as exc:
             response = self.handle_exception(exc)
 
         self.response = self.finalize_response(request, response, *args, **kwargs)
-
         return self.response
 
     def handle_exception(self, exc):
         """
         high jacking exception and handle with default_exception_handler
         """
         self.pre_handle_exception(exc)
@@ -324,51 +277,37 @@
 
     def has_auth(self):
         return self.request.user is not None and self.request.user.is_authenticated
 
     def get_meta(self, **kwargs):
         return kwargs
 
+    def get_query_params_dict(self):
+        result = {}
+        for key, value in self.request.query_params.lists():
+            if len(value) == 1:
+                result[key] = value[0]
+            else:
+                result[key] = value
+        return result
+
     def simple_response(self, result=None, status=200, meta=None, headers=None, **kwargs):
         response_data = {}
 
         if self.result_root:
             response_data[self.result_root] = result
             if self.result_meta:
                 meta = self.get_meta(**(meta or dict()))
                 response_data[self.result_meta] = meta
         else:
             response_data = result or dict()
 
         return Response(response_data, status=status, headers=headers, **kwargs)
 
 
-class DataPurifyMixin:
-    data_schema = None
-    query_params_schema = None
-
-    def get_purified_data(self, key=None, many=False):
-        schema = self.get_data_schema(key)
-        return purify(self.request.data, schema, many=many)
-
-    def get_data_schema(self, key=None):
-        if key in self.data_schema:
-            return self.data_schema[key]
-        return self.data_schema
-
-    def get_purified_query_params(self, key=None, many=False):
-        schema = self.get_query_params_schema(key)
-        return purify(self.request.query_params, schema, many=many)
-
-    def get_query_params_schema(self, key=None):
-        if key in self.query_params_schema:
-            return self.query_params_schema[key]
-        return self.query_params_schema
-
-
 class DjackalAPIView(BaseDjackalAPIView, QueryMixin, PageMixin, DataPurifyMixin):
     model = None
     queryset = None
 
     bind_kwargs_map = {}
 
     serializer_class = None
```

### Comparing `djackal-0.5.0/djackal/views/generics.py` & `djackal-0.5.3/djackal/views/generics.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/djackal/views/mixins.py` & `djackal-0.5.3/djackal/views/mixins.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/pyproject.toml` & `djackal-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djackal"
-version = "0.5.0"
+version = "0.5.3"
 description = "extension of Django REST Framework"
 authors = ["jrog <jrog612@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/jrog612/djackal'
 homepage = 'https://github.com/jrog612/djackal'
 packages = [
```

### Comparing `djackal-0.5.0/tests/model_mixins/test_extra_mixin.py` & `djackal-0.5.3/tests/model_mixins/test_extra_mixin.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/models.py` & `djackal-0.5.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/test_erra.py` & `djackal-0.5.3/tests/test_erra.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/test_exceptions.py` & `djackal-0.5.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/test_fields.py` & `djackal-0.5.3/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/test_initializer.py` & `djackal-0.5.3/tests/test_initializer.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/test_query_filter.py` & `djackal-0.5.3/tests/test_query_filter.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/tests/test_shortcuts.py` & `djackal-0.5.3/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `djackal-0.5.0/setup.py` & `djackal-0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['djangorestframework>=3.0.0,<4.0.0', 'puty>=0.0,<0.1']
 
 setup_kwargs = {
     'name': 'djackal',
-    'version': '0.5.0',
+    'version': '0.5.3',
     'description': 'extension of Django REST Framework',
     'long_description': '# Djackal, Django Rest Framework extension\n\n[![version badge](https://badge.fury.io/py/djackal.svg)](https://badge.fury.io/py/djackal)\n\n![djackal image](https://imgur.com/XnlU8T9.jpg)\n\n**Djackal** is extension of Django REST Framework(DRF)\nthat help you easily implement the necessary features on your web backend server.\n\n\n## Warning\n\nThis repository is on developing. Some bugs may exist, possible to change suddenly. And no document yet.\n\n\n## Installation\n\n    pip install djackal\n',
     'author': 'jrog',
     'author_email': 'jrog612@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jrog612/djackal',
```

### Comparing `djackal-0.5.0/PKG-INFO` & `djackal-0.5.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djackal
-Version: 0.5.0
+Version: 0.5.3
 Summary: extension of Django REST Framework
 Home-page: https://github.com/jrog612/djackal
 License: MIT
 Author: jrog
 Author-email: jrog612@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

