# Comparing `tmp/django_model_signals-0.4.0.tar.gz` & `tmp/django_model_signals-0.4.1.tar.gz`

## Comparing `django_model_signals-0.4.0.tar` & `django_model_signals-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/apps.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/dispatcher.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/manager.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/signals.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/django_model_signals/transceiver.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/README.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 django_model_signals-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/apps.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/dispatcher.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/manager.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/signals.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/django_model_signals/transceiver.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/README.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 django_model_signals-0.4.1/PKG-INFO
```

### Comparing `django_model_signals-0.4.0/.github/workflows/publish-to-pypi.yml` & `django_model_signals-0.4.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/django_model_signals/apps.py` & `django_model_signals-0.4.1/django_model_signals/apps.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/django_model_signals/dispatcher.py` & `django_model_signals-0.4.1/django_model_signals/dispatcher.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/django_model_signals/manager.py` & `django_model_signals-0.4.1/django_model_signals/manager.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/django_model_signals/signals.py` & `django_model_signals-0.4.1/django_model_signals/signals.py`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/django_model_signals/transceiver.py` & `django_model_signals-0.4.1/django_model_signals/transceiver.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,30 @@
                 pre_full_clean.send(sender=self.__class__, **signal_kwargs)
             super().full_clean(*args, **kwargs)
             if 'post_full_clean' in self.ModelSignalsMeta.signals:
                 post_full_clean.send(sender=self.__class__, **signal_kwargs)
             return True
         except Exception as error:
             if 'post_full_clean_error' in self.ModelSignalsMeta.signals:
-                return self.post_full_clean_error(error, self.pk is None)
+                return self.post_full_clean_error(
+                    error=error,
+                    created=self.pk is None
+                )
             else:
                 raise error
 
     def save(self, **kwargs):
         try:
             super().save()
         except Exception as error:
             if 'post_save_error' in self.ModelSignalsMeta.signals:
-                self.post_save_error(error, self.pk is None)
+                self.post_save_error(
+                    error=error,
+                    created=self.pk is None
+                )
             else:
                 raise error
 
     @classmethod
     def pre_bulk_save(cls, **kwargs):
       pass
```

### Comparing `django_model_signals-0.4.0/LICENSE.md` & `django_model_signals-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/README.md` & `django_model_signals-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_model_signals-0.4.0/pyproject.toml` & `django_model_signals-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-model-signals"
-version = "0.4.0"
+version = "0.4.1"
 authors = [
   { name="Digital Valley", email="techteam@digitalvalley.nl" }
 ]
 description = "Django Model Signals makes it easier to keep model related business logic in your Django models by allowing them to become transceivers of their own signals, including bulk signals."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_model_signals-0.4.0/PKG-INFO` & `django_model_signals-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-signals
-Version: 0.4.0
+Version: 0.4.1
 Summary: Django Model Signals makes it easier to keep model related business logic in your Django models by allowing them to become transceivers of their own signals, including bulk signals.
 Author-email: Digital Valley <techteam@digitalvalley.nl>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

