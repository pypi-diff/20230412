# Comparing `tmp/django_model_signals-0.4.1.tar.gz` & `tmp/django_model_signals-0.4.2.tar.gz`

## Comparing `django_model_signals-0.4.1.tar` & `django_model_signals-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/apps.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/dispatcher.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/manager.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/signals.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/transceiver.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/LICENSE.md
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/django_model_signals/__init__.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/django_model_signals/apps.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/django_model_signals/dispatcher.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/django_model_signals/manager.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/django_model_signals/models.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/django_model_signals/signals.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/LICENSE.md
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 django_model_signals-0.4.2/PKG-INFO
```

### Comparing `django_model_signals-0.4.1/.github/workflows/publish-to-pypi.yml` & `django_model_signals-0.4.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.1/django_model_signals/apps.py` & `django_model_signals-0.4.2/django_model_signals/apps.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 # Django
 from django.apps import apps, AppConfig
 
 # Django Model Signals
 from django_model_signals.dispatcher import ModelSignalsDispatcher
 from django_model_signals.signals import MODEL_SIGNALS
-from django_model_signals.transceiver import ModelSignalsTransceiver
 
 
 class DjangoModelSignalsConfig(AppConfig):
     name = 'django_model_signals'
 
     def ready(self):
 
         # Don't bind signals when applying migrations
         if 'manage.py' in sys.argv and 'migrate' in sys.argv:
             return
 
         models = apps.get_models()
         for model in models:
-            if issubclass(model, ModelSignalsTransceiver):
+            if hasattr(model, 'ModelSignalsMeta'):
                 for signal_name, signal in MODEL_SIGNALS.items():
                     if signal_name in model.ModelSignalsMeta.signals:
                         signal.connect(
                             ModelSignalsDispatcher.get_signal_method(
                                 signal_name
-                            )
+                            ),
+                            sender=model,
+                            dispatch_uid=model.__name__ + '.' + signal_name
                         )
```

### Comparing `django_model_signals-0.4.1/django_model_signals/manager.py` & `django_model_signals-0.4.2/django_model_signals/manager.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.1/django_model_signals/signals.py` & `django_model_signals-0.4.2/django_model_signals/signals.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.1/django_model_signals/transceiver.py` & `django_model_signals-0.4.2/django_model_signals/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,38 @@
 from django_model_signals.signals import pre_full_clean, post_full_clean
 
 
-class ModelSignalsTransceiver:
-
-    @classmethod
-    def pre_init(cls, **kwargs):
-        pass
-
-    def post_init(self, **kwargs):
-        pass
-
-    def pre_full_clean(self, **kwargs):
-        pass
-
-    def post_full_clean(self, **kwargs):
-        pass
-
-    def post_full_clean_error(self, **kwargs):
-        raise kwargs['error']
-
-    def pre_save(self, **kwargs):
-        pass
-
-    def post_save(self, **kwargs):
-        pass
-
-    def post_save_error(self, **kwargs):
-        raise kwargs['error']
-
-    def pre_delete(self, **kwargs):
-        pass
-
-    def post_delete(self, **kwargs):
-        pass
-
-    def m2m_changed(self, **kwargs):
-        pass
+class FullCleanSignalsMixin:
 
     def full_clean(self, *args, **kwargs):
         try:
             signal_kwargs = {
-                'instance': self
+                'instance': self,
+                'created': self._state.adding == True
             }
             if 'pre_full_clean' in self.ModelSignalsMeta.signals:
                 pre_full_clean.send(sender=self.__class__, **signal_kwargs)
-            super().full_clean(*args, **kwargs)
+            result = super().full_clean(*args, **kwargs)
+            signal_kwargs['result'] = result
             if 'post_full_clean' in self.ModelSignalsMeta.signals:
                 post_full_clean.send(sender=self.__class__, **signal_kwargs)
-            return True
+            return result
         except Exception as error:
             if 'post_full_clean_error' in self.ModelSignalsMeta.signals:
-                return self.post_full_clean_error(
-                    error=error,
-                    created=self.pk is None
-                )
+                signal_kwargs['error'] = error
+                return self.post_full_clean_error(**signal_kwargs)
             else:
                 raise error
 
+
+class PostSaveErrorSignalMixin:
     def save(self, **kwargs):
         try:
-            super().save()
+            return super().save()
         except Exception as error:
             if 'post_save_error' in self.ModelSignalsMeta.signals:
-                self.post_save_error(
+                return self.post_save_error(
                     error=error,
-                    created=self.pk is None
+                    created=self._state.adding == True
                 )
             else:
                 raise error
-
-    @classmethod
-    def pre_bulk_save(cls, **kwargs):
-      pass
-
-    @classmethod
-    def post_bulk_save(cls, **kwargs):
-      pass
-
-    class ModelSignalsMeta:
-        signals = []
```

### Comparing `django_model_signals-0.4.1/LICENSE.md` & `django_model_signals-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.1/README.md` & `django_model_signals-0.4.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,39 @@
     # ...
     'django_model_signals',
 ]
 ```
 
 ## Usage
 
-- Add the `ModelSignalsTransceiver` class to your Django model.
 - Add a `ModelSignalsMeta` inner class to your Django model and specify which
-signals you're interested in.
-- Add the `ModelSignalsManager` to your Django model's `objects` property to
-enable bulk signals.
-- Implement the signal receiver methods in your Django model.
+signals you want to connect.
+- To enable the `pre_bulk_save` and `post_bulk_save` signals, add the
+  `ModelSignalsManager` to your Django model's `objects` property.
+- To enable the `pre_full_clean`, `post_full_clean` and `post_full_clean_error`
+  signals, inherit from the `FullCleanSignalsMixin` in your Django model.
+- To enable the `post_save_error` signal, inherit from the
+  `PostSaveErrorSignalMixin` in your Django model.
+- Implement the receiver methods for the connected signals in your Django
+  model.
 
 
 ## Example
 ```python
 from django.db.models import Model
 from django_model_signals.manager import ModelSignalsManager
-from django_model_signals.transceiver import ModelSignalsTransceiver
+from django_model_signals.models import (
+  FullCleanSignalsMixin,
+  PostSaveErrorSignalMixin
+)
+
 
 class MyModel(
-    ModelSignalsTransceiver,
+    FullCleanSignalsMixin,
+    PostSaveErrorSignalMixin,
     Model
 ):
 
     @classmethod
     def pre_init(cls, **kwargs):
         pass
 
@@ -87,16 +96,18 @@
 
     class ModelSignalsMeta:
         signals = [
             'pre_init',
             'post_init',
             'pre_full_clean',
             'post_full_clean',
+            'post_full_clean_error',
             'pre_save',
             'post_save',
+            'post_save_error',
             'pre_delete',
             'post_delete',
             'm2m_changed',
             'pre_bulk_save',
             'post_bulk_save'
         ]
 ```
@@ -128,11 +139,14 @@
     signals.
 - To implement the `pre_full_clean` and `post_full_clean`,
   `post_full_clean_error` and `post_save_errors` signals, this library
   overrides the `full_clean` and `save` methods of Django models and calls the
   original method in a backwards compatible way. However, make sure the order
   of the classes inherited from is the same as the above example to ensure the
   proper method resolution order.
+- The `post_full_clean_error` and `post_save_error` signals are not actually
+  called as signals, but the receiver methods are called directly. This allows
+  you to suppress, change or re-raise the error.
 
 ## Resources
 
 - Django: https://www.djangoproject.com/
```

### Comparing `django_model_signals-0.4.1/pyproject.toml` & `django_model_signals-0.4.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-model-signals"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Digital Valley", email="techteam@digitalvalley.nl" }
 ]
 description = "Django Model Signals makes it easier to keep model related business logic in your Django models by allowing them to become transceivers of their own signals, including bulk signals."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_model_signals-0.4.1/PKG-INFO` & `django_model_signals-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-signals
-Version: 0.4.1
+Version: 0.4.2
 Summary: Django Model Signals makes it easier to keep model related business logic in your Django models by allowing them to become transceivers of their own signals, including bulk signals.
 Author-email: Digital Valley <techteam@digitalvalley.nl>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,30 +32,39 @@
     # ...
     'django_model_signals',
 ]
 ```
 
 ## Usage
 
-- Add the `ModelSignalsTransceiver` class to your Django model.
 - Add a `ModelSignalsMeta` inner class to your Django model and specify which
-signals you're interested in.
-- Add the `ModelSignalsManager` to your Django model's `objects` property to
-enable bulk signals.
-- Implement the signal receiver methods in your Django model.
+signals you want to connect.
+- To enable the `pre_bulk_save` and `post_bulk_save` signals, add the
+  `ModelSignalsManager` to your Django model's `objects` property.
+- To enable the `pre_full_clean`, `post_full_clean` and `post_full_clean_error`
+  signals, inherit from the `FullCleanSignalsMixin` in your Django model.
+- To enable the `post_save_error` signal, inherit from the
+  `PostSaveErrorSignalMixin` in your Django model.
+- Implement the receiver methods for the connected signals in your Django
+  model.
 
 
 ## Example
 ```python
 from django.db.models import Model
 from django_model_signals.manager import ModelSignalsManager
-from django_model_signals.transceiver import ModelSignalsTransceiver
+from django_model_signals.models import (
+  FullCleanSignalsMixin,
+  PostSaveErrorSignalMixin
+)
+
 
 class MyModel(
-    ModelSignalsTransceiver,
+    FullCleanSignalsMixin,
+    PostSaveErrorSignalMixin,
     Model
 ):
 
     @classmethod
     def pre_init(cls, **kwargs):
         pass
 
@@ -101,16 +110,18 @@
 
     class ModelSignalsMeta:
         signals = [
             'pre_init',
             'post_init',
             'pre_full_clean',
             'post_full_clean',
+            'post_full_clean_error',
             'pre_save',
             'post_save',
+            'post_save_error',
             'pre_delete',
             'post_delete',
             'm2m_changed',
             'pre_bulk_save',
             'post_bulk_save'
         ]
 ```
@@ -142,11 +153,14 @@
     signals.
 - To implement the `pre_full_clean` and `post_full_clean`,
   `post_full_clean_error` and `post_save_errors` signals, this library
   overrides the `full_clean` and `save` methods of Django models and calls the
   original method in a backwards compatible way. However, make sure the order
   of the classes inherited from is the same as the above example to ensure the
   proper method resolution order.
+- The `post_full_clean_error` and `post_save_error` signals are not actually
+  called as signals, but the receiver methods are called directly. This allows
+  you to suppress, change or re-raise the error.
 
 ## Resources
 
 - Django: https://www.djangoproject.com/
```

