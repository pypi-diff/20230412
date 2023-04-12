# Comparing `tmp/fyle-accounting-mappings-1.8.0.tar.gz` & `tmp/fyle-accounting-mappings-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyle-accounting-mappings-1.8.0.tar", last modified: Wed Mar 23 11:48:51 2022, max compression
+gzip compressed data, was "fyle-accounting-mappings-1.9.0.tar", last modified: Thu Mar 24 10:59:08 2022, max compression
```

## Comparing `fyle-accounting-mappings-1.8.0.tar` & `fyle-accounting-mappings-1.9.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:51.632201 fyle-accounting-mappings-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-03-23 11:48:51.632201 fyle-accounting-mappings-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:51.632201 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11692 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:51.632201 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0002_auto_20201117_0655.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0003_auto_20201221_1244.py
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0004_auto_20210127_1241.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0005_expenseattribute_auto_mapped.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0006_auto_20210305_0827.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0007_auto_20210409_1931.py
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0008_auto_20210604_0713.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0009_auto_20210618_1004.py
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0010_remove_mappingsetting_expense_field_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0011_categorymapping_employeemapping.py
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0012_auto_20211206_0600.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0013_auto_20220323_1133.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28393 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7479 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5730 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 11:48:51.632201 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-03-23 11:48:51.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-03-23 11:48:51.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 11:48:51.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-23 11:48:51.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-23 11:48:51.000000 fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 11:48:51.632201 fyle-accounting-mappings-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-03-23 11:48:41.000000 fyle-accounting-mappings-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:59:08.924479 fyle-accounting-mappings-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-03-24 10:59:08.920479 fyle-accounting-mappings-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:59:08.916479 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11692 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:59:08.920479 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      681 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0002_auto_20201117_0655.py
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0003_auto_20201221_1244.py
+-rw-r--r--   0 runner    (1001) docker     (121)      766 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0004_auto_20210127_1241.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0005_expenseattribute_auto_mapped.py
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0006_auto_20210305_0827.py
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0007_auto_20210409_1931.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0008_auto_20210604_0713.py
+-rw-r--r--   0 runner    (1001) docker     (121)      410 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0009_auto_20210618_1004.py
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0010_remove_mappingsetting_expense_field_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0011_categorymapping_employeemapping.py
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0012_auto_20211206_0600.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0013_auto_20220323_1133.py
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0014_mappingsetting_source_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28487 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7479 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 10:59:08.920479 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1699 2022-03-24 10:59:08.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-03-24 10:59:08.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 10:59:08.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-24 10:59:08.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-03-24 10:59:08.000000 fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-24 10:59:08.924479 fyle-accounting-mappings-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2022-03-24 10:58:57.000000 fyle-accounting-mappings-1.9.0/setup.py
```

### Comparing `fyle-accounting-mappings-1.8.0/LICENSE` & `fyle-accounting-mappings-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/PKG-INFO` & `fyle-accounting-mappings-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyle-accounting-mappings
-Version: 1.8.0
+Version: 1.9.0
 Summary: Django application to store the fyle accounting mappings in a generic manner
 Home-page: https://github.com/fylein/fyle-accounting-mappings
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Keywords: fyle,rest,django-rest-framework,api,python,accounting
 Platform: UNKNOWN
```

### Comparing `fyle-accounting-mappings-1.8.0/README.md` & `fyle-accounting-mappings-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/helpers.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/helpers.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0001_initial.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0002_auto_20201117_0655.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0002_auto_20201117_0655.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0003_auto_20201221_1244.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0003_auto_20201221_1244.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0004_auto_20210127_1241.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0004_auto_20210127_1241.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0006_auto_20210305_0827.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0006_auto_20210305_0827.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0007_auto_20210409_1931.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0007_auto_20210409_1931.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0008_auto_20210604_0713.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0008_auto_20210604_0713.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0011_categorymapping_employeemapping.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0011_categorymapping_employeemapping.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0012_auto_20211206_0600.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0012_auto_20211206_0600.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/migrations/0013_auto_20220323_1133.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/migrations/0013_auto_20220323_1133.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/models.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,14 +338,15 @@
     Mapping Settings
     """
     id = models.AutoField(primary_key=True)
     source_field = models.CharField(max_length=255, help_text='Source mapping field')
     destination_field = models.CharField(max_length=255, help_text='Destination mapping field')
     import_to_fyle = models.BooleanField(default=False, help_text='Import to Fyle or not')
     is_custom = models.BooleanField(default=False, help_text='Custom Field or not')
+    source_placeholder = models.TextField(help_text='placeholder of source field', null=True)
     workspace = models.ForeignKey(
         Workspace, on_delete=models.PROTECT, help_text='Reference to Workspace model',
         related_name='mapping_settings'
     )
     created_at = models.DateTimeField(auto_now_add=True, help_text='Created at datetime')
     updated_at = models.DateTimeField(auto_now=True, help_text='Updated at datetime')
```

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/serializers.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/serializers.py`

 * *Files identical despite different names*

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/urls.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.urls import path
 
 from .views import MappingSettingsView, MappingsView, EmployeeMappingsView, CategoryMappingsView,\
-    SearchDestinationAttributesView
+    SearchDestinationAttributesView, MappingStatsView
 
 urlpatterns = [
     path('settings/', MappingSettingsView.as_view()),
     path('employee/', EmployeeMappingsView.as_view()),
     path('category/', CategoryMappingsView.as_view()),
     path('destination_attributes/search/', SearchDestinationAttributesView.as_view()),
+    path('stats/', MappingStatsView.as_view()),
     path('', MappingsView.as_view())
 ]
```

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings/views.py` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -150,7 +150,38 @@
 
         destination_attributes = DestinationAttribute.objects.filter(
             value__icontains=destination_attribute_value,
             attribute_type=destination_attribute_type,
             workspace_id=self.kwargs['workspace_id']
         ).all()
         return destination_attributes
+
+
+class MappingStatsView(ListCreateAPIView):
+    """
+    Stats for total mapped and unmapped count for a given attribute type
+    """
+    def get(self, request, *args, **kwargs):
+        source_type = self.request.query_params.get('source_type')
+
+        assert_valid(source_type is not None, 'query param source_type not found')
+
+        total_attributes_count = ExpenseAttribute.objects.filter(
+            attribute_type=source_type, workspace_id=self.kwargs['workspace_id']
+        ).count()
+
+        if source_type == 'EMPLOYEE':
+            mapped_attributes_count = EmployeeMapping.objects.filter(
+                workspace_id=self.kwargs['workspace_id']
+            ).count()
+        else:
+            mapped_attributes_count = Mapping.objects.filter(
+                source_type=source_type, workspace_id=self.kwargs['workspace_id']
+            ).count()
+
+        return Response(
+            data={
+                'mapped_attributes_count': mapped_attributes_count,
+                'unmapped_attributes_count': total_attributes_count - mapped_attributes_count
+            },
+            status=status.HTTP_200_OK
+        )
```

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/PKG-INFO` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyle-accounting-mappings
-Version: 1.8.0
+Version: 1.9.0
 Summary: Django application to store the fyle accounting mappings in a generic manner
 Home-page: https://github.com/fylein/fyle-accounting-mappings
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Keywords: fyle,rest,django-rest-framework,api,python,accounting
 Platform: UNKNOWN
```

### Comparing `fyle-accounting-mappings-1.8.0/fyle_accounting_mappings.egg-info/SOURCES.txt` & `fyle-accounting-mappings-1.9.0/fyle_accounting_mappings.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 fyle_accounting_mappings/migrations/0007_auto_20210409_1931.py
 fyle_accounting_mappings/migrations/0008_auto_20210604_0713.py
 fyle_accounting_mappings/migrations/0009_auto_20210618_1004.py
 fyle_accounting_mappings/migrations/0010_remove_mappingsetting_expense_field_id.py
 fyle_accounting_mappings/migrations/0011_categorymapping_employeemapping.py
 fyle_accounting_mappings/migrations/0012_auto_20211206_0600.py
 fyle_accounting_mappings/migrations/0013_auto_20220323_1133.py
+fyle_accounting_mappings/migrations/0014_mappingsetting_source_placeholder.py
 fyle_accounting_mappings/migrations/__init__.py
```

### Comparing `fyle-accounting-mappings-1.8.0/setup.py` & `fyle-accounting-mappings-1.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='fyle-accounting-mappings',
-    version='1.8.0',
+    version='1.9.0',
     author='Shwetabh Kumar',
     author_email='shwetabh.kumar@fyle.in',
     description='Django application to store the fyle accounting mappings in a generic manner',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['fyle', 'rest', 'django-rest-framework', 'api', 'python', 'accounting'],
```

