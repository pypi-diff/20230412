# Comparing `tmp/djackal-0.4.1.tar.gz` & `tmp/djackal-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djackal-0.4.1.tar", max compression
+gzip compressed data, was "djackal-0.5.0.tar", max compression
```

## Comparing `djackal-0.4.1.tar` & `djackal-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1068 2021-04-27 09:26:04.461893 djackal-0.4.1/LICENSE
--rw-r--r--   0        0        0      484 2022-01-14 07:38:42.023715 djackal-0.4.1/README.md
--rw-r--r--   0        0        0        0 2021-04-27 10:13:03.376108 djackal-0.4.1/djackal/__init__.py
--rw-r--r--   0        0        0      118 2021-04-28 13:22:14.818993 djackal-0.4.1/djackal/apps.py
--rw-r--r--   0        0        0      541 2021-11-23 06:18:24.021837 djackal-0.4.1/djackal/erra.py
--rw-r--r--   0        0        0     2614 2022-04-16 11:25:48.492286 djackal-0.4.1/djackal/exceptions.py
--rw-r--r--   0        0        0      227 2021-02-25 12:42:37.423177 djackal-0.4.1/djackal/expressions.py
--rw-r--r--   0        0        0       34 2021-04-29 09:48:08.913022 djackal-0.4.1/djackal/fields/__init__.py
--rw-r--r--   0        0        0     2116 2021-04-29 09:48:08.917022 djackal-0.4.1/djackal/fields/json_field.py
--rw-r--r--   0        0        0      655 2022-06-01 07:29:57.471726 djackal-0.4.1/djackal/filters.py
--rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.345990 djackal-0.4.1/djackal/initializer.py
--rw-r--r--   0        0        0      161 2022-06-01 07:29:57.471726 djackal-0.4.1/djackal/loaders.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.4.1/djackal/management/__init__.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.4.1/djackal/management/commands/__init__.py
--rw-r--r--   0        0        0      370 2021-06-17 15:10:32.349990 djackal-0.4.1/djackal/management/commands/init.py
--rw-r--r--   0        0        0       36 2023-02-01 05:48:44.579388 djackal-0.4.1/djackal/model_mixins/__init__.py
--rw-r--r--   0        0        0     1222 2023-01-30 07:23:30.657224 djackal-0.4.1/djackal/model_mixins/extra_mixin.py
--rw-r--r--   0        0        0     2243 2022-06-01 07:29:57.471726 djackal-0.4.1/djackal/pagination.py
--rw-r--r--   0        0        0     2699 2022-04-16 11:25:48.492286 djackal-0.4.1/djackal/permissions.py
--rw-r--r--   0        0        0     1606 2021-06-28 06:44:58.185826 djackal-0.4.1/djackal/serializers.py
--rw-r--r--   0        0        0     3106 2023-02-13 09:29:41.681975 djackal-0.4.1/djackal/settings.py
--rw-r--r--   0        0        0     1638 2022-06-01 07:29:57.471726 djackal-0.4.1/djackal/shortcuts.py
--rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.4.1/djackal/storage/__init__.py
--rw-r--r--   0        0        0      126 2021-06-17 15:10:32.349990 djackal-0.4.1/djackal/storage/apps.py
--rw-r--r--   0        0        0      404 2021-06-17 15:10:32.349990 djackal-0.4.1/djackal/storage/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.4.1/djackal/storage/migrations/__init__.py
--rw-r--r--   0        0        0      658 2021-06-17 15:10:32.349990 djackal-0.4.1/djackal/storage/models.py
--rw-r--r--   0        0        0      760 2022-06-01 07:29:12.961130 djackal-0.4.1/djackal/tests.py
--rw-r--r--   0        0        0      512 2021-04-28 14:13:50.279047 djackal-0.4.1/djackal/utils.py
--rw-r--r--   0        0        0       79 2021-04-27 10:23:21.074040 djackal-0.4.1/djackal/views/__init__.py
--rw-r--r--   0        0        0    13341 2023-03-14 09:52:36.978878 djackal-0.4.1/djackal/views/base.py
--rw-r--r--   0        0        0     3316 2021-04-28 14:02:19.921014 djackal-0.4.1/djackal/views/generics.py
--rw-r--r--   0        0        0      379 2021-12-15 14:11:54.023043 djackal-0.4.1/djackal/views/handler.py
--rw-r--r--   0        0        0     2217 2023-02-13 09:40:58.569400 djackal-0.4.1/djackal/views/mixins.py
--rw-r--r--   0        0        0      574 2023-03-14 09:53:18.886952 djackal-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.4.1/tests/model_mixins/__init__.py
--rw-r--r--   0        0        0     2360 2023-02-01 05:48:23.658496 djackal-0.4.1/tests/model_mixins/test_extra_mixin.py
--rw-r--r--   0        0        0      515 2021-04-27 10:01:21.653305 djackal-0.4.1/tests/models.py
--rw-r--r--   0        0        0      494 2022-06-01 07:29:57.471726 djackal-0.4.1/tests/settings.py
--rw-r--r--   0        0        0      770 2022-06-01 07:29:57.471726 djackal-0.4.1/tests/test_erra.py
--rw-r--r--   0        0        0     3665 2022-06-01 07:29:57.471726 djackal-0.4.1/tests/test_exceptions.py
--rw-r--r--   0        0        0      631 2021-04-29 09:49:02.876011 djackal-0.4.1/tests/test_fields.py
--rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.353990 djackal-0.4.1/tests/test_initializer.py
--rw-r--r--   0        0        0      260 2022-06-01 07:29:57.471726 djackal-0.4.1/tests/test_loaders.py
--rw-r--r--   0        0        0     4139 2023-01-05 11:28:45.245418 djackal-0.4.1/tests/test_query_filter.py
--rw-r--r--   0        0        0      871 2022-06-01 07:29:57.471726 djackal-0.4.1/tests/test_settings.py
--rw-r--r--   0        0        0     2808 2022-06-01 07:29:57.471726 djackal-0.4.1/tests/test_shortcuts.py
--rw-r--r--   0        0        0      924 2021-04-28 14:13:50.263048 djackal-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 djackal-0.4.1/setup.py
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 djackal-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-04-27 09:26:04.461893 djackal-0.5.0/LICENSE
+-rw-r--r--   0        0        0      484 2022-01-14 07:38:42.023715 djackal-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2021-04-27 10:13:03.376108 djackal-0.5.0/djackal/__init__.py
+-rw-r--r--   0        0        0      118 2021-04-28 13:22:14.818993 djackal-0.5.0/djackal/apps.py
+-rw-r--r--   0        0        0      541 2021-11-23 06:18:24.021837 djackal-0.5.0/djackal/erra.py
+-rw-r--r--   0        0        0     2614 2022-04-16 11:25:48.492286 djackal-0.5.0/djackal/exceptions.py
+-rw-r--r--   0        0        0      227 2021-02-25 12:42:37.423177 djackal-0.5.0/djackal/expressions.py
+-rw-r--r--   0        0        0       34 2021-04-29 09:48:08.913022 djackal-0.5.0/djackal/fields/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-12 16:24:40.909639 djackal-0.5.0/djackal/fields/json_field.py
+-rw-r--r--   0        0        0      655 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/filters.py
+-rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.345990 djackal-0.5.0/djackal/initializer.py
+-rw-r--r--   0        0        0      161 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/loaders.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.0/djackal/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.423177 djackal-0.5.0/djackal/management/commands/__init__.py
+-rw-r--r--   0        0        0      370 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/management/commands/init.py
+-rw-r--r--   0        0        0       36 2023-02-01 05:48:44.579388 djackal-0.5.0/djackal/model_mixins/__init__.py
+-rw-r--r--   0        0        0     1222 2023-01-30 07:23:30.657224 djackal-0.5.0/djackal/model_mixins/extra_mixin.py
+-rw-r--r--   0        0        0     2243 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/pagination.py
+-rw-r--r--   0        0        0     2699 2022-04-16 11:25:48.492286 djackal-0.5.0/djackal/permissions.py
+-rw-r--r--   0        0        0     1606 2021-06-28 06:44:58.185826 djackal-0.5.0/djackal/serializers.py
+-rw-r--r--   0        0        0     3106 2023-02-13 09:29:41.681975 djackal-0.5.0/djackal/settings.py
+-rw-r--r--   0        0        0     1638 2022-06-01 07:29:57.471726 djackal-0.5.0/djackal/shortcuts.py
+-rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/__init__.py
+-rw-r--r--   0        0        0      126 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/apps.py
+-rw-r--r--   0        0        0      404 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/migrations/__init__.py
+-rw-r--r--   0        0        0      658 2021-06-17 15:10:32.349990 djackal-0.5.0/djackal/storage/models.py
+-rw-r--r--   0        0        0      760 2022-06-01 07:29:12.961130 djackal-0.5.0/djackal/tests.py
+-rw-r--r--   0        0        0      512 2021-04-28 14:13:50.279047 djackal-0.5.0/djackal/utils.py
+-rw-r--r--   0        0        0       79 2021-04-27 10:23:21.074040 djackal-0.5.0/djackal/views/__init__.py
+-rw-r--r--   0        0        0    13636 2023-04-12 16:24:40.865637 djackal-0.5.0/djackal/views/base.py
+-rw-r--r--   0        0        0     3316 2021-04-28 14:02:19.921014 djackal-0.5.0/djackal/views/generics.py
+-rw-r--r--   0        0        0      379 2021-12-15 14:11:54.023043 djackal-0.5.0/djackal/views/handler.py
+-rw-r--r--   0        0        0     2217 2023-02-13 09:40:58.569400 djackal-0.5.0/djackal/views/mixins.py
+-rw-r--r--   0        0        0      574 2023-04-12 16:24:40.905638 djackal-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-25 12:42:37.427177 djackal-0.5.0/tests/model_mixins/__init__.py
+-rw-r--r--   0        0        0     2360 2023-02-01 05:48:23.658496 djackal-0.5.0/tests/model_mixins/test_extra_mixin.py
+-rw-r--r--   0        0        0      515 2021-04-27 10:01:21.653305 djackal-0.5.0/tests/models.py
+-rw-r--r--   0        0        0      494 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/settings.py
+-rw-r--r--   0        0        0      770 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_erra.py
+-rw-r--r--   0        0        0     3665 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0      631 2021-04-29 09:49:02.876011 djackal-0.5.0/tests/test_fields.py
+-rw-r--r--   0        0        0     1165 2021-06-17 15:10:32.353990 djackal-0.5.0/tests/test_initializer.py
+-rw-r--r--   0        0        0      260 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_loaders.py
+-rw-r--r--   0        0        0     4139 2023-01-05 11:28:45.245418 djackal-0.5.0/tests/test_query_filter.py
+-rw-r--r--   0        0        0      871 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_settings.py
+-rw-r--r--   0        0        0     2808 2022-06-01 07:29:57.471726 djackal-0.5.0/tests/test_shortcuts.py
+-rw-r--r--   0        0        0      924 2021-04-28 14:13:50.263048 djackal-0.5.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 djackal-0.5.0/setup.py
+-rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 djackal-0.5.0/PKG-INFO
```

### Comparing `djackal-0.4.1/LICENSE` & `djackal-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/erra.py` & `djackal-0.5.0/djackal/erra.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/exceptions.py` & `djackal-0.5.0/djackal/exceptions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/fields/json_field.py` & `djackal-0.5.0/djackal/fields/json_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 def dumps(value):
     return json.dumps(
         value,
         cls=DjangoJSONEncoder,
         sort_keys=True,
         indent=2,
-        separators=(',', ': ')
+        separators=(',', ': '),
+        ensure_ascii=False,
     )
 
 
 class JSONField(TextField):
     def __init__(self, *args, **kwargs):
         self.serializer = kwargs.pop('serializer', dumps)
         self.deserializer = kwargs.pop('deserializer', json.loads)
```

### Comparing `djackal-0.4.1/djackal/filters.py` & `djackal-0.5.0/djackal/filters.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/initializer.py` & `djackal-0.5.0/djackal/initializer.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/model_mixins/extra_mixin.py` & `djackal-0.5.0/djackal/model_mixins/extra_mixin.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/pagination.py` & `djackal-0.5.0/djackal/pagination.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/permissions.py` & `djackal-0.5.0/djackal/permissions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/serializers.py` & `djackal-0.5.0/djackal/serializers.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/settings.py` & `djackal-0.5.0/djackal/settings.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/shortcuts.py` & `djackal-0.5.0/djackal/shortcuts.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/storage/models.py` & `djackal-0.5.0/djackal/storage/models.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/tests.py` & `djackal-0.5.0/djackal/tests.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/utils.py` & `djackal-0.5.0/djackal/utils.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/views/base.py` & `djackal-0.5.0/djackal/views/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from djackal.exceptions import NotFound
 from djackal.filters import DefaultFilterFunc
 from djackal.settings import djackal_settings
 from djackal.shortcuts import gen_q
 from djackal.utils import value_mapper, isiter
 
 
-class FilterMixin:
+class QueryMixin:
     lookup_map = {}
     filter_map = {}
     search_map = {}
     extra_map = {}
     ordering_map = {}
 
     search_keyword_key = 'search_keyword'
@@ -53,35 +53,35 @@
     def get_ordering_map(self, **additional):
         d = self.ordering_map or dict()
         return {**d, **additional}
 
     def get_user_field(self):
         return self.user_field
 
-    def filter_by_lookup_map(self, queryset, lookup_map=None):
+    def query_by_lookup_map(self, queryset, lookup_map=None):
         if lookup_map is None:
             lookup_map = self.get_lookup_map()
 
         mapped = value_mapper(lookup_map, self.kwargs)
         return queryset.filter(**mapped)
 
-    def filter_by_user(self, queryset, user_field=None):
+    def query_by_user(self, queryset, user_field=None):
         if user_field is None:
             user_field = self.get_user_field()
 
         if not self.has_auth() or not user_field:
             return queryset
         return queryset.filter(**{user_field: self.request.user})
 
-    def filter_by_extra_map(self, queryset, extra_map=None):
+    def query_by_extra_map(self, queryset, extra_map=None):
         if extra_map is None:
             extra_map = self.get_extra_map()
         return queryset.filter(**extra_map)
 
-    def filter_by_filter_map(self, queryset, filter_map=None):
+    def query_by_filter_map(self, queryset, filter_map=None):
         params = self.request.query_params
         if filter_map is None:
             filter_map = self.get_filter_map()
 
         for map_key, map_value in filter_map.items():
             if map_key.endswith('[]') and hasattr(params, 'getlist'):
                 value = params.getlist(map_key)
@@ -92,43 +92,43 @@
 
             split_key = map_key.split(':')
             if len(split_key) == 2:
                 value = self.filter_func_action(split_key[1], value)
 
             if map_value.startswith(self.custom_action_prefix):
                 keyword = map_value.replace(self.custom_action_prefix, '')
-                queryset = self.filter_by_filter_action(queryset, keyword, value)
+                queryset = self.query_by_filter_action(queryset, keyword, value)
                 continue
             if isiter(map_value):
                 queryset = queryset.filter(*gen_q(value, *map_value))
             else:
                 queryset = queryset.filter(**{map_value: value})
         return queryset
 
-    def filter_by_search_map(self, queryset, search_map=None):
+    def query_by_search_map(self, queryset, search_map=None):
         if search_map is None:
             search_map = self.get_search_map()
 
         params = self.request.query_params
         search_type = params.get(self.search_type_key)
         search_keyword = params.get(self.search_keyword_key)
-        map_value = search_map.get(search_type)
+        map_value = search_map.get(search_type, 'all')
 
         if not search_keyword or not map_value:
             return queryset
 
         if map_value.startswith(self.custom_action_prefix):
             keyword = map_value.replace(self.custom_action_prefix, '')
-            return self.filter_by_search_action(queryset, keyword, search_keyword)
+            return self.query_by_search_action(queryset, keyword, search_keyword)
         if isiter(map_value):
             return queryset.filter(gen_q(search_keyword, *map_value))
         else:
             return queryset.filter(**{map_value: search_keyword})
 
-    def filter_by_ordering(self, queryset, order_map=None):
+    def query_by_ordering(self, queryset, order_map=None):
         if order_map is None:
             order_map = self.get_ordering_map()
 
         params = self.request.query_params
         param_value = params.get(self.ordering_key)
 
         if order_map is not None:
@@ -139,48 +139,48 @@
         if not order_value:
             if not self.ordering_default:
                 return queryset
             order_value = self.ordering_default
 
         if order_value.start_with(self.custom_action_prefix):
             keyword = order_value.replace(self.custom_action_prefix, '')
-            return self.filter_by_order_action(queryset, keyword)
+            return self.query_by_order_action(queryset, keyword)
 
         order_by = order_value.split(',')
         return queryset.order_by(*order_by)
 
-    def filter_by_filter_action(self, queryset, keyword, value):
+    def query_by_filter_action(self, queryset, keyword, value):
         return queryset
 
-    def filter_by_search_action(self, queryset, keyword, value):
+    def query_by_search_action(self, queryset, keyword, value):
         return queryset
 
-    def filter_by_order_action(self, queryset, keyword):
+    def query_by_order_action(self, queryset, keyword):
         return queryset
 
     def get_filtered_queryset(self, queryset=None):
         if queryset is None:
             queryset = self.get_queryset()
 
-        queryset = self.filter_by_user(queryset)
-        queryset = self.filter_by_lookup_map(queryset)
-        queryset = self.filter_by_extra_map(queryset)
-        queryset = self.filter_by_filter_map(queryset)
-        queryset = self.filter_by_search_map(queryset)
-        queryset = self.filter_by_ordering(queryset)
+        queryset = self.query_by_user(queryset)
+        queryset = self.query_by_lookup_map(queryset)
+        queryset = self.query_by_extra_map(queryset)
+        queryset = self.query_by_filter_map(queryset)
+        queryset = self.query_by_search_map(queryset)
+        queryset = self.query_by_ordering(queryset)
 
         return queryset
 
     def get_object(self, queryset=None):
         if queryset is None:
             queryset = self.get_queryset()
 
-        queryset = self.filter_by_user(queryset)
-        queryset = self.filter_by_lookup_map(queryset)
-        queryset = self.filter_by_extra_map(queryset)
+        queryset = self.query_by_user(queryset)
+        queryset = self.query_by_lookup_map(queryset)
+        queryset = self.query_by_extra_map(queryset)
 
         obj = queryset.first()
         if obj is None:
             raise NotFound(model=queryset.model)
         self.check_object_permissions(request=self.request, obj=obj)
         return obj
 
@@ -340,26 +340,36 @@
             response_data = result or dict()
 
         return Response(response_data, status=status, headers=headers, **kwargs)
 
 
 class DataPurifyMixin:
     data_schema = None
+    query_params_schema = None
 
     def get_purified_data(self, key=None, many=False):
         schema = self.get_data_schema(key)
         return purify(self.request.data, schema, many=many)
 
     def get_data_schema(self, key=None):
         if key in self.data_schema:
             return self.data_schema[key]
         return self.data_schema
 
+    def get_purified_query_params(self, key=None, many=False):
+        schema = self.get_query_params_schema(key)
+        return purify(self.request.query_params, schema, many=many)
 
-class DjackalAPIView(BaseDjackalAPIView, FilterMixin, PageMixin, DataPurifyMixin):
+    def get_query_params_schema(self, key=None):
+        if key in self.query_params_schema:
+            return self.query_params_schema[key]
+        return self.query_params_schema
+
+
+class DjackalAPIView(BaseDjackalAPIView, QueryMixin, PageMixin, DataPurifyMixin):
     model = None
     queryset = None
 
     bind_kwargs_map = {}
 
     serializer_class = None
 
@@ -380,17 +390,14 @@
         queryset = self.get_queryset()
         assert queryset is not None, (
             '{} should include a `model` or `queryset` attribute'
             'or override the get_model() method'.format(self.__class__.__name__)
         )
         return queryset.model
 
-    def get_request_data(self, key=None):
-        return self.get_purified_data(key)
-
     def get_serializer_class(self):
         return self.serializer_class
 
     def get_serializer_context(self, **kwargs):
         return kwargs
 
     def get_serializer(self, instance, context=None, many=False, klass=None):
```

### Comparing `djackal-0.4.1/djackal/views/generics.py` & `djackal-0.5.0/djackal/views/generics.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/djackal/views/mixins.py` & `djackal-0.5.0/djackal/views/mixins.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/pyproject.toml` & `djackal-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djackal"
-version = "0.4.1"
+version = "0.5.0"
 description = "extension of Django REST Framework"
 authors = ["jrog <jrog612@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/jrog612/djackal'
 homepage = 'https://github.com/jrog612/djackal'
 packages = [
```

### Comparing `djackal-0.4.1/tests/model_mixins/test_extra_mixin.py` & `djackal-0.5.0/tests/model_mixins/test_extra_mixin.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/models.py` & `djackal-0.5.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_erra.py` & `djackal-0.5.0/tests/test_erra.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_exceptions.py` & `djackal-0.5.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_fields.py` & `djackal-0.5.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_initializer.py` & `djackal-0.5.0/tests/test_initializer.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_query_filter.py` & `djackal-0.5.0/tests/test_query_filter.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_settings.py` & `djackal-0.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_shortcuts.py` & `djackal-0.5.0/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/tests/test_utils.py` & `djackal-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `djackal-0.4.1/setup.py` & `djackal-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['djangorestframework>=3.0.0,<4.0.0', 'puty>=0.0,<0.1']
 
 setup_kwargs = {
     'name': 'djackal',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'extension of Django REST Framework',
     'long_description': '# Djackal, Django Rest Framework extension\n\n[![version badge](https://badge.fury.io/py/djackal.svg)](https://badge.fury.io/py/djackal)\n\n![djackal image](https://imgur.com/XnlU8T9.jpg)\n\n**Djackal** is extension of Django REST Framework(DRF)\nthat help you easily implement the necessary features on your web backend server.\n\n\n## Warning\n\nThis repository is on developing. Some bugs may exist, possible to change suddenly. And no document yet.\n\n\n## Installation\n\n    pip install djackal\n',
     'author': 'jrog',
     'author_email': 'jrog612@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jrog612/djackal',
```

### Comparing `djackal-0.4.1/PKG-INFO` & `djackal-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djackal
-Version: 0.4.1
+Version: 0.5.0
 Summary: extension of Django REST Framework
 Home-page: https://github.com/jrog612/djackal
 License: MIT
 Author: jrog
 Author-email: jrog612@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

