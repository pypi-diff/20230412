# Comparing `tmp/django-data-history-0.1.7.tar.gz` & `tmp/django-data-history-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-data-history-0.1.7.tar", last modified: Tue Jan 10 12:11:36 2023, max compression
+gzip compressed data, was "django-data-history-0.1.8.tar", last modified: Wed Apr 12 11:04:41 2023, max compression
```

## Comparing `django-data-history-0.1.7.tar` & `django-data-history-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.856261 django-data-history-0.1.7/
--rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-01 09:33:33.000000 django-data-history-0.1.7/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      225 2022-06-01 09:35:01.000000 django-data-history-0.1.7/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2932 2023-01-10 12:11:36.856082 django-data-history-0.1.7/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     2196 2023-01-10 08:05:06.000000 django-data-history-0.1.7/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.852309 django-data-history-0.1.7/django_data_history/
--rw-r--r--   0 test       (501) staff       (20)      551 2022-10-17 02:38:38.000000 django-data-history-0.1.7/django_data_history/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     3271 2023-01-10 08:09:27.000000 django-data-history-0.1.7/django_data_history/admin.py
--rw-r--r--   0 test       (501) staff       (20)      771 2022-06-22 05:33:42.000000 django-data-history-0.1.7/django_data_history/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.849251 django-data-history-0.1.7/django_data_history/locale/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.849297 django-data-history-0.1.7/django_data_history/locale/zh_Hans/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.854144 django-data-history-0.1.7/django_data_history/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 test       (501) staff       (20)     1449 2022-06-01 03:23:30.000000 django-data-history-0.1.7/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 test       (501) staff       (20)     3068 2022-06-01 03:23:26.000000 django-data-history-0.1.7/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.854725 django-data-history-0.1.7/django_data_history/migrations/
--rw-r--r--   0 test       (501) staff       (20)     1564 2022-06-01 08:48:42.000000 django-data-history-0.1.7/django_data_history/migrations/0001_initial.py
--rw-r--r--   0 test       (501) staff       (20)        0 2022-05-31 02:09:01.000000 django-data-history-0.1.7/django_data_history/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)    13830 2023-01-10 08:31:05.000000 django-data-history-0.1.7/django_data_history/models.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.849504 django-data-history-0.1.7/django_data_history/static/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.849623 django-data-history-0.1.7/django_data_history/static/django_data_history/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.854994 django-data-history-0.1.7/django_data_history/static/django_data_history/css/
--rw-r--r--   0 test       (501) staff       (20)      115 2022-06-01 09:13:04.000000 django-data-history-0.1.7/django_data_history/static/django_data_history/css/django_data_history.css
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.855252 django-data-history-0.1.7/django_data_history/static/django_data_history/js/
--rw-r--r--   0 test       (501) staff       (20)      359 2022-06-01 08:12:33.000000 django-data-history-0.1.7/django_data_history/static/django_data_history/js/django_data_history.js
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.849814 django-data-history-0.1.7/django_data_history/templates/
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.855510 django-data-history-0.1.7/django_data_history/templates/admin/
--rw-r--r--   0 test       (501) staff       (20)     3382 2022-06-01 09:06:49.000000 django-data-history-0.1.7/django_data_history/templates/admin/object_history.html
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.855759 django-data-history-0.1.7/django_data_history/templates/django_data_history/
--rw-r--r--   0 test       (501) staff       (20)      285 2022-05-31 09:43:28.000000 django-data-history-0.1.7/django_data_history/templates/django_data_history/userinfo.html
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:28.000000 django-data-history-0.1.7/django_data_history/tests.py
--rw-r--r--   0 test       (501) staff       (20)     1406 2022-06-22 05:33:17.000000 django-data-history-0.1.7/django_data_history/utils.py
--rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:25.000000 django-data-history-0.1.7/django_data_history/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2023-01-10 12:11:36.853336 django-data-history-0.1.7/django_data_history.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2932 2023-01-10 12:11:36.000000 django-data-history-0.1.7/django_data_history.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      989 2023-01-10 12:11:36.000000 django-data-history-0.1.7/django_data_history.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-01-10 12:11:36.000000 django-data-history-0.1.7/django_data_history.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2023-01-10 12:11:36.000000 django-data-history-0.1.7/django_data_history.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)      129 2023-01-10 12:11:36.000000 django-data-history-0.1.7/django_data_history.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       20 2023-01-10 12:11:36.000000 django-data-history-0.1.7/django_data_history.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)      129 2022-10-31 07:23:44.000000 django-data-history-0.1.7/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2023-01-10 12:11:36.856308 django-data-history-0.1.7/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1437 2023-01-10 08:37:29.000000 django-data-history-0.1.7/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.932333 django-data-history-0.1.8/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2022-06-01 09:33:33.000000 django-data-history-0.1.8/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      225 2022-06-01 09:35:01.000000 django-data-history-0.1.8/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     3777 2023-04-12 11:04:41.932207 django-data-history-0.1.8/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     3080 2023-04-12 11:03:38.000000 django-data-history-0.1.8/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.929398 django-data-history-0.1.8/django_data_history/
+-rw-r--r--   0 test       (501) staff       (20)      551 2022-10-17 02:38:38.000000 django-data-history-0.1.8/django_data_history/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3271 2023-01-10 08:09:27.000000 django-data-history-0.1.8/django_data_history/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      771 2022-06-22 05:33:42.000000 django-data-history-0.1.8/django_data_history/apps.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925297 django-data-history-0.1.8/django_data_history/locale/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925337 django-data-history-0.1.8/django_data_history/locale/zh_Hans/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.930694 django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 test       (501) staff       (20)     1449 2022-06-01 03:23:30.000000 django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 test       (501) staff       (20)     3068 2022-06-01 03:23:26.000000 django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931161 django-data-history-0.1.8/django_data_history/migrations/
+-rw-r--r--   0 test       (501) staff       (20)     1564 2022-06-01 08:48:42.000000 django-data-history-0.1.8/django_data_history/migrations/0001_initial.py
+-rw-r--r--   0 test       (501) staff       (20)        0 2022-05-31 02:09:01.000000 django-data-history-0.1.8/django_data_history/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)    14074 2023-04-12 09:22:30.000000 django-data-history-0.1.8/django_data_history/models.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925580 django-data-history-0.1.8/django_data_history/static/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925674 django-data-history-0.1.8/django_data_history/static/django_data_history/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931273 django-data-history-0.1.8/django_data_history/static/django_data_history/css/
+-rw-r--r--   0 test       (501) staff       (20)      115 2022-06-01 09:13:04.000000 django-data-history-0.1.8/django_data_history/static/django_data_history/css/django_data_history.css
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931473 django-data-history-0.1.8/django_data_history/static/django_data_history/js/
+-rw-r--r--   0 test       (501) staff       (20)      359 2022-06-01 08:12:33.000000 django-data-history-0.1.8/django_data_history/static/django_data_history/js/django_data_history.js
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.925826 django-data-history-0.1.8/django_data_history/templates/
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931664 django-data-history-0.1.8/django_data_history/templates/admin/
+-rw-r--r--   0 test       (501) staff       (20)     3382 2022-06-01 09:06:49.000000 django-data-history-0.1.8/django_data_history/templates/admin/object_history.html
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.931892 django-data-history-0.1.8/django_data_history/templates/django_data_history/
+-rw-r--r--   0 test       (501) staff       (20)      285 2022-05-31 09:43:28.000000 django-data-history-0.1.8/django_data_history/templates/django_data_history/userinfo.html
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:28.000000 django-data-history-0.1.8/django_data_history/tests.py
+-rw-r--r--   0 test       (501) staff       (20)     1603 2023-04-12 09:06:05.000000 django-data-history-0.1.8/django_data_history/utils.py
+-rw-r--r--   0 test       (501) staff       (20)      171 2022-06-22 05:33:25.000000 django-data-history-0.1.8/django_data_history/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2023-04-12 11:04:41.930246 django-data-history-0.1.8/django_data_history.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     3777 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      989 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)      129 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       20 2023-04-12 11:04:41.000000 django-data-history-0.1.8/django_data_history.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)      129 2022-10-31 07:23:44.000000 django-data-history-0.1.8/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2023-04-12 11:04:41.932367 django-data-history-0.1.8/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1437 2023-04-12 08:46:41.000000 django-data-history-0.1.8/setup.py
```

### Comparing `django-data-history-0.1.7/LICENSE` & `django-data-history-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/PKG-INFO` & `django-data-history-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: django-data-history
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Django application that allows you to store detailed data in the change log and display the detailed information in object's history view.
-Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: django-data-history
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -76,15 +74,40 @@
 # ]
 DO_NOT_SAVE_DATA_HISTORIES_FOR = [
     "your_app2.model_name2",
 ]
 
 ```
 
-## Instance's history view
+## Deep usage
+
+### How to ignore some fields' values?
+
+Some fields' value are inessential so that we want to ignore their changes.
+Simply add django_data_history_excludes in the model.
+
+```
+class TestModel(models.Model):
+
+    django_data_history_excludes = ["mod_time"]
+
+    mod_time = models.DateTimeField(auto_now=True)
+```
+
+If only mod_time changed, we are not treat the event as a change event, so that we will not make a new record.
+
+### How to save data history in separate table?
+
+Simply add `DATA_HISTORY_STORAGE_CLASS` property to the model class.
+A new `DATA_HISTORY_STORAGE_CLASS` must a subclass of `django_data_history.models.DataHistoryBase`.
+A `DATA_HISTORY_STORAGE_CLASS` can be a real class or a `absolute-dot-path` to the real class.
+
+### 
+
+## Instance's history view image
 
 ![django-date-history-view-preview](https://github.com/zencore-dobetter/pypi-images/raw/main/django-data-history/django-data-history.png)
 
 ## Releases
 
 ### v0.1.0
 
@@ -110,8 +133,11 @@
 
 - Fix requirements in setup.py.
 
 ### v0.1.7
 
 - Fix DataHistoryModelAdmin.get_data_histories function problem.
 
+### v0.1.8
 
+- Fix problems in working together with django-import-export.
+- Add django_data_history_excludes support.
```

### Comparing `django-data-history-0.1.7/README.md` & `django-data-history-0.1.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -57,15 +57,40 @@
 # ]
 DO_NOT_SAVE_DATA_HISTORIES_FOR = [
     "your_app2.model_name2",
 ]
 
 ```
 
-## Instance's history view
+## Deep usage
+
+### How to ignore some fields' values?
+
+Some fields' value are inessential so that we want to ignore their changes.
+Simply add django_data_history_excludes in the model.
+
+```
+class TestModel(models.Model):
+
+    django_data_history_excludes = ["mod_time"]
+
+    mod_time = models.DateTimeField(auto_now=True)
+```
+
+If only mod_time changed, we are not treat the event as a change event, so that we will not make a new record.
+
+### How to save data history in separate table?
+
+Simply add `DATA_HISTORY_STORAGE_CLASS` property to the model class.
+A new `DATA_HISTORY_STORAGE_CLASS` must a subclass of `django_data_history.models.DataHistoryBase`.
+A `DATA_HISTORY_STORAGE_CLASS` can be a real class or a `absolute-dot-path` to the real class.
+
+### 
+
+## Instance's history view image
 
 ![django-date-history-view-preview](https://github.com/zencore-dobetter/pypi-images/raw/main/django-data-history/django-data-history.png)
 
 ## Releases
 
 ### v0.1.0
 
@@ -90,7 +115,12 @@
 ### v0.1.6
 
 - Fix requirements in setup.py.
 
 ### v0.1.7
 
 - Fix DataHistoryModelAdmin.get_data_histories function problem.
+
+### v0.1.8
+
+- Fix problems in working together with django-import-export.
+- Add django_data_history_excludes support.
```

### Comparing `django-data-history-0.1.7/django_data_history/__init__.py` & `django-data-history-0.1.8/django_data_history/__init__.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/admin.py` & `django-data-history-0.1.8/django_data_history/admin.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/apps.py` & `django-data-history-0.1.8/django_data_history/apps.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po` & `django-data-history-0.1.8/django_data_history/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/migrations/0001_initial.py` & `django-data-history-0.1.8/django_data_history/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/models.py` & `django-data-history-0.1.8/django_data_history/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,19 @@
     @classmethod
     def get_data_history(cls, app_label, model_name, item_id):
         latest_history_item = cls.objects.filter(app_label=app_label, model_name=model_name, item_id=item_id).order_by("-version").first()
         return latest_history_item
 
     @classmethod
     def add_data_history(cls, item, action, username=None, userinfo=None, save=True, ignore_unchanged_version=True):
+    
+        # django-import-export 导入数据时，会调用add_data_history，但此时item却为空。
+        if item is None:
+            return
+
         nowtime = timezone.now()
         request = get_request()
         request_id = get_request_id()
 
         app_label = item._meta.app_label
         model_name = item._meta.model_name
         latest_history_item = cls.get_data_history(app_label, model_name, item.pk)
@@ -226,15 +231,18 @@
 class DataHistory(DataHistoryBase):
 
     class Meta:
         verbose_name = _("Data History")
         verbose_name_plural = _("Data Histories")
 
 def get_data_history_storage_class(instance_or_model_class):
-    return getattr(instance_or_model_class, "DATA_HISTORY_STORAGE_CLASS", DataHistory)
+    klass = getattr(instance_or_model_class, "DATA_HISTORY_STORAGE_CLASS", DataHistory)
+    if isinstance(klass, str):
+        klass = import_from_string(klass)
+    return klass
 
 def save_data_histories_for_fk_instance(instance):
     for field in instance._meta.fields:
         if isinstance(field, models.ForeignKey):
             fk_instance = getattr(instance, field.name)
             DataHistoryModel = get_data_history_storage_class(fk_instance)
             DataHistoryModel.add_data_history(fk_instance, action=DataHistoryModel.CHANGE, ignore_unchanged_version=True, save=True)
```

### Comparing `django-data-history-0.1.7/django_data_history/templates/admin/object_history.html` & `django-data-history-0.1.8/django_data_history/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/django_data_history/utils.py` & `django-data-history-0.1.8/django_data_history/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,8 +38,13 @@
         data2 = []
         for info in infos:
             data3 = info["fields"]
             data3["id"] = info["pk"]
             data2.append(data3)
         data[name] = data2
 
+    django_data_history_excludes = getattr(item.__class__, "django_data_history_excludes", [])
+    for field in django_data_history_excludes:
+        if field in data:
+            del data[field]
+
     return data
```

### Comparing `django-data-history-0.1.7/django_data_history.egg-info/PKG-INFO` & `django-data-history-0.1.8/django_data_history.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: django-data-history
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Django application that allows you to store detailed data in the change log and display the detailed information in object's history view.
-Home-page: UNKNOWN
 Author: zencore
 Author-email: dobetter@zencore.cn
 License: MIT
 Keywords: django-data-history
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
@@ -76,15 +74,40 @@
 # ]
 DO_NOT_SAVE_DATA_HISTORIES_FOR = [
     "your_app2.model_name2",
 ]
 
 ```
 
-## Instance's history view
+## Deep usage
+
+### How to ignore some fields' values?
+
+Some fields' value are inessential so that we want to ignore their changes.
+Simply add django_data_history_excludes in the model.
+
+```
+class TestModel(models.Model):
+
+    django_data_history_excludes = ["mod_time"]
+
+    mod_time = models.DateTimeField(auto_now=True)
+```
+
+If only mod_time changed, we are not treat the event as a change event, so that we will not make a new record.
+
+### How to save data history in separate table?
+
+Simply add `DATA_HISTORY_STORAGE_CLASS` property to the model class.
+A new `DATA_HISTORY_STORAGE_CLASS` must a subclass of `django_data_history.models.DataHistoryBase`.
+A `DATA_HISTORY_STORAGE_CLASS` can be a real class or a `absolute-dot-path` to the real class.
+
+### 
+
+## Instance's history view image
 
 ![django-date-history-view-preview](https://github.com/zencore-dobetter/pypi-images/raw/main/django-data-history/django-data-history.png)
 
 ## Releases
 
 ### v0.1.0
 
@@ -110,8 +133,11 @@
 
 - Fix requirements in setup.py.
 
 ### v0.1.7
 
 - Fix DataHistoryModelAdmin.get_data_histories function problem.
 
+### v0.1.8
 
+- Fix problems in working together with django-import-export.
+- Add django_data_history_excludes support.
```

### Comparing `django-data-history-0.1.7/django_data_history.egg-info/SOURCES.txt` & `django-data-history-0.1.8/django_data_history.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-data-history-0.1.7/setup.py` & `django-data-history-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open(os.path.join(here, 'requirements.txt'), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 
 setup(
     name="django-data-history",
-    version="0.1.7",
+    version="0.1.8",
     description="A Django application that allows you to store detailed data in the change log and display the detailed information in object's history view.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="zencore",
     author_email="dobetter@zencore.cn",
     license="MIT",
     classifiers=[
```

